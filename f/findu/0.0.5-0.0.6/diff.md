# Comparing `tmp/findu-0.0.5.tar.gz` & `tmp/findu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findu-0.0.5.tar", max compression
+gzip compressed data, was "findu-0.0.6.tar", max compression
```

## Comparing `findu-0.0.5.tar` & `findu-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,19 @@
--rw-r--r--   0        0        0       74 2023-06-04 11:17:27.224382 findu-0.0.5/findu/__init__.py
--rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.5/findu/findu.py
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.5/findu/translations/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.5/findu/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.5/findu/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.5/LICENSE
--rw-r--r--   0        0        0     1329 2023-06-04 11:17:45.287165 findu-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.5/README.md
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 findu-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      112 2023-04-16 06:26:44.829145 findu-0.0.6/findu/__init__.py
+-rw-r--r--   0        0        0      562 2023-04-16 06:26:44.829145 findu-0.0.6/findu/__main__.py
+-rw-r--r--   0        0        0     1729 2023-06-04 10:55:09.603956 findu-0.0.6/findu/findu.py
+-rw-r--r--   0        0        0     8894 2023-04-16 06:26:44.830142 findu-0.0.6/findu/notify.py
+-rw-r--r--   0        0        0    89825 2023-04-16 06:36:03.209430 findu-0.0.6/findu/resources/data.json
+-rw-r--r--   0        0        0     3201 2023-04-16 06:26:44.832137 findu-0.0.6/findu/result.py
+-rw-r--r--   0        0        0    32714 2023-04-16 06:26:44.833138 findu-0.0.6/findu/sherlock.py
+-rw-r--r--   0        0        0     9242 2023-04-16 06:26:44.834132 findu-0.0.6/findu/sites.py
+-rw-r--r--   0        0        0       87 2023-04-16 06:26:44.835128 findu-0.0.6/findu/tests/__init__.py
+-rw-r--r--   0        0        0     7377 2023-04-16 06:26:44.836134 findu-0.0.6/findu/tests/all.py
+-rw-r--r--   0        0        0     8812 2023-04-16 06:26:44.836134 findu-0.0.6/findu/tests/base.py
+-rw-r--r--   0        0        0      948 2023-04-16 06:26:44.837124 findu-0.0.6/findu/tests/test_multiple_usernames.py
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575262 findu-0.0.6/findu/translations/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.6/findu/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0       52 2023-06-04 08:36:11.575000 findu-0.0.6/findu/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 findu-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1329 2023-06-04 12:52:44.189396 findu-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      603 2023-06-04 11:00:56.443625 findu-0.0.6/README.md
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 findu-0.0.6/PKG-INFO
```

### Comparing `findu-0.0.5/findu/findu.py` & `findu-0.0.6/findu/findu.py`

 * *Files identical despite different names*

### Comparing `findu-0.0.5/LICENSE` & `findu-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `findu-0.0.5/pyproject.toml` & `findu-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "findu"
-version = "0.0.5"
+version = "0.0.6"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/findu"
 repository = "https://github.com/MarkHoo/findu"
 classifiers = [
```

### Comparing `findu-0.0.5/README.md` & `findu-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `findu-0.0.5/PKG-INFO` & `findu-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findu
-Version: 0.0.5
+Version: 0.0.6
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/findu
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

