# Comparing `tmp/michiko-0.8.1.tar.gz` & `tmp/michiko-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michiko-0.8.1.tar", last modified: Sun Jun  4 05:38:17 2023, max compression
+gzip compressed data, was "michiko-0.8.3.tar", last modified: Sun Jun  4 06:24:00 2023, max compression
```

## Comparing `michiko-0.8.1.tar` & `michiko-0.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:38:17.979388 michiko-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 05:37:59.000000 michiko-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-04 05:37:59.000000 michiko-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-04 05:38:17.979388 michiko-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 05:37:59.000000 michiko-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 05:37:59.000000 michiko-0.8.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:38:17.975387 michiko-0.8.1/michiko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 05:38:17.000000 michiko-0.8.1/michiko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 05:38:17.979388 michiko-0.8.1/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-04 05:37:59.000000 michiko-0.8.1/pkg/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-04 05:37:59.000000 michiko-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 05:38:17.979388 michiko-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 05:37:59.000000 michiko-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:24:00.410235 michiko-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-04 06:23:42.000000 michiko-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-04 06:23:42.000000 michiko-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-04 06:24:00.410235 michiko-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 06:23:42.000000 michiko-0.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 06:23:42.000000 michiko-0.8.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:24:00.410235 michiko-0.8.3/michiko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-04 06:24:00.000000 michiko-0.8.3/michiko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-04 06:24:00.000000 michiko-0.8.3/michiko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:24:00.000000 michiko-0.8.3/michiko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 06:24:00.000000 michiko-0.8.3/michiko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-04 06:24:00.000000 michiko-0.8.3/michiko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:24:00.410235 michiko-0.8.3/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 06:23:42.000000 michiko-0.8.3/pkg/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-04 06:23:42.000000 michiko-0.8.3/pkg/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-04 06:23:42.000000 michiko-0.8.3/pkg/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-04 06:23:42.000000 michiko-0.8.3/pkg/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-04 06:23:42.000000 michiko-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 06:24:00.410235 michiko-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-04 06:23:42.000000 michiko-0.8.3/setup.py
```

### Comparing `michiko-0.8.1/LICENSE` & `michiko-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `michiko-0.8.1/pkg/test_app.py` & `michiko-0.8.3/pkg/test_app.py`

 * *Files identical despite different names*

### Comparing `michiko-0.8.1/pyproject.toml` & `michiko-0.8.3/pyproject.toml`

 * *Files identical despite different names*

