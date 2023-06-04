# Comparing `tmp/findu-0.0.4.tar.gz` & `tmp/findu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.4.tar", max compression
+gzip compressed data, was "findu-0.0.5.tar", max compression
```

## Comparing `findu-0.0.4.tar` & `findu-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       74 2023-06-04 10:57:31.573532 findu-0.0.4/findu/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.4/findu/findu.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.4/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.4/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.4/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.4/LICENSE
--rw-r--r--   0        0        0     1311 2023-06-04 10:57:39.037930 findu-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.4/README.md
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 findu-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-06-04 11:17:27.224382 findu-0.0.5/findu/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.5/findu/findu.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.5/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.5/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.5/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1329 2023-06-04 11:17:45.287165 findu-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.5/README.md
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 findu-0.0.5/PKG-INFO
```

### Comparing `findu-0.0.4/findu/findu.py` & `findu-0.0.5/findu/findu.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.4/LICENSE` & `findu-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.4/pyproject.toml` & `findu-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.4"
+version = "0.0.5"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
@@ -29,12 +29,13 @@
     { include = "findu" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MarkHoo/findu/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
+click = "^8.1.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findu-0.0.4/README.md` & `findu-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.4/PKG-INFO` & `findu-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.4
+Version: 0.0.5
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/MarkHoo/findu/issues
 Project-URL: Repository, https://github.com/MarkHoo/findu
 Description-Content-Type: text/markdown
 
 # findu
 
 #### Installing
```

