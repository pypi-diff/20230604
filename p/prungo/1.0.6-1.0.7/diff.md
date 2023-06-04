# Comparing `tmp/prungo-1.0.6.tar.gz` & `tmp/prungo-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prungo-1.0.6.tar", max compression
+gzip compressed data, was "prungo-1.0.7.tar", max compression
```

## Comparing `prungo-1.0.6.tar` & `prungo-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1497 2023-06-04 03:52:15.729837 prungo-1.0.6/LICENSE
--rw-r--r--   0        0        0      185 2023-06-04 03:52:15.729837 prungo-1.0.6/README.md
--rw-r--r--   0        0        0       97 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/__init__.py
--rw-r--r--   0        0        0      103 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/constants.py
--rw-r--r--   0        0        0     2090 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/decorators.py
--rw-r--r--   0        0        0      445 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/interfaces.py
--rw-r--r--   0        0        0        0 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/models.py
--rw-r--r--   0        0        0     2127 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/utils.py
--rw-r--r--   0        0        0      785 2023-06-04 03:52:26.641993 prungo-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 prungo-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-04 07:08:32.535797 prungo-1.0.7/LICENSE
+-rw-r--r--   0        0        0      185 2023-06-04 07:08:32.535797 prungo-1.0.7/README.md
+-rw-r--r--   0        0        0       97 2023-06-04 07:08:32.535797 prungo-1.0.7/prungo/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-04 07:08:32.535797 prungo-1.0.7/prungo/constants.py
+-rw-r--r--   0        0        0     3118 2023-06-04 07:08:32.535797 prungo-1.0.7/prungo/decorators.py
+-rw-r--r--   0        0        0      445 2023-06-04 07:08:32.535797 prungo-1.0.7/prungo/interfaces.py
+-rw-r--r--   0        0        0        0 2023-06-04 07:08:32.535797 prungo-1.0.7/prungo/models.py
+-rw-r--r--   0        0        0     2127 2023-06-04 07:08:32.535797 prungo-1.0.7/prungo/utils.py
+-rw-r--r--   0        0        0      785 2023-06-04 07:08:46.132391 prungo-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 prungo-1.0.7/PKG-INFO
```

### Comparing `prungo-1.0.6/LICENSE` & `prungo-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prungo-1.0.6/prungo/decorators.py` & `prungo-1.0.7/prungo/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import logging
 from functools import wraps
 from inspect import signature
 from typing import Any, Callable, ParamSpec, TypeVar
 
-from prungo.constants import LOG_CALL_LIMIT, SENTINEL, SERVICE_NAME
+from prungo.constants import (
+    CALLED_STR,
+    FAILED_STR,
+    LOG_CALL_LIMIT,
+    SENTINEL,
+    SERVICE_NAME,
+    SUCCESS_STR,
+)
 from prungo.interfaces import logger_type
 from prungo.utils import DisplayStyle, dynamic_fstring, introspect_params, safe_cast
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 logger = logging.getLogger(SERVICE_NAME)
@@ -34,36 +41,69 @@
 def log_call(
     method: Callable | None = None,
     *,
     log: logger_type = logging.getLogger(SERVICE_NAME),
     static: Any = None,
     param_name: Any = None,
     log_length: int = LOG_CALL_LIMIT,
+    success: bool = False,
     separator: str = "|",
     filler: str = "-",
 ):
     """
     :method: function being passed to `log_call` unless other params are being used
     :log: optional logger - uses default if left blank
     :static: a static value to be logged
     :param_name: the parameter name to be logged
+    :log_length: maximum length of the decorations added to the log message
+    :success: log twice, on call and success/failure; provides context
+    :separator: separate segments by this character
+    :filler: add this character repeated to the outside of the message
     """
 
     @make_decorator
     def decorator(func: Callable, *args, **kwargs):
         logs = []
         logs.append(func.__name__)
+        sep = f" {separator.strip()} "
+
+        def execute_log():
+            clean_logs = list(filter(lambda x: x is not SENTINEL, logs))
+            log_text = f" {sep.join(clean_logs).strip()} "
+            display_log = dynamic_fstring(
+                text=log_text,
+                wrapping_char=filler,
+                style=DisplayStyle.CENTRE,
+                limit=log_length,
+            )
+            log.info(display_log)
+
+        def check_success(
+            param: Any,
+            success_str: str = SUCCESS_STR,
+            fail_str: str = FAILED_STR,
+        ):
+            if not param:
+                return fail_str
+
+            return success_str
 
         if static is not None:
             logs.append(safe_cast(static, str, SENTINEL))
 
         if param_name is not None:
             logs.append(introspect_params(param_name, args, kwargs, func))
 
-        logs = list(filter(lambda x: x is not SENTINEL, logs))
+        if success:
+            logs.append(CALLED_STR)
 
-        sep = f" {separator.strip()} "
-        log_text = f" {sep.join(logs).strip()} "
-        log.info(dynamic_fstring(log_text, filler, DisplayStyle.CENTRE, log_length))
-        return func(*args, **kwargs)
+        execute_log()
+        response = func(*args, **kwargs)
+
+        if success:
+            logs.pop(-1)
+            logs.append(check_success(response))
+            execute_log()
+
+        return response
 
     return decorator if method is None else decorator(method)
```

### Comparing `prungo-1.0.6/prungo/utils.py` & `prungo-1.0.7/prungo/utils.py`

 * *Files identical despite different names*

### Comparing `prungo-1.0.6/pyproject.toml` & `prungo-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prungo"
-version = "1.0.6"
+version = "1.0.7"
 description = "A package for basic utility functions/classes"
 authors = ["c-prungo"]
 packages = [{include = "prungo"}]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/c-prungo/prungo-util"
 repository = "https://github.com/c-prungo/prungo-util"
```

### Comparing `prungo-1.0.6/PKG-INFO` & `prungo-1.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prungo
-Version: 1.0.6
+Version: 1.0.7
 Summary: A package for basic utility functions/classes
 Home-page: https://github.com/c-prungo/prungo-util
 License: MIT
 Author: c-prungo
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

