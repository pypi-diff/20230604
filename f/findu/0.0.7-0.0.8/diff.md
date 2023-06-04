# Comparing `tmp/findu-0.0.7.tar.gz` & `tmp/findu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.7.tar", max compression
+gzip compressed data, was "findu-0.0.8.tar", max compression
```

## Comparing `findu-0.0.7.tar` & `findu-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      112 2023-04-16 06:26:44.829145 findu-0.0.7/findu/__init__.py
--rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.7/findu/__main__.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.7/findu/findu.py
--rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.7/findu/notify.py
--rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.7/findu/resources/data.json
--rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.7/findu/result.py
--rw-r--r--   0        0        0    32714 2023-04-16 06:26:44.833138 findu-0.0.7/findu/sherlock.py
--rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.7/findu/sites.py
--rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.7/findu/tests/__init__.py
--rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.7/findu/tests/all.py
--rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.7/findu/tests/base.py
--rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.7/findu/tests/test_multiple_usernames.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.7/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.7/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.7/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.7/LICENSE
--rw-r--r--   0        0        0     1545 2023-06-04 13:01:15.153425 findu-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.7/README.md
--rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 findu-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-04-16 06:26:44.829145 findu-0.0.8/findu/__init__.py
+-rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.8/findu/__main__.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.8/findu/findu.py
+-rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.8/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.8/findu/resources/data.json
+-rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.8/findu/result.py
+-rw-r--r--   0        0        0    32714 2023-04-16 06:26:44.833138 findu-0.0.8/findu/sherlock.py
+-rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.8/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.8/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.8/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.8/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.8/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.8/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.8/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.8/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1545 2023-06-04 13:09:55.413439 findu-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.8/README.md
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 findu-0.0.8/PKG-INFO
```

### Comparing `findu-0.0.7/findu/__main__.py` & `findu-0.0.8/findu/__main__.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/findu.py` & `findu-0.0.8/findu/findu.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/notify.py` & `findu-0.0.8/findu/notify.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/resources/data.json` & `findu-0.0.8/findu/resources/data.json`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/result.py` & `findu-0.0.8/findu/result.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/sherlock.py` & `findu-0.0.8/findu/sherlock.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/sites.py` & `findu-0.0.8/findu/sites.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/tests/all.py` & `findu-0.0.8/findu/tests/all.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/tests/base.py` & `findu-0.0.8/findu/tests/base.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/findu/tests/test_multiple_usernames.py` & `findu-0.0.8/findu/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/LICENSE` & `findu-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/pyproject.toml` & `findu-0.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.7"
+version = "0.0.8"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
@@ -31,21 +31,21 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MarkHoo/findu/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
-certifi = "^2019.6.16"
+certifi = "^2022.12.7"
 colorama = "^0.4.1"
 PySocks = "^1.7.0"
-requests = "^2.22.0"
+requests = "^2.30.0"
 requests-futures = "^1.0.0"
 stem = "^1.8.0"
 torrequest = "^0.1.0"
-pandas = "^1.0.0"
+pandas = "^2.0.0"
 openpyxl = "^3.0.10"
 exrex = "^0.11.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `findu-0.0.7/README.md` & `findu-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.7/PKG-INFO` & `findu-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.7
+Version: 0.0.8
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -20,21 +20,21 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: PySocks (>=1.7.0,<2.0.0)
-Requires-Dist: certifi (>=2019.6.16,<2020.0.0)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.1,<0.5.0)
 Requires-Dist: exrex (>=0.11.0,<0.12.0)
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: pandas (>=1.0.0,<2.0.0)
-Requires-Dist: requests (>=2.22.0,<3.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: requests-futures (>=1.0.0,<2.0.0)
 Requires-Dist: stem (>=1.8.0,<2.0.0)
 Requires-Dist: torrequest (>=0.1.0,<0.2.0)
 Project-URL: Bug Tracker, https://github.com/MarkHoo/findu/issues
 Project-URL: Repository, https://github.com/MarkHoo/findu
 Description-Content-Type: text/markdown
```

