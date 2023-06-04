# Comparing `tmp/opentherm-web-api-0.1.5.tar.gz` & `tmp/opentherm-web-api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentherm-web-api-0.1.5.tar", last modified: Sun Jun  4 10:11:54 2023, max compression
+gzip compressed data, was "opentherm-web-api-0.1.6.tar", last modified: Sun Jun  4 10:22:34 2023, max compression
```

## Comparing `opentherm-web-api-0.1.5.tar` & `opentherm-web-api-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.224042 opentherm-web-api-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/src/opentherm_web_api/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_web_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 10:11:54.000000 opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:11:54.228042 opentherm-web-api-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 10:11:39.000000 opentherm-web-api-0.1.5/tests/test_opentherm_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:22:34.989896 opentherm-web-api-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 10:22:34.989896 opentherm-web-api-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 10:22:34.989896 opentherm-web-api-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:22:34.985896 opentherm-web-api-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:22:34.989896 opentherm-web-api-0.1.6/src/opentherm_web_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/src/opentherm_web_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/src/opentherm_web_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/src/opentherm_web_api/opentherm_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/src/opentherm_web_api/opentherm_web_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:22:34.989896 opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 10:22:34.000000 opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-04 10:22:34.000000 opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:22:34.000000 opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 10:22:34.000000 opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 10:22:34.000000 opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:22:34.989896 opentherm-web-api-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 10:22:25.000000 opentherm-web-api-0.1.6/tests/test_opentherm_controller.py
```

### Comparing `opentherm-web-api-0.1.5/LICENSE` & `opentherm-web-api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.5/PKG-INFO` & `opentherm-web-api-0.1.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentherm-web-api
-Version: 0.1.5
+Version: 0.1.6
 Summary: WebAPI Connector for OpenThermWeb
 Home-page: https://github.com/Lake292/opentherm-web-api
 Author: Lake292
 Author-email: lake.erik@gmail.com
 Project-URL: Bug Reports, https://github.com/Lake292/opentherm-web-api/issues
 Keywords: openthermweb
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentherm-web-api-0.1.5/setup.py` & `opentherm-web-api-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_controller.py` & `opentherm-web-api-0.1.6/src/opentherm_web_api/opentherm_controller.py`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.5/src/opentherm_web_api/opentherm_web_api.py` & `opentherm-web-api-0.1.6/src/opentherm_web_api/opentherm_web_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,25 +73,25 @@
 
         api_url = urllib.parse.urljoin(self.host, "/opentherm/controller")
         data = self.controller.get_json()
         requests.put(api_url, headers=headers, json=data, timeout=TIMEOUT)
 
     def set_room_temperature(self, temperature: float) -> None:
         """Set room temperature."""
-        self.room_setpoint = temperature
+        self.controller.room_setpoint = temperature
         self.push_change()
 
     def set_dhw_temperature(self, temperature: float) -> None:
         """Set domestic hot water temperature."""
-        self.dhw_setpoint = temperature
+        self.controller.dhw_setpoint = temperature
         self.push_change()
 
     def set_away_mode(self, away_mode: bool) -> None:
         """Set away mode."""
-        self.away = away_mode
+        self.controller.away = away_mode
         self.push_change()
 
     def set_hvac_mode(self, enabled: bool) -> None:
         """Set HVAC mode."""
-        self.enabled = enabled
+        self.controller.enabled = enabled
         self.push_change()
```

### Comparing `opentherm-web-api-0.1.5/src/opentherm_web_api.egg-info/PKG-INFO` & `opentherm-web-api-0.1.6/src/opentherm_web_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentherm-web-api
-Version: 0.1.5
+Version: 0.1.6
 Summary: WebAPI Connector for OpenThermWeb
 Home-page: https://github.com/Lake292/opentherm-web-api
 Author: Lake292
 Author-email: lake.erik@gmail.com
 Project-URL: Bug Reports, https://github.com/Lake292/opentherm-web-api/issues
 Keywords: openthermweb
 Classifier: Development Status :: 5 - Production/Stable
```

