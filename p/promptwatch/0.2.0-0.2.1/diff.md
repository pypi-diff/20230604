# Comparing `tmp/promptwatch-0.2.0.tar.gz` & `tmp/promptwatch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.0.tar", last modified: Wed May 31 21:52:59 2023, max compression
+gzip compressed data, was "promptwatch-0.2.1.tar", last modified: Sun Jun  4 13:25:55 2023, max compression
```

## Comparing `promptwatch-0.2.0.tar` & `promptwatch-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.873867 promptwatch-0.2.0/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-31 21:52:59.873675 promptwatch-0.2.0/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.0/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.0/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-31 21:52:59.873924 promptwatch-0.2.0/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.0/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.863236 promptwatch-0.2.0/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.866986 promptwatch-0.2.0/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-05-31 21:34:10.000000 promptwatch-0.2.0/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.0/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.0/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5459 2023-05-30 20:36:31.000000 promptwatch-0.2.0/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.0/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.870533 promptwatch-0.2.0/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.0/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.0/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    29625 2023-05-31 09:25:01.000000 promptwatch-0.2.0/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-05-31 18:53:06.000000 promptwatch-0.2.0/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.872453 promptwatch-0.2.0/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.0/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.0/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-31 21:52:59.869110 promptwatch-0.2.0/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.0/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-31 21:52:59.000000 promptwatch-0.2.0/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.370855 promptwatch-0.2.1/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-04 13:25:55.370697 promptwatch-0.2.1/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.1/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.1/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-06-04 13:25:55.370897 promptwatch-0.2.1/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.1/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.363488 promptwatch-0.2.1/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.366706 promptwatch-0.2.1/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-06-04 13:23:24.000000 promptwatch-0.2.1/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.1/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.1/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5459 2023-05-30 20:36:31.000000 promptwatch-0.2.1/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.1/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.369254 promptwatch-0.2.1/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.1/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.1/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    29649 2023-06-04 13:06:19.000000 promptwatch-0.2.1/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    17902 2023-05-31 18:53:06.000000 promptwatch-0.2.1/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.370332 promptwatch-0.2.1/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.1/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1105 2023-05-24 13:30:08.000000 promptwatch-0.2.1/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-06-04 13:25:55.367854 promptwatch-0.2.1/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.1/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-06-04 13:25:55.000000 promptwatch-0.2.1/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.0/PKG-INFO` & `promptwatch-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.0
+Version: 0.2.1
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.0/README.md` & `promptwatch-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/setup.py` & `promptwatch-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/caching.py` & `promptwatch-0.2.1/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/client.py` & `promptwatch-0.2.1/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/data_model.py` & `promptwatch-0.2.1/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/decorators.py` & `promptwatch-0.2.1/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.1/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.1/src/promptwatch/langchain/langchain_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
 
     Yields:
         Tuple(): _description_
     """
 
     is_tool=isinstance(root_chain,BaseTool) 
     for field_key, field_value in root_chain.__dict__.items():
-        if field_value is None or field_value in _ignore_chains:
+        if field_value is None or any(field_value is value for value in _ignore_chains):
             continue
         if is_tool and isinstance(field_value, types.MethodType):
             # tools have a "func" field that is bound to the tool it self
             if field_value.__self__ in _ignore_chains:
                 continue
 
             _ignore_chains.append(field_value.__self__)
```

### Comparing `promptwatch-0.2.0/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.1/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.1/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.1/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.1/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.1/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch/utils.py` & `promptwatch-0.2.1/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.0/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.1/src/promptwatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.0
+Version: 0.2.1
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.0/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.1/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

