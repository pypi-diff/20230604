# Comparing `tmp/coolpy-0.0.50.tar.gz` & `tmp/coolpy-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpy-0.0.50.tar", last modified: Fri Mar  3 13:44:19 2023, max compression
+gzip compressed data, was "coolpy-0.0.51.tar", last modified: Sun Jun  4 12:41:25 2023, max compression
```

## Comparing `coolpy-0.0.50.tar` & `coolpy-0.0.51.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-03-03 13:44:19.808375 coolpy-0.0.50/
--rw-r--r--   0 bernd      (501) staff       (20)     1206 2023-03-03 13:44:19.807913 coolpy-0.0.50/PKG-INFO
--rw-r--r--   0 bernd      (501) staff       (20)      436 2022-02-20 13:45:18.000000 coolpy-0.0.50/README.md
--rw-r--r--   0 bernd      (501) staff       (20)       38 2023-03-03 13:44:19.808645 coolpy-0.0.50/setup.cfg
--rw-r--r--   0 bernd      (501) staff       (20)     1255 2023-03-03 13:42:47.000000 coolpy-0.0.50/setup.py
-drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-03-03 13:44:19.803353 coolpy-0.0.50/src/
-drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-03-03 13:44:19.807399 coolpy-0.0.50/src/coolpy.egg-info/
--rw-r--r--   0 bernd      (501) staff       (20)     1206 2023-03-03 13:44:19.000000 coolpy-0.0.50/src/coolpy.egg-info/PKG-INFO
--rw-r--r--   0 bernd      (501) staff       (20)      187 2023-03-03 13:44:19.000000 coolpy-0.0.50/src/coolpy.egg-info/SOURCES.txt
--rw-r--r--   0 bernd      (501) staff       (20)        1 2023-03-03 13:44:19.000000 coolpy-0.0.50/src/coolpy.egg-info/dependency_links.txt
--rw-r--r--   0 bernd      (501) staff       (20)       65 2023-03-03 13:44:19.000000 coolpy-0.0.50/src/coolpy.egg-info/requires.txt
--rw-r--r--   0 bernd      (501) staff       (20)       11 2023-03-03 13:44:19.000000 coolpy-0.0.50/src/coolpy.egg-info/top_level.txt
+drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:41:25.558397 coolpy-0.0.51/
+-rw-r--r--   0 bernd      (501) staff       (20)     1158 2023-06-04 12:41:25.558163 coolpy-0.0.51/PKG-INFO
+-rw-r--r--   0 bernd      (501) staff       (20)      436 2022-02-20 13:45:18.000000 coolpy-0.0.51/README.md
+-rw-r--r--   0 bernd      (501) staff       (20)       38 2023-06-04 12:41:25.558512 coolpy-0.0.51/setup.cfg
+-rw-r--r--   0 bernd      (501) staff       (20)     1208 2023-06-04 12:39:33.000000 coolpy-0.0.51/setup.py
+drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:41:25.555021 coolpy-0.0.51/src/
+drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:41:25.557770 coolpy-0.0.51/src/coolpy.egg-info/
+-rw-r--r--   0 bernd      (501) staff       (20)     1158 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/PKG-INFO
+-rw-r--r--   0 bernd      (501) staff       (20)      187 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/SOURCES.txt
+-rw-r--r--   0 bernd      (501) staff       (20)        1 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/dependency_links.txt
+-rw-r--r--   0 bernd      (501) staff       (20)       65 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/requires.txt
+-rw-r--r--   0 bernd      (501) staff       (20)       11 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/top_level.txt
```

### Comparing `coolpy-0.0.50/PKG-INFO` & `coolpy-0.0.51/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: coolpy
-Version: 0.0.50
+Version: 0.0.51
 Summary: Muon ionization simulation program
 Home-page: https://github.com/BerndStechauner/coolpy
 Author: Bernd Stechauner
 Author-email: bernd.stechauner@cern.ch
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: iOS
```

### Comparing `coolpy-0.0.50/setup.py` & `coolpy-0.0.51/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='coolpy',
-    version='0.0.50',
+    version='0.0.51',
     description='Muon ionization simulation program',
     py_modules=["quadrupole"],
     package_dir={'': 'src'},
     classifiers =[
         "Natural Language :: English",
-        "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
         "Operating System :: OS Independent",
         "Operating System :: iOS",
```

### Comparing `coolpy-0.0.50/src/coolpy.egg-info/PKG-INFO` & `coolpy-0.0.51/src/coolpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: coolpy
-Version: 0.0.50
+Version: 0.0.51
 Summary: Muon ionization simulation program
 Home-page: https://github.com/BerndStechauner/coolpy
 Author: Bernd Stechauner
 Author-email: bernd.stechauner@cern.ch
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: iOS
```

