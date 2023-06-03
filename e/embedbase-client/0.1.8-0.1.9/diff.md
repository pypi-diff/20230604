# Comparing `tmp/embedbase_client-0.1.8.tar.gz` & `tmp/embedbase_client-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_client-0.1.8.tar", max compression
+gzip compressed data, was "embedbase_client-0.1.9.tar", max compression
```

## Comparing `embedbase_client-0.1.8.tar` & `embedbase_client-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1077 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/LICENSE
--rw-r--r--   0        0        0     1005 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/README.md
--rw-r--r--   0        0        0      389 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/__init__.py
--rw-r--r--   0        0        0    19402 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/async_client.py
--rw-r--r--   0        0        0      913 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/base.py
--rw-r--r--   0        0        0     1150 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/errors.py
--rw-r--r--   0        0        0     1645 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/model.py
--rw-r--r--   0        0        0     3388 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/split.py
--rw-r--r--   0        0        0    19336 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/sync_client.py
--rw-r--r--   0        0        0     2051 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/embedbase_client/utils.py
--rw-r--r--   0        0        0     3535 2023-05-30 06:18:37.370885 embedbase_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1005 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/README.md
+-rw-r--r--   0        0        0      389 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/__init__.py
+-rw-r--r--   0        0        0    19420 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/async_client.py
+-rw-r--r--   0        0        0      913 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/base.py
+-rw-r--r--   0        0        0     1150 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/errors.py
+-rw-r--r--   0        0        0     1645 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/model.py
+-rw-r--r--   0        0        0     3388 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/split.py
+-rw-r--r--   0        0        0    19348 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/sync_client.py
+-rw-r--r--   0        0        0     2051 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/embedbase_client/utils.py
+-rw-r--r--   0        0        0     3535 2023-06-03 22:33:12.754612 embedbase_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 embedbase_client-0.1.9/PKG-INFO
```

### Comparing `embedbase_client-0.1.8/LICENSE` & `embedbase_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/README.md` & `embedbase_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/embedbase_client/async_client.py` & `embedbase_client-0.1.9/embedbase_client/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,24 +520,24 @@
             A list of documents.
 
         Example usage:
             documents = [
                 {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
                 {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
             ]
-            results = await embedbase.batch_add("my_dataset", documents)
+            results = await embedbase.chunk_and_batch_add("my_dataset", documents)
         """
         chunks = []
         for document_index, document in enumerate(documents):
             for chunk_index, chunk in enumerate(split_text(document["data"])):
                 chunks.append(
                     {
                         "data": chunk.chunk,
                         "metadata": {
-                            **document["metadata"],
+                            **document.get("metadata", {}),
                             "documentIndex": document_index,
                             "chunkIndex": chunk_index,
                             "chunkStart": chunk.start,
                             "chunkEnd": chunk.end,
                         },
                     }
                 )
```

### Comparing `embedbase_client-0.1.8/embedbase_client/base.py` & `embedbase_client-0.1.9/embedbase_client/base.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/embedbase_client/errors.py` & `embedbase_client-0.1.9/embedbase_client/errors.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/embedbase_client/model.py` & `embedbase_client-0.1.9/embedbase_client/model.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/embedbase_client/split.py` & `embedbase_client-0.1.9/embedbase_client/split.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/embedbase_client/sync_client.py` & `embedbase_client-0.1.9/embedbase_client/sync_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,24 +540,24 @@
             A list of documents.
 
         Example usage:
             documents = [
                 {"data": "Python is a programming language.", metadata: {"topic": "programming"}},
                 {"data": "Java is also a programming language.", metadata: {"topic": "programming"}},
             ]
-            results = await embedbase.batch_add("my_dataset", documents)
+            results = embedbase.chunk_and_batch_add("my_dataset", documents)
         """
         chunks = []
         for document_index, document in enumerate(documents):
             for chunk_index, chunk in enumerate(split_text(document["data"])):
                 chunks.append(
                     {
                         "data": chunk.chunk,
                         "metadata": {
-                            **document["metadata"],
+                            **document.get("metadata", {}),
                             "documentIndex": document_index,
                             "chunkIndex": chunk_index,
                             "chunkStart": chunk.start,
                             "chunkEnd": chunk.end,
                         },
                     }
                 )
```

### Comparing `embedbase_client-0.1.8/embedbase_client/utils.py` & `embedbase_client-0.1.9/embedbase_client/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase_client-0.1.8/pyproject.toml` & `embedbase_client-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase-client"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python client for Embedbase"
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
 homepage = "https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py"
```

### Comparing `embedbase_client-0.1.8/PKG-INFO` & `embedbase_client-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for Embedbase
 Home-page: https://github.com/different-ai/embedbase/tree/main/sdk/embedbase-py
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.8 Summary: Python
+Metadata-Version: 2.1 Name: embedbase-client Version: 0.1.9 Summary: Python
 client for Embedbase Home-page: https://github.com/different-ai/embedbase/tree/
 main/sdk/embedbase-py License: MIT Keywords: embeddings,machine
 learning,artificial intelligence,llm Author: Different AI Author-email:
 louis@embedbase.xyz Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

