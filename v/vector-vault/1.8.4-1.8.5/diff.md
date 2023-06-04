# Comparing `tmp/vector_vault-1.8.4.tar.gz` & `tmp/vector_vault-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.4.tar", last modified: Sun Jun  4 18:05:00 2023, max compression
+gzip compressed data, was "vector_vault-1.8.5.tar", last modified: Sun Jun  4 18:26:58 2023, max compression
```

## Comparing `vector_vault-1.8.4.tar` & `vector_vault-1.8.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 18:05:00.878695 vector_vault-1.8.4/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.4/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 18:05:00.878531 vector_vault-1.8.4/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.4/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 18:05:00.878733 vector_vault-1.8.4/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 18:04:52.000000 vector_vault-1.8.4/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 18:05:00.875949 vector_vault-1.8.4/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 18:05:00.000000 vector_vault-1.8.4/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 18:05:00.000000 vector_vault-1.8.4/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 18:05:00.000000 vector_vault-1.8.4/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 18:05:00.000000 vector_vault-1.8.4/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 18:05:00.000000 vector_vault-1.8.4/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 18:05:00.878224 vector_vault-1.8.4/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.4/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    10751 2023-06-04 02:08:51.000000 vector_vault-1.8.4/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.4/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.4/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.4/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-04 02:49:54.000000 vector_vault-1.8.4/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.4/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26507 2023-06-04 18:04:00.000000 vector_vault-1.8.4/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.4/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.4/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 18:26:58.738705 vector_vault-1.8.5/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.5/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 18:26:58.738516 vector_vault-1.8.5/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.5/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 18:26:58.738747 vector_vault-1.8.5/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 18:26:50.000000 vector_vault-1.8.5/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 18:26:58.735860 vector_vault-1.8.5/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 18:26:58.000000 vector_vault-1.8.5/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 18:26:58.000000 vector_vault-1.8.5/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 18:26:58.000000 vector_vault-1.8.5/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 18:26:58.000000 vector_vault-1.8.5/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 18:26:58.000000 vector_vault-1.8.5/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 18:26:58.738095 vector_vault-1.8.5/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.5/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    10755 2023-06-04 18:24:37.000000 vector_vault-1.8.5/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-04 02:49:49.000000 vector_vault-1.8.5/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.5/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.5/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-04 02:49:54.000000 vector_vault-1.8.5/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.5/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26720 2023-06-04 18:26:42.000000 vector_vault-1.8.5/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.5/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.5/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.4/LICENSE` & `vector_vault-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/PKG-INFO` & `vector_vault-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.8.4
+Version: 1.8.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.4/README.md` & `vector_vault-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/setup.py` & `vector_vault-1.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.4",
+    version="1.8.5",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.4/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.5/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.8.4
+Version: 1.8.5
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.4/vectorvault/__init__.py` & `vector_vault-1.8.5/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/ai.py` & `vector_vault-1.8.5/vectorvault/ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         Our Conversation History (if any): {history}
 
         Additional Context: {context}
 
         Question: {question}
 
-        (Answer the question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
+        (Respond to the Question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
         Answer:"""
 
         intokes = self.get_tokens(user_input)
         contokes = self.get_tokens(context)
         history = history if history else ""
         histokes = self.get_tokens(history)
```

### Comparing `vector_vault-1.8.4/vectorvault/cloudmanager.py` & `vector_vault-1.8.5/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/creds.py` & `vector_vault-1.8.5/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/download.py` & `vector_vault-1.8.5/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/itemize.py` & `vector_vault-1.8.5/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/signup.py` & `vector_vault-1.8.5/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/vault.py` & `vector_vault-1.8.5/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,14 +409,16 @@
                         user_input = segment + history if history_search else segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
+                        if self.ai.get_tokens(user_input) > 4000:
+                            user_input = user_input[-13000:]
                         if include_context_meta:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                             for text in context:
@@ -523,21 +525,23 @@
                 print(f"Time calc'd to sleep: {self.needed_sleep_time}")
 
             while True:
                 try:
                     if summary and not get_context:
                         response += self.ai.summarize(segment, model=model)
                     elif get_context and not summary:
-                        user_input = segment + history if history_search else segment
+                        user_input = segment
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-16000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-15000:]
                         if self.ai.get_tokens(user_input) > 4000:
                             user_input = user_input[-14000:]
+                        if self.ai.get_tokens(user_input) > 4000:
+                            user_input = user_input[-13000:]
                         if include_context_meta:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = str(context)
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
```

### Comparing `vector_vault-1.8.4/vectorvault/vecreq.py` & `vector_vault-1.8.5/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.4/vectorvault/wrap.py` & `vector_vault-1.8.5/vectorvault/wrap.py`

 * *Files identical despite different names*

