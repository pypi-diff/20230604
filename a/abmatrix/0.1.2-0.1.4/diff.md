# Comparing `tmp/abmatrix-0.1.2.tar.gz` & `tmp/abmatrix-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.1.2.tar", last modified: Sat Jun  3 22:09:28 2023, max compression
+gzip compressed data, was "abmatrix-0.1.4.tar", last modified: Sat Jun  3 22:34:58 2023, max compression
```

## Comparing `abmatrix-0.1.2.tar` & `abmatrix-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:28.487953 abmatrix-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:09:28.487953 abmatrix-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-03 22:09:12.000000 abmatrix-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:28.487953 abmatrix-0.1.2/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:12.000000 abmatrix-0.1.2/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-03 22:09:12.000000 abmatrix-0.1.2/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:09:28.487953 abmatrix-0.1.2/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 22:09:28.000000 abmatrix-0.1.2/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-03 22:09:12.000000 abmatrix-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:09:28.487953 abmatrix-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.785984 abmatrix-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:34:58.785984 abmatrix-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-03 22:34:49.000000 abmatrix-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-03 22:34:49.000000 abmatrix-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:34:58.785984 abmatrix-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.781984 abmatrix-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.781984 abmatrix-0.1.4/src/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:49.000000 abmatrix-0.1.4/src/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-03 22:34:49.000000 abmatrix-0.1.4/src/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.785984 abmatrix-0.1.4/src/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/top_level.txt
```

### Comparing `abmatrix-0.1.2/abmatrix/abmatrix.py` & `abmatrix-0.1.4/src/abmatrix/abmatrix.py`

 * *Files identical despite different names*

