# Comparing `tmp/michiko-0.0.4.tar.gz` & `tmp/michiko-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michiko-0.0.4.tar", last modified: Fri Oct 14 02:50:24 2022, max compression
+gzip compressed data, was "michiko-0.2.2.tar", last modified: Sun Jun  4 05:11:51 2023, max compression
```

## Comparing `michiko-0.0.4.tar` & `michiko-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 mohsen    (1000) mohsen    (1000)        0 2022-10-14 02:50:24.196467 michiko-0.0.4/
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)    35149 2022-06-02 20:01:24.000000 michiko-0.0.4/LICENSE
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       26 2022-10-14 00:18:56.000000 michiko-0.0.4/MANIFEST.in
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)    42569 2022-10-14 02:50:24.196467 michiko-0.0.4/PKG-INFO
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1555 2022-10-14 02:48:55.000000 michiko-0.0.4/README.rst
-drwxrwxr-x   0 mohsen    (1000) mohsen    (1000)        0 2022-10-14 02:50:24.196467 michiko-0.0.4/michiko/
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     9842 2022-10-14 01:49:14.000000 michiko-0.0.4/michiko/Drive.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       20 2022-10-13 05:27:59.000000 michiko-0.0.4/michiko/__init__.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1330 2022-09-11 22:12:04.000000 michiko-0.0.4/michiko/app.py
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1625 2022-07-10 04:40:56.000000 michiko-0.0.4/michiko/mime.py
-drwxrwxr-x   0 mohsen    (1000) mohsen    (1000)        0 2022-10-14 02:50:24.196467 michiko-0.0.4/michiko.egg-info/
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)    42569 2022-10-14 02:50:24.000000 michiko-0.0.4/michiko.egg-info/PKG-INFO
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      276 2022-10-14 02:50:24.000000 michiko-0.0.4/michiko.egg-info/SOURCES.txt
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)        1 2022-10-14 02:50:24.000000 michiko-0.0.4/michiko.egg-info/dependency_links.txt
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      107 2022-10-14 02:50:24.000000 michiko-0.0.4/michiko.egg-info/requires.txt
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)        8 2022-10-14 02:50:24.000000 michiko-0.0.4/michiko.egg-info/top_level.txt
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)     1704 2022-10-14 02:50:13.000000 michiko-0.0.4/pyproject.toml
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)       38 2022-10-14 02:50:24.196467 michiko-0.0.4/setup.cfg
--rw-rw-r--   0 mohsen    (1000) mohsen    (1000)      170 2022-06-19 23:27:17.000000 michiko-0.0.4/setup.py
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-04 05:11:51.388132 michiko-0.2.2/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)    35149 2023-06-04 03:01:44.000000 michiko-0.2.2/LICENSE
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      150 2023-06-04 03:01:44.000000 michiko-0.2.2/MANIFEST.in
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      511 2023-06-04 05:11:51.388132 michiko-0.2.2/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       16 2023-06-04 03:01:44.000000 michiko-0.2.2/README.rst
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        5 2023-06-04 04:53:14.000000 michiko-0.2.2/VERSION
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-04 05:11:51.388132 michiko-0.2.2/michiko.egg-info/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      511 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/PKG-INFO
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      269 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/SOURCES.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        1 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/dependency_links.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       46 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/requires.txt
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)        4 2023-06-04 05:11:51.000000 michiko-0.2.2/michiko.egg-info/top_level.txt
+drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-06-04 05:11:51.388132 michiko-0.2.2/pkg/
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       32 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/app.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      201 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/args.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      166 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/sample.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      524 2023-06-04 03:01:44.000000 michiko-0.2.2/pkg/test_app.py
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)     1147 2023-06-04 04:54:17.000000 michiko-0.2.2/pyproject.toml
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-06-04 05:11:51.388132 michiko-0.2.2/setup.cfg
+-rw-r--r--   0 mohsen    (1000) mohsen    (1000)      170 2023-06-04 03:01:44.000000 michiko-0.2.2/setup.py
```

### Comparing `michiko-0.0.4/LICENSE` & `michiko-0.2.2/LICENSE`

 * *Files identical despite different names*

