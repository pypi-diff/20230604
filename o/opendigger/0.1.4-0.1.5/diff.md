# Comparing `tmp/opendigger-0.1.4.tar.gz` & `tmp/opendigger-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opendigger-0.1.4.tar", last modified: Sat Jun  3 11:46:13 2023, max compression
+gzip compressed data, was "opendigger-0.1.5.tar", last modified: Sat Jun  3 11:48:45 2023, max compression
```

## Comparing `opendigger-0.1.4.tar` & `opendigger-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:46:13.002182 opendigger-0.1.4/
--rw-r--r--   0 tangyue    (501) staff       (20)     1068 2023-06-02 11:20:46.000000 opendigger-0.1.4/LICENSE
--rw-r--r--   0 tangyue    (501) staff       (20)       33 2023-06-02 11:15:07.000000 opendigger-0.1.4/MANIFEST.in
--rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:46:13.001854 opendigger-0.1.4/PKG-INFO
--rw-r--r--   0 tangyue    (501) staff       (20)        0 2023-06-02 11:19:50.000000 opendigger-0.1.4/README.md
-drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:46:13.000558 opendigger-0.1.4/opendigger/
--rw-r--r--   0 tangyue    (501) staff       (20)       27 2023-06-03 11:19:25.000000 opendigger-0.1.4/opendigger/__init__.py
--rw-r--r--   0 tangyue    (501) staff       (20)    11829 2023-06-03 11:32:49.000000 opendigger-0.1.4/opendigger/opendigger.py
-drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:46:13.001617 opendigger-0.1.4/opendigger.egg-info/
--rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:46:12.000000 opendigger-0.1.4/opendigger.egg-info/PKG-INFO
--rw-r--r--   0 tangyue    (501) staff       (20)      292 2023-06-03 11:46:12.000000 opendigger-0.1.4/opendigger.egg-info/SOURCES.txt
--rw-r--r--   0 tangyue    (501) staff       (20)        1 2023-06-03 11:46:12.000000 opendigger-0.1.4/opendigger.egg-info/dependency_links.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       47 2023-06-03 11:46:12.000000 opendigger-0.1.4/opendigger.egg-info/entry_points.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       25 2023-06-03 11:46:12.000000 opendigger-0.1.4/opendigger.egg-info/requires.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       11 2023-06-03 11:46:12.000000 opendigger-0.1.4/opendigger.egg-info/top_level.txt
--rw-r--r--   0 tangyue    (501) staff       (20)       38 2023-06-03 11:46:13.002252 opendigger-0.1.4/setup.cfg
--rw-r--r--   0 tangyue    (501) staff       (20)      905 2023-06-03 11:45:59.000000 opendigger-0.1.4/setup.py
+drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:48:45.968253 opendigger-0.1.5/
+-rw-r--r--   0 tangyue    (501) staff       (20)     1068 2023-06-02 11:20:46.000000 opendigger-0.1.5/LICENSE
+-rw-r--r--   0 tangyue    (501) staff       (20)       33 2023-06-02 11:15:07.000000 opendigger-0.1.5/MANIFEST.in
+-rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:48:45.967929 opendigger-0.1.5/PKG-INFO
+-rw-r--r--   0 tangyue    (501) staff       (20)        0 2023-06-02 11:19:50.000000 opendigger-0.1.5/README.md
+drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:48:45.966529 opendigger-0.1.5/opendigger/
+-rw-r--r--   0 tangyue    (501) staff       (20)        0 2023-06-03 11:48:40.000000 opendigger-0.1.5/opendigger/__init__.py
+-rw-r--r--   0 tangyue    (501) staff       (20)    11829 2023-06-03 11:32:49.000000 opendigger-0.1.5/opendigger/opendigger.py
+drwxr-xr-x   0 tangyue    (501) staff       (20)        0 2023-06-03 11:48:45.967711 opendigger-0.1.5/opendigger.egg-info/
+-rw-r--r--   0 tangyue    (501) staff       (20)      617 2023-06-03 11:48:45.000000 opendigger-0.1.5/opendigger.egg-info/PKG-INFO
+-rw-r--r--   0 tangyue    (501) staff       (20)      292 2023-06-03 11:48:45.000000 opendigger-0.1.5/opendigger.egg-info/SOURCES.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)        1 2023-06-03 11:48:45.000000 opendigger-0.1.5/opendigger.egg-info/dependency_links.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       58 2023-06-03 11:48:45.000000 opendigger-0.1.5/opendigger.egg-info/entry_points.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       25 2023-06-03 11:48:45.000000 opendigger-0.1.5/opendigger.egg-info/requires.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       11 2023-06-03 11:48:45.000000 opendigger-0.1.5/opendigger.egg-info/top_level.txt
+-rw-r--r--   0 tangyue    (501) staff       (20)       38 2023-06-03 11:48:45.968333 opendigger-0.1.5/setup.cfg
+-rw-r--r--   0 tangyue    (501) staff       (20)      916 2023-06-03 11:48:40.000000 opendigger-0.1.5/setup.py
```

### Comparing `opendigger-0.1.4/LICENSE` & `opendigger-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opendigger-0.1.4/PKG-INFO` & `opendigger-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendigger
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool for fetching OpenDigger metrics
 Home-page: https://github.com/TOMYUE/opendigger-cli
 Author: TOMYUE
 Author-email: tomyue2002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opendigger-0.1.4/opendigger/opendigger.py` & `opendigger-0.1.5/opendigger/opendigger.py`

 * *Files identical despite different names*

### Comparing `opendigger-0.1.4/opendigger.egg-info/PKG-INFO` & `opendigger-0.1.5/opendigger.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendigger
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool for fetching OpenDigger metrics
 Home-page: https://github.com/TOMYUE/opendigger-cli
 Author: TOMYUE
 Author-email: tomyue2002@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `opendigger-0.1.4/setup.py` & `opendigger-0.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="opendigger",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "plotext",
         "matplotlib",
     ],
     entry_points={
         "console_scripts": [
-            "opendigger = opendigger:main",
+            "opendigger = opendigger.opendigger:main",
         ],
     },
     author="TOMYUE",
     author_email="tomyue2002@gmail.com",
     description="A CLI tool for fetching OpenDigger metrics",
     url="https://github.com/TOMYUE/opendigger-cli",
     classifiers=[
```

