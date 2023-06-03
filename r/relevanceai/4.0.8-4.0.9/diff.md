# Comparing `tmp/relevanceai-4.0.8.tar.gz` & `tmp/relevanceai-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relevanceai-4.0.8.tar", last modified: Sat Jun  3 19:23:11 2023, max compression
+gzip compressed data, was "relevanceai-4.0.9.tar", last modified: Sat Jun  3 19:38:26 2023, max compression
```

## Comparing `relevanceai-4.0.8.tar` & `relevanceai-4.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:23:11.884739 relevanceai-4.0.8/
--rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.8/LICENSE
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 19:23:11.884574 relevanceai-4.0.8/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.8/README.md
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:23:11.882339 relevanceai-4.0.8/relevanceai/
--rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 19:22:21.000000 relevanceai-4.0.8/relevanceai/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.8/relevanceai/_request.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.8/relevanceai/auth.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 05:16:32.000000 relevanceai-4.0.8/relevanceai/chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.8/relevanceai/datasets.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.8/relevanceai/env.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.8/relevanceai/params.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:23:11.884374 relevanceai-4.0.8/relevanceai/steps/
--rw-r--r--   0 jackykoh   (502) staff       (20)      643 2023-06-03 19:22:25.000000 relevanceai-4.0.8/relevanceai/steps/__init__.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2669 2023-06-03 18:49:06.000000 relevanceai-4.0.8/relevanceai/steps/_base.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/api_call.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/execute_javascript.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/generate_vector_embedding.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      777 2023-06-03 19:13:42.000000 relevanceai-4.0.8/relevanceai/steps/get_webpage.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/prompt_completion.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/redis_vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.8/relevanceai/steps/run_chain.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2816 2023-06-03 18:56:08.000000 relevanceai-4.0.8/relevanceai/steps/run_step.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/vector_search.py
--rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.8/relevanceai/steps/vectorize_and_search.py
-drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:23:11.882991 relevanceai-4.0.8/relevanceai.egg-info/
--rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 19:23:11.000000 relevanceai-4.0.8/relevanceai.egg-info/PKG-INFO
--rw-r--r--   0 jackykoh   (502) staff       (20)      779 2023-06-03 19:23:11.000000 relevanceai-4.0.8/relevanceai.egg-info/SOURCES.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 19:23:11.000000 relevanceai-4.0.8/relevanceai.egg-info/dependency_links.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 19:23:11.000000 relevanceai-4.0.8/relevanceai.egg-info/requires.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 19:23:11.000000 relevanceai-4.0.8/relevanceai.egg-info/top_level.txt
--rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 19:23:11.884779 relevanceai-4.0.8/setup.cfg
--rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.8/setup.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:38:26.615889 relevanceai-4.0.9/
+-rw-r--r--   0 jackykoh   (502) staff       (20)    11547 2023-06-03 05:15:28.000000 relevanceai-4.0.9/LICENSE
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 19:38:26.615755 relevanceai-4.0.9/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      953 2023-06-03 07:08:05.000000 relevanceai-4.0.9/README.md
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:38:26.613646 relevanceai-4.0.9/relevanceai/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      272 2023-06-03 19:38:20.000000 relevanceai-4.0.9/relevanceai/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      112 2023-06-03 05:16:32.000000 relevanceai-4.0.9/relevanceai/_request.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2085 2023-06-03 05:16:32.000000 relevanceai-4.0.9/relevanceai/auth.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     6447 2023-06-03 19:37:23.000000 relevanceai-4.0.9/relevanceai/chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3288 2023-06-03 16:21:52.000000 relevanceai-4.0.9/relevanceai/datasets.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1010 2023-06-03 05:16:32.000000 relevanceai-4.0.9/relevanceai/env.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     4404 2023-06-03 05:16:32.000000 relevanceai-4.0.9/relevanceai/params.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:38:26.615594 relevanceai-4.0.9/relevanceai/steps/
+-rw-r--r--   0 jackykoh   (502) staff       (20)      643 2023-06-03 19:22:25.000000 relevanceai-4.0.9/relevanceai/steps/__init__.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2669 2023-06-03 18:49:06.000000 relevanceai-4.0.9/relevanceai/steps/_base.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1933 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/api_call.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1121 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/execute_javascript.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1246 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/generate_vector_embedding.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      777 2023-06-03 19:13:42.000000 relevanceai-4.0.9/relevanceai/steps/get_webpage.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     3676 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/prompt_completion.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1670 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/redis_vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)      985 2023-06-03 14:40:31.000000 relevanceai-4.0.9/relevanceai/steps/run_chain.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2816 2023-06-03 18:56:08.000000 relevanceai-4.0.9/relevanceai/steps/run_step.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     2059 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/vector_search.py
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1679 2023-06-03 06:58:35.000000 relevanceai-4.0.9/relevanceai/steps/vectorize_and_search.py
+drwxr-xr-x   0 jackykoh   (502) staff       (20)        0 2023-06-03 19:38:26.614181 relevanceai-4.0.9/relevanceai.egg-info/
+-rw-r--r--   0 jackykoh   (502) staff       (20)     1165 2023-06-03 19:38:26.000000 relevanceai-4.0.9/relevanceai.egg-info/PKG-INFO
+-rw-r--r--   0 jackykoh   (502) staff       (20)      779 2023-06-03 19:38:26.000000 relevanceai-4.0.9/relevanceai.egg-info/SOURCES.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        1 2023-06-03 19:38:26.000000 relevanceai-4.0.9/relevanceai.egg-info/dependency_links.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)        9 2023-06-03 19:38:26.000000 relevanceai-4.0.9/relevanceai.egg-info/requires.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       12 2023-06-03 19:38:26.000000 relevanceai-4.0.9/relevanceai.egg-info/top_level.txt
+-rw-r--r--   0 jackykoh   (502) staff       (20)       38 2023-06-03 19:38:26.615924 relevanceai-4.0.9/setup.cfg
+-rw-r--r--   0 jackykoh   (502) staff       (20)      551 2023-06-03 05:17:49.000000 relevanceai-4.0.9/setup.py
```

### Comparing `relevanceai-4.0.8/LICENSE` & `relevanceai-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/PKG-INFO` & `relevanceai-4.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.8
+Version: 4.0.9
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.8/README.md` & `relevanceai-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/auth.py` & `relevanceai-4.0.9/relevanceai/auth.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/chain.py` & `relevanceai-4.0.9/relevanceai/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 
     def _json(self):
         data = {
             "title": self.name,
             "description": self.description,
             "version": "latest",
             "project": self.auth.project,
-            "public": False,
+            "public": True,
             "params_schema": {"properties": self.parameters.to_json()},
             "transformations": {"steps": self._transform_steps(self.steps)},
         }
         data["studio_id"] = self.id
         return data
 
     def deploy(self):
