# Comparing `tmp/prungo-1.0.4.tar.gz` & `tmp/prungo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prungo-1.0.4.tar", max compression
+gzip compressed data, was "prungo-1.0.5.tar", max compression
```

## Comparing `prungo-1.0.4.tar` & `prungo-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1497 2023-05-28 12:05:01.469931 prungo-1.0.4/LICENSE
--rw-r--r--   0        0        0       58 2023-05-28 12:05:01.469931 prungo-1.0.4/README.md
--rw-r--r--   0        0        0       93 2023-05-28 12:05:01.469931 prungo-1.0.4/prungo/__init__.py
--rw-r--r--   0        0        0      873 2023-05-28 12:05:01.469931 prungo-1.0.4/prungo/decorators.py
--rw-r--r--   0        0        0      521 2023-05-28 12:05:01.469931 prungo-1.0.4/prungo/models.py
--rw-r--r--   0        0        0      693 2023-05-28 12:05:33.921893 prungo-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 prungo-1.0.4/setup.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 prungo-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-04 03:36:29.207519 prungo-1.0.5/LICENSE
+-rw-r--r--   0        0        0      190 2023-06-04 03:36:29.207519 prungo-1.0.5/README.md
+-rw-r--r--   0        0        0       97 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/constants.py
+-rw-r--r--   0        0        0     2090 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/decorators.py
+-rw-r--r--   0        0        0      445 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/interfaces.py
+-rw-r--r--   0        0        0        0 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/models.py
+-rw-r--r--   0        0        0     1717 2023-06-04 03:36:29.207519 prungo-1.0.5/prungo/utils.py
+-rw-r--r--   0        0        0      786 2023-06-04 03:36:41.411515 prungo-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 prungo-1.0.5/PKG-INFO
```

### Comparing `prungo-1.0.4/LICENSE` & `prungo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prungo-1.0.4/pyproject.toml` & `prungo-1.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prungo"
-version = "1.0.4"
+version = "v1.0.5"
 description = "A package for basic utility functions/classes"
 authors = ["c-prungo"]
 packages = [{include = "prungo"}]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/c-prungo/prungo-util"
 repository = "https://github.com/c-prungo/prungo-util"
@@ -19,12 +19,19 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "^1.10.8"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
+hypothesis = "^6.75.9"
+isort = "^5.12.0"
+black = "^23.3.0"
+
+
+[tool.isort]
+profile = "black"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

