# Comparing `tmp/vector_vault-1.7.9.tar.gz` & `tmp/vector_vault-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.9.tar", last modified: Sat Jun  3 22:53:42 2023, max compression
+gzip compressed data, was "vector_vault-1.8.0.tar", last modified: Sat Jun  3 22:58:11 2023, max compression
```

## Comparing `vector_vault-1.7.9.tar` & `vector_vault-1.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:53:42.377618 vector_vault-1.7.9/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.9/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:53:42.377131 vector_vault-1.7.9/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.9/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 22:53:42.377663 vector_vault-1.7.9/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 22:53:18.000000 vector_vault-1.7.9/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:53:42.373736 vector_vault-1.7.9/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:53:42.376767 vector_vault-1.7.9/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.9/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7797 2023-06-03 22:42:23.000000 vector_vault-1.7.9/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3120 2023-06-03 22:41:30.000000 vector_vault-1.7.9/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.9/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.9/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1638 2023-06-03 22:41:23.000000 vector_vault-1.7.9/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.9/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26197 2023-06-03 22:53:12.000000 vector_vault-1.7.9/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.9/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.9/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:58:11.919441 vector_vault-1.8.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:58:11.919152 vector_vault-1.8.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 22:58:11.919483 vector_vault-1.8.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 22:58:04.000000 vector_vault-1.8.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:58:11.915916 vector_vault-1.8.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:58:11.918722 vector_vault-1.8.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7797 2023-06-03 22:42:23.000000 vector_vault-1.8.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 22:57:44.000000 vector_vault-1.8.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 22:57:48.000000 vector_vault-1.8.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26201 2023-06-03 22:57:56.000000 vector_vault-1.8.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.9/LICENSE` & `vector_vault-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/PKG-INFO` & `vector_vault-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.9
+Version: 1.8.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.9/README.md` & `vector_vault-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/setup.py` & `vector_vault-1.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.9",
+    version="1.8.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.9/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.0/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.9
+Version: 1.8.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.9/vectorvault/__init__.py` & `vector_vault-1.8.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/vectorvault/ai.py` & `vector_vault-1.8.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/vectorvault/cloudmanager.py` & `vector_vault-1.8.0/vectorvault/cloudmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import tempfile
 import os
 import json
-from creds import CustomCredentials
-from vecreq import call_proj
-from itemize import cloud_name
+from .creds import CustomCredentials
+from .vecreq import call_proj
+from .itemize import cloud_name
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = user
         self.api = api_key
```

### Comparing `vector_vault-1.7.9/vectorvault/creds.py` & `vector_vault-1.8.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/vectorvault/download.py` & `vector_vault-1.8.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/vectorvault/itemize.py` & `vector_vault-1.8.0/vectorvault/itemize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime 
-from vecreq import call_name_vecs, call_buildpath
+from .vecreq import call_name_vecs, call_buildpath
 from annoy import AnnoyIndex
 import threading
 from copy import deepcopy
 
 def itemize(vault, x, meta=None, text=None, name=None):
     meta = deepcopy(meta) if meta else {}
     if 'name' not in meta and name is not None:
```

### Comparing `vector_vault-1.7.9/vectorvault/signup.py` & `vector_vault-1.8.0/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/vectorvault/vault.py` & `vector_vault-1.8.0/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import tempfile
 import os
 import time
 import re
 import openai
 import json
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from cloudmanager import CloudManager
-from ai import AI
-from itemize import itemize, name_vecs, get_item, get_vectors
-from vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
+from .cloudmanager import CloudManager
+from .ai import AI
+from .itemize import itemize, name_vecs, get_item, get_vectors
+from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
```

### Comparing `vector_vault-1.7.9/vectorvault/vecreq.py` & `vector_vault-1.8.0/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.9/vectorvault/wrap.py` & `vector_vault-1.8.0/vectorvault/wrap.py`

 * *Files identical despite different names*

