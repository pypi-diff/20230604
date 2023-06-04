# Comparing `tmp/mangowg-0.1.4.tar.gz` & `tmp/mangowg-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangowg-0.1.4.tar", max compression
+gzip compressed data, was "mangowg-0.1.5.tar", max compression
```

## Comparing `mangowg-0.1.4.tar` & `mangowg-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.4/mangowg.py
--rw-r--r--   0        0        0     1035 2023-06-04 10:26:01.535513 mangowg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      722 2023-06-04 10:16:29.662720 mangowg-0.1.4/README.md
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mangowg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3939 2023-06-04 09:20:49.661833 mangowg-0.1.5/mangowg/DataScraper.py
+-rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.5/mangowg/mangowg.py
+-rw-r--r--   0        0        0    12584 2023-06-04 06:40:26.992771 mangowg-0.1.5/mangowg/TemplateGeneratorYattag.py
+-rw-r--r--   0        0        0     1043 2023-06-04 10:33:41.938801 mangowg-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      722 2023-06-04 10:16:29.662720 mangowg-0.1.5/README.md
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mangowg-0.1.5/PKG-INFO
```

### Comparing `mangowg-0.1.4/mangowg.py` & `mangowg-0.1.5/mangowg/mangowg.py`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.4/pyproject.toml` & `mangowg-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mangowg"
-version = "0.1.4"
+version = "0.1.5"
 description = "A portfolio website generator"
 authors = ["Amelia <53657436+AmeliaTYR@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ansicon = "1.89.0"
@@ -41,8 +41,8 @@
 yattag = "1.15.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-mangowg = "mangowg:cli"
+mangowg = "mangowg.mangowg:cli"
```

### Comparing `mangowg-0.1.4/README.md` & `mangowg-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.4/PKG-INFO` & `mangowg-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangowg
-Version: 0.1.4
+Version: 0.1.5
 Summary: A portfolio website generator
 Author: Amelia
 Author-email: 53657436+AmeliaTYR@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

