# Comparing `tmp/opentherm-web-api-0.1.4.tar.gz` & `tmp/opentherm-web-api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentherm-web-api-0.1.4.tar", last modified: Sun Jun  4 09:54:54 2023, max compression
+gzip compressed data, was "opentherm-web-api-0.1.5.tar", last modified: Sun Jun  4 10:11:54 2023, max compression
```

## Comparing `opentherm-web-api-0.1.4.tar` & `opentherm-web-api-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/src/opentherm_web_api/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/src/opentherm_web_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/src/opentherm_web_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/src/opentherm_web_api/opentherm_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/src/opentherm_web_api/opentherm_web_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 09:54:54.000000 opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-04 09:54:54.000000 opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:54:54.000000 opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 09:54:54.000000 opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 09:54:54.000000 opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:54:54.578514 opentherm-web-api-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 09:54:41.000000 opentherm-web-api-0.1.4/tests/test_opentherm_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.224042 opentherm-web-api-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/src/opentherm_web_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_web_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/tests/test_opentherm_controller.py
```

### Comparing `opentherm-web-api-0.1.4/LICENSE` & `opentherm-web-api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.4/PKG-INFO` & `opentherm-web-api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentherm-web-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: WebAPI Connector for OpenThermWeb
 Home-page: https://github.com/Lake292/opentherm-web-api
 Author: Lake292
 Author-email: lake.erik@gmail.com
 Project-URL: Bug Reports, https://github.com/Lake292/opentherm-web-api/issues
 Keywords: openthermweb
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentherm-web-api-0.1.4/setup.py` & `opentherm-web-api-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.4/src/opentherm_web_api/opentherm_controller.py` & `opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_controller.py`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.4/src/opentherm_web_api/opentherm_web_api.py` & `opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_web_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {token}",
         }
 
         api_url = urllib.parse.urljoin(self.host, "/opentherm/controller")
         response = requests.get(api_url, headers=headers, timeout=TIMEOUT)
-        self.controller = OpenThermController(self, response)
+        self.controller = OpenThermController(response)
         return self.controller
 
     def push_change(self) -> None:
         """Push controller."""
         token = self.get_token()
         headers = {
             "Content-Type": "application/json",
```

### Comparing `opentherm-web-api-0.1.4/src/opentherm_web_api.egg-info/PKG-INFO` & `opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentherm-web-api
-Version: 0.1.4
+Version: 0.1.5
 Summary: WebAPI Connector for OpenThermWeb
 Home-page: https://github.com/Lake292/opentherm-web-api
 Author: Lake292
 Author-email: lake.erik@gmail.com
 Project-URL: Bug Reports, https://github.com/Lake292/opentherm-web-api/issues
 Keywords: openthermweb
 Classifier: Development Status :: 5 - Production/Stable
```

