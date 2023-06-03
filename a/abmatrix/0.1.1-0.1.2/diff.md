# Comparing `tmp/abmatrix-0.1.1.tar.gz` & `tmp/abmatrix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.1.1.tar", last modified: Sat Jun  3 20:03:55 2023, max compression
+gzip compressed data, was "abmatrix-0.1.2.tar", last modified: Sat Jun  3 22:09:28 2023, max compression
```

## Comparing `abmatrix-0.1.1.tar` & `abmatrix-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:55.987375 abmatrix-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 20:03:55.987375 abmatrix-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-03 20:03:46.000000 abmatrix-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-03 20:03:46.000000 abmatrix-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:03:55.987375 abmatrix-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:55.983375 abmatrix-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:55.987375 abmatrix-0.1.1/src/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:46.000000 abmatrix-0.1.1/src/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-03 20:03:46.000000 abmatrix-0.1.1/src/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:55.987375 abmatrix-0.1.1/src/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 20:03:55.000000 abmatrix-0.1.1/src/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 20:03:55.000000 abmatrix-0.1.1/src/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:03:55.000000 abmatrix-0.1.1/src/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 20:03:55.000000 abmatrix-0.1.1/src/abmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:28.487953 abmatrix-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:09:28.487953 abmatrix-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-03 22:09:12.000000 abmatrix-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:28.487953 abmatrix-0.1.2/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:12.000000 abmatrix-0.1.2/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-03 22:09:12.000000 abmatrix-0.1.2/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:28.487953 abmatrix-0.1.2/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-03 22:09:12.000000 abmatrix-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:09:28.487953 abmatrix-0.1.2/setup.cfg
```

### Comparing `abmatrix-0.1.1/src/abmatrix/abmatrix.py` & `abmatrix-0.1.2/abmatrix/abmatrix.py`

 * *Files identical despite different names*

