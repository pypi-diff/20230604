# Comparing `tmp/mangowg-0.1.2.tar.gz` & `tmp/mangowg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangowg-0.1.2.tar", max compression
+gzip compressed data, was "mangowg-0.1.3.tar", max compression
```

## Comparing `mangowg-0.1.2.tar` & `mangowg-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.2/mangowg.py
--rw-r--r--   0        0        0      987 2023-06-04 10:14:06.617713 mangowg-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      354 2023-06-04 10:07:46.184832 mangowg-0.1.2/README.md
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 mangowg-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.3/mangowg.py
+-rw-r--r--   0        0        0      989 2023-06-04 10:19:52.099533 mangowg-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      722 2023-06-04 10:16:29.662720 mangowg-0.1.3/README.md
+-rw-r--r--   0        0        0     2233 1970-01-01 00:00:00.000000 mangowg-0.1.3/PKG-INFO
```

### Comparing `mangowg-0.1.2/mangowg.py` & `mangowg-0.1.3/mangowg.py`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.2/pyproject.toml` & `mangowg-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mangowg"
-version = "0.1.2"
+version = "0.1.3"
 description = "A portfolio website generator"
 authors = ["Amelia <53657436+AmeliaTYR@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ansicon = "1.89.0"
@@ -37,10 +37,9 @@
 typing_extensions = "4.6.3"
 urllib3 = "2.0.2"
 wcwidth = "0.2.6"
 wrapt = "1.15.0"
 yattag = "1.15.1"
 
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
+build-backend = "setuptools.build_meta"
+requires = ["setuptools", "wheel"]
```

### Comparing `mangowg-0.1.2/PKG-INFO` & `mangowg-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangowg
-Version: 0.1.2
+Version: 0.1.3
 Summary: A portfolio website generator
 Author: Amelia
 Author-email: 53657436+AmeliaTYR@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -49,14 +49,28 @@
 ## Python Venv
 
 * `python -m venv venv`
 * `venv\Scripts\activate.bat`
 * `pip install -r requirements.txt`
 * `pip freeze > requirements.txt`
 
+## Usage
+Get started `python mangowg.py --help`
+
+To use command selection rather than typing the command name, use `python mangowg.py cut` then select the command to be executed.
+
+
 ## PyPi publish 
+Publish new package
 
 * install poetry
 * `poetry init`
 * `poetry build`
 * `poetry publish -u USERNAME -p PASSWORD`
     * use pypi password for this step
+
+To update version number:
+
+* `poetry version 0.1.2`
+* `poetry build`
+* `poetry publish -u USERNAME -p PASSWORD`
+    * use github password for this step
```

