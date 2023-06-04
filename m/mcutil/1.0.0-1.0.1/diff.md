# Comparing `tmp/mcutil-1.0.0.tar.gz` & `tmp/mcutil-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcutil-1.0.0.tar", last modified: Sun Jun  4 12:07:37 2023, max compression
+gzip compressed data, was "mcutil-1.0.1.tar", last modified: Sun Jun  4 12:24:43 2023, max compression
```

## Comparing `mcutil-1.0.0.tar` & `mcutil-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 cuongdm   (1000) cuongdm   (1000)        0 2023-06-04 12:07:37.662501 mcutil-1.0.0/
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)    11357 2023-06-04 11:43:24.000000 mcutil-1.0.0/LICENSE
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      727 2023-06-04 12:07:37.662501 mcutil-1.0.0/PKG-INFO
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)       47 2023-06-04 12:04:57.000000 mcutil-1.0.0/README.md
-drwxrwxr-x   0 cuongdm   (1000) cuongdm   (1000)        0 2023-06-04 12:07:37.662501 mcutil-1.0.0/mcutil/
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)       51 2023-06-04 11:54:17.000000 mcutil-1.0.0/mcutil/__init__.py
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      201 2023-06-04 11:52:44.000000 mcutil-1.0.0/mcutil/printer.py
-drwxrwxr-x   0 cuongdm   (1000) cuongdm   (1000)        0 2023-06-04 12:07:37.662501 mcutil-1.0.0/mcutil.egg-info/
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      727 2023-06-04 12:07:37.000000 mcutil-1.0.0/mcutil.egg-info/PKG-INFO
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      222 2023-06-04 12:07:37.000000 mcutil-1.0.0/mcutil.egg-info/SOURCES.txt
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)        1 2023-06-04 12:07:37.000000 mcutil-1.0.0/mcutil.egg-info/dependency_links.txt
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)        1 2023-06-04 11:56:43.000000 mcutil-1.0.0/mcutil.egg-info/not-zip-safe
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)        7 2023-06-04 12:07:37.000000 mcutil-1.0.0/mcutil.egg-info/top_level.txt
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      232 2023-06-04 12:07:37.662501 mcutil-1.0.0/setup.cfg
--rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)     1344 2023-06-04 12:07:34.000000 mcutil-1.0.0/setup.py
+drwxrwxr-x   0 cuongdm   (1000) cuongdm   (1000)        0 2023-06-04 12:24:43.584410 mcutil-1.0.1/
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)    11357 2023-06-04 11:43:24.000000 mcutil-1.0.1/LICENSE
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      727 2023-06-04 12:24:43.584410 mcutil-1.0.1/PKG-INFO
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)       47 2023-06-04 12:04:57.000000 mcutil-1.0.1/README.md
+drwxrwxr-x   0 cuongdm   (1000) cuongdm   (1000)        0 2023-06-04 12:24:43.584410 mcutil-1.0.1/mcutil/
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)       51 2023-06-04 12:23:55.000000 mcutil-1.0.1/mcutil/__init__.py
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      201 2023-06-04 11:52:44.000000 mcutil-1.0.1/mcutil/printer.py
+drwxrwxr-x   0 cuongdm   (1000) cuongdm   (1000)        0 2023-06-04 12:24:43.584410 mcutil-1.0.1/mcutil.egg-info/
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      727 2023-06-04 12:24:43.000000 mcutil-1.0.1/mcutil.egg-info/PKG-INFO
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      222 2023-06-04 12:24:43.000000 mcutil-1.0.1/mcutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)        1 2023-06-04 12:24:43.000000 mcutil-1.0.1/mcutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)        1 2023-06-04 12:22:53.000000 mcutil-1.0.1/mcutil.egg-info/not-zip-safe
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)        7 2023-06-04 12:24:43.000000 mcutil-1.0.1/mcutil.egg-info/top_level.txt
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)      232 2023-06-04 12:24:43.584410 mcutil-1.0.1/setup.cfg
+-rw-rw-r--   0 cuongdm   (1000) cuongdm   (1000)     1341 2023-06-04 12:24:39.000000 mcutil-1.0.1/setup.py
```

### Comparing `mcutil-1.0.0/LICENSE` & `mcutil-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcutil-1.0.0/PKG-INFO` & `mcutil-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcutil
-Version: 1.0.0
+Version: 1.0.1
 Summary: Some simple utilities for Python
 Home-page: https://github.com/cuongpiger/mcutil
 Author: Cuong. Duong Manh
 Author-email: cuongdm8499@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `mcutil-1.0.0/mcutil.egg-info/PKG-INFO` & `mcutil-1.0.1/mcutil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcutil
-Version: 1.0.0
+Version: 1.0.1
 Summary: Some simple utilities for Python
 Home-page: https://github.com/cuongpiger/mcutil
 Author: Cuong. Duong Manh
 Author-email: cuongdm8499@gmail.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `mcutil-1.0.0/setup.py` & `mcutil-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import re
 import os
 
 from setuptools import setup
 
-version = "1.0.0"
+version = None
 with open('mcutil/__init__.py', 'r') as f:
     for line in f:
         m = re.match(r'^__version__\s*=\s*(["\'])([^"\']+)\1', line)
         if m:
             version = m.group(2)
             break
```

