# Comparing `tmp/opower-0.0.7.tar.gz` & `tmp/opower-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opower-0.0.7.tar", last modified: Thu May 18 18:10:38 2023, max compression
+gzip compressed data, was "opower-0.0.8.tar", last modified: Sun Jun  4 05:53:19 2023, max compression
```

## Comparing `opower-0.0.7.tar` & `opower-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 18:10:19.000000 opower-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-18 18:10:38.479838 opower-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-18 18:10:19.000000 opower-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-18 18:10:19.000000 opower-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-18 18:10:38.479838 opower-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.475838 opower-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-18 18:10:19.000000 opower-0.0.7/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.475838 opower-0.0.7/src/opower/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/opower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/src/opower/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/pge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-18 18:10:19.000000 opower-0.0.7/src/opower/utilities/pse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/src/opower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 18:10:38.000000 opower-0.0.7/src/opower.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 18:10:38.479838 opower-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-18 18:10:19.000000 opower-0.0.7/tests/test_opower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 05:53:10.000000 opower-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-04 05:53:19.625353 opower-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-04 05:53:10.000000 opower-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-04 05:53:10.000000 opower-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-04 05:53:19.625353 opower-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.621353 opower-0.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-04 05:53:10.000000 opower-0.0.8/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.621353 opower-0.0.8/src/opower/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/opower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/src/opower/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/pge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-04 05:53:10.000000 opower-0.0.8/src/opower/utilities/pse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/src/opower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 05:53:19.000000 opower-0.0.8/src/opower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:53:19.625353 opower-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-04 05:53:10.000000 opower-0.0.8/tests/test_opower.py
```

### Comparing `opower-0.0.7/LICENSE` & `opower-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `opower-0.0.7/PKG-INFO` & `opower-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # opower
+
 A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&amp;E.
 
-To add support for a new utility that uses opower JSON API (you can tell if the energy dashboard of your utility is hosted on opower.com, e.g. pge.opower.com) add a file similar to [pge.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pge.py).
+To add support for a new utility that uses opower JSON API (you can tell if the energy dashboard of your utility is hosted on opower.com, e.g. pge.opower.com) add a file similar to [pge.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pge.py) or [pse.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pse.py).
 
 ## Example
 
 See [demo.py](https://github.com/tronikos/opower/blob/main/src/demo.py)
 
 ## Development environment
```

### Comparing `opower-0.0.7/README.md` & `opower-0.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # opower
+
 A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&amp;E.
 
-To add support for a new utility that uses opower JSON API (you can tell if the energy dashboard of your utility is hosted on opower.com, e.g. pge.opower.com) add a file similar to [pge.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pge.py).
+To add support for a new utility that uses opower JSON API (you can tell if the energy dashboard of your utility is hosted on opower.com, e.g. pge.opower.com) add a file similar to [pge.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pge.py) or [pse.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pse.py).
 
 ## Example
 
 See [demo.py](https://github.com/tronikos/opower/blob/main/src/demo.py)
 
 ## Development environment
```

### Comparing `opower-0.0.7/pyproject.toml` & `opower-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opower"
-version = "0.0.7"
+version = "0.0.8"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -59,21 +59,21 @@
     "UP",  # pyupgrade
     "W",  # pycodestyle
 ]
 
 ignore = [
     "D203",  # 1 blank line required before class docstring
     "D213",  # Multi-line docstring summary should start at the second line
+    # keep-runtime-annotations
+    'UP006', # Non PEP585 annotations
+    'UP007', # Non PEP604 annotations
 ]
 
 [tool.ruff.flake8-pytest-style]
 fixture-parentheses = false
 
-[tool.ruff.pyupgrade]
-keep-runtime-typing = true
-
 [tool.ruff.per-file-ignores]
 # Allow for demo script to write to stdout
 "demo.py" = ["T201"]
 
 [tool.ruff.mccabe]
 max-complexity = 25
