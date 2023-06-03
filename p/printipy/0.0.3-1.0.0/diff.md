# Comparing `tmp/printipy-0.0.3.tar.gz` & `tmp/printipy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "printipy-0.0.3.tar", last modified: Mon Mar 20 20:56:59 2023, max compression
+gzip compressed data, was "printipy-1.0.0.tar", last modified: Sat Jun  3 23:47:20 2023, max compression
```

## Comparing `printipy-0.0.3.tar` & `printipy-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:56:59.024531 printipy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-20 20:56:44.000000 printipy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-03-20 20:56:59.024531 printipy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-03-20 20:56:44.000000 printipy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:56:59.024531 printipy-0.0.3/printipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 20:56:44.000000 printipy-0.0.3/printipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28807 2023-03-20 20:56:44.000000 printipy-0.0.3/printipy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:56:59.024531 printipy-0.0.3/printipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-03-20 20:56:59.000000 printipy-0.0.3/printipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-20 20:56:59.000000 printipy-0.0.3/printipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 20:56:59.000000 printipy-0.0.3/printipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-20 20:56:59.000000 printipy-0.0.3/printipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 20:56:59.000000 printipy-0.0.3/printipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 20:56:59.024531 printipy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-03-20 20:56:44.000000 printipy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:47:20.834224 printipy-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-03 23:47:12.000000 printipy-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-03 23:47:20.834224 printipy-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-03 23:47:12.000000 printipy-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:47:20.834224 printipy-1.0.0/printipy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:47:12.000000 printipy-1.0.0/printipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71424 2023-06-03 23:47:12.000000 printipy-1.0.0/printipy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37420 2023-06-03 23:47:12.000000 printipy-1.0.0/printipy/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-03 23:47:12.000000 printipy-1.0.0/printipy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:47:20.834224 printipy-1.0.0/printipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-03 23:47:20.000000 printipy-1.0.0/printipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-03 23:47:20.000000 printipy-1.0.0/printipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:47:20.000000 printipy-1.0.0/printipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 23:47:20.000000 printipy-1.0.0/printipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 23:47:20.000000 printipy-1.0.0/printipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 23:47:20.834224 printipy-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-03 23:47:12.000000 printipy-1.0.0/setup.py
```

### Comparing `printipy-0.0.3/LICENSE` & `printipy-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `printipy-0.0.3/setup.py` & `printipy-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="printipy",
-    version="0.0.3",
+    version="1.0.0",
     author="Lawrence Weikum",
     description="Printify API for Python",
     url="https://github.com/lawrencemq/printipy",
     keywords=['printify', 'print on demand', 'api'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

