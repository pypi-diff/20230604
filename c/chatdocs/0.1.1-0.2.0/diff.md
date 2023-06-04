# Comparing `tmp/chatdocs-0.1.1.tar.gz` & `tmp/chatdocs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatdocs-0.1.1.tar", last modified: Sat Jun  3 12:54:50 2023, max compression
+gzip compressed data, was "chatdocs-0.2.0.tar", last modified: Sun Jun  4 09:41:07 2023, max compression
```

## Comparing `chatdocs-0.1.1.tar` & `chatdocs-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-03 12:54:50.515591 chatdocs-0.1.1/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-03 12:54:50.515591 chatdocs-0.1.1/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2279 2023-06-02 20:59:47.000000 chatdocs-0.1.1/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-03 12:54:50.515591 chatdocs-0.1.1/chatdocs/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.1.1/chatdocs/__init__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.1.1/chatdocs/__main__.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     6201 2023-06-02 17:41:03.000000 chatdocs-0.1.1/chatdocs/add.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3142 2023-06-03 11:09:24.000000 chatdocs-0.1.1/chatdocs/chat.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      178 2023-06-02 17:43:46.000000 chatdocs-0.1.1/chatdocs/config.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      290 2023-06-02 20:37:18.000000 chatdocs-0.1.1/chatdocs/download.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2454 2023-06-02 11:45:11.000000 chatdocs-0.1.1/chatdocs/main.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-03 12:54:50.515591 chatdocs-0.1.1/chatdocs.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3994 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      375 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/entry_points.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      313 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-03 12:54:50.000000 chatdocs-0.1.1/chatdocs.egg-info/top_level.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-03 12:54:50.515591 chatdocs-0.1.1/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1979 2023-06-03 12:51:50.000000 chatdocs-0.1.1/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7086 2023-06-04 09:41:07.061561 chatdocs-0.2.0/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     4651 2023-06-04 09:35:47.000000 chatdocs-0.2.0/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/chatdocs/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        0 2023-06-01 18:46:12.000000 chatdocs-0.2.0/chatdocs/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       29 2023-06-01 19:38:54.000000 chatdocs-0.2.0/chatdocs/__main__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5657 2023-06-04 03:56:33.000000 chatdocs-0.2.0/chatdocs/add.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      447 2023-06-04 05:02:07.000000 chatdocs-0.2.0/chatdocs/chains.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1284 2023-06-04 05:03:43.000000 chatdocs-0.2.0/chatdocs/chat.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      665 2023-06-04 04:02:06.000000 chatdocs-0.2.0/chatdocs/config.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/chatdocs/data/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      444 2023-06-04 08:12:22.000000 chatdocs-0.2.0/chatdocs/data/chatdocs.yml
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      232 2023-06-04 02:56:51.000000 chatdocs-0.2.0/chatdocs/download.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      491 2023-06-04 01:27:28.000000 chatdocs-0.2.0/chatdocs/embeddings.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1046 2023-06-04 01:41:19.000000 chatdocs-0.2.0/chatdocs/llms.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1129 2023-06-04 06:27:56.000000 chatdocs-0.2.0/chatdocs/main.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      368 2023-06-04 01:08:37.000000 chatdocs-0.2.0/chatdocs/utils.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      914 2023-06-04 03:51:59.000000 chatdocs-0.2.0/chatdocs/vectorstores.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-06-04 09:41:07.061561 chatdocs-0.2.0/chatdocs.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     7086 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      504 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       48 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/entry_points.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      391 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-06-04 09:41:07.000000 chatdocs-0.2.0/chatdocs.egg-info/top_level.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-06-04 09:41:07.061561 chatdocs-0.2.0/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2127 2023-06-04 09:40:27.000000 chatdocs-0.2.0/setup.py
```

### Comparing `chatdocs-0.1.1/chatdocs/add.py` & `chatdocs-0.2.0/chatdocs/add.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import glob
-from typing import List
+from typing import Any, Dict, List
 from multiprocessing import Pool
 
 from tqdm import tqdm
 from langchain.document_loaders import (
     CSVLoader,
     EverNoteLoader,
     PDFMinerLoader,
@@ -14,20 +14,17 @@
     UnstructuredHTMLLoader,
     UnstructuredMarkdownLoader,
     UnstructuredODTLoader,
     UnstructuredPowerPointLoader,
     UnstructuredWordDocumentLoader,
 )
 from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain.vectorstores import Chroma