```

### Comparing `opower-0.0.7/src/demo.py` & `opower-0.0.8/src/demo.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.7/src/opower/opower.py` & `opower-0.0.8/src/opower/opower.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 import json
 import logging
 import re
 from typing import Any
 from urllib.parse import urlencode
 
 import aiohttp
+from aiohttp.client_exceptions import ClientResponseError
 import arrow
 from multidict import CIMultiDict
 
+from .exceptions import CannotConnect, InvalidAuth
 from .utilities import UtilityBase
 
 _LOGGER = logging.getLogger(__file__)
 DEBUG_LOG_RESPONSE = False
 
 
 class MeterType(Enum):
@@ -142,18 +144,28 @@
         self.session._raise_for_status = True
         self.utility: type[UtilityBase] = _select_utility(utility)
         self.username = username
         self.password = password
         self.customer = None
 
     async def async_login(self) -> None:
-        """Login to the utility website and authorize opower.com for access."""
-        url = await self.utility.login(self.session, self.username, self.password)
-        if url is not None:
-            await self._async_authorize(url)
+        """Login to the utility website and authorize opower.com for access.
+
+        :raises InvalidAuth: if login information is incorrect
+        :raises CannotConnect: if we receive any HTTP error
+        """
+        try:
+            url = await self.utility.login(self.session, self.username, self.password)
+            if url is not None:
+                await self._async_authorize(url)
+        except ClientResponseError as err:
+            if err.status in (401, 403):
+                raise InvalidAuth(err)
+            else:
+                raise CannotConnect(err)
 
     async def _async_authorize(self, url: str) -> None:
         # Fetch the URL on the utility website to get RelayState and SAMLResponse.
         async with self.session.get(url) as resp:
             result = await resp.text()
         action_url, hidden_inputs = _get_form_action_url_and_hidden_inputs(result)
         assert action_url == "https://sso2.opower.com/sp/ACS.saml2"
@@ -380,12 +392,19 @@
                 start_date.date() if convert_to_date else start_date
             ).isoformat()
         if end_date:
             params["endDate"] = (
                 end_date.date() if convert_to_date else end_date
             ).isoformat()
         _LOGGER.debug("Fetching: %s?%s", url, urlencode(params))
-        async with self.session.get(url, params=params) as resp:
-            result = await resp.json()
-            if DEBUG_LOG_RESPONSE:
-                _LOGGER.debug("Fetched: %s", json.dumps(result, indent=2))
-            return result["reads"]
+        try:
+            async with self.session.get(url, params=params) as resp:
+                result = await resp.json()
+                if DEBUG_LOG_RESPONSE:
+                    _LOGGER.debug("Fetched: %s", json.dumps(result, indent=2))
+                return result["reads"]
+        except ClientResponseError as err:
+            # Ignore server errors for BILL requests
+            # that can happen if end_date is before account activation
+            if err.status == 500 and aggregate_type == AggregateType.BILL:
+                return []
+            raise err
```

### Comparing `opower-0.0.7/src/opower/utilities/base.py` & `opower-0.0.8/src/opower/utilities/base.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.7/src/opower/utilities/pge.py` & `opower-0.0.8/src/opower/utilities/pge.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.7/src/opower/utilities/pse.py` & `opower-0.0.8/src/opower/utilities/pse.py`

 * *Files identical despite different names*

### Comparing `opower-0.0.7/src/opower.egg-info/PKG-INFO` & `opower-0.0.8/src/opower.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # opower
+
 A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&amp;E.
 
-To add support for a new utility that uses opower JSON API (you can tell if the energy dashboard of your utility is hosted on opower.com, e.g. pge.opower.com) add a file similar to [pge.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pge.py).
+To add support for a new utility that uses opower JSON API (you can tell if the energy dashboard of your utility is hosted on opower.com, e.g. pge.opower.com) add a file similar to [pge.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pge.py) or [pse.py](https://github.com/tronikos/opower/blob/main/src/opower/utilities/pse.py).
 
 ## Example
 
 See [demo.py](https://github.com/tronikos/opower/blob/main/src/demo.py)
 
 ## Development environment
```

