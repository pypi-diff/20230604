# Comparing `tmp/pyloggor-1.1.3.tar.gz` & `tmp/pyloggor-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloggor-1.1.3.tar", last modified: Wed May 17 17:28:43 2023, max compression
+gzip compressed data, was "pyloggor-1.1.4.tar", last modified: Sun Jun  4 19:46:17 2023, max compression
```

## Comparing `pyloggor-1.1.3.tar` & `pyloggor-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:28:43.310967 pyloggor-1.1.3/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 17:28:43.310464 pyloggor-1.1.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:28:43.305507 pyloggor-1.1.3/pyloggor/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.3/pyloggor/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7431 2023-05-17 17:27:06.000000 pyloggor-1.1.3/pyloggor/pyloggor.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 17:28:43.309523 pyloggor-1.1.3/pyloggor.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     6134 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      227 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2023-05-17 17:28:43.000000 pyloggor-1.1.3/pyloggor.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-17 17:28:43.311121 pyloggor-1.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      640 2023-05-17 17:27:59.000000 pyloggor-1.1.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 19:46:17.266557 pyloggor-1.1.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-09 10:25:32.000000 pyloggor-1.1.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-06-04 19:46:17.265771 pyloggor-1.1.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5673 2023-05-09 10:25:30.000000 pyloggor-1.1.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 19:46:17.258958 pyloggor-1.1.4/pyloggor/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-05-09 10:25:30.000000 pyloggor-1.1.4/pyloggor/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7408 2023-06-04 19:45:36.000000 pyloggor-1.1.4/pyloggor/pyloggor.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-04 19:46:17.264333 pyloggor-1.1.4/pyloggor.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     6134 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      196 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2023-06-04 19:46:17.000000 pyloggor-1.1.4/pyloggor.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-06-04 19:46:17.266877 pyloggor-1.1.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      609 2023-06-04 19:45:11.000000 pyloggor-1.1.4/setup.py
```

### Comparing `pyloggor-1.1.3/LICENSE` & `pyloggor-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.3/PKG-INFO` & `pyloggor-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.3
+Version: 1.1.4
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
```

### Comparing `pyloggor-1.1.3/README.md` & `pyloggor-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyloggor-1.1.3/pyloggor/pyloggor.py` & `pyloggor-1.1.4/pyloggor/pyloggor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import inspect
 import os
 import threading
 import time
 from datetime import datetime
 from typing import Literal, Optional
 
-import pytz
-
 
 class FileHandler:
     def __init__(self, fn, log_freq):
         self.log_freq = log_freq
         self.fn = fn
         self.cache = []
         open(fn, "w") if not os.path.exists(fn) else ...
@@ -131,15 +129,15 @@
         msg="NoMessage",  # I don't know why people do this
         extras: Optional[dict] = None,
         console_output: bool = None,
         file_output: bool = None,
     ):
         level = level.title() if self.title_level else level.upper()
 
-        time_str = datetime.fromtimestamp(time.time(), tz=pytz.UTC).strftime(self.datefmt)
+        time_str = datetime.utcfromtimestamp(time.time()).strftime(self.datefmt)
 
         if extras:
             extras_str = f"{self.delim} {self.extras_builder(extras)}"
         else:
             extras_str = ""
 
         if level in self.level_symbols.keys():
```

### Comparing `pyloggor-1.1.3/pyloggor.egg-info/PKG-INFO` & `pyloggor-1.1.4/pyloggor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloggor
-Version: 1.1.3
+Version: 1.1.4
 Summary: An incredibly versatile yet simple logging system.
 Home-page: https://www.github.com/PrivatePandaCO/pyloggor
 Author: Parth Mittal
 Author-email: parth@privatepanda.co
 License: MIT
 Project-URL: Documentation, https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md
 Project-URL: Github, https://github.com/PrivatePandaCO/pyloggor
```

### Comparing `pyloggor-1.1.3/setup.py` & `pyloggor-1.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from distutils.core import setup
 
 setup(
     name="pyloggor",
-    version="1.1.3",
+    version="1.1.4",
     description="An incredibly versatile yet simple logging system.",
     author="Parth Mittal",
     author_email="parth@privatepanda.co",
     url="https://www.github.com/PrivatePandaCO/pyloggor",
     license="MIT",
     packages=["pyloggor"],
-    install_requires=["pytz"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://github.com/PrivatePandaCO/pyloggor/blob/master/README.md",
         "Github": "https://github.com/PrivatePandaCO/pyloggor",
     },
 )
```

