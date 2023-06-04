# Comparing `tmp/miskibin-1.1.3.tar.gz` & `tmp/miskibin-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miskibin-1.1.3.tar", last modified: Wed Feb 22 17:22:00 2023, max compression
+gzip compressed data, was "miskibin-1.2.0.tar", last modified: Sun Jun  4 13:23:54 2023, max compression
```

## Comparing `miskibin-1.1.3.tar` & `miskibin-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:22:00.767220 miskibin-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-02-22 17:22:00.767220 miskibin-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:22:00.767220 miskibin-1.1.3/miskibin/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-22 17:21:50.000000 miskibin-1.1.3/miskibin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-02-22 17:21:50.000000 miskibin-1.1.3/miskibin/_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-22 17:21:50.000000 miskibin-1.1.3/miskibin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 17:22:00.767220 miskibin-1.1.3/miskibin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-02-22 17:22:00.000000 miskibin-1.1.3/miskibin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-22 17:22:00.000000 miskibin-1.1.3/miskibin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 17:22:00.000000 miskibin-1.1.3/miskibin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 17:22:00.000000 miskibin-1.1.3/miskibin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 17:22:00.767220 miskibin-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-22 17:21:50.000000 miskibin-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:23:54.068455 miskibin-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-04 13:23:54.068455 miskibin-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:23:54.068455 miskibin-1.2.0/miskibin/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-04 13:23:37.000000 miskibin-1.2.0/miskibin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-04 13:23:37.000000 miskibin-1.2.0/miskibin/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-04 13:23:37.000000 miskibin-1.2.0/miskibin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:23:54.068455 miskibin-1.2.0/miskibin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-04 13:23:54.000000 miskibin-1.2.0/miskibin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-04 13:23:54.000000 miskibin-1.2.0/miskibin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:23:54.000000 miskibin-1.2.0/miskibin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 13:23:54.000000 miskibin-1.2.0/miskibin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:23:54.068455 miskibin-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-04 13:23:37.000000 miskibin-1.2.0/setup.py
```

### Comparing `miskibin-1.1.3/PKG-INFO` & `miskibin-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miskibin
-Version: 1.1.3
+Version: 1.2.0
 Summary: My personal package for colored logs. Highly customizable.
 Home-page: https://github.com/michalskibinski109/miskibin
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miskibin-1.1.3/miskibin/_logging_utils.py` & `miskibin-1.2.0/miskibin/_logging_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from logging import _Level
 
 
 class ColoredFormatter(logging.Formatter):
     def __init__(self, fmt, datefmt):
         super().__init__()
         self.fmt = fmt
         blue = "\x1b[0;34m"
```

### Comparing `miskibin-1.1.3/miskibin.egg-info/PKG-INFO` & `miskibin-1.2.0/miskibin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miskibin
-Version: 1.1.3
+Version: 1.2.0
 Summary: My personal package for colored logs. Highly customizable.
 Home-page: https://github.com/michalskibinski109/miskibin
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miskibin-1.1.3/setup.py` & `miskibin-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 <img src="https://user-images.githubusercontent.com/77834536/201939466-228b110f-21de-4461-9c86-55f8f46652ef.png" width="500"/>
 
 """
 
 setuptools.setup(
     name="miskibin",
-    version="1.1.3",
+    version="1.2.0",
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     description="My personal package for colored logs. Highly customizable.",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     files_to_include=["miskibin"],
     url="https://github.com/michalskibinski109/miskibin",
```

