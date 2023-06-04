# Comparing `tmp/opentherm-web-api-0.1.0.tar.gz` & `tmp/opentherm-web-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentherm-web-api-0.1.0.tar", last modified: Sat Jun  3 22:11:56 2023, max compression
+gzip compressed data, was "opentherm-web-api-0.1.1.tar", last modified: Sun Jun  4 09:34:32 2023, max compression
```

## Comparing `opentherm-web-api-0.1.0.tar` & `opentherm-web-api-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:11:56.031590 opentherm-web-api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-03 22:11:56.031590 opentherm-web-api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-03 22:11:56.031590 opentherm-web-api-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:11:56.027590 opentherm-web-api-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:11:56.027590 opentherm-web-api-0.1.0/src/opentherm_web_api/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/src/opentherm_web_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/src/opentherm_web_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/src/opentherm_web_api/opentherm_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/src/opentherm_web_api/opentherm_web_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:11:56.027590 opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-03 22:11:55.000000 opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-03 22:11:56.000000 opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:11:55.000000 opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-03 22:11:55.000000 opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 22:11:55.000000 opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:11:56.031590 opentherm-web-api-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-03 22:11:46.000000 opentherm-web-api-0.1.0/tests/test_opentherm_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:34:32.853078 opentherm-web-api-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 09:34:32.853078 opentherm-web-api-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-04 09:34:32.853078 opentherm-web-api-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:34:32.849078 opentherm-web-api-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:34:32.853078 opentherm-web-api-0.1.1/src/opentherm_web_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/src/opentherm_web_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/src/opentherm_web_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/src/opentherm_web_api/opentherm_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/src/opentherm_web_api/opentherm_web_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:34:32.853078 opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 09:34:32.000000 opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-04 09:34:32.000000 opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:34:32.000000 opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-04 09:34:32.000000 opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-04 09:34:32.000000 opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:34:32.853078 opentherm-web-api-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-04 09:34:24.000000 opentherm-web-api-0.1.1/tests/test_opentherm_controller.py
```

### Comparing `opentherm-web-api-0.1.0/LICENSE` & `opentherm-web-api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.0/PKG-INFO` & `opentherm-web-api-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentherm-web-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: WebAPI Connector for OpenThermWeb
 Home-page: https://github.com/Lake292/opentherm-web-api
 Author: Lake292
 Author-email: lake.erik@gmail.com
 Project-URL: Bug Reports, https://github.com/Lake292/opentherm-web-api/issues
 Keywords: openthermweb
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `opentherm-web-api-0.1.0/setup.py` & `opentherm-web-api-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `opentherm-web-api-0.1.0/src/opentherm_web_api.egg-info/PKG-INFO` & `opentherm-web-api-0.1.1/src/opentherm_web_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentherm-web-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: WebAPI Connector for OpenThermWeb
 Home-page: https://github.com/Lake292/opentherm-web-api
 Author: Lake292
 Author-email: lake.erik@gmail.com
 Project-URL: Bug Reports, https://github.com/Lake292/opentherm-web-api/issues
 Keywords: openthermweb
 Classifier: Development Status :: 5 - Production/Stable
```

