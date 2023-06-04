# Comparing `tmp/vector_vault-1.8.0.tar.gz` & `tmp/vector_vault-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.8.0.tar", last modified: Sat Jun  3 22:58:11 2023, max compression
+gzip compressed data, was "vector_vault-1.8.1.tar", last modified: Sun Jun  4 02:47:20 2023, max compression
```

## Comparing `vector_vault-1.8.0.tar` & `vector_vault-1.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:58:11.919441 vector_vault-1.8.0/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.0/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:58:11.919152 vector_vault-1.8.0/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.0/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-03 22:58:11.919483 vector_vault-1.8.0/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-03 22:58:04.000000 vector_vault-1.8.0/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:58:11.915916 vector_vault-1.8.0/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-03 22:58:11.000000 vector_vault-1.8.0/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-03 22:58:11.918722 vector_vault-1.8.0/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.0/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     7797 2023-06-03 22:42:23.000000 vector_vault-1.8.0/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3123 2023-06-03 22:57:44.000000 vector_vault-1.8.0/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.0/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.0/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1639 2023-06-03 22:57:48.000000 vector_vault-1.8.0/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.0/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    26201 2023-06-03 22:57:56.000000 vector_vault-1.8.0/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.0/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.0/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:47:20.278526 vector_vault-1.8.1/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.8.1/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:47:20.278283 vector_vault-1.8.1/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    19356 2023-05-31 07:01:35.000000 vector_vault-1.8.1/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-06-04 02:47:20.278562 vector_vault-1.8.1/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-06-04 02:47:11.000000 vector_vault-1.8.1/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:47:20.274669 vector_vault-1.8.1/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    20081 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      428 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-06-04 02:47:20.000000 vector_vault-1.8.1/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-06-04 02:47:20.277887 vector_vault-1.8.1/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      703 2023-05-30 23:38:32.000000 vector_vault-1.8.1/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    10751 2023-06-04 02:08:51.000000 vector_vault-1.8.1/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3120 2023-06-04 02:01:30.000000 vector_vault-1.8.1/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1858 2023-06-02 08:00:20.000000 vector_vault-1.8.1/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.8.1/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1638 2023-06-04 02:01:44.000000 vector_vault-1.8.1/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      912 2023-05-27 23:34:48.000000 vector_vault-1.8.1/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    26318 2023-06-04 02:30:10.000000 vector_vault-1.8.1/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3970 2023-05-31 06:48:55.000000 vector_vault-1.8.1/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.8.1/vectorvault/wrap.py
```

### Comparing `vector_vault-1.8.0/LICENSE` & `vector_vault-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/PKG-INFO` & `vector_vault-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.8.0
+Version: 1.8.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.0/README.md` & `vector_vault-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/setup.py` & `vector_vault-1.8.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.8.0",
+    version="1.8.1",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.8.0/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.8.1/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.8.0
+Version: 1.8.1
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
```

### Comparing `vector_vault-1.8.0/vectorvault/__init__.py` & `vector_vault-1.8.1/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/vectorvault/ai.py` & `vector_vault-1.8.1/vectorvault/ai.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import tiktoken
 
 class AI:
     def __init__(self) -> None:
         pass
 
     # This function returns a ChatGPT completion based on a provided input.
-    def llm(self, user_input, history=None, model='gpt-3.5-turbo', stream=False):
+    def llm(self, user_input, history=None, model='gpt-3.5-turbo'):
         inchar = len(user_input)
         histchar = len(history) if history else 0
         if inchar + histchar > 16000:
             char_left = 16000 - inchar
             if history:
                 history = history[-char_left:]
         if history:
@@ -35,38 +35,23 @@
                     {"role": "system", "content": f"{history}"},
                     {"role": "user", "content": f"{user_input}"}]
             )
         else:
             # 'model' is the name of the model to use
             # 'messages' is a list of message objects that mimics a conversation.
             # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
