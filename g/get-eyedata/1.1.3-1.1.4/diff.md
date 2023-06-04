# Comparing `tmp/get_eyedata-1.1.3.tar.gz` & `tmp/get_eyedata-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_eyedata-1.1.3.tar", last modified: Sun Jun  4 08:53:24 2023, max compression
+gzip compressed data, was "get_eyedata-1.1.4.tar", last modified: Sun Jun  4 09:16:50 2023, max compression
```

## Comparing `get_eyedata-1.1.3.tar` & `get_eyedata-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 08:53:24.702631 get_eyedata-1.1.3/
--rw-rw-rw-   0        0        0     1091 2023-04-27 05:56:35.000000 get_eyedata-1.1.3/LICENCE
--rw-rw-rw-   0        0        0     1930 2023-06-04 08:53:24.701633 get_eyedata-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1407 2023-05-13 00:34:57.000000 get_eyedata-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 08:53:24.668630 get_eyedata-1.1.3/get_eyedata/
--rw-rw-rw-   0        0        0       53 2023-06-04 08:43:45.000000 get_eyedata-1.1.3/get_eyedata/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-06-04 07:07:15.000000 get_eyedata-1.1.3/get_eyedata/frame_utils.py
--rw-rw-rw-   0        0        0     1546 2023-06-04 01:13:59.000000 get_eyedata-1.1.3/get_eyedata/make_eyedataset.py
--rw-rw-rw-   0        0        0        0 2023-05-13 00:34:57.000000 get_eyedata-1.1.3/get_eyedata/ow2.py
--rw-rw-rw-   0        0        0     3258 2023-06-04 08:53:03.000000 get_eyedata-1.1.3/get_eyedata/valo.py
-drwxrwxrwx   0        0        0        0 2023-06-04 08:53:24.696631 get_eyedata-1.1.3/get_eyedata.egg-info/
--rw-rw-rw-   0        0        0     1930 2023-06-04 08:53:24.000000 get_eyedata-1.1.3/get_eyedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-04 08:53:24.000000 get_eyedata-1.1.3/get_eyedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 08:53:24.000000 get_eyedata-1.1.3/get_eyedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      195 2023-06-04 08:53:24.000000 get_eyedata-1.1.3/get_eyedata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-04 08:53:24.000000 get_eyedata-1.1.3/get_eyedata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 08:53:24.702631 get_eyedata-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1492 2023-06-04 08:53:17.000000 get_eyedata-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:16:50.527707 get_eyedata-1.1.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-27 05:56:35.000000 get_eyedata-1.1.4/LICENCE
+-rw-rw-rw-   0        0        0     1930 2023-06-04 09:16:50.526708 get_eyedata-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1407 2023-05-13 00:34:57.000000 get_eyedata-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 09:16:50.503704 get_eyedata-1.1.4/get_eyedata/
+-rw-rw-rw-   0        0        0        6 2023-06-04 09:16:22.000000 get_eyedata-1.1.4/get_eyedata/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-06-04 07:07:15.000000 get_eyedata-1.1.4/get_eyedata/frame_utils.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 00:34:57.000000 get_eyedata-1.1.4/get_eyedata/ow2.py
+-rw-rw-rw-   0        0        0     3258 2023-06-04 08:53:03.000000 get_eyedata-1.1.4/get_eyedata/valo.py
+drwxrwxrwx   0        0        0        0 2023-06-04 09:16:50.521702 get_eyedata-1.1.4/get_eyedata.egg-info/
+-rw-rw-rw-   0        0        0     1930 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      195 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-04 09:16:50.000000 get_eyedata-1.1.4/get_eyedata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 09:16:50.527707 get_eyedata-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1492 2023-06-04 09:16:38.000000 get_eyedata-1.1.4/setup.py
```

### Comparing `get_eyedata-1.1.3/LICENCE` & `get_eyedata-1.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `get_eyedata-1.1.3/PKG-INFO` & `get_eyedata-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_eyedata
-Version: 1.1.3
+Version: 1.1.4
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
```

### Comparing `get_eyedata-1.1.3/README.md` & `get_eyedata-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `get_eyedata-1.1.3/get_eyedata/frame_utils.py` & `get_eyedata-1.1.4/get_eyedata/frame_utils.py`

 * *Files identical despite different names*

### Comparing `get_eyedata-1.1.3/get_eyedata/valo.py` & `get_eyedata-1.1.4/get_eyedata/valo.py`

 * *Files identical despite different names*

### Comparing `get_eyedata-1.1.3/get_eyedata.egg-info/PKG-INFO` & `get_eyedata-1.1.4/get_eyedata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-eyedata
-Version: 1.1.3
+Version: 1.1.4
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
```

### Comparing `get_eyedata-1.1.3/setup.py` & `get_eyedata-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 DESCRIPTION = 'gat gaze data form record.'
 NAME = 'get_eyedata'
 AUTHOR = 'ikrfun'
 AUTHOR_EMAIL = 't.nobuto130625@gmail.com'
 URL = 'https://github.com/ikrfun/get_eyedata'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '1.1.3'
+VERSION = '1.1.4'
 PYTHON_REQUIRES = '>=3.10'
 INSTALL_REQUIRES = [
     'matplotlib>=3.7.1',
     'moviepy>=1.0.3',
     'numpy>=1.24.3',
     'opencv_contrib_python>=4.6.0.66',
     'opencv_python>=4.7.0.72',
```

