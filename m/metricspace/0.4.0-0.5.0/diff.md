# Comparing `tmp/metricspace-0.4.0.tar.gz` & `tmp/metricspace-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricspace-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metricspace-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metricspace-0.4.0.tar` & `metricspace-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       15 2023-05-31 03:34:59.307740 metricspace-0.4.0/.gitattributes
--rw-r--r--   0        0        0      207 2023-06-03 20:32:15.687932 metricspace-0.4.0/.gitignore
--rw-r--r--   0        0        0     1092 2023-06-03 20:34:39.576899 metricspace-0.4.0/LICENSE
--rw-r--r--   0        0        0     2516 2023-05-31 03:34:59.312741 metricspace-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 23:54:22.575801 metricspace-0.4.0/examples/ex_distances.py
--rw-r--r--   0        0        0      368 2023-06-03 20:42:47.249595 metricspace-0.4.0/metricspace.egg-info/PKG-INFO
--rw-r--r--   0        0        0      625 2023-06-03 20:42:47.271461 metricspace-0.4.0/metricspace.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-06-03 20:42:47.250297 metricspace-0.4.0/metricspace.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       12 2023-06-03 20:42:47.250297 metricspace-0.4.0/metricspace.egg-info/top_level.txt
--rw-r--r--   0        0        0      175 2023-06-03 20:42:23.565089 metricspace-0.4.0/metricspace/__init__.py
--rw-r--r--   0        0        0      310 2023-06-03 20:32:56.972513 metricspace-0.4.0/metricspace/entropy/__init__.py
--rw-r--r--   0        0        0      898 2023-06-03 20:27:52.969199 metricspace-0.4.0/metricspace/entropy/histbi.py
--rw-r--r--   0        0        0      540 2023-06-03 20:27:52.969199 metricspace-0.4.0/metricspace/entropy/histinfo.py
--rw-r--r--   0        0        0      687 2023-06-03 20:27:52.969915 metricspace-0.4.0/metricspace/entropy/histjabi.py
--rw-r--r--   0        0        0      703 2023-06-03 20:27:52.969915 metricspace-0.4.0/metricspace/entropy/histtpbi.py
--rw-r--r--   0        0        0      987 2023-06-03 20:27:52.970909 metricspace-0.4.0/metricspace/entropy/tblxbi.py
--rw-r--r--   0        0        0      405 2023-06-03 20:27:52.970909 metricspace-0.4.0/metricspace/entropy/tblxinfo.py
--rw-r--r--   0        0        0     1322 2023-06-03 20:27:52.970909 metricspace-0.4.0/metricspace/entropy/tblxtpbi.py
--rw-r--r--   0        0        0      119 2023-06-03 20:27:52.971909 metricspace-0.4.0/metricspace/model/__init__.py
--rw-r--r--   0        0        0       74 2023-06-03 20:27:52.972909 metricspace-0.4.0/metricspace/model/calculate_spkd/__init__.py
--rw-r--r--   0        0        0     7378 2023-06-03 20:27:52.972909 metricspace-0.4.0/metricspace/model/calculate_spkd/spkd_functions.py
--rw-r--r--   0        0        0     6263 2023-06-03 20:27:52.972909 metricspace-0.4.0/metricspace/model/distclust.py
--rw-r--r--   0        0        0     1447 2023-06-03 20:27:52.973910 metricspace-0.4.0/metricspace/model/spkd.py
--rw-r--r--   0        0        0      851 2023-06-03 22:56:08.046083 metricspace-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       49 2023-06-03 19:43:56.794865 metricspace-0.4.0/requirements.txt
--rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 metricspace-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-31 03:34:59.307740 metricspace-0.5.0/.gitattributes
+-rw-r--r--   0        0        0      207 2023-06-03 20:32:15.687932 metricspace-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1092 2023-06-03 20:34:39.576899 metricspace-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4121 2023-06-04 00:01:05.996089 metricspace-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 23:54:22.575801 metricspace-0.5.0/examples/ex_distances.py
+-rw-r--r--   0        0        0      368 2023-06-03 20:42:47.249595 metricspace-0.5.0/metricspace.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      625 2023-06-03 20:42:47.271461 metricspace-0.5.0/metricspace.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-06-03 20:42:47.250297 metricspace-0.5.0/metricspace.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       12 2023-06-03 20:42:47.250297 metricspace-0.5.0/metricspace.egg-info/top_level.txt
+-rw-r--r--   0        0        0      175 2023-06-03 20:42:23.565089 metricspace-0.5.0/metricspace/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-03 20:32:56.972513 metricspace-0.5.0/metricspace/entropy/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-03 20:27:52.969199 metricspace-0.5.0/metricspace/entropy/histbi.py
+-rw-r--r--   0        0        0      540 2023-06-03 20:27:52.969199 metricspace-0.5.0/metricspace/entropy/histinfo.py
+-rw-r--r--   0        0        0      687 2023-06-03 20:27:52.969915 metricspace-0.5.0/metricspace/entropy/histjabi.py
+-rw-r--r--   0        0        0      703 2023-06-03 20:27:52.969915 metricspace-0.5.0/metricspace/entropy/histtpbi.py
+-rw-r--r--   0        0        0      987 2023-06-03 20:27:52.970909 metricspace-0.5.0/metricspace/entropy/tblxbi.py
+-rw-r--r--   0        0        0      405 2023-06-03 20:27:52.970909 metricspace-0.5.0/metricspace/entropy/tblxinfo.py
+-rw-r--r--   0        0        0     1322 2023-06-03 20:27:52.970909 metricspace-0.5.0/metricspace/entropy/tblxtpbi.py
+-rw-r--r--   0        0        0      119 2023-06-03 20:27:52.971909 metricspace-0.5.0/metricspace/model/__init__.py
+-rw-r--r--   0        0        0       74 2023-06-03 20:27:52.972909 metricspace-0.5.0/metricspace/model/calculate_spkd/__init__.py
+-rw-r--r--   0        0        0     7378 2023-06-03 20:27:52.972909 metricspace-0.5.0/metricspace/model/calculate_spkd/spkd_functions.py
+-rw-r--r--   0        0        0     6263 2023-06-03 20:27:52.972909 metricspace-0.5.0/metricspace/model/distclust.py
+-rw-r--r--   0        0        0     1447 2023-06-03 20:27:52.973910 metricspace-0.5.0/metricspace/model/spkd.py
+-rw-r--r--   0        0        0      853 2023-06-04 00:03:20.640991 metricspace-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-06-03 19:43:56.794865 metricspace-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 metricspace-0.5.0/PKG-INFO
```

### Comparing `metricspace-0.4.0/LICENSE` & `metricspace-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace.egg-info/SOURCES.txt` & `metricspace-0.5.0/metricspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/entropy/histbi.py` & `metricspace-0.5.0/metricspace/entropy/histbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/entropy/histinfo.py` & `metricspace-0.5.0/metricspace/entropy/histinfo.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/entropy/histjabi.py` & `metricspace-0.5.0/metricspace/entropy/histjabi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/entropy/histtpbi.py` & `metricspace-0.5.0/metricspace/entropy/histtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/entropy/tblxbi.py` & `metricspace-0.5.0/metricspace/entropy/tblxbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/entropy/tblxtpbi.py` & `metricspace-0.5.0/metricspace/entropy/tblxtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/model/calculate_spkd/spkd_functions.py` & `metricspace-0.5.0/metricspace/model/calculate_spkd/spkd_functions.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/model/distclust.py` & `metricspace-0.5.0/metricspace/model/distclust.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/metricspace/model/spkd.py` & `metricspace-0.5.0/metricspace/model/spkd.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.4.0/pyproject.toml` & `metricspace-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metricspace"
-version = "0.4.0"
+version = "0.5.0"
 description = "A python translation of code originally theorized in: Metric-space analysis of spike trains: theory, algorithms, and application Jonathan D. Victor and Keith Purpura Network 8, 127-164 (1997)"
 authors = [
     {name = "Flynn OConnell", email = "flynnoconnell@gmail.com"},
     {name = "Jonathan D Victor", email = "jdvicto@med.cornell.edu"}
 ]
+
 readme = "README.md"
 homepage = "https://github.com/NeuroPyPy/metricspace"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

