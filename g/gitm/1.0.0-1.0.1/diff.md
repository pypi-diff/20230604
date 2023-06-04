# Comparing `tmp/gitm-1.0.0.tar.gz` & `tmp/gitm-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitm-1.0.0.tar", last modified: Sun Jun  4 19:58:45 2023, max compression
+gzip compressed data, was "gitm-1.0.1.tar", last modified: Sun Jun  4 20:14:43 2023, max compression
```

## Comparing `gitm-1.0.0.tar` & `gitm-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 19:58:45.464146 gitm-1.0.0/
--rw-r--r--   0 abb       (1000) abb       (1000)    11357 2023-02-28 00:36:32.000000 gitm-1.0.0/LICENSE
--rw-r--r--   0 abb       (1000) abb       (1000)    25168 2023-06-04 19:58:45.464146 gitm-1.0.0/PKG-INFO
--rw-r--r--   0 abb       (1000) abb       (1000)    11690 2023-06-04 19:42:31.000000 gitm-1.0.0/README.md
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 19:58:45.464146 gitm-1.0.0/gitm/
--rw-r--r--   0 abb       (1000) abb       (1000)       23 2023-02-28 01:31:51.000000 gitm-1.0.0/gitm/__init__.py
--rw-r--r--   0 abb       (1000) abb       (1000)     1485 2023-06-04 19:48:45.000000 gitm-1.0.0/gitm/__main__.py
--rw-r--r--   0 abb       (1000) abb       (1000)      528 2023-06-04 16:27:38.000000 gitm-1.0.0/gitm/connection.py
--rw-r--r--   0 abb       (1000) abb       (1000)      352 2023-06-04 16:05:52.000000 gitm-1.0.0/gitm/db.py
--rw-r--r--   0 abb       (1000) abb       (1000)    11161 2023-06-04 19:46:16.000000 gitm-1.0.0/gitm/pattern.py
-drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 19:58:45.464146 gitm-1.0.0/gitm.egg-info/
--rw-r--r--   0 abb       (1000) abb       (1000)    25168 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/PKG-INFO
--rw-r--r--   0 abb       (1000) abb       (1000)      291 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/SOURCES.txt
--rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/dependency_links.txt
--rw-r--r--   0 abb       (1000) abb       (1000)       43 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/entry_points.txt
--rw-r--r--   0 abb       (1000) abb       (1000)       42 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/requires.txt
--rw-r--r--   0 abb       (1000) abb       (1000)        5 2023-06-04 19:58:45.000000 gitm-1.0.0/gitm.egg-info/top_level.txt
--rw-r--r--   0 abb       (1000) abb       (1000)     1154 2023-06-04 19:41:11.000000 gitm-1.0.0/pyproject.toml
--rw-r--r--   0 abb       (1000) abb       (1000)       38 2023-06-04 19:58:45.464146 gitm-1.0.0/setup.cfg
--rw-r--r--   0 abb       (1000) abb       (1000)       38 2023-02-28 00:45:14.000000 gitm-1.0.0/setup.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 20:14:43.520710 gitm-1.0.1/
+-rw-r--r--   0 abb       (1000) abb       (1000)    11357 2023-02-28 00:36:32.000000 gitm-1.0.1/LICENSE
+-rw-r--r--   0 abb       (1000) abb       (1000)    25168 2023-06-04 20:14:43.520710 gitm-1.0.1/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)    11690 2023-06-04 19:42:31.000000 gitm-1.0.1/README.md
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 20:14:43.517375 gitm-1.0.1/gitm/
+-rw-r--r--   0 abb       (1000) abb       (1000)       23 2023-02-28 01:31:51.000000 gitm-1.0.1/gitm/__init__.py
+-rw-r--r--   0 abb       (1000) abb       (1000)     1486 2023-06-04 20:13:49.000000 gitm-1.0.1/gitm/__main__.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      528 2023-06-04 16:27:38.000000 gitm-1.0.1/gitm/connection.py
+-rw-r--r--   0 abb       (1000) abb       (1000)      352 2023-06-04 16:05:52.000000 gitm-1.0.1/gitm/db.py
+-rw-r--r--   0 abb       (1000) abb       (1000)    11161 2023-06-04 19:46:16.000000 gitm-1.0.1/gitm/pattern.py
+drwxr-xr-x   0 abb       (1000) abb       (1000)        0 2023-06-04 20:14:43.517375 gitm-1.0.1/gitm.egg-info/
+-rw-r--r--   0 abb       (1000) abb       (1000)    25168 2023-06-04 20:14:43.000000 gitm-1.0.1/gitm.egg-info/PKG-INFO
+-rw-r--r--   0 abb       (1000) abb       (1000)      291 2023-06-04 20:14:43.000000 gitm-1.0.1/gitm.egg-info/SOURCES.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        1 2023-06-04 20:14:43.000000 gitm-1.0.1/gitm.egg-info/dependency_links.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)       43 2023-06-04 20:14:43.000000 gitm-1.0.1/gitm.egg-info/entry_points.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)       42 2023-06-04 20:14:43.000000 gitm-1.0.1/gitm.egg-info/requires.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)        5 2023-06-04 20:14:43.000000 gitm-1.0.1/gitm.egg-info/top_level.txt
+-rw-r--r--   0 abb       (1000) abb       (1000)     1154 2023-06-04 20:13:58.000000 gitm-1.0.1/pyproject.toml
+-rw-r--r--   0 abb       (1000) abb       (1000)       38 2023-06-04 20:14:43.520710 gitm-1.0.1/setup.cfg
+-rw-r--r--   0 abb       (1000) abb       (1000)       38 2023-02-28 00:45:14.000000 gitm-1.0.1/setup.py
```

### Comparing `gitm-1.0.0/LICENSE` & `gitm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitm-1.0.0/PKG-INFO` & `gitm-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Git emoji cli application
 Author-email: AmirBahador Bahadori <amirbahador.pv@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `gitm-1.0.0/README.md` & `gitm-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gitm-1.0.0/gitm/__main__.py` & `gitm-1.0.1/gitm/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import typer
-from pattern import get_msg, patterns
+from .pattern import get_msg, patterns
 import subprocess
 
 
 app = typer.Typer()
 
 
 @app.command()
```

### Comparing `gitm-1.0.0/gitm/connection.py` & `gitm-1.0.1/gitm/connection.py`

 * *Files identical despite different names*

### Comparing `gitm-1.0.0/gitm/pattern.py` & `gitm-1.0.1/gitm/pattern.py`

 * *Files identical despite different names*

### Comparing `gitm-1.0.0/gitm.egg-info/PKG-INFO` & `gitm-1.0.1/gitm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Git emoji cli application
 Author-email: AmirBahador Bahadori <amirbahador.pv@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `gitm-1.0.0/pyproject.toml` & `gitm-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitm"
-version = "1.0.0"
+version = "1.0.1"
 description = "Git emoji cli application"
 readme = "README.md"
 authors = [
     { name = "AmirBahador Bahadori", email = "amirbahador.pv@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