@@ -164,15 +164,15 @@
             f"You can share/visualize your chain as an app in our low code notebook here: https://chain.relevanceai.com/notebook/{self.auth.region}/{self.auth.project}/{self.id}/app"
         )
         print("\n=============with Requests================")
         print("Here is an example of how to run the chain with API: ")
         print(
             f"""
 import requests
-requests.post(https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.id}/trigger_limited", json={{
+requests.post("https://api-{self.auth.region}.stack.tryrelevance.com/latest/studios/{self.id}/trigger_limited", json={{
     "project": "{self.auth.project}",
     "params": {{
         YOUR PARAMS HERE
     }}
 }})
             """
         )
```

### Comparing `relevanceai-4.0.8/relevanceai/datasets.py` & `relevanceai-4.0.9/relevanceai/datasets.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/env.py` & `relevanceai-4.0.9/relevanceai/env.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/params.py` & `relevanceai-4.0.9/relevanceai/params.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/__init__.py` & `relevanceai-4.0.9/relevanceai/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/_base.py` & `relevanceai-4.0.9/relevanceai/steps/_base.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/api_call.py` & `relevanceai-4.0.9/relevanceai/steps/api_call.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/execute_javascript.py` & `relevanceai-4.0.9/relevanceai/steps/execute_javascript.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/generate_vector_embedding.py` & `relevanceai-4.0.9/relevanceai/steps/generate_vector_embedding.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/get_webpage.py` & `relevanceai-4.0.9/relevanceai/steps/get_webpage.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/prompt_completion.py` & `relevanceai-4.0.9/relevanceai/steps/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/redis_vector_search.py` & `relevanceai-4.0.9/relevanceai/steps/redis_vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/run_chain.py` & `relevanceai-4.0.9/relevanceai/steps/run_chain.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/run_step.py` & `relevanceai-4.0.9/relevanceai/steps/run_step.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/vector_search.py` & `relevanceai-4.0.9/relevanceai/steps/vector_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai/steps/vectorize_and_search.py` & `relevanceai-4.0.9/relevanceai/steps/vectorize_and_search.py`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/relevanceai.egg-info/PKG-INFO` & `relevanceai-4.0.9/relevanceai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relevanceai
-Version: 4.0.8
+Version: 4.0.9
 Home-page: https://relevanceai.com/
 Author: Relevance AI
 Author-email: jacky@relevanceai.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Relevance AI - The platform for building and deploying AI chains and Agents
```

### Comparing `relevanceai-4.0.8/relevanceai.egg-info/SOURCES.txt` & `relevanceai-4.0.9/relevanceai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relevanceai-4.0.8/setup.py` & `relevanceai-4.0.9/setup.py`

 * *Files identical despite different names*

