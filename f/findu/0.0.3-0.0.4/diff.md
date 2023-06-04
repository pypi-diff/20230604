# Comparing `tmp/findu-0.0.3.tar.gz` & `tmp/findu-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.3.tar", max compression
+gzip compressed data, was "findu-0.0.4.tar", max compression
```

## Comparing `findu-0.0.3.tar` & `findu-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0       77 2023-06-03 08:56:53.544295 findu-0.0.3/findu/__init__.py
--rw-r--r--   0        0        0       39 2023-06-03 08:57:11.572937 findu-0.0.3/findu/findu.py
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.3/LICENSE
--rw-r--r--   0        0        0     1311 2023-06-03 08:57:18.180528 findu-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      609 2023-06-03 07:50:38.419853 findu-0.0.3/README.md
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 findu-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-06-04 10:57:31.573532 findu-0.0.4/findu/__init__.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.4/findu/findu.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.4/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.4/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.4/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1311 2023-06-04 10:57:39.037930 findu-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.4/README.md
+-rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 findu-0.0.4/PKG-INFO
```

### Comparing `findu-0.0.3/LICENSE` & `findu-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.3/pyproject.toml` & `findu-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.3"
+version = "0.0.4"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
```

### Comparing `findu-0.0.3/README.md` & `findu-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 ```
 $ pip install -U findu
 ```
 
 #### A Simple Example
 
-```python
-import findu
+```sh
+findu jack
 ```
 
 #### Links
 
 - Documentation: [https://github.com/MarkHoo/findu](https://github.com/MarkHoo/findu)
 - PyPI Releases: [https://pypi.org/project/findu/](https://pypi.org/project/findu/)
 - Source Code: [https://github.com/MarkHoo/findu](https://github.com/MarkHoo/findu)
```

### Comparing `findu-0.0.3/PKG-INFO` & `findu-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.3
+Version: 0.0.4
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -35,16 +35,16 @@
 
 ```
 $ pip install -U findu
 ```
 
 #### A Simple Example
 
-```python
-import findu
+```sh
+findu jack
 ```
 
 #### Links
 
 - Documentation: [https://github.com/MarkHoo/findu](https://github.com/MarkHoo/findu)
 - PyPI Releases: [https://pypi.org/project/findu/](https://pypi.org/project/findu/)
 - Source Code: [https://github.com/MarkHoo/findu](https://github.com/MarkHoo/findu)
```

