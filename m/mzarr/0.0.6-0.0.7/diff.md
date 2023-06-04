# Comparing `tmp/mzarr-0.0.6.tar.gz` & `tmp/mzarr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mzarr-0.0.6.tar", last modified: Fri Jun  2 09:21:28 2023, max compression
+gzip compressed data, was "mzarr-0.0.7.tar", last modified: Sun Jun  4 09:27:25 2023, max compression
```

## Comparing `mzarr-0.0.6.tar` & `mzarr-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.849953 mzarr-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 09:21:08.000000 mzarr-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 09:21:08.000000 mzarr-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:21:28.849953 mzarr-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-02 09:21:08.000000 mzarr-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.845953 mzarr-0.0.6/mzarr/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.849953 mzarr-0.0.6/mzarr/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/nifti2mzarr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-02 09:21:08.000000 mzarr-0.0.6/mzarr/tiff2mzarr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:21:28.849953 mzarr-0.0.6/mzarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 09:21:28.000000 mzarr-0.0.6/mzarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 09:21:08.000000 mzarr-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-02 09:21:28.849953 mzarr-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:27:25.155039 mzarr-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-04 09:27:09.000000 mzarr-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-04 09:27:09.000000 mzarr-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-04 09:27:25.155039 mzarr-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-04 09:27:09.000000 mzarr-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:27:25.155039 mzarr-0.0.7/mzarr/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-04 09:27:09.000000 mzarr-0.0.7/mzarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:27:25.155039 mzarr-0.0.7/mzarr/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 09:27:09.000000 mzarr-0.0.7/mzarr/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-06-04 09:27:09.000000 mzarr-0.0.7/mzarr/mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-04 09:27:09.000000 mzarr-0.0.7/mzarr/nifti2mzarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-04 09:27:09.000000 mzarr-0.0.7/mzarr/tiff2mzarr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:27:25.155039 mzarr-0.0.7/mzarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-04 09:27:25.000000 mzarr-0.0.7/mzarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 09:27:25.000000 mzarr-0.0.7/mzarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:27:25.000000 mzarr-0.0.7/mzarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-04 09:27:25.000000 mzarr-0.0.7/mzarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 09:27:25.000000 mzarr-0.0.7/mzarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-04 09:27:09.000000 mzarr-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-04 09:27:25.155039 mzarr-0.0.7/setup.cfg
```

### Comparing `mzarr-0.0.6/LICENSE` & `mzarr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.6/PKG-INFO` & `mzarr-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mzarr-0.0.6/README.md` & `mzarr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.6/mzarr/mzarr.py` & `mzarr-0.0.7/mzarr/mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.6/mzarr/nifti2mzarr.py` & `mzarr-0.0.7/mzarr/nifti2mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.6/mzarr/tiff2mzarr.py` & `mzarr-0.0.7/mzarr/tiff2mzarr.py`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.6/mzarr.egg-info/PKG-INFO` & `mzarr-0.0.7/mzarr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzarr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mzarr (Multi-Resolution Zarr) is a Python library for working with the Mzarr image format
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mzarr-0.0.6/pyproject.toml` & `mzarr-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mzarr-0.0.6/setup.cfg` & `mzarr-0.0.7/setup.cfg`

 * *Files identical despite different names*

