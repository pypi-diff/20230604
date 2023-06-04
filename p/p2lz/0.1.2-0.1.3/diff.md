# Comparing `tmp/p2lz-0.1.2.tar.gz` & `tmp/p2lz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p2lz-0.1.2.tar", last modified: Tue May  9 01:33:13 2023, max compression
+gzip compressed data, was "p2lz-0.1.3.tar", last modified: Sun Jun  4 02:54:59 2023, max compression
```

## Comparing `p2lz-0.1.2.tar` & `p2lz-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.016212 p2lz-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-09 01:32:57.000000 p2lz-0.1.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-09 01:32:57.000000 p2lz-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 01:32:57.000000 p2lz-0.1.2/.tool-versions
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 01:32:57.000000 p2lz-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-09 01:32:57.000000 p2lz-0.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 01:33:13.012212 p2lz-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-09 01:32:57.000000 p2lz-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 01:32:57.000000 p2lz-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 01:33:13.016212 p2lz-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/src/p2lz/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-09 01:32:57.000000 p2lz-0.1.2/src/p2lz/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-09 01:32:57.000000 p2lz-0.1.2/src/p2lz/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-09 01:32:57.000000 p2lz-0.1.2/src/p2lz/tools_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 01:33:13.012212 p2lz-0.1.2/src/p2lz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-09 01:33:13.000000 p2lz-0.1.2/src/p2lz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-09 01:33:12.000000 p2lz-0.1.2/src/p2lz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:54:59.837290 p2lz-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:54:59.837290 p2lz-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:54:59.837290 p2lz-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-04 02:54:45.000000 p2lz-0.1.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-04 02:54:45.000000 p2lz-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-04 02:54:45.000000 p2lz-0.1.3/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-04 02:54:45.000000 p2lz-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-04 02:54:45.000000 p2lz-0.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-04 02:54:59.837290 p2lz-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-04 02:54:45.000000 p2lz-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-04 02:54:45.000000 p2lz-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:54:59.837290 p2lz-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:54:59.837290 p2lz-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:54:59.837290 p2lz-0.1.3/src/p2lz/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-04 02:54:45.000000 p2lz-0.1.3/src/p2lz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 02:54:59.000000 p2lz-0.1.3/src/p2lz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-04 02:54:45.000000 p2lz-0.1.3/src/p2lz/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-04 02:54:45.000000 p2lz-0.1.3/src/p2lz/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 02:54:45.000000 p2lz-0.1.3/src/p2lz/tools_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:54:59.837290 p2lz-0.1.3/src/p2lz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-04 02:54:59.000000 p2lz-0.1.3/src/p2lz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-04 02:54:59.000000 p2lz-0.1.3/src/p2lz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:54:59.000000 p2lz-0.1.3/src/p2lz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 02:54:59.000000 p2lz-0.1.3/src/p2lz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 02:54:59.000000 p2lz-0.1.3/src/p2lz.egg-info/top_level.txt
```

### Comparing `p2lz-0.1.2/.github/workflows/publish.yaml` & `p2lz-0.1.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `p2lz-0.1.2/LICENSE.txt` & `p2lz-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `p2lz-0.1.2/src/p2lz/dynamodb.py` & `p2lz-0.1.3/src/p2lz/dynamodb.py`

 * *Files identical despite different names*

### Comparing `p2lz-0.1.2/src/p2lz/tools.py` & `p2lz-0.1.3/src/p2lz/tools.py`

 * *Files identical despite different names*

