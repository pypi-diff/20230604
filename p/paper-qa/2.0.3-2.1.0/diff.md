# Comparing `tmp/paper-qa-2.0.3.tar.gz` & `tmp/paper-qa-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-2.0.3.tar", last modified: Fri Jun  2 20:24:12 2023, max compression
+gzip compressed data, was "paper-qa-2.1.0.tar", last modified: Sun Jun  4 01:29:31 2023, max compression
```

## Comparing `paper-qa-2.0.3.tar` & `paper-qa-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 20:23:34.000000 paper-qa-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-02 20:24:12.469730 paper-qa-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-06-02 20:23:34.000000 paper-qa-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.465730 paper-qa-2.0.3/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 20:24:12.000000 paper-qa-2.0.3/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 20:23:34.000000 paper-qa-2.0.3/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:24:12.469730 paper-qa-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-02 20:23:34.000000 paper-qa-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:24:12.469730 paper-qa-2.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-06-02 20:23:34.000000 paper-qa-2.0.3/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.464349 paper-qa-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 01:28:55.000000 paper-qa-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-04 01:29:31.464349 paper-qa-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-06-04 01:28:55.000000 paper-qa-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.460349 paper-qa-2.1.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-04 01:29:31.000000 paper-qa-2.1.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.460349 paper-qa-2.1.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.464349 paper-qa-2.1.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22971 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 01:28:55.000000 paper-qa-2.1.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 01:29:31.464349 paper-qa-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-04 01:28:55.000000 paper-qa-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:29:31.464349 paper-qa-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-06-04 01:28:55.000000 paper-qa-2.1.0/tests/test_paperqa.py
```

### Comparing `paper-qa-2.0.3/LICENSE` & `paper-qa-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/PKG-INFO` & `paper-qa-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.0.3
+Version: 2.1.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.0.3/README.md` & `paper-qa-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/paper_qa.egg-info/PKG-INFO` & `paper-qa-2.1.0/paper_qa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.0.3
+Version: 2.1.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.0.3/paperqa/agent.py` & `paper-qa-2.1.0/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/paperqa/contrib/zotero.py` & `paper-qa-2.1.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/paperqa/docs.py` & `paper-qa-2.1.0/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
         """Add chunked texts to the collection. This is useful if you have already chunked the texts yourself.
 
         The metadatas should have the following keys: citation, dockey (same as key arg), and key (unique key for each chunk).
         The hash is a unique identifier for the document. It is used to check if the document has already been added.
         """
         if len(texts) != len(metadatas):
             raise ValueError("texts and metadatas must have the same length.")
+
+        if hash in [d["hash"] for d in self.docs]:
+            raise ValueError(f"Document already in collection.")
+
         key = metadatas[0]["dockey"]
         citation = metadatas[0]["citation"]
         if key in self.keys:
             new_key = self.get_unique_key(key)
             for metadata in metadatas:
                 metadata["dockey"] = new_key
                 metadata["key"] = metadata["key"].replace(key, new_key)
@@ -422,14 +426,15 @@
                 raise e
             c = Context(
                 key=doc.metadata["key"],
                 citation=doc.metadata["citation"],
                 context=context,
                 text=doc.page_content,
                 score=get_score(context),
+                dockey=doc.metadata["dockey"],
             )
             if "not applicable" not in c.context.casefold():
                 return c, callbacks[0]
             return None, None
 
         results = await gather_with_concurrency(
             self.max_concurrent, *[process(doc) for doc in docs]
```

### Comparing `paper-qa-2.0.3/paperqa/qaprompts.py` & `paper-qa-2.1.0/paperqa/qaprompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/paperqa/readers.py` & `paper-qa-2.1.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/paperqa/types.py` & `paper-qa-2.1.0/paperqa/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,32 +9,33 @@
 class Context:
     """A class to hold the context of a question."""
 
     key: str
     citation: str
     context: str
     text: str
+    dockey: str
     score: int = 5
 
     def __str__(self) -> str:
         """Return the context as a string."""
         return self.context
 
 
 @dataclass
 class Answer:
     """A class to hold the answer to a question."""
 
     question: str
     answer: str = ""
     context: str = ""
-    contexts: List[Context] = None
+    contexts: Optional[List[Context]] = None
     references: str = ""
     formatted_answer: str = ""
-    passages: Dict[str, str] = None
+    passages: Optional[Dict[str, str]] = None
     tokens: int = 0
     cost: float = 0
     key_filter: Optional[str] = None
 
     def __post_init__(self):
         """Initialize the answer."""
         if self.contexts is None:
```

### Comparing `paper-qa-2.0.3/paperqa/utils.py` & `paper-qa-2.1.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/setup.py` & `paper-qa-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.3/tests/test_paperqa.py` & `paper-qa-2.1.0/tests/test_paperqa.py`

 * *Files identical despite different names*

