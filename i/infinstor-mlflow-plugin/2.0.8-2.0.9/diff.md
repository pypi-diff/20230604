# Comparing `tmp/infinstor-mlflow-plugin-2.0.8.tar.gz` & `tmp/infinstor-mlflow-plugin-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/infinstor-mlflow-plugin-2.0.8.tar", last modified: Fri Jun  4 18:31:46 2021, max compression
+gzip compressed data, was "dist/infinstor-mlflow-plugin-2.0.9.tar", last modified: Mon Jul 19 05:49:24 2021, max compression
```

## Comparing `infinstor-mlflow-plugin-2.0.8.tar` & `infinstor-mlflow-plugin-2.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jagane    (1000) jagane    (1000)        0 2021-06-04 18:31:46.699623 infinstor-mlflow-plugin-2.0.8/
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      217 2021-06-04 18:31:46.699623 infinstor-mlflow-plugin-2.0.8/PKG-INFO
-drwxrwxr-x   0 jagane    (1000) jagane    (1000)        0 2021-06-04 18:31:46.699623 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/
--rw-rw-r--   0 jagane    (1000) jagane    (1000)        0 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/__init__.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)    29708 2021-06-03 05:03:00.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/cognito_auth_rest_store.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)     1382 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/gc.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      217 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/infinstor_artifact.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)     7506 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/infinstor_backend.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)     1750 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/infinstor_deployment_plugin.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)     6548 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/login.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      286 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/run_context_provider.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      111 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/servicedefs.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      371 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/sql_store_alchemy.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)     4120 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/tokenfile.py
--rw-rw-r--   0 jagane    (1000) jagane    (1000)    12218 2021-05-30 06:12:55.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/transformers.py
-drwxrwxr-x   0 jagane    (1000) jagane    (1000)        0 2021-06-04 18:31:46.699623 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      217 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      797 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 jagane    (1000) jagane    (1000)        1 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 jagane    (1000) jagane    (1000)      651 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 jagane    (1000) jagane    (1000)        7 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/requires.txt
--rw-rw-r--   0 jagane    (1000) jagane    (1000)       24 2021-06-04 18:31:46.000000 infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/top_level.txt
--rw-rw-r--   0 jagane    (1000) jagane    (1000)       38 2021-06-04 18:31:46.699623 infinstor-mlflow-plugin-2.0.8/setup.cfg
--rw-rw-r--   0 jagane    (1000) jagane    (1000)     1727 2021-06-04 18:31:07.000000 infinstor-mlflow-plugin-2.0.8/setup.py
+drwxrwxr-x   0 jagane    (1000) jagane    (1000)        0 2021-07-19 05:49:24.124624 infinstor-mlflow-plugin-2.0.9/
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      217 2021-07-19 05:49:24.124624 infinstor-mlflow-plugin-2.0.9/PKG-INFO
+drwxrwxr-x   0 jagane    (1000) jagane    (1000)        0 2021-07-19 05:49:24.124624 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)        0 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/__init__.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)    29708 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/cognito_auth_rest_store.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)     1382 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/gc.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      217 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/infinstor_artifact.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)     7506 2021-07-18 21:52:34.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/infinstor_backend.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)     1750 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/infinstor_deployment_plugin.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)     6498 2021-07-19 05:49:05.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/login.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      286 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/run_context_provider.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      111 2021-07-19 05:49:23.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/servicedefs.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      371 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/sql_store_alchemy.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)     4120 2021-07-19 05:42:09.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/tokenfile.py
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)    12218 2021-06-21 00:36:50.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/transformers.py
+drwxrwxr-x   0 jagane    (1000) jagane    (1000)        0 2021-07-19 05:49:24.124624 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      217 2021-07-19 05:49:24.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      797 2021-07-19 05:49:24.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)        1 2021-07-19 05:49:24.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)      651 2021-07-19 05:49:24.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)        7 2021-07-19 05:49:24.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/requires.txt
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)       24 2021-07-19 05:49:24.000000 infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/top_level.txt
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)       38 2021-07-19 05:49:24.124624 infinstor-mlflow-plugin-2.0.9/setup.cfg
+-rw-rw-r--   0 jagane    (1000) jagane    (1000)     1727 2021-07-19 05:47:51.000000 infinstor-mlflow-plugin-2.0.9/setup.py
```

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/cognito_auth_rest_store.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/cognito_auth_rest_store.py`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/gc.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/gc.py`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/infinstor_backend.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/infinstor_backend.py`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/infinstor_deployment_plugin.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/infinstor_deployment_plugin.py`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/login.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import builtins
 from . import servicedefs
 from infinstor_mlflow_plugin.tokenfile import read_token_file, write_token_file, get_token
 from requests.exceptions import HTTPError
 import requests
 from os.path import expanduser
 from os.path import sep as separator
-import datetime
+import time
 import configparser
 from urllib.parse import unquote
 import os
 
 def get_creds():
     if sys.stdin.isatty():
         print("Enter your InfinStor service username and password")
@@ -100,15 +100,15 @@
                 builtins.service = oneattr['Value']
                 print('Found serviceName ' + builtins.service + ' in cognito user')
                 break
     if (builtins.service == None):
         print('Could not determine service')
         raise Exception('login', 'Could not determine service')
 
-    token_time = round(datetime.datetime.timestamp(datetime.datetime.utcnow()))
+    token_time = int(time.time())
     tokfile = expanduser("~") + separator + '.infinstor' + separator + 'token'
     write_token_file(tokfile, token_time, token, refresh_token, builtins.clientid,\
                 builtins.service)
 
     payload = ("ProductCode=" + builtins.prodcode)
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded',
```

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/tokenfile.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/tokenfile.py`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin/transformers.py` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin/transformers.py`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/SOURCES.txt` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/infinstor_mlflow_plugin.egg-info/entry_points.txt` & `infinstor-mlflow-plugin-2.0.9/infinstor_mlflow_plugin.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `infinstor-mlflow-plugin-2.0.8/setup.py` & `infinstor-mlflow-plugin-2.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="infinstor-mlflow-plugin",
-    version="2.0.8",
+    version="2.0.9",
     description="InfinStor plugin for MLflow",
     packages=find_packages(),
     # Require MLflow as a dependency of the plugin, so that plugin users can simply install
     # the plugin & then immediately use it with MLflow
     install_requires=["mlflow"],
     entry_points={
         # Define a Tracking Store plugin for tracking URIs with scheme 'infinstor'
```

