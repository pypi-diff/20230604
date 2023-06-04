# Comparing `tmp/vector_vault-1.8.2.tar.gz` & `tmp/vector_vault-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.2.tar", last modified: Sun Jun  4 02:50:22 2023, max compression
+gzip compressed data, was "vector_vault-1.8.3.tar", last modified: Sun Jun  4 05:08:12 2023, max compression
```

## Comparing `vector_vault-1.8.2.tar` & `vector_vault-1.8.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:50:22.643395 vector_vault-1.8.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:50:22.643203 vector_vault-1.8.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 02:50:22.643442 vector_vault-1.8.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 02:50:19.000000 vector_vault-1.8.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:50:22.640486 vector_vault-1.8.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 02:50:22.000000 vector_vault-1.8.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:50:22.642806 vector_vault-1.8.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    10751 2023-06-04 02:08:51.000000 vector_vault-1.8.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-04 02:49:54.000000 vector_vault-1.8.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.2/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26322 2023-06-04 02:50:07.000000 vector_vault-1.8.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 05:08:12.103820 vector_vault-1.8.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 05:08:12.103655 vector_vault-1.8.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 05:08:12.103860 vector_vault-1.8.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 05:06:52.000000 vector_vault-1.8.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 05:08:12.100448 vector_vault-1.8.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 05:08:12.000000 vector_vault-1.8.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 05:08:12.000000 vector_vault-1.8.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 05:08:12.000000 vector_vault-1.8.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 05:08:12.000000 vector_vault-1.8.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 05:08:12.000000 vector_vault-1.8.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 05:08:12.103235 vector_vault-1.8.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    10751 2023-06-04 02:08:51.000000 vector_vault-1.8.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-04 02:49:54.000000 vector_vault-1.8.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.3/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26283 2023-06-04 05:07:58.000000 vector_vault-1.8.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.3/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.2/LICENSE` & `vector_vault-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/PKG-INFO` & `vector_vault-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.8.2
+Version: 1.8.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.2/README.md` & `vector_vault-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/setup.py` & `vector_vault-1.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.2",
+    version="1.8.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.8.2
+Version: 1.8.3
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.2/vectorvault/__init__.py` & `vector_vault-1.8.3/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/ai.py` & `vector_vault-1.8.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/cloudmanager.py` & `vector_vault-1.8.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/creds.py` & `vector_vault-1.8.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/download.py` & `vector_vault-1.8.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/itemize.py` & `vector_vault-1.8.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/signup.py` & `vector_vault-1.8.3/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/vault.py` & `vector_vault-1.8.3/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,15 +536,15 @@
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
                             input_ += text['data']
 
                         if return_context: # send the ai stream, then the vault data
-                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, stream=True):
+                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model):
                                 yield word
                             for item in context:
                                 if type(metatag) is not list:
                                     for tag in item['metadata']:
                                         yield str(item['metadata'][f'{tag}'])
                                 else:
                                     if metatag_prefixes:
@@ -553,19 +553,19 @@
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
                             yield '!END'
                         else: # No context return and just send back the ai stream only 
-                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, stream=True):
+                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model):
                                 yield word
                             yield '!END'
                     else:
-                        for word in self.ai.llm_stream(segment, history, model=model, stream=True):
+                        for word in self.ai.llm_stream(segment, history, model=model):
                             yield word
                         yield '!END'
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     time.sleep(5)
```

### Comparing `vector_vault-1.8.2/vectorvault/vecreq.py` & `vector_vault-1.8.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.2/vectorvault/wrap.py` & `vector_vault-1.8.3/vectorvault/wrap.py`

 * *Files identical despite different names*

