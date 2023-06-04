# Comparing `tmp/prungo-1.0.5.tar.gz` & `tmp/prungo-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prungo-1.0.5.tar", max compression
+gzip compressed data, was "prungo-1.0.6.tar", max compression
```

## Comparing `prungo-1.0.5.tar` & `prungo-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1497 2023-06-04 03:36:29.207519 prungo-1.0.5/LICENSE
--rw-r--r--   0        0        0      190 2023-06-04 03:36:29.207519 prungo-1.0.5/README.md
--rw-r--r--   0        0        0       97 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/__init__.py
--rw-r--r--   0        0        0      103 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/constants.py
--rw-r--r--   0        0        0     2090 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/decorators.py
--rw-r--r--   0        0        0      445 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/interfaces.py
--rw-r--r--   0        0        0        0 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/models.py
--rw-r--r--   0        0        0     1717 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/utils.py
--rw-r--r--   0        0        0      786 2023-06-04 03:36:41.411515 prungo-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 prungo-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-04 03:52:15.729837 prungo-1.0.6/LICENSE
+-rw-r--r--   0        0        0      185 2023-06-04 03:52:15.729837 prungo-1.0.6/README.md
+-rw-r--r--   0        0        0       97 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/constants.py
+-rw-r--r--   0        0        0     2090 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/decorators.py
+-rw-r--r--   0        0        0      445 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/interfaces.py
+-rw-r--r--   0        0        0        0 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/models.py
+-rw-r--r--   0        0        0     2127 2023-06-04 03:52:15.729837 prungo-1.0.6/prungo/utils.py
+-rw-r--r--   0        0        0      785 2023-06-04 03:52:26.641993 prungo-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 prungo-1.0.6/PKG-INFO
```

### Comparing `prungo-1.0.5/LICENSE` & `prungo-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prungo-1.0.5/prungo/decorators.py` & `prungo-1.0.6/prungo/decorators.py`

 * *Files identical despite different names*

### Comparing `prungo-1.0.5/prungo/utils.py` & `prungo-1.0.6/prungo/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,28 +13,33 @@
 ) -> Any | None:
     if index < len(iter):
         return iter[index]
 
     return default
 
 
-def safe_cast(
-    value: Any,
-    cast_type: type,
-    default: Any = None,
-):
-    try:
-        return cast_type(value)
-    except TypeError:
-        pass
+def safe_cast(val: Any, to_type: type, default: Any = None):
+    """Safely cast a value to type, and if failed, returned default if exists.
+    Optional: Pass default value. Returned if casting fails.
+
+    :val: Value to be cast.
+    :to_type: Safely cast to a specific type.
+    :default: Default if casting fails.
+    :return: Return casted value or default.
+    """
+    if val is None:
+        return default
 
-    if default is None:
-        return value
+    try:
+        return to_type(val)
+    except (ValueError, TypeError) as e:
+        if default is not None:
+            return default
 
-    return default
+        raise type(e)(f"{e}, {val}: {type(val).__name__} to {to_type.__name__}")
 
 
 def introspect_params(key: str, args: tuple, kwargs: dict, func: Callable):
     param = kwargs.get(key, SENTINEL)
     if param is not SENTINEL:
         return param
```

### Comparing `prungo-1.0.5/pyproject.toml` & `prungo-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prungo"
-version = "v1.0.5"
+version = "1.0.6"
 description = "A package for basic utility functions/classes"
 authors = ["c-prungo"]
 packages = [{include = "prungo"}]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/c-prungo/prungo-util"
 repository = "https://github.com/c-prungo/prungo-util"
```

### Comparing `prungo-1.0.5/PKG-INFO` & `prungo-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: prungo
-Version: 1.0.5
+Version: 1.0.6
 Summary: A package for basic utility functions/classes
 Home-page: https://github.com/c-prungo/prungo-util
 License: MIT
 Author: c-prungo
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Project-URL: Repository, https://github.com/c-prungo/prungo-util
 Description-Content-Type: text/markdown
 
-# prungo-util
+# prungo
 
 basic utility package for boiler-plate and helper functions
 
 ---
 
 ## resources
```

