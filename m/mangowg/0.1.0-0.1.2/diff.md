# Comparing `tmp/mangowg-0.1.0.tar.gz` & `tmp/mangowg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangowg-0.1.0.tar", max compression
+gzip compressed data, was "mangowg-0.1.2.tar", max compression
```

## Comparing `mangowg-0.1.0.tar` & `mangowg-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.0/mangowg.py
--rw-r--r--   0        0        0      988 2023-06-04 09:56:42.553099 mangowg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      196 2023-06-03 03:48:05.709806 mangowg-0.1.0/README.md
--rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 mangowg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5704 2023-06-04 09:18:30.195315 mangowg-0.1.2/mangowg.py
+-rw-r--r--   0        0        0      987 2023-06-04 10:14:06.617713 mangowg-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      354 2023-06-04 10:07:46.184832 mangowg-0.1.2/README.md
+-rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 mangowg-0.1.2/PKG-INFO
```

### Comparing `mangowg-0.1.0/mangowg.py` & `mangowg-0.1.2/mangowg.py`

 * *Files identical despite different names*

### Comparing `mangowg-0.1.0/pyproject.toml` & `mangowg-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "mangowg"
-version = "0.1.0"
+version = "0.1.2"
 description = "A portfolio website generator"
 authors = ["Amelia <53657436+AmeliaTYR@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 ansicon = "1.89.0"
 blessed = "1.20.0"
 certifi = "2023.5.7"
 cffi = "1.15.1"
 charset-normalizer = "3.1.0"
 click = "8.1.3"
 colorama = "0.4.6"
```

