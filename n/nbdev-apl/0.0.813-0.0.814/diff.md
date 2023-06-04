# Comparing `tmp/nbdev-apl-0.0.813.tar.gz` & `tmp/nbdev-apl-0.0.814.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-apl-0.0.813.tar", last modified: Sun Jun  4 01:44:53 2023, max compression
+gzip compressed data, was "nbdev-apl-0.0.814.tar", last modified: Sun Jun  4 13:18:11 2023, max compression
```

## Comparing `nbdev-apl-0.0.813.tar` & `nbdev-apl-0.0.814.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:44:53.153090 nbdev-apl-0.0.813/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 01:35:00.000000 nbdev-apl-0.0.813/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-04 01:35:00.000000 nbdev-apl-0.0.813/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-04 01:44:53.153090 nbdev-apl-0.0.813/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-04 01:35:00.000000 nbdev-apl-0.0.813/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:44:53.153090 nbdev-apl-0.0.813/nbdev_apl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 01:44:52.000000 nbdev-apl-0.0.813/nbdev_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-04 01:35:00.000000 nbdev-apl-0.0.813/nbdev_apl/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-04 01:44:52.000000 nbdev-apl-0.0.813/nbdev_apl/_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:44:53.153090 nbdev-apl-0.0.813/nbdev_apl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 01:44:53.000000 nbdev-apl-0.0.813/nbdev_apl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-04 01:44:52.000000 nbdev-apl-0.0.813/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 01:44:53.153090 nbdev-apl-0.0.813/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-04 01:35:00.000000 nbdev-apl-0.0.813/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:18:11.716099 nbdev-apl-0.0.814/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-04 13:05:09.000000 nbdev-apl-0.0.814/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-04 13:05:09.000000 nbdev-apl-0.0.814/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-04 13:18:11.716099 nbdev-apl-0.0.814/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-04 13:05:09.000000 nbdev-apl-0.0.814/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:18:11.712099 nbdev-apl-0.0.814/nbdev_apl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-04 13:05:09.000000 nbdev-apl-0.0.814/nbdev_apl/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl/_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:18:11.716099 nbdev-apl-0.0.814/nbdev_apl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/nbdev_apl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-04 13:18:11.000000 nbdev-apl-0.0.814/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:18:11.716099 nbdev-apl-0.0.814/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-04 13:05:09.000000 nbdev-apl-0.0.814/setup.py
```

### Comparing `nbdev-apl-0.0.813/LICENSE` & `nbdev-apl-0.0.814/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.813/PKG-INFO` & `nbdev-apl-0.0.814/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.813
+Version: 0.0.814
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.813/nbdev_apl/_modidx.py` & `nbdev-apl-0.0.814/nbdev_apl/_modidx.py`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.813/nbdev_apl.egg-info/PKG-INFO` & `nbdev-apl-0.0.814/nbdev_apl.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.813
+Version: 0.0.814
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.813/settings.ini` & `nbdev-apl-0.0.814/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = fastai
 description = nbdev docs lookup for numpy
 keywords = nbdev fastai python
 author = Jeremy Howard
 author_email = info@fast.ai
 copyright = fast.ai, inc
 branch = master
-version = 0.0.813
+version = 0.0.814
 min_python = 3.6
 audience = Developers
 language = English
 license = apache2
 status = 2
 lib_path = nbdev_apl
 nbs_path = .
```

### Comparing `nbdev-apl-0.0.813/setup.py` & `nbdev-apl-0.0.814/setup.py`

 * *Files identical despite different names*

