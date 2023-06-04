# Comparing `tmp/michiko-0.2.2.tar.gz` & `tmp/michiko-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michiko-0.2.2.tar", last modified: Sun Jun  4 05:11:51 2023, max compression
+gzip compressed data, was "michiko-0.8.1.tar", last modified: Sun Jun  4 05:38:17 2023, max compression
```

## Comparing `michiko-0.2.2.tar` & `michiko-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-04 05:11:51.388132 michiko-0.2.2/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-06-04 03:01:44.000000 michiko-0.2.2/LICENSE
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      150 2023-06-04 03:01:44.000000 michiko-0.2.2/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      511 2023-06-04 05:11:51.388132 michiko-0.2.2/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       16 2023-06-04 03:01:44.000000 michiko-0.2.2/README.rst
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-06-04 04:53:14.000000 michiko-0.2.2/VERSION
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-04 05:11:51.388132 michiko-0.2.2/michiko.egg-info/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      511 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/PKG-INFO
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      269 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/SOURCES.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/dependency_links.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/requires.txt
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)        4 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/top_level.txt
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-04 05:11:51.388132 michiko-0.2.2/pkg/
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       32 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/app.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      201 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/args.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      166 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/sample.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      524 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/test_app.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1147 2023-06-04 04:54:17.000000 michiko-0.2.2/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-06-04 05:11:51.388132 michiko-0.2.2/setup.cfg
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-06-04 03:01:44.000000 michiko-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:38:17.979388 michiko-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 05:37:59.000000 michiko-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-04 05:37:59.000000 michiko-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-04 05:38:17.979388 michiko-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 05:37:59.000000 michiko-0.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 05:37:59.000000 michiko-0.8.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:38:17.975387 michiko-0.8.1/michiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:38:17.979388 michiko-0.8.1/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-04 05:37:59.000000 michiko-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 05:38:17.979388 michiko-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 05:37:59.000000 michiko-0.8.1/setup.py
```

### Comparing `michiko-0.2.2/LICENSE` & `michiko-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `michiko-0.2.2/pkg/test_app.py` & `michiko-0.8.1/pkg/test_app.py`

 * *Files identical despite different names*

### Comparing `michiko-0.2.2/pyproject.toml` & `michiko-0.8.1/pyproject.toml`

 * *Files identical despite different names*

