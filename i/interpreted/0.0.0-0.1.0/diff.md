# Comparing `tmp/interpreted-0.0.0.tar.gz` & `tmp/interpreted-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpreted-0.0.0.tar", last modified: Sun Jun  4 10:56:05 2023, max compression
+gzip compressed data, was "interpreted-0.1.0.tar", last modified: Sun Jun  4 12:17:45 2023, max compression
```

## Comparing `interpreted-0.0.0.tar` & `interpreted-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 10:56:05.951906 interpreted-0.0.0/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-06-04 10:55:45.000000 interpreted-0.0.0/LICENSE
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1461 2023-06-04 10:56:05.951964 interpreted-0.0.0/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      567 2023-06-04 10:55:45.000000 interpreted-0.0.0/README.md
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1182 2023-06-04 10:56:05.952295 interpreted-0.0.0/setup.cfg
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2023-06-04 10:55:45.000000 interpreted-0.0.0/setup.py
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 10:56:05.949471 interpreted-0.0.0/src/
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 10:56:05.950983 interpreted-0.0.0/src/interpreted/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      142 2023-06-04 10:55:45.000000 interpreted-0.0.0/src/interpreted/__init__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      136 2023-06-04 10:55:45.000000 interpreted-0.0.0/src/interpreted/__main__.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      132 2023-06-04 10:55:45.000000 interpreted-0.0.0/src/interpreted/cli.py
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2023-06-04 10:55:45.000000 interpreted-0.0.0/src/interpreted/py.typed
-drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 10:56:05.951795 interpreted-0.0.0/src/interpreted.egg-info/
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1461 2023-06-04 10:56:05.000000 interpreted-0.0.0/src/interpreted.egg-info/PKG-INFO
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)      376 2023-06-04 10:56:05.000000 interpreted-0.0.0/src/interpreted.egg-info/SOURCES.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-06-04 10:56:05.000000 interpreted-0.0.0/src/interpreted.egg-info/dependency_links.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       52 2023-06-04 10:56:05.000000 interpreted-0.0.0/src/interpreted.egg-info/entry_points.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       40 2023-06-04 10:56:05.000000 interpreted-0.0.0/src/interpreted.egg-info/requires.txt
--rw-r--r--   0 tusharsadhwani   (501) staff       (20)       12 2023-06-04 10:56:05.000000 interpreted-0.0.0/src/interpreted.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 12:17:45.990274 interpreted-0.1.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-06-04 10:55:45.000000 interpreted-0.1.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1829 2023-06-04 12:17:45.990371 interpreted-0.1.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      935 2023-06-04 11:03:44.000000 interpreted-0.1.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1183 2023-06-04 12:17:45.990711 interpreted-0.1.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       37 2023-06-04 11:45:13.000000 interpreted-0.1.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 12:17:45.988531 interpreted-0.1.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 12:17:45.989430 interpreted-0.1.0/src/interpreted/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      219 2023-06-04 11:46:03.000000 interpreted-0.1.0/src/interpreted/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      154 2023-06-04 11:42:59.000000 interpreted-0.1.0/src/interpreted/__main__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      535 2023-06-04 12:09:54.000000 interpreted-0.1.0/src/interpreted/cli.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       59 2023-06-04 10:55:45.000000 interpreted-0.1.0/src/interpreted/py.typed
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-06-04 12:17:45.990175 interpreted-0.1.0/src/interpreted.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1829 2023-06-04 12:17:45.000000 interpreted-0.1.0/src/interpreted.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      376 2023-06-04 12:17:45.000000 interpreted-0.1.0/src/interpreted.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-06-04 12:17:45.000000 interpreted-0.1.0/src/interpreted.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       52 2023-06-04 12:17:45.000000 interpreted-0.1.0/src/interpreted.egg-info/entry_points.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       40 2023-06-04 12:17:45.000000 interpreted-0.1.0/src/interpreted.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       12 2023-06-04 12:17:45.000000 interpreted-0.1.0/src/interpreted.egg-info/top_level.txt
```

### Comparing `interpreted-0.0.0/LICENSE` & `interpreted-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interpreted-0.0.0/PKG-INFO` & `interpreted-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpreted
-Version: 0.0.0
+Version: 0.1.0
 Summary: A Python interpreter, in Python.
 Home-page: https://github.com/tusharsadhwani/interpreted
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,40 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # interpreted
 
-A Python interpreter, in Python.
+A Python interpreter, written from scratch in Python.
+
+This interpreter is made solely as the base for my talk,
+"Writing a Python interpreter from scratch, in half an hour."
+
+## Installation
+
+```bash
+pip install interpreted
+```
+
+## Usage
+
+```console
+$ cat foo.py
+print("2 + 2 is", 2 + 2)
+
+def greet(name='User'):
+	print('Hello,', name + '!')
+
+greet()
+
+$ interpreted foo.py
+2 + 2 is 4
+Hello, User!
+```
 
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

### Comparing `interpreted-0.0.0/README.md` & `interpreted-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,35 @@
 # interpreted
 
-A Python interpreter, in Python.
+A Python interpreter, written from scratch in Python.
+
+This interpreter is made solely as the base for my talk,
+"Writing a Python interpreter from scratch, in half an hour."
+
+## Installation
+
+```bash
+pip install interpreted
+```
+
+## Usage
+
+```console
+$ cat foo.py
+print("2 + 2 is", 2 + 2)
+
+def greet(name='User'):
+	print('Hello,', name + '!')
+
+greet()
+
+$ interpreted foo.py
+2 + 2 is 4
+Hello, User!
+```
 
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

### Comparing `interpreted-0.0.0/setup.cfg` & `interpreted-0.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = interpreted
-version = 0.0.0
+version = 0.1.0
 description = A Python interpreter, in Python.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/interpreted
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

### Comparing `interpreted-0.0.0/src/interpreted.egg-info/PKG-INFO` & `interpreted-0.1.0/src/interpreted.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpreted
-Version: 0.0.0
+Version: 0.1.0
 Summary: A Python interpreter, in Python.
 Home-page: https://github.com/tusharsadhwani/interpreted
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,40 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # interpreted
 
-A Python interpreter, in Python.
+A Python interpreter, written from scratch in Python.
+
+This interpreter is made solely as the base for my talk,
+"Writing a Python interpreter from scratch, in half an hour."
+
+## Installation
+
+```bash
+pip install interpreted
+```
+
+## Usage
+
+```console
+$ cat foo.py
+print("2 + 2 is", 2 + 2)
+
+def greet(name='User'):
+	print('Hello,', name + '!')
+
+greet()
+
+$ interpreted foo.py
+2 + 2 is 4
+Hello, User!
+```
 
 ## Local Development / Testing
 
 - Create and activate a virtual environment
 - Run `pip install -r requirements-dev.txt` to do an editable install
 - Run `pytest` to run tests
```

