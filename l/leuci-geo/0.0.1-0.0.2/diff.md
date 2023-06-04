# Comparing `tmp/leuci-geo-0.0.1.tar.gz` & `tmp/leuci-geo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-geo-0.0.1.tar", last modified: Thu May 25 20:12:59 2023, max compression
+gzip compressed data, was "leuci-geo-0.0.2.tar", last modified: Sun Jun  4 14:01:08 2023, max compression
```

## Comparing `leuci-geo-0.0.1.tar` & `leuci-geo-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-05-25 20:12:59.322922 leuci-geo-0.0.1/
--rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.1/LICENSE
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-05-25 20:12:59.322922 leuci-geo-0.0.1/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.1/README.md
--rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.1/pyproject.toml
--rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-05-25 20:12:59.322922 leuci-geo-0.0.1/setup.cfg
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-05-25 20:12:59.312922 leuci-geo-0.0.1/src/
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-05-25 20:12:59.312922 leuci-geo-0.0.1/src/leuci_geo/
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.1/src/leuci_geo/__init__.py
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-05-25 20:12:59.322922 leuci-geo-0.0.1/src/leuci_geo.egg-info/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-05-25 20:12:59.000000 leuci-geo-0.0.1/src/leuci_geo.egg-info/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      216 2023-05-25 20:12:59.000000 leuci-geo-0.0.1/src/leuci_geo.egg-info/SOURCES.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-05-25 20:12:59.000000 leuci-geo-0.0.1/src/leuci_geo.egg-info/dependency_links.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-05-25 20:12:59.000000 leuci-geo-0.0.1/src/leuci_geo.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.2/LICENSE
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.2/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.2/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.480136 leuci-geo-0.0.2/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.480136 leuci-geo-0.0.2/src/leuci_geo/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.2/src/leuci_geo/__init__.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.2/src/leuci_geo/geocalculator.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    27001 2023-06-04 13:12:00.000000 leuci-geo-0.0.2/src/leuci_geo/pdbgeometry.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.2/src/leuci_geo/pdbloader.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.2/src/leuci_geo/pdbobject.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.2/src/leuci_geo/pdbspace.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/src/leuci_geo.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      356 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/top_level.txt
```

### Comparing `leuci-geo-0.0.1/LICENSE` & `leuci-geo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.1/PKG-INFO` & `leuci-geo-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.1
+Version: 0.0.2
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leuci-geo-0.0.1/setup.cfg` & `leuci-geo-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = leuci-geo
-version = 0.0.1
+version = 0.0.2
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = geometric paramaters and searches of protein structures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `leuci-geo-0.0.1/src/leuci_geo.egg-info/PKG-INFO` & `leuci-geo-0.0.2/src/leuci_geo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.1
+Version: 0.0.2
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

