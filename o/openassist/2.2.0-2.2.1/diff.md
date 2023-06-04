# Comparing `tmp/openassist-2.2.0.tar.gz` & `tmp/openassist-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openassist-2.2.0.tar", max compression
+gzip compressed data, was "openassist-2.2.1.tar", max compression
```

## Comparing `openassist-2.2.0.tar` & `openassist-2.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1087 2023-06-04 14:20:56.512929 openassist-2.2.0/LICENSE
--rw-r--r--   0        0        0      474 2023-06-04 14:25:06.816406 openassist-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      169 2023-06-04 14:18:32.984583 openassist-2.2.0/README.md
--rw-r--r--   0        0        0       55 2023-06-04 14:23:45.664873 openassist-2.2.0/src/openassist/__init__.py
--rw-r--r--   0        0        0    20110 2023-06-04 14:22:10.572141 openassist-2.2.0/src/openassist/openassist.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 openassist-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-06-04 14:20:56.512929 openassist-2.2.1/LICENSE
+-rw-r--r--   0        0        0      474 2023-06-04 14:35:33.977102 openassist-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      169 2023-06-04 14:18:32.984583 openassist-2.2.1/README.md
+-rw-r--r--   0        0        0       55 2023-06-04 14:23:45.664873 openassist-2.2.1/src/openassist/__init__.py
+-rw-r--r--   0        0        0    20110 2023-06-04 14:22:10.572141 openassist-2.2.1/src/openassist/openassist.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 openassist-2.2.1/PKG-INFO
```

### Comparing `openassist-2.2.0/LICENSE` & `openassist-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openassist-2.2.0/src/openassist/openassist.py` & `openassist-2.2.1/src/openassist/openassist.py`

 * *Files identical despite different names*

### Comparing `openassist-2.2.0/PKG-INFO` & `openassist-2.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openassist
-Version: 2.2.0
+Version: 2.2.1
 Summary: OpenAssist is a module for Python that allows you to create an AI assistant using import openai with ease.
 License: MIT
 Author: Free Zoloft
 Author-email: mybusinessemaildbb@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

