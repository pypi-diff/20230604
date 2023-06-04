# Comparing `tmp/python-fluepdot-0.0.1.tar.gz` & `tmp/python-fluepdot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-fluepdot-0.0.1.tar", last modified: Fri Jun  2 21:52:48 2023, max compression
+gzip compressed data, was "python-fluepdot-0.0.2.tar", last modified: Sun Jun  4 08:06:27 2023, max compression
```

## Comparing `python-fluepdot-0.0.1.tar` & `python-fluepdot-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-02 21:52:48.022774 python-fluepdot-0.0.1/
--rw-r--r--   0 ks        (1000) users      (985)     1074 2023-05-30 17:08:37.000000 python-fluepdot-0.0.1/LICENSE
--rw-r--r--   0 ks        (1000) users      (985)     2072 2023-06-02 21:52:48.022774 python-fluepdot-0.0.1/PKG-INFO
--rw-r--r--   0 ks        (1000) users      (985)     1517 2022-09-08 06:58:59.000000 python-fluepdot-0.0.1/README.md
--rw-r--r--   0 ks        (1000) users      (985)      630 2023-05-30 17:08:37.000000 python-fluepdot-0.0.1/pyproject.toml
--rw-r--r--   0 ks        (1000) users      (985)       38 2023-06-02 21:52:48.022774 python-fluepdot-0.0.1/setup.cfg
-drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-02 21:52:48.018774 python-fluepdot-0.0.1/src/
-drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-02 21:52:48.020774 python-fluepdot-0.0.1/src/fluepdot/
--rw-r--r--   0 ks        (1000) users      (985)       37 2023-05-30 17:08:37.000000 python-fluepdot-0.0.1/src/fluepdot/__init__.py
--rw-r--r--   0 ks        (1000) users      (985)     3424 2023-05-30 17:08:37.000000 python-fluepdot-0.0.1/src/fluepdot/fluepdot.py
-drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-02 21:52:48.021774 python-fluepdot-0.0.1/src/python_fluepdot.egg-info/
--rw-r--r--   0 ks        (1000) users      (985)     2072 2023-06-02 21:52:48.000000 python-fluepdot-0.0.1/src/python_fluepdot.egg-info/PKG-INFO
--rw-r--r--   0 ks        (1000) users      (985)      254 2023-06-02 21:52:48.000000 python-fluepdot-0.0.1/src/python_fluepdot.egg-info/SOURCES.txt
--rw-r--r--   0 ks        (1000) users      (985)        1 2023-06-02 21:52:48.000000 python-fluepdot-0.0.1/src/python_fluepdot.egg-info/dependency_links.txt
--rw-r--r--   0 ks        (1000) users      (985)        9 2023-06-02 21:52:48.000000 python-fluepdot-0.0.1/src/python_fluepdot.egg-info/top_level.txt
+drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-04 08:06:27.614873 python-fluepdot-0.0.2/
+-rw-r--r--   0 ks        (1000) users      (985)     1074 2023-05-30 17:08:37.000000 python-fluepdot-0.0.2/LICENSE
+-rw-r--r--   0 ks        (1000) users      (985)     2177 2023-06-04 08:06:27.613873 python-fluepdot-0.0.2/PKG-INFO
+-rw-r--r--   0 ks        (1000) users      (985)     1622 2023-06-04 08:03:21.000000 python-fluepdot-0.0.2/README.md
+-rw-r--r--   0 ks        (1000) users      (985)      630 2023-06-04 08:03:58.000000 python-fluepdot-0.0.2/pyproject.toml
+-rw-r--r--   0 ks        (1000) users      (985)       38 2023-06-04 08:06:27.614873 python-fluepdot-0.0.2/setup.cfg
+drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-04 08:06:27.606873 python-fluepdot-0.0.2/src/
+drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-04 08:06:27.611873 python-fluepdot-0.0.2/src/fluepdot/
+-rw-r--r--   0 ks        (1000) users      (985)       37 2023-05-30 17:08:37.000000 python-fluepdot-0.0.2/src/fluepdot/__init__.py
+-rw-r--r--   0 ks        (1000) users      (985)     4043 2023-06-04 08:03:21.000000 python-fluepdot-0.0.2/src/fluepdot/fluepdot.py
+-rw-r--r--   0 ks        (1000) users      (985)     7487 2023-06-04 08:05:07.000000 python-fluepdot-0.0.2/src/fluepdot/mock_server.py
+drwxr-xr-x   0 ks        (1000) users      (985)        0 2023-06-04 08:06:27.613873 python-fluepdot-0.0.2/src/python_fluepdot.egg-info/
+-rw-r--r--   0 ks        (1000) users      (985)     2177 2023-06-04 08:06:27.000000 python-fluepdot-0.0.2/src/python_fluepdot.egg-info/PKG-INFO
+-rw-r--r--   0 ks        (1000) users      (985)      282 2023-06-04 08:06:27.000000 python-fluepdot-0.0.2/src/python_fluepdot.egg-info/SOURCES.txt
+-rw-r--r--   0 ks        (1000) users      (985)        1 2023-06-04 08:06:27.000000 python-fluepdot-0.0.2/src/python_fluepdot.egg-info/dependency_links.txt
+-rw-r--r--   0 ks        (1000) users      (985)        9 2023-06-04 08:06:27.000000 python-fluepdot-0.0.2/src/python_fluepdot.egg-info/top_level.txt
```

### Comparing `python-fluepdot-0.0.1/LICENSE` & `python-fluepdot-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-fluepdot-0.0.1/PKG-INFO` & `python-fluepdot-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,30 @@
-Metadata-Version: 2.1
-Name: python-fluepdot
-Version: 0.0.1
-Summary: A small collection of functions for interacting with a fluepdot module.
-Author-email: KS-HTK <ks-htk@flipdot.org>
-Project-URL: Homepage, https://github.com/KS-HTK/python-fluepdot
-Project-URL: Bug-Tracker, https://github.com/KS-HTK/python-fluepdot/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # python-fluepdot
 
 This is a small collection of functions for interacting with a
 [fluepdot](https://fluepdot.readthedocs.io/en/latest/) module.
 
-the first call after importing should always be to set the URL at
-which the module can be reached.
+import Fluepdot class and create an instance with link as the first arg
 
 ```python
-import fluepdot as fd
+from fluepdot import Fluepdot
 
-fd.set_url("module.local")
+fd = Fluepdot("http://module.local")
 ```
 
 ## Functions
 
 
 function | args | default values | return type | description
 ---|---|---|---|---
+_init_ | baseURL: str, width: int, height: int | x=115, y=16 | fluepdot.Fluepdot | Constructor for Fluepdot class
 post_time ||| None | indefinitly sets the module to display the current time.
 get_size ||| (int, int) | returns the size of the connected display
 get_frame ||| str | returns the current frame stored by the module
 get_pixel | x: int, y: int | x=0, y=0 | returns the state of a single pixel
 get_fonts ||| None | prints a list of fonts installed on the module
 get_mode ||| fluepdot.Mode | returns the mode the module is in
 post_text | text: str, x: int, y: int, font: str | x=0, y=0, font="DejaVuSans12" | requests.Response | posts a text to the module and returns the requests response
 post_frame | frame: List[List[bool]] || requests.Response | posts a frame to the module and returns the requests response
 set_pixel | x: int, y: int | x=0, y=0 | requests.Response | sets a pixel on the display to active and returns the requests response
 unset_pixel | x: int, y: int | x=0, y=0 | sets a pixel on thes display to inactive and returns the requests response
-set_mode | mode: fluepdot.Mode | mode=Mode.FULL | requests.Response | sets the module to FULL or DIFFERENTIAL update mode and returns the requests response
+set_mode | mode: fluepdot.Mode | mode=Mode.FULL | requests.Response | sets the module to FULL or DIFFERENTIAL update mode and returns the requests response
```

### Comparing `python-fluepdot-0.0.1/pyproject.toml` & `python-fluepdot-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-fluepdot"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="KS-HTK", email="ks-htk@flipdot.org" },
 ]
 description = "A small collection of functions for interacting with a fluepdot module."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `python-fluepdot-0.0.1/src/python_fluepdot.egg-info/PKG-INFO` & `python-fluepdot-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-fluepdot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small collection of functions for interacting with a fluepdot module.
 Author-email: KS-HTK <ks-htk@flipdot.org>
 Project-URL: Homepage, https://github.com/KS-HTK/python-fluepdot
 Project-URL: Bug-Tracker, https://github.com/KS-HTK/python-fluepdot/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,28 @@
 License-File: LICENSE
 
 # python-fluepdot
 
 This is a small collection of functions for interacting with a
 [fluepdot](https://fluepdot.readthedocs.io/en/latest/) module.
 
-the first call after importing should always be to set the URL at
-which the module can be reached.
+import Fluepdot class and create an instance with link as the first arg
 
 ```python
-import fluepdot as fd
+from fluepdot import Fluepdot
 
-fd.set_url("module.local")
+fd = Fluepdot("http://module.local")
 ```
 
 ## Functions
 
 
 function | args | default values | return type | description
 ---|---|---|---|---
+_init_ | baseURL: str, width: int, height: int | x=115, y=16 | fluepdot.Fluepdot | Constructor for Fluepdot class
 post_time ||| None | indefinitly sets the module to display the current time.
 get_size ||| (int, int) | returns the size of the connected display
 get_frame ||| str | returns the current frame stored by the module
 get_pixel | x: int, y: int | x=0, y=0 | returns the state of a single pixel
 get_fonts ||| None | prints a list of fonts installed on the module
 get_mode ||| fluepdot.Mode | returns the mode the module is in
 post_text | text: str, x: int, y: int, font: str | x=0, y=0, font="DejaVuSans12" | requests.Response | posts a text to the module and returns the requests response
```

