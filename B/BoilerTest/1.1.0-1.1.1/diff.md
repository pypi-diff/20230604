# Comparing `tmp/BoilerTest-1.1.0.tar.gz` & `tmp/BoilerTest-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BoilerTest-1.1.0.tar", last modified: Sat Jun  3 23:36:11 2023, max compression
+gzip compressed data, was "BoilerTest-1.1.1.tar", last modified: Sat Jun  3 23:53:19 2023, max compression
```

## Comparing `BoilerTest-1.1.0.tar` & `BoilerTest-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 23:36:11.199759 BoilerTest-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-03 23:36:11.146040 BoilerTest-1.1.0/BoilerTest/
--rw-rw-rw-   0        0        0     6061 2023-06-03 23:19:58.000000 BoilerTest-1.1.0/BoilerTest/BoilerTest.py
--rw-rw-rw-   0        0        0        0 2023-06-03 23:05:23.000000 BoilerTest-1.1.0/BoilerTest/__init__.py
--rw-rw-rw-   0        0        0      658 2023-06-03 23:10:18.000000 BoilerTest-1.1.0/BoilerTest/main.py
-drwxrwxrwx   0        0        0        0 2023-06-03 23:36:11.183058 BoilerTest-1.1.0/BoilerTest.egg-info/
--rw-rw-rw-   0        0        0      516 2023-06-03 23:36:10.000000 BoilerTest-1.1.0/BoilerTest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-03 23:36:11.000000 BoilerTest-1.1.0/BoilerTest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 23:36:10.000000 BoilerTest-1.1.0/BoilerTest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-03 23:36:10.000000 BoilerTest-1.1.0/BoilerTest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 23:36:10.000000 BoilerTest-1.1.0/BoilerTest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      516 2023-06-03 23:36:11.189051 BoilerTest-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-06-03 22:23:50.000000 BoilerTest-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-03 23:36:11.200259 BoilerTest-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-06-03 23:34:40.000000 BoilerTest-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:53:19.059896 BoilerTest-1.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-03 23:53:19.007589 BoilerTest-1.1.1/BoilerTest/
+-rw-rw-rw-   0        0        0     6061 2023-06-03 23:19:58.000000 BoilerTest-1.1.1/BoilerTest/BoilerTest.py
+-rw-rw-rw-   0        0        0        0 2023-06-03 23:05:23.000000 BoilerTest-1.1.1/BoilerTest/__init__.py
+-rw-rw-rw-   0        0        0      658 2023-06-03 23:10:18.000000 BoilerTest-1.1.1/BoilerTest/main.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:53:19.045445 BoilerTest-1.1.1/BoilerTest.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-06-03 23:53:18.000000 BoilerTest-1.1.1/BoilerTest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-03 23:53:18.000000 BoilerTest-1.1.1/BoilerTest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 23:53:18.000000 BoilerTest-1.1.1/BoilerTest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-03 23:53:18.000000 BoilerTest-1.1.1/BoilerTest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-06-03 23:53:18.000000 BoilerTest-1.1.1/BoilerTest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      516 2023-06-03 23:53:19.051064 BoilerTest-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2023-06-03 22:23:50.000000 BoilerTest-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-03 23:53:19.060019 BoilerTest-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      770 2023-06-03 23:53:06.000000 BoilerTest-1.1.1/setup.py
```

### Comparing `BoilerTest-1.1.0/BoilerTest/BoilerTest.py` & `BoilerTest-1.1.1/BoilerTest/BoilerTest.py`

 * *Files identical despite different names*

### Comparing `BoilerTest-1.1.0/BoilerTest/main.py` & `BoilerTest-1.1.1/BoilerTest/main.py`

 * *Files identical despite different names*

### Comparing `BoilerTest-1.1.0/BoilerTest.egg-info/PKG-INFO` & `BoilerTest-1.1.1/BoilerTest.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BoilerTest
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python test file generator
 Home-page: https://github.com/Juliusolsson05/BoilerTest.git
 Author: Julius Olsson
 Author-email: julius.olsson05@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `BoilerTest-1.1.0/PKG-INFO` & `BoilerTest-1.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BoilerTest
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python test file generator
 Home-page: https://github.com/Juliusolsson05/BoilerTest.git
 Author: Julius Olsson
 Author-email: julius.olsson05@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `BoilerTest-1.1.0/setup.py` & `BoilerTest-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name="BoilerTest",
-    version="1.1.0",
+    version="1.1.1",
     description="Python test file generator",
     long_description="A utility for automatically creating test files for Python classes",
     author="Julius Olsson",
     author_email="julius.olsson05@gmail.com",
     url="https://github.com/Juliusolsson05/BoilerTest.git",
     packages=["BoilerTest"],
     entry_points={
         "console_scripts": [
-            "boilertest=BoilerTest.main:main",
+            "boilertest=boiler_test.main:main",
         ],
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

