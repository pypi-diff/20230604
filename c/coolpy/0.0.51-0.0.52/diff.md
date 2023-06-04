# Comparing `tmp/coolpy-0.0.51.tar.gz` & `tmp/coolpy-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpy-0.0.51.tar", last modified: Sun Jun  4 12:41:25 2023, max compression
+gzip compressed data, was "coolpy-0.0.52.tar", last modified: Sun Jun  4 12:51:45 2023, max compression
```

## Comparing `coolpy-0.0.51.tar` & `coolpy-0.0.52.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:41:25.558397 coolpy-0.0.51/
--rw-r--r--   0 bernd      (501) staff       (20)     1158 2023-06-04 12:41:25.558163 coolpy-0.0.51/PKG-INFO
--rw-r--r--   0 bernd      (501) staff       (20)      436 2022-02-20 13:45:18.000000 coolpy-0.0.51/README.md
--rw-r--r--   0 bernd      (501) staff       (20)       38 2023-06-04 12:41:25.558512 coolpy-0.0.51/setup.cfg
--rw-r--r--   0 bernd      (501) staff       (20)     1208 2023-06-04 12:39:33.000000 coolpy-0.0.51/setup.py
-drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:41:25.555021 coolpy-0.0.51/src/
-drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:41:25.557770 coolpy-0.0.51/src/coolpy.egg-info/
--rw-r--r--   0 bernd      (501) staff       (20)     1158 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/PKG-INFO
--rw-r--r--   0 bernd      (501) staff       (20)      187 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/SOURCES.txt
--rw-r--r--   0 bernd      (501) staff       (20)        1 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/dependency_links.txt
--rw-r--r--   0 bernd      (501) staff       (20)       65 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/requires.txt
--rw-r--r--   0 bernd      (501) staff       (20)       11 2023-06-04 12:41:25.000000 coolpy-0.0.51/src/coolpy.egg-info/top_level.txt
+drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:51:45.808601 coolpy-0.0.52/
+-rw-r--r--   0 bernd      (501) staff       (20)     1205 2023-06-04 12:51:45.808331 coolpy-0.0.52/PKG-INFO
+-rw-r--r--   0 bernd      (501) staff       (20)      436 2022-02-20 13:45:18.000000 coolpy-0.0.52/README.md
+-rw-r--r--   0 bernd      (501) staff       (20)       38 2023-06-04 12:51:45.808772 coolpy-0.0.52/setup.cfg
+-rw-r--r--   0 bernd      (501) staff       (20)     1254 2023-06-04 12:50:34.000000 coolpy-0.0.52/setup.py
+drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:51:45.805238 coolpy-0.0.52/src/
+drwxr-xr-x   0 bernd      (501) staff       (20)        0 2023-06-04 12:51:45.807889 coolpy-0.0.52/src/coolpy.egg-info/
+-rw-r--r--   0 bernd      (501) staff       (20)     1205 2023-06-04 12:51:45.000000 coolpy-0.0.52/src/coolpy.egg-info/PKG-INFO
+-rw-r--r--   0 bernd      (501) staff       (20)      187 2023-06-04 12:51:45.000000 coolpy-0.0.52/src/coolpy.egg-info/SOURCES.txt
+-rw-r--r--   0 bernd      (501) staff       (20)        1 2023-06-04 12:51:45.000000 coolpy-0.0.52/src/coolpy.egg-info/dependency_links.txt
+-rw-r--r--   0 bernd      (501) staff       (20)       65 2023-06-04 12:51:45.000000 coolpy-0.0.52/src/coolpy.egg-info/requires.txt
+-rw-r--r--   0 bernd      (501) staff       (20)       11 2023-06-04 12:51:45.000000 coolpy-0.0.52/src/coolpy.egg-info/top_level.txt
```

### Comparing `coolpy-0.0.51/PKG-INFO` & `coolpy-0.0.52/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: coolpy
-Version: 0.0.51
+Version: 0.0.52
 Summary: Muon ionization simulation program
 Home-page: https://github.com/BerndStechauner/coolpy
 Author: Bernd Stechauner
 Author-email: bernd.stechauner@cern.ch
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: iOS
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # coolpy
 
 This is a project demonstrating how publich a muon beam cooling module to PyPI
```

### Comparing `coolpy-0.0.51/setup.py` & `coolpy-0.0.52/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name='coolpy',
-    version='0.0.51',
+    version='0.0.52',
     description='Muon ionization simulation program',
     py_modules=["quadrupole"],
     package_dir={'': 'src'},
     classifiers =[
         "Natural Language :: English",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
         "Operating System :: OS Independent",
         "Operating System :: iOS",
         "Operating System :: MacOS",
+        "Operating System :: POSIX :: Linux",
         
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     install_requires = [
         "blessings ~= 1.7",
```

### Comparing `coolpy-0.0.51/src/coolpy.egg-info/PKG-INFO` & `coolpy-0.0.52/src/coolpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: coolpy
-Version: 0.0.51
+Version: 0.0.52
 Summary: Muon ionization simulation program
 Home-page: https://github.com/BerndStechauner/coolpy
 Author: Bernd Stechauner
 Author-email: bernd.stechauner@cern.ch
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: iOS
 Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # coolpy
 
 This is a project demonstrating how publich a muon beam cooling module to PyPI
```

