# Comparing `tmp/metricspace-0.3.1.tar.gz` & `tmp/metricspace-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metricspace-0.3.1.tar", last modified: Sat Jun  3 20:42:47 2023, max compression
+gzip compressed data, was "metricspace-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metricspace-0.3.1.tar` & `metricspace-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 20:42:47.306568 metricspace-0.3.1/
--rw-rw-rw-   0        0        0     1092 2023-06-03 20:34:39.000000 metricspace-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      368 2023-06-03 20:42:47.306568 metricspace-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2516 2023-05-31 03:34:59.000000 metricspace-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 20:42:47.283180 metricspace-0.3.1/metricspace/
--rw-rw-rw-   0        0        0      175 2023-06-03 20:42:23.000000 metricspace-0.3.1/metricspace/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 20:42:47.300571 metricspace-0.3.1/metricspace/entropy/
--rw-rw-rw-   0        0        0      310 2023-06-03 20:32:56.000000 metricspace-0.3.1/metricspace/entropy/__init__.py
--rw-rw-rw-   0        0        0      898 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/histbi.py
--rw-rw-rw-   0        0        0      540 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/histinfo.py
--rw-rw-rw-   0        0        0      687 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/histjabi.py
--rw-rw-rw-   0        0        0      703 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/histtpbi.py
--rw-rw-rw-   0        0        0      987 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/tblxbi.py
--rw-rw-rw-   0        0        0      405 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/tblxinfo.py
--rw-rw-rw-   0        0        0     1322 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/entropy/tblxtpbi.py
-drwxrwxrwx   0        0        0        0 2023-06-03 20:42:47.303568 metricspace-0.3.1/metricspace/model/
--rw-rw-rw-   0        0        0      119 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 20:42:47.305568 metricspace-0.3.1/metricspace/model/calculate_spkd/
--rw-rw-rw-   0        0        0       74 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/model/calculate_spkd/__init__.py
--rw-rw-rw-   0        0        0     7378 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/model/calculate_spkd/spkd_functions.py
--rw-rw-rw-   0        0        0     6263 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/model/distclust.py
--rw-rw-rw-   0        0        0     1447 2023-06-03 20:27:52.000000 metricspace-0.3.1/metricspace/model/spkd.py
-drwxrwxrwx   0        0        0        0 2023-06-03 20:42:47.293489 metricspace-0.3.1/metricspace.egg-info/
--rw-rw-rw-   0        0        0      368 2023-06-03 20:42:47.000000 metricspace-0.3.1/metricspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-03 20:42:47.000000 metricspace-0.3.1/metricspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 20:42:47.000000 metricspace-0.3.1/metricspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-03 20:42:47.000000 metricspace-0.3.1/metricspace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 20:42:47.306568 metricspace-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      461 2023-06-03 20:42:45.000000 metricspace-0.3.1/setup.py
+-rw-r--r--   0        0        0       15 2023-05-31 03:34:59.307740 metricspace-0.4.0/.gitattributes
+-rw-r--r--   0        0        0      207 2023-06-03 20:32:15.687932 metricspace-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1092 2023-06-03 20:34:39.576899 metricspace-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2516 2023-05-31 03:34:59.312741 metricspace-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 23:54:22.575801 metricspace-0.4.0/examples/ex_distances.py
+-rw-r--r--   0        0        0      368 2023-06-03 20:42:47.249595 metricspace-0.4.0/metricspace.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      625 2023-06-03 20:42:47.271461 metricspace-0.4.0/metricspace.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-06-03 20:42:47.250297 metricspace-0.4.0/metricspace.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       12 2023-06-03 20:42:47.250297 metricspace-0.4.0/metricspace.egg-info/top_level.txt
+-rw-r--r--   0        0        0      175 2023-06-03 20:42:23.565089 metricspace-0.4.0/metricspace/__init__.py
+-rw-r--r--   0        0        0      310 2023-06-03 20:32:56.972513 metricspace-0.4.0/metricspace/entropy/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-03 20:27:52.969199 metricspace-0.4.0/metricspace/entropy/histbi.py
+-rw-r--r--   0        0        0      540 2023-06-03 20:27:52.969199 metricspace-0.4.0/metricspace/entropy/histinfo.py
+-rw-r--r--   0        0        0      687 2023-06-03 20:27:52.969915 metricspace-0.4.0/metricspace/entropy/histjabi.py
+-rw-r--r--   0        0        0      703 2023-06-03 20:27:52.969915 metricspace-0.4.0/metricspace/entropy/histtpbi.py
+-rw-r--r--   0        0        0      987 2023-06-03 20:27:52.970909 metricspace-0.4.0/metricspace/entropy/tblxbi.py
+-rw-r--r--   0        0        0      405 2023-06-03 20:27:52.970909 metricspace-0.4.0/metricspace/entropy/tblxinfo.py
+-rw-r--r--   0        0        0     1322 2023-06-03 20:27:52.970909 metricspace-0.4.0/metricspace/entropy/tblxtpbi.py
+-rw-r--r--   0        0        0      119 2023-06-03 20:27:52.971909 metricspace-0.4.0/metricspace/model/__init__.py
+-rw-r--r--   0        0        0       74 2023-06-03 20:27:52.972909 metricspace-0.4.0/metricspace/model/calculate_spkd/__init__.py
+-rw-r--r--   0        0        0     7378 2023-06-03 20:27:52.972909 metricspace-0.4.0/metricspace/model/calculate_spkd/spkd_functions.py
+-rw-r--r--   0        0        0     6263 2023-06-03 20:27:52.972909 metricspace-0.4.0/metricspace/model/distclust.py
+-rw-r--r--   0        0        0     1447 2023-06-03 20:27:52.973910 metricspace-0.4.0/metricspace/model/spkd.py
+-rw-r--r--   0        0        0      851 2023-06-03 22:56:08.046083 metricspace-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-06-03 19:43:56.794865 metricspace-0.4.0/requirements.txt
+-rw-r--r--   0        0        0     3069 1970-01-01 00:00:00.000000 metricspace-0.4.0/PKG-INFO
```

### Comparing `metricspace-0.3.1/LICENSE` & `metricspace-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/README.md` & `metricspace-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/entropy/histbi.py` & `metricspace-0.4.0/metricspace/entropy/histbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/entropy/histinfo.py` & `metricspace-0.4.0/metricspace/entropy/histinfo.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/entropy/histjabi.py` & `metricspace-0.4.0/metricspace/entropy/histjabi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/entropy/histtpbi.py` & `metricspace-0.4.0/metricspace/entropy/histtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/entropy/tblxbi.py` & `metricspace-0.4.0/metricspace/entropy/tblxbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/entropy/tblxtpbi.py` & `metricspace-0.4.0/metricspace/entropy/tblxtpbi.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/model/calculate_spkd/spkd_functions.py` & `metricspace-0.4.0/metricspace/model/calculate_spkd/spkd_functions.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/model/distclust.py` & `metricspace-0.4.0/metricspace/model/distclust.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace/model/spkd.py` & `metricspace-0.4.0/metricspace/model/spkd.py`

 * *Files identical despite different names*

### Comparing `metricspace-0.3.1/metricspace.egg-info/SOURCES.txt` & `metricspace-0.4.0/metricspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