-            if stream == False:
-                response = openai.ChatCompletion.create(
-                    model=model,
-                    messages=[{"role": "user", "content": f"{user_input}"}]
-                )
-                return response['choices'][0]['message']['content']
-            elif stream == True:
-                response = openai.ChatCompletion.create(
-                    model=model,
-                    messages=[{"role": "user", "content": f"{user_input}"}],
-                    stream=True
-                )
-            # The API responds with a 'choices' array containing the 'message' object.
-                for message in response:
-                    choices = message.get('choices', [])
-                    if choices:
-                        delta = choices[0].get('delta', {})
-                        if 'content' in delta:
-                            content = delta['content']
-                            yield content
+            response = openai.ChatCompletion.create(
+                model=model,
+                messages=[{"role": "user", "content": f"{user_input}"}]
+            )
+            return response['choices'][0]['message']['content']
                         
                     
     # This function returns a ChatGPT completion based contextual input
-    def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo', stream=False):
+    def llm_w_context(self, user_input, context, history=None, model='gpt-3.5-turbo'):
         prompt_template = """
         Use the following Context to answer the Question at the end. 
         Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
 
         Our Conversation History (if any): {history}
 
         Additional Context: {context}
@@ -103,36 +88,115 @@
                     remainder = double_check - 4096
                     char_to_take_away = remainder * 5
                     context = context[char_to_take_away:]
 
         # Format the prompt
         user_input = history + user_input
         prompt = prompt_template.format(context=context, history=history, question=user_input)
-        if stream == False:
+        response = openai.ChatCompletion.create(
+            model=model,
+            messages=[
+                {"role": "user", "content": f"{prompt}"}],
+        )
+        return response['choices'][0]['message']['content']
+
+    # This function returns a ChatGPT completion based on a provided input.
+    def llm_stream(self, user_input, history=None, model='gpt-3.5-turbo'):
+        inchar = len(user_input)
+        histchar = len(history) if history else 0
+        if inchar + histchar > 16000:
+            char_left = 16000 - inchar
+            if history:
+                history = history[-char_left:]
+        if history:
             response = openai.ChatCompletion.create(
                 model=model,
                 messages=[
-                    {"role": "user", "content": f"{prompt}"}],
+                    {"role": "system", "content": f"{history}"},
+                    {"role": "user", "content": f"{user_input}"}]
             )
-            return response['choices'][0]['message']['content']
-        elif stream == True:
+        else:
+            # 'model' is the name of the model to use
+            # 'messages' is a list of message objects that mimics a conversation.
+            # Each object has a 'role' that can be 'system', 'user', or 'assistant', and a 'content' which is the actual content of the message.
             response = openai.ChatCompletion.create(
                 model=model,
-                messages=[
-                    {"role": "user", "content": f"{prompt}"}],
+                messages=[{"role": "user", "content": f"{user_input}"}],
                 stream=True
             )
         # The API responds with a 'choices' array containing the 'message' object.
             for message in response:
                 choices = message.get('choices', [])
                 if choices:
                     delta = choices[0].get('delta', {})
                     if 'content' in delta:
                         content = delta['content']
                         yield content
+                        
+                    
+    # This function returns a ChatGPT completion based contextual input
+    def llm_w_context_stream(self, user_input, context, history=None, model='gpt-3.5-turbo'):
+        prompt_template = """
+        Use the following Context to answer the Question at the end. 
+        Answer as if you were the modern voice of the context, without referencing the context or mentioning that fact any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
+
+        Our Conversation History (if any): {history}
+
+        Additional Context: {context}
+
+        Question: {question}
+
+        (Answer the question directly. Be the voice of the context, and most importantly: be interesting, engaging, and helpful) 
+        Answer:"""
+
+        intokes = self.get_tokens(user_input)
+        contokes = self.get_tokens(context)
+        history = history if history else ""
+        histokes = self.get_tokens(history)
+
+        if intokes + contokes + histokes > 4000:
+            tokes_left = 4000 - intokes
+            if len(history) > 1:
+                tokes_left = 2000 - intokes 
+                char_left = tokes_left * 4
+                history = history[-char_left:]
+                tokes_left_after_hist = 4000 - self.get_tokens(user_input + history)
+                char_left_after_hist = tokes_left_after_hist * 4
+                context = context[-char_left_after_hist:]
+                double_check = self.get_tokens(user_input+history+context)
+                if double_check > 4096: 
+                    remainder = double_check - 4096
+                    char_to_take_away = remainder * 5
+                    context = context[-char_to_take_away:] 
+            else:
+                char_left = tokes_left * 4 
+                context = context[-char_left:]
+                double_check = self.get_tokens(user_input + context)
+                if double_check > 4096:
+                    remainder = double_check - 4096
+                    char_to_take_away = remainder * 5
+                    context = context[char_to_take_away:]
+
+        # Format the prompt
+        user_input = history + user_input
+        prompt = prompt_template.format(context=context, history=history, question=user_input)
+        response = openai.ChatCompletion.create(
+            model=model,
+            messages=[
+                {"role": "user", "content": f"{prompt}"}],
+            stream=True
+        )
+    # The API responds with a 'choices' array containing the 'message' object.
+        for message in response:
+            choices = message.get('choices', [])
+            if choices:
+                delta = choices[0].get('delta', {})
+                if 'content' in delta:
+                    content = delta['content']
+                    yield content
 
 
     def summarize(self, user_input, model='gpt-3.5-turbo'):    
         response = openai.ChatCompletion.create(
             model=model,
             messages=[{"role": "user", "content": f"Summarize the following: {user_input}"}]
         )
```

### Comparing `vector_vault-1.8.0/vectorvault/cloudmanager.py` & `vector_vault-1.8.1/vectorvault/cloudmanager.py`

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

### Comparing `vector_vault-1.8.0/vectorvault/creds.py` & `vector_vault-1.8.1/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/vectorvault/download.py` & `vector_vault-1.8.1/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/vectorvault/itemize.py` & `vector_vault-1.8.1/vectorvault/itemize.py`

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

### Comparing `vector_vault-1.8.0/vectorvault/signup.py` & `vector_vault-1.8.1/vectorvault/signup.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/vectorvault/vault.py` & `vector_vault-1.8.1/vectorvault/vault.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 import numpy as np
 import tempfile
 import os
 import time
 import re
 import openai
 import json
+import traceback
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
@@ -68,16 +69,17 @@
         self.saved_already = True
         start_time = time.time()
         self.vectors.build(trees)
 
         total_saved_items = 0
 
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(self.cloud_manager.upload, *get_item(item)) for item in self.items}
-            for future in as_completed(futures):
+            for item in self.items:
+                item_text, item_id, item_meta = get_item(item)
+                executor.submit(self.cloud_manager.upload, item_id, item_text, item_meta)
                 total_saved_items += 1
 
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             self.vectors.save(temp_file.name)
             byte = os.path.getsize(temp_file.name)
             self.cloud_manager.upload_temp_file(temp_file.name, name_vecs(self.vault, self.user, self.api, byte))
 
@@ -419,14 +421,15 @@
                                 input_ += text['data']
                         response = self.ai.llm_w_context(segment, input_, history, model=model)
                     else:
                         response = self.ai.llm(segment, history, model=model)
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
+                    print(traceback.format_exc())
                     time.sleep(5)
                     
             self.last_chat_time = start_time
 
         if self.verbose == True:
             print("get chat time --- %s seconds ---" % (time.time() - start_time))
 
@@ -533,15 +536,15 @@
                         else:
                             context = self.get_similar(user_input, n=n_context)
                             input_ = ''
                         for text in context:
                             input_ += text['data']
 
                         if return_context: # send the ai stream, then the vault data
-                            for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
+                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, stream=True):
                                 yield word
                             for item in context:
                                 if type(metatag) is not list:
                                     for tag in item['metadata']:
                                         yield str(item['metadata'][f'{tag}'])
                                 else:
                                     if metatag_prefixes:
@@ -550,19 +553,19 @@
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
                             yield '!END'
                         else: # No context return and just send back the ai stream only 
-                            for word in self.ai.llm_w_context(segment, input_, history, model=model, stream=True):
+                            for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, stream=True):
                                 yield word
                             yield '!END'
                     else:
-                        for word in self.ai.llm(segment, history, model=model, stream=True):
+                        for word in self.ai.llm_stream(segment, history, model=model, stream=True):
                             yield word
                         yield '!END'
                     break
                 except Exception as e:
                     print(f"API Error: {e}. Sleeping 5 seconds")
                     time.sleep(5)
```

### Comparing `vector_vault-1.8.0/vectorvault/vecreq.py` & `vector_vault-1.8.1/vectorvault/vecreq.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.8.0/vectorvault/wrap.py` & `vector_vault-1.8.1/vectorvault/wrap.py`

 * *Files identical despite different names*

