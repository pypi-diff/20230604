# Comparing `tmp/vector_vault-1.8.1.tar.gz` & `tmp/vector_vault-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.1.tar", last modified: Sun Jun  4 02:47:20 2023, max compression
+gzip compressed data, was "vector_vault-1.8.2.tar", last modified: Sun Jun  4 02:50:22 2023, max compression
```

## Comparing `vector_vault-1.8.1.tar` & `vector_vault-1.8.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:47:20.278526 vector_vault-1.8.1/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.1/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:47:20.278283 vector_vault-1.8.1/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.1/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 02:47:20.278562 vector_vault-1.8.1/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 02:47:11.000000 vector_vault-1.8.1/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:47:20.274669 vector_vault-1.8.1/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:47:20.277887 vector_vault-1.8.1/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.1/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    10751 2023-06-04 02:08:51.000000 vector_vault-1.8.1/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3120 2023-06-04 02:01:30.000000 vector_vault-1.8.1/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.1/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.1/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1638 2023-06-04 02:01:44.000000 vector_vault-1.8.1/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.1/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26318 2023-06-04 02:30:10.000000 vector_vault-1.8.1/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.1/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.1/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:50:22.643395 vector_vault-1.8.2/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.2/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:50:22.643203 vector_vault-1.8.2/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.2/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 02:50:22.643442 vector_vault-1.8.2/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 02:50:19.000000 vector_vault-1.8.2/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:50:22.640486 vector_vault-1.8.2/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:50:22.642806 vector_vault-1.8.2/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.2/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    10751 2023-06-04 02:08:51.000000 vector_vault-1.8.2/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.2/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.2/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.2/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-04 02:49:54.000000 vector_vault-1.8.2/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.2/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26322 2023-06-04 02:50:07.000000 vector_vault-1.8.2/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.2/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.2/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.1/LICENSE` & `vector_vault-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/PKG-INFO` & `vector_vault-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.8.1
+Version: 1.8.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.1/README.md` & `vector_vault-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/setup.py` & `vector_vault-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.1",
+    version="1.8.2",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.1/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.2/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.8.1
+Version: 1.8.2
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.1/vectorvault/__init__.py` & `vector_vault-1.8.2/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/vectorvault/ai.py` & `vector_vault-1.8.2/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/vectorvault/cloudmanager.py` & `vector_vault-1.8.2/vectorvault/cloudmanager.py`

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

### Comparing `vector_vault-1.8.1/vectorvault/creds.py` & `vector_vault-1.8.2/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/vectorvault/download.py` & `vector_vault-1.8.2/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/vectorvault/itemize.py` & `vector_vault-1.8.2/vectorvault/itemize.py`

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

### Comparing `vector_vault-1.8.1/vectorvault/signup.py` & `vector_vault-1.8.2/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/vectorvault/vault.py` & `vector_vault-1.8.2/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 import os
 import time
 import re
 import openai
 import json
 import traceback
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

### Comparing `vector_vault-1.8.1/vectorvault/vecreq.py` & `vector_vault-1.8.2/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.1/vectorvault/wrap.py` & `vector_vault-1.8.2/vectorvault/wrap.py`

 * *Files identical despite different names*

