# Comparing `tmp/bground-0.0.3.tar.gz` & `tmp/bground-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bground-0.0.3.tar", last modified: Sat Oct  1 22:18:58 2022, max compression
+gzip compressed data, was "bground-0.1.0.tar", last modified: Sat Jun  3 22:08:10 2023, max compression
```

## Comparing `bground-0.0.3.tar` & `bground-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-10-01 22:18:58.274621 bground-0.0.3/
--rw-rw-rw-   0        0        0     1093 2021-08-03 08:16:52.000000 bground-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1251 2022-10-01 22:18:58.273626 bground-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      703 2022-09-30 17:42:22.000000 bground-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 bground-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-01 22:18:58.274621 bground-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1266 2022-09-13 06:31:08.000000 bground-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-01 22:18:58.236858 bground-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2022-10-01 22:18:58.265649 bground-0.0.3/src/bground/
--rw-rw-rw-   0        0        0      278 2022-09-30 17:39:06.000000 bground-0.0.3/src/bground/__init__.py
--rw-rw-rw-   0        0        0     2849 2021-07-27 09:55:38.000000 bground-0.0.3/src/bground/bdata.py
--rw-rw-rw-   0        0        0     7359 2022-10-01 21:33:17.000000 bground-0.0.3/src/bground/butils.py
--rw-rw-rw-   0        0        0    10508 2022-10-01 20:10:44.000000 bground-0.0.3/src/bground/iplot.py
--rw-rw-rw-   0        0        0     1856 2022-10-01 19:10:59.000000 bground-0.0.3/src/bground/ui.py
-drwxrwxrwx   0        0        0        0 2022-10-01 22:18:58.271633 bground-0.0.3/src/bground.egg-info/
--rw-rw-rw-   0        0        0     1251 2022-10-01 22:18:58.000000 bground-0.0.3/src/bground.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2022-10-01 22:18:58.000000 bground-0.0.3/src/bground.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-01 22:18:58.000000 bground-0.0.3/src/bground.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-10-01 22:18:58.000000 bground-0.0.3/src/bground.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.805137 bground-0.1.0/
+-rw-rw-rw-   0        0        0     1093 2021-12-06 08:05:53.000000 bground-0.1.0/LICENCE
+-rw-rw-rw-   0        0        0     1438 2023-06-03 22:08:10.803614 bground-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-06-03 22:03:35.000000 bground-0.1.0/README.md
+-rw-rw-rw-   0        0        0      108 2021-08-03 08:03:10.000000 bground-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 22:08:10.805137 bground-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1266 2022-09-13 06:31:08.000000 bground-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.725491 bground-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.792494 bground-0.1.0/src/bground/
+-rw-rw-rw-   0        0        0      646 2023-05-31 07:50:35.000000 bground-0.1.0/src/bground/__init__.py
+-rw-rw-rw-   0        0        0     4189 2023-05-28 16:35:34.000000 bground-0.1.0/src/bground/bdata.py
+-rw-rw-rw-   0        0        0     4036 2023-05-30 17:11:54.000000 bground-0.1.0/src/bground/bfunc.py
+-rw-rw-rw-   0        0        0    14413 2023-05-31 08:20:46.000000 bground-0.1.0/src/bground/iplot.py
+-rw-rw-rw-   0        0        0     2746 2023-05-31 09:18:16.000000 bground-0.1.0/src/bground/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-03 22:08:10.801119 bground-0.1.0/src/bground.egg-info/
+-rw-rw-rw-   0        0        0     1438 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-03 22:08:10.000000 bground-0.1.0/src/bground.egg-info/top_level.txt
```

### Comparing `bground-0.0.3/LICENSE.txt` & `bground-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `bground-0.0.3/PKG-INFO` & `bground-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: bground
-Version: 0.0.3
+Version: 0.1.0
 Summary: Interactive subtraction of background from XY-data
 Home-page: https://github.com/mirekslouf/bground/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/bground/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENCE
 
-BGROUND :: interactive subtraction of background in XY-data
------------------------------------------------------------
+BGROUND :: interactive background subtraction
+---------------------------------------------
 
-* BGROUND draws a plot from XY-data
-* A user subtracts backgound with mouse and keyboard
-* XY-data is arbitrary text file containing two columns X-data and Y-data
+* BGROUND draws an interactive plot of XY-data.
+* The user can define and subtract backgound using mouse and keyboard.
+* XY-data is an arbitrary text file containing two columns: [X-data, Y-data].
 
 Documentation, help and examples
 --------------------------------
 
-More detailed help, demo and source code including documentation *will be*
-in [GitHub](https://mirekslouf.github.io/bground).
+* [PyPI](https://pypi.org/project/bground) repository.
+* [GitHub](https://mirekslouf.github.io/bground) repository.
+* [GitHub Pages](https://mirekslouf.github.io/bground/)
+  with [documentation](https://mirekslouf.github.io/bground/docs).
 
 Versions of BGROUND
 -------------------
 
 * Version 0.0.1 = an incomplete testing version
-* Version 0.0.2 = a small improvement of algorithm
-* Version 0.0.3 = a small improvement of docstrings and messages
+* Version 0.0.2 = the basic algorithm works
+* Version 0.0.3 = a small improvement of code and docstrings
+* Version 0.1.0 = better arrangement of funcs in modules + semi-complete docs
+
```

### Comparing `bground-0.0.3/setup.py` & `bground-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bground-0.0.3/src/bground.egg-info/PKG-INFO` & `bground-0.1.0/src/bground.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: bground
-Version: 0.0.3
+Version: 0.1.0
 Summary: Interactive subtraction of background from XY-data
 Home-page: https://github.com/mirekslouf/bground/
 Author: Mirek Slouf
 Author-email: mirek.slouf@gmail.com
 License: MIT
 Project-URL: Documentation, https://mirekslouf.github.io/bground/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENCE
 
-BGROUND :: interactive subtraction of background in XY-data
------------------------------------------------------------
+BGROUND :: interactive background subtraction
+---------------------------------------------
 
-* BGROUND draws a plot from XY-data
-* A user subtracts backgound with mouse and keyboard
-* XY-data is arbitrary text file containing two columns X-data and Y-data
+* BGROUND draws an interactive plot of XY-data.
+* The user can define and subtract backgound using mouse and keyboard.
+* XY-data is an arbitrary text file containing two columns: [X-data, Y-data].
 
 Documentation, help and examples
 --------------------------------
 
-More detailed help, demo and source code including documentation *will be*
-in [GitHub](https://mirekslouf.github.io/bground).
+* [PyPI](https://pypi.org/project/bground) repository.
+* [GitHub](https://mirekslouf.github.io/bground) repository.
+* [GitHub Pages](https://mirekslouf.github.io/bground/)
+  with [documentation](https://mirekslouf.github.io/bground/docs).
 
 Versions of BGROUND
 -------------------
 
 * Version 0.0.1 = an incomplete testing version
-* Version 0.0.2 = a small improvement of algorithm
-* Version 0.0.3 = a small improvement of docstrings and messages
+* Version 0.0.2 = the basic algorithm works
+* Version 0.0.3 = a small improvement of code and docstrings
+* Version 0.1.0 = better arrangement of funcs in modules + semi-complete docs
+
```

