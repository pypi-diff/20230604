# Comparing `tmp/openassist-2.2.3.tar.gz` & `tmp/openassist-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openassist-2.2.3.tar", max compression
+gzip compressed data, was "openassist-2.2.4.tar", max compression
```

## Comparing `openassist-2.2.3.tar` & `openassist-2.2.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1087 2023-06-04 14:20:56.512929 openassist-2.2.3/LICENSE
--rw-r--r--   0        0        0      474 2023-06-04 14:41:25.477096 openassist-2.2.3/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-04 14:40:15.813810 openassist-2.2.3/README.md
--rw-r--r--   0        0        0       55 2023-06-04 14:23:45.664873 openassist-2.2.3/src/openassist/__init__.py
--rw-r--r--   0        0        0    20110 2023-06-04 14:22:10.572141 openassist-2.2.3/src/openassist/openassist.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 openassist-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-04 14:20:56.512929 openassist-2.2.4/LICENSE
+-rw-r--r--   0        0        0      499 2023-06-04 14:51:20.631925 openassist-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-06-04 14:46:06.584862 openassist-2.2.4/README.md
+-rw-r--r--   0        0        0       55 2023-06-04 14:23:45.664873 openassist-2.2.4/src/openassist/__init__.py
+-rw-r--r--   0        0        0    20110 2023-06-04 14:22:10.572141 openassist-2.2.4/src/openassist/openassist.py
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 openassist-2.2.4/PKG-INFO
```

### Comparing `openassist-2.2.3/LICENSE` & `openassist-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openassist-2.2.3/src/openassist/openassist.py` & `openassist-2.2.4/src/openassist/openassist.py`

 * *Files identical despite different names*

### Comparing `openassist-2.2.3/PKG-INFO` & `openassist-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassist
-Version: 2.2.3
+Version: 2.2.4
 Summary: OpenAssist is a module for Python that allows you to create an AI assistant using import openai with ease.
 License: MIT
 Author: Free Zoloft
 Author-email: mybusinessemaildbb@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,7 +17,8 @@
 
 OpenAssist is a module for Python that allows you to create an AI assistant using openai with ease.
 
 ## Installation
 
 ```bash
 pip install openassist
+```
```

