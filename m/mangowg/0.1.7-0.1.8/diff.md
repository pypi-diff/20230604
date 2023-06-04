# Comparing `tmp/mangowg-0.1.7.tar.gz` & `tmp/mangowg-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangowg-0.1.7.tar", max compression
+gzip compressed data, was "mangowg-0.1.8.tar", max compression
```

## Comparing `mangowg-0.1.7.tar` & `mangowg-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3939 2023-06-04 09:20:49.661833 mangowg-0.1.7/mangowg/DataScraper.py
--rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.7/mangowg/mangowg.py
--rw-r--r--   0        0        0    12584 2023-06-04 06:40:26.992771 mangowg-0.1.7/mangowg/TemplateGeneratorYattag.py
--rw-r--r--   0        0        0     1092 2023-06-04 10:37:37.122655 mangowg-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      722 2023-06-04 10:16:29.662720 mangowg-0.1.7/README.md
--rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mangowg-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3939 2023-06-04 09:20:49.661833 mangowg-0.1.8/mangowg/DataScraper.py
+-rw-r--r--   0        0        0     5730 2023-06-04 10:38:54.968325 mangowg-0.1.8/mangowg/mangowg.py
+-rw-r--r--   0        0        0    12584 2023-06-04 06:40:26.992771 mangowg-0.1.8/mangowg/TemplateGeneratorYattag.py
+-rw-r--r--   0        0        0     1092 2023-06-04 10:39:02.521684 mangowg-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      722 2023-06-04 10:16:29.662720 mangowg-0.1.8/README.md
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mangowg-0.1.8/PKG-INFO
```

### Comparing `mangowg-0.1.7/mangowg/DataScraper.py` & `mangowg-0.1.8/mangowg/DataScraper.py`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.7/mangowg/mangowg.py` & `mangowg-0.1.8/mangowg/mangowg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
-import DataScraper
-import TemplateGeneratorYattag
+from mangowg import DataScraper
+from mangowg import TemplateGeneratorYattag
 
 from pprint import pprint
 import inquirer
 
 import time
 import typer
 from rich.progress import track
```

### Comparing `mangowg-0.1.7/mangowg/TemplateGeneratorYattag.py` & `mangowg-0.1.8/mangowg/TemplateGeneratorYattag.py`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.7/pyproject.toml` & `mangowg-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mangowg"
-version = "0.1.7"
+version = "0.1.8"
 description = "A portfolio website generator"
 authors = ["Amelia <53657436+AmeliaTYR@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ansicon = "1.89.0"
```

### Comparing `mangowg-0.1.7/README.md` & `mangowg-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.7/PKG-INFO` & `mangowg-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangowg
-Version: 0.1.7
+Version: 0.1.8
 Summary: A portfolio website generator
 Author: Amelia
 Author-email: 53657436+AmeliaTYR@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

