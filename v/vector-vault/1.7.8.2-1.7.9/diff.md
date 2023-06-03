# Comparing `tmp/vector_vault-1.7.8.2.tar.gz` & `tmp/vector_vault-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.7.8.2.tar", last modified: Sat Jun  3 22:37:52 2023, max compression
+gzip compressed data, was "vector_vault-1.7.9.tar", last modified: Sat Jun  3 22:53:42 2023, max compression
```

## Comparing `vector_vault-1.7.8.2.tar` & `vector_vault-1.7.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:37:52.065369 vector_vault-1.7.8.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.8.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20083 2023-06-03 22:37:52.065209 vector_vault-1.7.8.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.8.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 22:37:52.065412 vector_vault-1.7.8.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1077 2023-06-03 22:37:45.000000 vector_vault-1.7.8.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:37:52.062211 vector_vault-1.7.8.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20083 2023-06-03 22:37:52.000000 vector_vault-1.7.8.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 22:37:52.000000 vector_vault-1.7.8.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 22:37:52.000000 vector_vault-1.7.8.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 22:37:52.000000 vector_vault-1.7.8.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 22:37:52.000000 vector_vault-1.7.8.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:37:52.064889 vector_vault-1.7.8.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.8.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7779 2023-06-03 22:37:39.000000 vector_vault-1.7.8.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 21:45:10.000000 vector_vault-1.7.8.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.8.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.8.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 21:45:08.000000 vector_vault-1.7.8.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.8.2/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26431 2023-06-03 21:45:19.000000 vector_vault-1.7.8.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.8.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.8.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:53:42.377618 vector_vault-1.7.9/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.7.9/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:53:42.377131 vector_vault-1.7.9/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.7.9/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 22:53:42.377663 vector_vault-1.7.9/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 22:53:18.000000 vector_vault-1.7.9/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:53:42.373736 vector_vault-1.7.9/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 22:53:42.000000 vector_vault-1.7.9/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:53:42.376767 vector_vault-1.7.9/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.7.9/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     7797 2023-06-03 22:42:23.000000 vector_vault-1.7.9/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3120 2023-06-03 22:41:30.000000 vector_vault-1.7.9/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.7.9/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.7.9/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1638 2023-06-03 22:41:23.000000 vector_vault-1.7.9/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.7.9/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26197 2023-06-03 22:53:12.000000 vector_vault-1.7.9/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.7.9/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.7.9/vectorvault/wrap.py
```

### Comparing `vector_vault-1.7.8.2/LICENSE` & `vector_vault-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/PKG-INFO` & `vector_vault-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.7.8.2
+Version: 1.7.9
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.8.2/README.md` & `vector_vault-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/setup.py` & `vector_vault-1.7.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.7.8.2",
+    version="1.7.9",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.7.8.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.7.9/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.7.8.2
+Version: 1.7.9
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.7.8.2/vectorvault/__init__.py` & `vector_vault-1.7.9/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/vectorvault/ai.py` & `vector_vault-1.7.9/vectorvault/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                             yield content
                         
                     
     # This function returns a ChatGPT completion based contextual input
     def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', stream=False):
         prompt_template = """
         Use the following Context to answer the Question at the end. 
-        Answer as if you were the modern voice of the context, without mentioning or implying that your response is based on it. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+        Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Our Conversation History (if any): {history}
 
         Additional Context: {context}
 
         Question: {question}
```

### Comparing `vector_vault-1.7.8.2/vectorvault/cloudmanager.py` & `vector_vault-1.7.9/vectorvault/cloudmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # Dissemination of this information or reproduction of this material
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault.
 
 import tempfile
 import os
 import json
-from .creds import CustomCredentials
-from .vecreq import call_proj
-from .itemize import cloud_name
+from creds import CustomCredentials
+from vecreq import call_proj
+from itemize import cloud_name
 from google.cloud import storage
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str):
         self.user = user
         self.api = api_key
```

### Comparing `vector_vault-1.7.8.2/vectorvault/creds.py` & `vector_vault-1.7.9/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/vectorvault/download.py` & `vector_vault-1.7.9/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/vectorvault/itemize.py` & `vector_vault-1.7.9/vectorvault/itemize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime 
-from .vecreq import call_name_vecs, call_buildpath
+from vecreq import call_name_vecs, call_buildpath
 from annoy import AnnoyIndex
 import threading
 from copy import deepcopy
 
 def itemize(vault, x, meta=None, text=None, name=None):
     meta = deepcopy(meta) if meta else {}
     if 'name' not in meta and name is not None:
```

### Comparing `vector_vault-1.7.8.2/vectorvault/signup.py` & `vector_vault-1.7.9/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/vectorvault/vault.py` & `vector_vault-1.7.9/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import tempfile
 import os
 import time
 import re
 import openai
 import json
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from .cloudmanager import CloudManager
-from .ai import AI
-from .itemize import itemize, name_vecs, get_item, get_vectors
-from .vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
+from cloudmanager import CloudManager
+from ai import AI
+from itemize import itemize, name_vecs, get_item, get_vectors
+from vecreq import call_items_by_vector, call_get_total_vectors, call_get_vaults, call_get_similar, call_get_chat
 
 
 class Vault:
     def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.api = api_key
@@ -531,46 +531,40 @@
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
                             input_ += text['data']
-                        for i in range(2):
-                            if i==0:
-                                for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
-                                    yield word
-                            if i==1:
-                                yield '!END'
-
-                        if return_context:
-                            for i in range(2):
-                                if i==0:
-                                    for item in context:
-                                        if type(metatag) is not list:
-                                            for tag in item['metadata']:
-                                                yield str(item['metadata'][f'{tag}'])
+
+                        if return_context: # send the ai stream, then the vault data
+                            for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
+                                yield word
+                            for item in context:
+                                if type(metatag) is not list:
+                                    for tag in item['metadata']:
+                                        yield str(item['metadata'][f'{tag}'])
+                                else:
+                                    if metatag_prefixes:
+                                        if metatag_suffixes:
+                                            for i in range(len(metatag)):
+                                                yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
-                                            if metatag_prefixes:
-                                                if metatag_suffixes:
-                                                    for i in range(len(metatag)):
-                                                        yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
-                                                else:
-                                                    for i in range(len(metatag)):
-                                                        yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
-                                        yield item['data']
-                                if i==1:
-                                    yield '!END'
+                                            for i in range(len(metatag)):
+                                                yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
+                                yield item['data']
+                            yield '!END'
+                        else: # No context return and just send back the ai stream only 
+                            for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
+                                yield word
+                            yield '!END'
                     else:
-                        for i in range(2):
-                            if i==0:
-                                for word in self.ai.llm(segment, history, model=model, stream=True):
-                                    yield word
-                                if i==1:
-                                    yield '!END'
+                        for word in self.ai.llm(segment, history, model=model, stream=True):
+                            yield word
+                        yield '!END'
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     time.sleep(5)
                     
             self.last_chat_time = start_time
```

### Comparing `vector_vault-1.7.8.2/vectorvault/vecreq.py` & `vector_vault-1.7.9/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.7.8.2/vectorvault/wrap.py` & `vector_vault-1.7.9/vectorvault/wrap.py`

 * *Files identical despite different names*

