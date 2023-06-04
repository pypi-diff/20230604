# Comparing `tmp/casbin_redis_adapter-1.0.0.tar.gz` & `tmp/casbin_redis_adapter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_redis_adapter-1.0.0.tar", last modified: Sun Jun  4 10:04:04 2023, max compression
+gzip compressed data, was "casbin_redis_adapter-1.0.1.tar", last modified: Sun Jun  4 12:16:06 2023, max compression
```

## Comparing `casbin_redis_adapter-1.0.0.tar` & `casbin_redis_adapter-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:04:04.309716 casbin_redis_adapter-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-04 10:04:04.309716 casbin_redis_adapter-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:04:04.309716 casbin_redis_adapter-1.0.0/casbin_redis_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:04:04.309716 casbin_redis_adapter-1.0.0/casbin_redis_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-04 10:04:04.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-04 10:04:04.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 10:04:04.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 10:04:04.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 10:04:04.000000 casbin_redis_adapter-1.0.0/casbin_redis_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 10:04:04.309716 casbin_redis_adapter-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 10:04:04.309716 casbin_redis_adapter-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-04 10:03:33.000000 casbin_redis_adapter-1.0.0/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/casbin_redis_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-04 12:16:06.000000 casbin_redis_adapter-1.0.1/casbin_redis_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:16:06.399042 casbin_redis_adapter-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-04 12:15:37.000000 casbin_redis_adapter-1.0.1/tests/test_adapter.py
```

### Comparing `casbin_redis_adapter-1.0.0/LICENSE` & `casbin_redis_adapter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_redis_adapter-1.0.0/casbin_redis_adapter/adapter.py` & `casbin_redis_adapter-1.0.1/casbin_redis_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin_redis_adapter-1.0.0/setup.py` & `casbin_redis_adapter-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `casbin_redis_adapter-1.0.0/tests/test_adapter.py` & `casbin_redis_adapter-1.0.1/tests/test_adapter.py`

 * *Files identical despite different names*

