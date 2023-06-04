# Comparing `tmp/polugins-0.1.0.tar.gz` & `tmp/polugins-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polugins-0.1.0.tar", max compression
+gzip compressed data, was "polugins-0.2.0.tar", max compression
```

## Comparing `polugins-0.1.0.tar` & `polugins-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1439 2023-06-03 13:54:04.156678 polugins-0.1.0/README.md
--rw-r--r--   0        0        0      642 2023-06-03 13:58:13.726248 polugins-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-03 11:00:47.063275 polugins-0.1.0/src/polugins/__init__.py
--rw-r--r--   0        0        0     2641 2023-06-03 13:38:00.649172 polugins-0.1.0/src/polugins/main.py
--rw-r--r--   0        0        0      422 2023-06-03 13:26:52.238165 polugins-0.1.0/src/polugins/namespace.py
--rw-r--r--   0        0        0      108 2023-06-03 13:45:25.064765 polugins-0.1.0/src/polugins/polars.py
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 polugins-0.1.0/setup.py
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 polugins-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-03 14:22:39.475145 polugins-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3731 2023-06-04 09:57:06.128065 polugins-0.2.0/README.md
+-rw-r--r--   0        0        0      621 2023-06-04 10:01:16.489291 polugins-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-04 09:45:22.347349 polugins-0.2.0/src/polugins/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-04 09:40:25.769765 polugins-0.2.0/src/polugins/_types.py
+-rw-r--r--   0        0        0     2583 2023-06-04 09:12:49.097182 polugins-0.2.0/src/polugins/create_types.py
+-rw-r--r--   0        0        0     2435 2023-06-04 09:45:29.187321 polugins-0.2.0/src/polugins/main.py
+-rw-r--r--   0        0        0      746 2023-06-04 09:45:03.783429 polugins-0.2.0/src/polugins/namespace.py
+-rw-r--r--   0        0        0      133 2023-06-04 09:45:57.027218 polugins-0.2.0/src/polugins/pl.py
+-rw-r--r--   0        0        0     4585 1970-01-01 00:00:00.000000 polugins-0.2.0/setup.py
+-rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 polugins-0.2.0/PKG-INFO
```

### Comparing `polugins-0.1.0/pyproject.toml` & `polugins-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [tool.poetry]
 name = "polugins"
-version = "0.1.0"
+version = "0.2.0"
 description = "Plugin system for Polars."
 authors = ["StefanBRas <opensource@bruhn.io>"]
 readme = "README.md"
 packages = [{include = "polugins", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 polars = "^0.18.0"
 importlib-metadata = "^6.6.0"
-
-# Used for testing
+mypy = "^1.3.0"
 # example-package = {path = "tests/pkgs/example_package"}
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-# Used for testing
-#[tool.poetry.plugins."polugins.lazyframe"]
-#"internal" = "polugins.namespace:EntryPointNameSpace"
+# [tool.poetry.plugins."polugins.lazyframe"]
+# "internal" = "polugins.namespace:EntryPointNameSpace"
```

