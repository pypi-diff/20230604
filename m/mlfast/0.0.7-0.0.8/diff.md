# Comparing `tmp/mlfast-0.0.7.tar.gz` & `tmp/mlfast-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfast-0.0.7.tar", last modified: Thu May 18 15:53:11 2023, max compression
+gzip compressed data, was "mlfast-0.0.8.tar", last modified: Sat Jun  3 22:16:07 2023, max compression
```

## Comparing `mlfast-0.0.7.tar` & `mlfast-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:11.747190 mlfast-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 15:51:53.000000 mlfast-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-18 15:53:11.747190 mlfast-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-18 15:51:53.000000 mlfast-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-18 15:51:53.000000 mlfast-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-18 15:53:11.747190 mlfast-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-18 15:51:53.000000 mlfast-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:11.739190 mlfast-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:11.743190 mlfast-0.0.7/src/mlfast/
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-05-18 15:51:53.000000 mlfast-0.0.7/src/mlfast/Classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-18 15:51:53.000000 mlfast-0.0.7/src/mlfast/Regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-18 15:51:53.000000 mlfast-0.0.7/src/mlfast/Text_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 15:51:53.000000 mlfast-0.0.7/src/mlfast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-18 15:51:53.000000 mlfast-0.0.7/src/mlfast/custom_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-18 15:51:53.000000 mlfast-0.0.7/src/mlfast/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:53:11.747190 mlfast-0.0.7/src/mlfast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-18 15:53:11.000000 mlfast-0.0.7/src/mlfast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-18 15:53:11.000000 mlfast-0.0.7/src/mlfast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:53:11.000000 mlfast-0.0.7/src/mlfast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-18 15:53:11.000000 mlfast-0.0.7/src/mlfast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 15:53:11.000000 mlfast-0.0.7/src/mlfast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:16:07.818027 mlfast-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-03 22:14:29.000000 mlfast-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-03 22:16:07.818027 mlfast-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-03 22:14:29.000000 mlfast-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 22:14:29.000000 mlfast-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-03 22:16:07.818027 mlfast-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-03 22:14:29.000000 mlfast-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:16:07.814027 mlfast-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:16:07.814027 mlfast-0.0.8/src/mlfast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/Chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/Classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/Regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/Text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/custom_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-03 22:14:29.000000 mlfast-0.0.8/src/mlfast/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:16:07.818027 mlfast-0.0.8/src/mlfast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-03 22:16:07.000000 mlfast-0.0.8/src/mlfast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-03 22:16:07.000000 mlfast-0.0.8/src/mlfast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:16:07.000000 mlfast-0.0.8/src/mlfast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 22:16:07.000000 mlfast-0.0.8/src/mlfast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-03 22:16:07.000000 mlfast-0.0.8/src/mlfast.egg-info/top_level.txt
```

### Comparing `mlfast-0.0.7/LICENSE` & `mlfast-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.7/PKG-INFO` & `mlfast-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfast
-Version: 0.0.7
+Version: 0.0.8
 Summary: its a python machine learning package
 Home-page: https://github.com/Abdul-Jaweed/mlfast
 Author: Abdul-Jaweed
 Author-email: jdgaming7320@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Abdul-Jaweed/mlfast/issues
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `mlfast-0.0.7/README.md` & `mlfast-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.7/setup.cfg` & `mlfast-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.7/setup.py` & `mlfast-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 REPO_NAME = "mlfast"
 AUTHOR_USER_NAME = "Abdul-Jaweed"
 SRC_REPO = "mlfast"
 AUTHOR_EMAIL = "jdgaming7320@gmail.com"
 
 setuptools.setup(
```

### Comparing `mlfast-0.0.7/src/mlfast/Classification.py` & `mlfast-0.0.8/src/mlfast/Classification.py`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.7/src/mlfast/Regression.py` & `mlfast-0.0.8/src/mlfast/Regression.py`

 * *Files identical despite different names*

### Comparing `mlfast-0.0.7/src/mlfast/Text_preprocessing.py` & `mlfast-0.0.8/src/mlfast/Text_preprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import nltk
 
 nltk.download("stopwords")
 from nltk.corpus import stopwords
 
 stopwords.words("english")
-nltk.download('punkt')
-nltk.download('wordnet')
+nltk.download("punkt")
+nltk.download("wordnet")
 from nltk.tokenize import word_tokenize
 from nltk.stem import PorterStemmer, WordNetLemmatizer
 import re
 
 
 def Text_preprocessing(
     text,
@@ -31,33 +31,31 @@
         url_pattern = re.compile(r"https?://\S+|www\.\S+")
         text = url_pattern.sub("", text)
 
     # # Removing emojis
     # if remove_emoji:
     #     text = emoji.demojize(text)
     #     text = re.sub(r":[a-zA-Z_]+:", "", text)
-        
-    
+
     # Removing emojis
     if remove_emoji:
-        emoji_pattern = re.compile("["
-                               u"\U0001F600-\U0001F64F"  # emoticons
-                               u"\U0001F300-\U0001F5FF"  # symbols & pictographs
-                               u"\U0001F680-\U0001F6FF"  # transport & map symbols
-                               u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
-                               u"\U00002702-\U000027B0"  # other miscellaneous symbols
-                               u"\U000024C2-\U0001F251" 
-                               "]+", flags=re.UNICODE)
+        emoji_pattern = re.compile(
+            "["
+            "\U0001F600-\U0001F64F"  # emoticons
+            "\U0001F300-\U0001F5FF"  # symbols & pictographs
+            "\U0001F680-\U0001F6FF"  # transport & map symbols
+            "\U0001F1E0-\U0001F1FF"  # flags (iOS)
+            "\U00002702-\U000027B0"  # other miscellaneous symbols
+            "\U000024C2-\U0001F251"
+            "]+",
+            flags=re.UNICODE,
+        )
     text = emoji_pattern.sub(r"", text)
     text = re.sub(r":[a-zA-Z_]+:", "", text)  # Remove emoji names within colons
     text = re.sub(r"\s+", " ", text)  # Remove extra spaces
-    
-    
-    
-    
 
     # Removing special characters
     if remove_special_chars:
         text = re.sub(r"[^a-zA-Z0-9\s]", "", text)
 
     # Removing extra spaces
     if remove_extra_spaces:
```

### Comparing `mlfast-0.0.7/src/mlfast.egg-info/PKG-INFO` & `mlfast-0.0.8/src/mlfast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfast
-Version: 0.0.7
+Version: 0.0.8
 Summary: its a python machine learning package
 Home-page: https://github.com/Abdul-Jaweed/mlfast
 Author: Abdul-Jaweed
 Author-email: jdgaming7320@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Abdul-Jaweed/mlfast/issues
 Classifier: Programming Language :: Python :: 3.7
```

