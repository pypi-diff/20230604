# Comparing `tmp/appwee-0.1.0.tar.gz` & `tmp/appwee-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appwee-0.1.0.tar", last modified: Sun Jun  4 14:10:12 2023, max compression
+gzip compressed data, was "appwee-0.1.1.tar", last modified: Sun Jun  4 14:34:12 2023, max compression
```

## Comparing `appwee-0.1.0.tar` & `appwee-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:10:12.218241 appwee-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 14:09:48.000000 appwee-0.1.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-04 14:10:12.218241 appwee-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-04 14:09:48.000000 appwee-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 14:10:12.218241 appwee-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:10:12.218241 appwee-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:10:12.218241 appwee-0.1.0/src/appwee/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 14:09:48.000000 appwee-0.1.0/src/appwee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-04 14:09:48.000000 appwee-0.1.0/src/appwee/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:10:12.218241 appwee-0.1.0/src/appwee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-04 14:10:12.000000 appwee-0.1.0/src/appwee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-04 14:10:12.000000 appwee-0.1.0/src/appwee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 14:10:12.000000 appwee-0.1.0/src/appwee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 14:10:12.000000 appwee-0.1.0/src/appwee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-04 14:10:12.000000 appwee-0.1.0/src/appwee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:34:12.282487 appwee-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 14:33:54.000000 appwee-0.1.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-04 14:34:12.282487 appwee-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-04 14:33:54.000000 appwee-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-04 14:33:54.000000 appwee-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 14:34:12.282487 appwee-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:34:12.278488 appwee-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:34:12.282487 appwee-0.1.1/src/appwee/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-04 14:33:54.000000 appwee-0.1.1/src/appwee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-04 14:33:54.000000 appwee-0.1.1/src/appwee/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 14:34:12.282487 appwee-0.1.1/src/appwee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-04 14:34:12.000000 appwee-0.1.1/src/appwee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-04 14:34:12.000000 appwee-0.1.1/src/appwee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 14:34:12.000000 appwee-0.1.1/src/appwee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-04 14:34:12.000000 appwee-0.1.1/src/appwee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-04 14:34:12.000000 appwee-0.1.1/src/appwee.egg-info/top_level.txt
```

### Comparing `appwee-0.1.0/LICENCE.md` & `appwee-0.1.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `appwee-0.1.0/pyproject.toml` & `appwee-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "appwee"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Highghlow", email="highghlow@proton.me" },
 ]
 description = "Wrapper around peewee with some QoL features"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `appwee-0.1.0/src/appwee/app.py` & `appwee-0.1.1/src/appwee/app.py`

 * *Files identical despite different names*

