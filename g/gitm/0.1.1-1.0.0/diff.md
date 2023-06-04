# Comparing `tmp/gitm-0.1.1.tar.gz` & `tmp/gitm-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitm-0.1.1.tar", last modified: Tue Feb 28 01:33:04 2023, max compression
+gzip compressed data, was "gitm-1.0.0.tar", last modified: Sun Jun  4 19:58:45 2023, max compression
```

## Comparing `gitm-0.1.1.tar` & `gitm-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 01:33:04.054301 gitm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-28 01:32:43.000000 gitm-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-02-28 01:33:04.054301 gitm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-28 01:32:43.000000 gitm-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 01:33:04.054301 gitm-0.1.1/gitm/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-28 01:32:43.000000 gitm-0.1.1/gitm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-28 01:32:43.000000 gitm-0.1.1/gitm/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 01:33:04.054301 gitm-0.1.1/gitm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-02-28 01:33:04.000000 gitm-0.1.1/gitm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-28 01:33:04.000000 gitm-0.1.1/gitm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 01:33:04.000000 gitm-0.1.1/gitm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-28 01:33:04.000000 gitm-0.1.1/gitm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-28 01:33:04.000000 gitm-0.1.1/gitm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-28 01:33:04.000000 gitm-0.1.1/gitm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-28 01:32:43.000000 gitm-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 01:33:04.054301 gitm-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 01:32:43.000000 gitm-0.1.1/setup.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 19:58:45.464146 gitm-1.0.0/
+-rw-r--r--   0 abb       (1000) abb       (1000)    11357 2023-02-28 00:36:32.000000 gitm-1.0.0/LICENSE
+-rw-r--r--   0 abb       (1000) abb       (1000)    25168 2023-06-04 19:58:45.464146 gitm-1.0.0/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)    11690 2023-06-04 19:42:31.000000 gitm-1.0.0/README.md
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 19:58:45.464146 gitm-1.0.0/gitm/
+-rw-r--r--   0 abb       (1000) abb       (1000)       23 2023-02-28 01:31:51.000000 gitm-1.0.0/gitm/__init__.py
+-rw-r--r--   0 abb       (1000) abb       (1000)     1485 2023-06-04 19:48:45.000000 gitm-1.0.0/gitm/__main__.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      528 2023-06-04 16:27:38.000000 gitm-1.0.0/gitm/connection.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      352 2023-06-04 16:05:52.000000 gitm-1.0.0/gitm/db.py
+-rw-r--r--   0 abb       (1000) abb       (1000)    11161 2023-06-04 19:46:16.000000 gitm-1.0.0/gitm/pattern.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 19:58:45.464146 gitm-1.0.0/gitm.egg-info/
+-rw-r--r--   0 abb       (1000) abb       (1000)    25168 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)      291 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/SOURCES.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/dependency_links.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)       43 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/entry_points.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)       42 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/requires.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        5 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/top_level.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)     1154 2023-06-04 19:41:11.000000 gitm-1.0.0/pyproject.toml
+-rw-r--r--   0 abb       (1000) abb       (1000)       38 2023-06-04 19:58:45.464146 gitm-1.0.0/setup.cfg
+-rw-r--r--   0 abb       (1000) abb       (1000)       38 2023-02-28 00:45:14.000000 gitm-1.0.0/setup.py
```

### Comparing `gitm-0.1.1/LICENSE` & `gitm-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitm-0.1.1/pyproject.toml` & `gitm-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitm"
-version = "0.1.1"
+version = "1.0.0"
 description = "Git emoji cli application"
 readme = "README.md"
 authors = [
     { name = "AmirBahador Bahadori", email = "amirbahador.pv@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

