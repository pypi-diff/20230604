# Comparing `tmp/rest_helper-0.0.2.tar.gz` & `tmp/rest_helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_helper-0.0.2.tar", last modified: Sun Jun  4 13:35:26 2023, max compression
+gzip compressed data, was "rest_helper-0.0.3.tar", last modified: Sun Jun  4 13:38:26 2023, max compression
```

## Comparing `rest_helper-0.0.2.tar` & `rest_helper-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:35:26.001877 rest_helper-0.0.2/
--rw-r--r--   0 norbertgocze   (502) staff       (20)     1060 2023-06-04 13:16:35.000000 rest_helper-0.0.2/LICENSE
--rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:35:26.001725 rest_helper-0.0.2/PKG-INFO
--rw-r--r--   0 norbertgocze   (502) staff       (20)      755 2023-06-04 13:14:43.000000 rest_helper-0.0.2/README.md
-drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:35:26.000655 rest_helper-0.0.2/rest_helper/
--rw-r--r--   0 norbertgocze   (502) staff       (20)       26 2023-06-04 13:31:36.000000 rest_helper-0.0.2/rest_helper/__init__.py
--rw-r--r--   0 norbertgocze   (502) staff       (20)     2698 2023-06-04 13:14:43.000000 rest_helper-0.0.2/rest_helper/rest_helper.py
-drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:35:26.001542 rest_helper-0.0.2/rest_helper.egg-info/
--rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/PKG-INFO
--rw-r--r--   0 norbertgocze   (502) staff       (20)      251 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/SOURCES.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)        1 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/dependency_links.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)        7 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/requires.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)       12 2023-06-04 13:35:25.000000 rest_helper-0.0.2/rest_helper.egg-info/top_level.txt
--rw-r--r--   0 norbertgocze   (502) staff       (20)       38 2023-06-04 13:35:26.001911 rest_helper-0.0.2/setup.cfg
--rw-r--r--   0 norbertgocze   (502) staff       (20)      612 2023-06-04 13:35:23.000000 rest_helper-0.0.2/setup.py
+drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:38:26.825139 rest_helper-0.0.3/
+-rw-r--r--   0 norbertgocze   (502) staff       (20)     1060 2023-06-04 13:16:35.000000 rest_helper-0.0.3/LICENSE
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:38:26.825024 rest_helper-0.0.3/PKG-INFO
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      755 2023-06-04 13:14:43.000000 rest_helper-0.0.3/README.md
+drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:38:26.824101 rest_helper-0.0.3/rest_helper/
+-rw-r--r--   0 norbertgocze   (502) staff       (20)       27 2023-06-04 13:37:10.000000 rest_helper-0.0.3/rest_helper/__init__.py
+-rw-r--r--   0 norbertgocze   (502) staff       (20)     2698 2023-06-04 13:14:43.000000 rest_helper-0.0.3/rest_helper/rest_helper.py
+drwxr-xr-x   0 norbertgocze   (502) staff       (20)        0 2023-06-04 13:38:26.824858 rest_helper-0.0.3/rest_helper.egg-info/
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      277 2023-06-04 13:38:26.000000 rest_helper-0.0.3/rest_helper.egg-info/PKG-INFO
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      251 2023-06-04 13:38:26.000000 rest_helper-0.0.3/rest_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)        1 2023-06-04 13:38:26.000000 rest_helper-0.0.3/rest_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)        7 2023-06-04 13:38:26.000000 rest_helper-0.0.3/rest_helper.egg-info/requires.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)       12 2023-06-04 13:38:26.000000 rest_helper-0.0.3/rest_helper.egg-info/top_level.txt
+-rw-r--r--   0 norbertgocze   (502) staff       (20)       38 2023-06-04 13:38:26.825173 rest_helper-0.0.3/setup.cfg
+-rw-r--r--   0 norbertgocze   (502) staff       (20)      612 2023-06-04 13:38:21.000000 rest_helper-0.0.3/setup.py
```

### Comparing `rest_helper-0.0.2/LICENSE` & `rest_helper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_helper-0.0.2/README.md` & `rest_helper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rest_helper-0.0.2/rest_helper/rest_helper.py` & `rest_helper-0.0.3/rest_helper/rest_helper.py`

 * *Files identical despite different names*

### Comparing `rest_helper-0.0.2/setup.py` & `rest_helper-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'docopt',
 ]
 
 
 setup(
     author='Norbert Gocze',
     author_email='gnorbi951@gmail.com',
-    version='0.0.2',
+    version='0.0.3',
     python_requires=python_version,
     description="Utility tool used for parsing specific .ini files",
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords='rest_helper',
     name='rest_helper',
     packages=packages,
```