-from langchain.embeddings import HuggingFaceInstructEmbeddings
 from langchain.docstore.document import Document
-from chromadb.config import Settings
 
-from . import config
+from .vectorstores import get_vectorstore, get_vectorstore_from_documents
 
 
 # Custom document loaders
 class MyElmLoader(UnstructuredEmailLoader):
     """Wrapper to fallback to text/plain when default does not work"""
 
     def load(self) -> List[Document]:
@@ -139,44 +136,28 @@
             )
             # At least 3 documents are needed in a working vectorstore
             if len(list_index_files) > 3:
                 return True
     return False
 
 
-def add(source_directory: str, persist_directory: str) -> None:
-    # Create embeddings
-    embeddings = HuggingFaceInstructEmbeddings(model_name=config.EMBEDDINGS_MODEL)
-    chroma_settings = Settings(
-        chroma_db_impl=config.CHROMA_DB_IMPL,
-        persist_directory=persist_directory,
-        anonymized_telemetry=False,
-    )
-
+def add(config: Dict[str, Any], source_directory: str) -> None:
+    persist_directory = config["chroma"]["persist_directory"]
     if does_vectorstore_exist(persist_directory):
         # Update and store locally vectorstore
         print(f"Appending to existing vectorstore at {persist_directory}")
-        db = Chroma(
-            persist_directory=persist_directory,
-            embedding_function=embeddings,
-            client_settings=chroma_settings,
-        )
+        db = get_vectorstore(config)
         collection = db.get()
         texts = process_documents(
             source_directory,
             [metadata["source"] for metadata in collection["metadatas"]],
         )
         print(f"Creating embeddings. May take a few minutes...")
         db.add_documents(texts)
     else:
         # Create and store locally vectorstore
         print("Creating new vectorstore")
         texts = process_documents(source_directory)
         print(f"Creating embeddings. May take a few minutes...")
-        db = Chroma.from_documents(
-            texts,
-            embeddings,
-            persist_directory=persist_directory,
-            client_settings=chroma_settings,
-        )
+        db = get_vectorstore_from_documents(config, texts)
     db.persist()
     db = None
```

### Comparing `chatdocs-0.1.1/setup.py` & `chatdocs-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,41 +3,44 @@
 with open("README.md") as f:
     long_description = f.read()
 
 name = "chatdocs"
 
 setup(
     name=name,
-    version="0.1.1",
+    version="0.2.0",
     description="Chat with your documents offline using AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ravindra Marella",
     author_email="mv.ravindra007@gmail.com",
     url="https://github.com/marella/{}".format(name),
     license="MIT",
     packages=[name],
+    package_data={name: ["data/chatdocs.yml"]},
     entry_points={
         "console_scripts": [
             f"{name} = {name}.main:app",
         ],
     },
     install_requires=[
         "chromadb>=0.3.0,<0.4.0",
         "ctransformers>=0.2.5,<0.3.0",
-        "InstructorEmbedding>=1.0.1",
+        "deepmerge>=1.1.0,<2.0.0",
+        "InstructorEmbedding>=1.0.1,<2.0.0",
         "langchain>=0.0.181",
-        "sentence-transformers>=2.2.2",
-        "tqdm>=4.64.1",
+        "pyyaml>=6.0",
+        "sentence-transformers>=2.2.2,<3.0.0",
+        "tqdm>=4.64.1,<5.0.0",
         "typer>=0.9.0",
-        "typing-extensions>=4.4.0",
+        "typing-extensions>=4.4.0,<5.0.0",
         # Document Loaders
         "extract-msg>=0.41.0,<0.42.0",
-        "pandoc==2.3",
-        "pypandoc==1.11",
+        "pandoc>=2.3,<3.0.0",
+        "pypandoc>=1.11,<2.0.0",
         "pdfminer.six==20221105",
         "unstructured>=0.6.0,<0.7.0",
         # Temporary fix for `rich`, `numpy` version conflicts.
         "argilla==1.8.0",
     ],
     extras_require={
         "tests": [
```

