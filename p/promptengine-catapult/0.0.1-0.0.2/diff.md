# Comparing `tmp/promptengine_catapult-0.0.1.tar.gz` & `tmp/promptengine_catapult-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptengine_catapult-0.0.1.tar", last modified: Sun Jun  4 17:50:39 2023, max compression
+gzip compressed data, was "promptengine_catapult-0.0.2.tar", last modified: Sun Jun  4 18:17:50 2023, max compression
```

## Comparing `promptengine_catapult-0.0.1.tar` & `promptengine_catapult-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 17:50:39.942448 promptengine_catapult-0.0.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.1/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-04 17:50:39.942448 promptengine_catapult-0.0.1/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.1/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 17:50:39.942448 promptengine_catapult-0.0.1/promptengine_catapult/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 13:44:01.000000 promptengine_catapult-0.0.1/promptengine_catapult/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.1/promptengine_catapult/config.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5735 2023-06-04 17:27:58.000000 promptengine_catapult-0.0.1/promptengine_catapult/prompt_engine.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      789 2023-06-04 13:28:26.000000 promptengine_catapult-0.0.1/promptengine_catapult/utils.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 17:50:39.942448 promptengine_catapult-0.0.1/promptengine_catapult.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-04 17:50:39.000000 promptengine_catapult-0.0.1/promptengine_catapult.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-04 17:50:39.000000 promptengine_catapult-0.0.1/promptengine_catapult.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-04 17:50:39.000000 promptengine_catapult-0.0.1/promptengine_catapult.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       51 2023-06-04 17:50:39.000000 promptengine_catapult-0.0.1/promptengine_catapult.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-04 17:50:39.000000 promptengine_catapult-0.0.1/promptengine_catapult.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-04 17:50:39.942448 promptengine_catapult-0.0.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1447 2023-06-04 17:45:57.000000 promptengine_catapult-0.0.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 18:17:50.953016 promptengine_catapult-0.0.2/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2023-06-03 16:31:18.000000 promptengine_catapult-0.0.2/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-04 18:17:50.953016 promptengine_catapult-0.0.2/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2141 2023-06-04 13:35:51.000000 promptengine_catapult-0.0.2/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 18:17:50.953016 promptengine_catapult-0.0.2/promptengine_catapult/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       40 2023-06-04 18:14:53.000000 promptengine_catapult-0.0.2/promptengine_catapult/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2312 2023-06-03 18:34:00.000000 promptengine_catapult-0.0.2/promptengine_catapult/config.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     5735 2023-06-04 17:27:58.000000 promptengine_catapult-0.0.2/promptengine_catapult/prompt_engine.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      789 2023-06-04 13:28:26.000000 promptengine_catapult-0.0.2/promptengine_catapult/utils.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-06-04 18:17:50.953016 promptengine_catapult-0.0.2/promptengine_catapult.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2751 2023-06-04 18:17:50.000000 promptengine_catapult-0.0.2/promptengine_catapult.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      386 2023-06-04 18:17:50.000000 promptengine_catapult-0.0.2/promptengine_catapult.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-06-04 18:17:50.000000 promptengine_catapult-0.0.2/promptengine_catapult.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       51 2023-06-04 18:17:50.000000 promptengine_catapult-0.0.2/promptengine_catapult.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       22 2023-06-04 18:17:50.000000 promptengine_catapult-0.0.2/promptengine_catapult.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-06-04 18:17:50.953016 promptengine_catapult-0.0.2/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1447 2023-06-04 18:17:29.000000 promptengine_catapult-0.0.2/setup.py
```

### Comparing `promptengine_catapult-0.0.1/LICENSE` & `promptengine_catapult-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.1/PKG-INFO` & `promptengine_catapult-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine_catapult
-Version: 0.0.1
+Version: 0.0.2
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.1/README.md` & `promptengine_catapult-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.1/promptengine_catapult/config.py` & `promptengine_catapult-0.0.2/promptengine_catapult/config.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.1/promptengine_catapult/prompt_engine.py` & `promptengine_catapult-0.0.2/promptengine_catapult/prompt_engine.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.1/promptengine_catapult/utils.py` & `promptengine_catapult-0.0.2/promptengine_catapult/utils.py`

 * *Files identical despite different names*

### Comparing `promptengine_catapult-0.0.1/promptengine_catapult.egg-info/PKG-INFO` & `promptengine_catapult-0.0.2/promptengine_catapult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptengine-catapult
-Version: 0.0.1
+Version: 0.0.2
 Summary: PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model.
 Author: Bharat Bodkhe
 Author-email: akybharat02@gmail.com
 Keywords: python,interview,chatbot,AI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `promptengine_catapult-0.0.1/setup.py` & `promptengine_catapult-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "PromptEngine is a Python library for conducting interview sessions using OpenAI's ChatGPT model."
 LONG_DESCRIPTION = """
 PromptEngine is a Python library that provides an interface for conducting interview sessions using OpenAI's ChatGPT model. It allows you to interact with the AI assistant to simulate interview conversations and generate responses based on candidate input.
 """
 
 # Setting up
 setup(
```

