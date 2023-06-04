# Comparing `tmp/cdktf-gke-auth-1.1.0.tar.gz` & `tmp/cdktf-gke-auth-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-gke-auth-1.1.0.tar", last modified: Sun Jun  4 13:16:17 2023, max compression
+gzip compressed data, was "cdktf-gke-auth-1.1.1.tar", last modified: Sun Jun  4 13:27:10 2023, max compression
```

## Comparing `cdktf-gke-auth-1.1.0.tar` & `cdktf-gke-auth-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.148796 cdktf-gke-auth-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/_jsii/cdktf-gke-auth@1.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:16:02.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:16:17.152796 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 13:16:17.000000 cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:27:10.562147 cdktf-gke-auth-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 13:27:10.562147 cdktf-gke-auth-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:27:10.562147 cdktf-gke-auth-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:27:10.558147 cdktf-gke-auth-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:27:10.562147 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:27:10.562147 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19438 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/_jsii/cdktf-gke-auth@1.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:26:56.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:27:10.562147 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-04 13:27:10.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-04 13:27:10.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:27:10.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-04 13:27:10.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 13:27:10.000000 cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/top_level.txt
```

### Comparing `cdktf-gke-auth-1.1.0/LICENSE` & `cdktf-gke-auth-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-gke-auth-1.1.0/PKG-INFO` & `cdktf-gke-auth-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-gke-auth
-Version: 1.1.0
+Version: 1.1.1
 Summary: cdktf-gke-auth
 Home-page: https://github.com/01walid/cdktf-gke-auth.git
 Author: Walid Ziouche<hi@walid.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/01walid/cdktf-gke-auth.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-gke-auth-1.1.0/README.md` & `cdktf-gke-auth-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-gke-auth-1.1.0/setup.py` & `cdktf-gke-auth-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-gke-auth",
-    "version": "1.1.0",
+    "version": "1.1.1",
     "description": "cdktf-gke-auth",
     "license": "Apache-2.0",
     "url": "https://github.com/01walid/cdktf-gke-auth.git",
     "long_description_content_type": "text/markdown",
     "author": "Walid Ziouche<hi@walid.dev>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_gke_auth",
         "cdktf_gke_auth._jsii"
     ],
     "package_data": {
         "cdktf_gke_auth._jsii": [
-            "cdktf-gke-auth@1.1.0.jsii.tgz"
+            "cdktf-gke-auth@1.1.1.jsii.tgz"
         ],
         "cdktf_gke_auth": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-gke-auth-1.1.0/src/cdktf_gke_auth/__init__.py` & `cdktf-gke-auth-1.1.1/src/cdktf_gke_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-gke-auth-1.1.0/src/cdktf_gke_auth.egg-info/PKG-INFO` & `cdktf-gke-auth-1.1.1/src/cdktf_gke_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-gke-auth
-Version: 1.1.0
+Version: 1.1.1
 Summary: cdktf-gke-auth
 Home-page: https://github.com/01walid/cdktf-gke-auth.git
 Author: Walid Ziouche<hi@walid.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/01walid/cdktf-gke-auth.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

