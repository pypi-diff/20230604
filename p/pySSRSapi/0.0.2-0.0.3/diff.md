# Comparing `tmp/pySSRSapi-0.0.2.tar.gz` & `tmp/pySSRSapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySSRSapi-0.0.2.tar", last modified: Sat Jun  3 20:19:03 2023, max compression
+gzip compressed data, was "pySSRSapi-0.0.3.tar", last modified: Sat Jun  3 22:43:53 2023, max compression
```

## Comparing `pySSRSapi-0.0.2.tar` & `pySSRSapi-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 20:19:03.720236 pySSRSapi-0.0.2/
--rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 20:19:03.719709 pySSRSapi-0.0.2/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.2/README.md
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 20:19:03.712626 pySSRSapi-0.0.2/pySSRSapi/
--rw-r--r--   0 quaik8     (501) staff       (20)     8870 2023-06-03 20:15:20.000000 pySSRSapi-0.0.2/pySSRSapi/__init__.py
-drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 20:19:03.718939 pySSRSapi-0.0.2/pySSRSapi.egg-info/
--rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/PKG-INFO
--rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/SOURCES.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/dependency_links.txt
--rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/requires.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-03 20:19:03.000000 pySSRSapi-0.0.2/pySSRSapi.egg-info/top_level.txt
--rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-03 20:19:03.720350 pySSRSapi-0.0.2/setup.cfg
--rw-r--r--   0 quaik8     (501) staff       (20)      800 2023-06-03 20:18:30.000000 pySSRSapi-0.0.2/setup.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 22:43:53.631508 pySSRSapi-0.0.3/
+-rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 22:43:53.630801 pySSRSapi-0.0.3/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)       15 2023-06-03 18:55:05.000000 pySSRSapi-0.0.3/README.md
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 22:43:53.626665 pySSRSapi-0.0.3/pySSRSapi/
+-rw-r--r--   0 quaik8     (501) staff       (20)     8751 2023-06-03 22:43:05.000000 pySSRSapi-0.0.3/pySSRSapi/__init__.py
+drwxr-xr-x   0 quaik8     (501) staff       (20)        0 2023-06-03 22:43:53.629965 pySSRSapi-0.0.3/pySSRSapi.egg-info/
+-rw-r--r--   0 quaik8     (501) staff       (20)      532 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/PKG-INFO
+-rw-r--r--   0 quaik8     (501) staff       (20)      204 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/SOURCES.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        1 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/dependency_links.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)        9 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/requires.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       10 2023-06-03 22:43:53.000000 pySSRSapi-0.0.3/pySSRSapi.egg-info/top_level.txt
+-rw-r--r--   0 quaik8     (501) staff       (20)       38 2023-06-03 22:43:53.631706 pySSRSapi-0.0.3/setup.cfg
+-rw-r--r--   0 quaik8     (501) staff       (20)      800 2023-06-03 22:43:45.000000 pySSRSapi-0.0.3/setup.py
```

### Comparing `pySSRSapi-0.0.2/PKG-INFO` & `pySSRSapi-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pySSRSapi-0.0.2/pySSRSapi/__init__.py` & `pySSRSapi-0.0.3/pySSRSapi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import base64
 import json
 import requests
 from requests.auth import HTTPBasicAuth
 
 EP_API = '/api/v2.0'
-EP_ME = '/Me'
-EP_CATALOG_ITEMS = '/CatalogItems'
-EP_FOLDERS = '/Folders'
-EP_REPORTS = '/Reports'
-EP_DATASOURCES = '/DataSources'
-# find a way to get this ID
-ROOT_FOLDER_ID = 'fb44eb1c-1b98-4dc7-beee-8cbc9dc3ed6e'
+EP_ME = '/me'
+EP_FOLDERS = '/folders'
+EP_REPORTS = '/reports'
+EP_DATASOURCES = '/datasources'
 
 class User:
     def __init__(self, Id: str, Username: str, DisplayName: str):
         self.Id = Id
         self.Username = Username
         self.DisplayName = DisplayName
```

### Comparing `pySSRSapi-0.0.2/pySSRSapi.egg-info/PKG-INFO` & `pySSRSapi-0.0.3/pySSRSapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySSRSapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python SSRS API
 Home-page: https://pypi.org/project/pySSRSapi/
 Author: quaik8
 Author-email: mail@example.com
 License: MIT license
 Keywords: SSRS,API
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pySSRSapi-0.0.2/setup.py` & `pySSRSapi-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pySSRSapi',
-    version='0.0.2',
+    version='0.0.3',
     description='Python SSRS API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='SSRS, API',
     author='quaik8',
     author_email='mail@example.com',
     url='https://pypi.org/project/pySSRSapi/',
```

