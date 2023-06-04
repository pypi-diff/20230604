# Comparing `tmp/rest_helper-0.0.1.tar.gz` & `tmp/rest_helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_helper-0.0.1.tar", last modified: Sun Jun  4 13:27:21 2023, max compression
+gzip compressed data, was "rest_helper-0.0.2.tar", last modified: Sun Jun  4 13:35:26 2023, max compression
```

## Comparing `rest_helper-0.0.1.tar` & `rest_helper-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:27:21.835671 rest_helper-0.0.1/
--rw-r--r--   0 norbertgocze   (502) staff       (20)     1060 2023-06-04 13:16:35.000000 rest_helper-0.0.1/LICENSE
--rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:27:21.835559 rest_helper-0.0.1/PKG-INFO
--rw-r--r--   0 norbertgocze   (502) staff       (20)      755 2023-06-04 13:14:43.000000 rest_helper-0.0.1/README.md
-drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:27:21.834580 rest_helper-0.0.1/rest_helper/
--rw-r--r--   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:21:06.000000 rest_helper-0.0.1/rest_helper/__init__.py
--rw-r--r--   0 norbertgocze   (502) staff       (20)     2698 2023-06-04 13:14:43.000000 rest_helper-0.0.1/rest_helper/rest_helper.py
-drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:27:21.835399 rest_helper-0.0.1/rest_helper.egg-info/
--rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:27:21.000000 rest_helper-0.0.1/rest_helper.egg-info/PKG-INFO
--rw-r--r--   0 norbertgocze   (502) staff       (20)      251 2023-06-04 13:27:21.000000 rest_helper-0.0.1/rest_helper.egg-info/SOURCES.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)        1 2023-06-04 13:27:21.000000 rest_helper-0.0.1/rest_helper.egg-info/dependency_links.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)        7 2023-06-04 13:27:21.000000 rest_helper-0.0.1/rest_helper.egg-info/requires.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)       12 2023-06-04 13:27:21.000000 rest_helper-0.0.1/rest_helper.egg-info/top_level.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)       38 2023-06-04 13:27:21.835703 rest_helper-0.0.1/setup.cfg
--rw-r--r--   0 norbertgocze   (502) staff       (20)      612 2023-06-04 12:28:00.000000 rest_helper-0.0.1/setup.py
+drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:35:26.001877 rest_helper-0.0.2/
+-rw-r--r--   0 norbertgocze   (502) staff       (20)     1060 2023-06-04 13:16:35.000000 rest_helper-0.0.2/LICENSE
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:35:26.001725 rest_helper-0.0.2/PKG-INFO
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      755 2023-06-04 13:14:43.000000 rest_helper-0.0.2/README.md
+drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:35:26.000655 rest_helper-0.0.2/rest_helper/
+-rw-r--r--   0 norbertgocze   (502) staff       (20)       26 2023-06-04 13:31:36.000000 rest_helper-0.0.2/rest_helper/__init__.py
+-rw-r--r--   0 norbertgocze   (502) staff       (20)     2698 2023-06-04 13:14:43.000000 rest_helper-0.0.2/rest_helper/rest_helper.py
+drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:35:26.001542 rest_helper-0.0.2/rest_helper.egg-info/
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/PKG-INFO
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      251 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)        1 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)        7 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/requires.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)       12 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/top_level.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)       38 2023-06-04 13:35:26.001911 rest_helper-0.0.2/setup.cfg
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      612 2023-06-04 13:35:23.000000 rest_helper-0.0.2/setup.py
```

### Comparing `rest_helper-0.0.1/LICENSE` & `rest_helper-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_helper-0.0.1/README.md` & `rest_helper-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rest_helper-0.0.1/rest_helper/rest_helper.py` & `rest_helper-0.0.2/rest_helper/rest_helper.py`

 * *Files identical despite different names*

### Comparing `rest_helper-0.0.1/setup.py` & `rest_helper-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'docopt',
 ]
 
 
 setup(
     author='Norbert Gocze',
     author_email='gnorbi951@gmail.com',
-    version='0.0.1',
+    version='0.0.2',
     python_requires=python_version,
     description="Utility tool used for parsing specific .ini files",
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='rest_helper',
     name='rest_helper',
     packages=packages,
```

