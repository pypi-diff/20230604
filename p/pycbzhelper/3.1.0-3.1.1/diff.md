# Comparing `tmp/pycbzhelper-3.1.0.tar.gz` & `tmp/pycbzhelper-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycbzhelper-3.1.0.tar", last modified: Sun Jun  4 13:58:40 2023, max compression
+gzip compressed data, was "pycbzhelper-3.1.1.tar", last modified: Sun Jun  4 14:12:40 2023, max compression
```

## Comparing `pycbzhelper-3.1.0.tar` & `pycbzhelper-3.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:58:40.375295 pycbzhelper-3.1.0/
--rw-rw-rw-   0        0        0    35823 2023-06-03 15:03:22.000000 pycbzhelper-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     2916 2023-06-04 13:58:40.375295 pycbzhelper-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1988 2023-06-04 13:54:51.000000 pycbzhelper-3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 13:58:40.356012 pycbzhelper-3.1.0/pycbzhelper/
--rw-rw-rw-   0        0        0      102 2023-06-04 13:32:18.000000 pycbzhelper-3.1.0/pycbzhelper/__init__.py
--rw-rw-rw-   0        0        0     1585 2023-06-03 15:19:04.000000 pycbzhelper-3.1.0/pycbzhelper/comicinfo.py
--rw-rw-rw-   0        0        0      439 2023-06-03 18:55:42.000000 pycbzhelper-3.1.0/pycbzhelper/exceptions.py
--rw-rw-rw-   0        0        0     6892 2023-06-04 13:24:33.000000 pycbzhelper-3.1.0/pycbzhelper/helper.py
--rw-rw-rw-   0        0        0     1647 2023-06-04 13:56:16.000000 pycbzhelper-3.1.0/pycbzhelper/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:58:40.374301 pycbzhelper-3.1.0/pycbzhelper.egg-info/
--rw-rw-rw-   0        0        0     2916 2023-06-04 13:58:40.000000 pycbzhelper-3.1.0/pycbzhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-06-04 13:58:40.000000 pycbzhelper-3.1.0/pycbzhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:58:40.000000 pycbzhelper-3.1.0/pycbzhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-04 13:58:40.000000 pycbzhelper-3.1.0/pycbzhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-04 13:58:40.000000 pycbzhelper-3.1.0/pycbzhelper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 13:58:40.375295 pycbzhelper-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1272 2023-06-04 13:32:18.000000 pycbzhelper-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:12:40.000823 pycbzhelper-3.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-03 15:03:22.000000 pycbzhelper-3.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3254 2023-06-04 14:12:39.999823 pycbzhelper-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2023-06-04 14:07:19.000000 pycbzhelper-3.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 14:12:39.986764 pycbzhelper-3.1.1/pycbzhelper/
+-rw-rw-rw-   0        0        0      102 2023-06-04 14:08:50.000000 pycbzhelper-3.1.1/pycbzhelper/__init__.py
+-rw-rw-rw-   0        0        0     1585 2023-06-03 15:19:04.000000 pycbzhelper-3.1.1/pycbzhelper/comicinfo.py
+-rw-rw-rw-   0        0        0      439 2023-06-03 18:55:42.000000 pycbzhelper-3.1.1/pycbzhelper/exceptions.py
+-rw-rw-rw-   0        0        0     6892 2023-06-04 13:24:33.000000 pycbzhelper-3.1.1/pycbzhelper/helper.py
+-rw-rw-rw-   0        0        0     1647 2023-06-04 13:56:16.000000 pycbzhelper-3.1.1/pycbzhelper/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:12:39.998818 pycbzhelper-3.1.1/pycbzhelper.egg-info/
+-rw-rw-rw-   0        0        0     3254 2023-06-04 14:12:39.000000 pycbzhelper-3.1.1/pycbzhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-04 14:12:39.000000 pycbzhelper-3.1.1/pycbzhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:12:39.000000 pycbzhelper-3.1.1/pycbzhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-04 14:12:39.000000 pycbzhelper-3.1.1/pycbzhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-04 14:12:39.000000 pycbzhelper-3.1.1/pycbzhelper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:12:40.000823 pycbzhelper-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1272 2023-06-04 14:08:50.000000 pycbzhelper-3.1.1/setup.py
```

### Comparing `pycbzhelper-3.1.0/LICENSE` & `pycbzhelper-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycbzhelper-3.1.0/PKG-INFO` & `pycbzhelper-3.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycbzhelper
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library for creating CBZ files with metadata.
 Home-page: https://github.com/hyugogirubato/pycbzhelper
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: metadata,manga,comics,ebooks,cbz
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyCBZHelper
 
-[![License](https://img.shields.io/github/license/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pycbzhelper)](https://pypi.org/project/pycbzhelper/)
 
 PyCBZHelper is a Python library for creating CBZ (Comic Book Zip) files with metadata. It provides functionality to
 generate a CBZ file from a list of image pages and associated comic book metadata.
 
 ## Features
@@ -77,12 +77,21 @@
     helper = Helper(metadata)
 
     # Create the CBZ file
     helper.create_cbz(output_path)
 ````
 
 For more information on how to use PyCBZHelper, please refer to
-the [documentation](https://github.com/hyugogirubato/pycbzhelper/blob/master/docs/schema).
+the [documentation](https://github.com/hyugogirubato/pycbzhelper/blob/main/docs/schema).
+
+### Exceptions
+
+The following exceptions can be raised by PyCBZHelper:
+
+- `InvalidKeyValue`: Raised when a key value is invalid.
+- `MissingPageFile`: Raised when no page files are available.
+- `InvalidFileExtension`: Raised when an invalid file extension is used.
+- `FileNotFound`: Raised when the specified source file is not found.
 
 ### License
 
-This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pycbzhelper/blob/master/LICENSE).
+This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pycbzhelper/blob/main/LICENSE).
```

### Comparing `pycbzhelper-3.1.0/README.md` & `pycbzhelper-3.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # PyCBZHelper
 
-[![License](https://img.shields.io/github/license/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pycbzhelper)](https://pypi.org/project/pycbzhelper/)
 
 PyCBZHelper is a Python library for creating CBZ (Comic Book Zip) files with metadata. It provides functionality to
 generate a CBZ file from a list of image pages and associated comic book metadata.
 
 ## Features
@@ -53,12 +53,21 @@
     helper = Helper(metadata)
 
     # Create the CBZ file
     helper.create_cbz(output_path)
 ````
 
 For more information on how to use PyCBZHelper, please refer to
-the [documentation](https://github.com/hyugogirubato/pycbzhelper/blob/master/docs/schema).
+the [documentation](https://github.com/hyugogirubato/pycbzhelper/blob/main/docs/schema).
+
+### Exceptions
+
+The following exceptions can be raised by PyCBZHelper:
+
+- `InvalidKeyValue`: Raised when a key value is invalid.
+- `MissingPageFile`: Raised when no page files are available.
+- `InvalidFileExtension`: Raised when an invalid file extension is used.
+- `FileNotFound`: Raised when the specified source file is not found.
 
 ### License
 
-This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pycbzhelper/blob/master/LICENSE).
+This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pycbzhelper/blob/main/LICENSE).
```

### Comparing `pycbzhelper-3.1.0/pycbzhelper/comicinfo.py` & `pycbzhelper-3.1.1/pycbzhelper/comicinfo.py`

 * *Files identical despite different names*

### Comparing `pycbzhelper-3.1.0/pycbzhelper/helper.py` & `pycbzhelper-3.1.1/pycbzhelper/helper.py`

 * *Files identical despite different names*

### Comparing `pycbzhelper-3.1.0/pycbzhelper/utils.py` & `pycbzhelper-3.1.1/pycbzhelper/utils.py`

 * *Files identical despite different names*

### Comparing `pycbzhelper-3.1.0/pycbzhelper.egg-info/PKG-INFO` & `pycbzhelper-3.1.1/pycbzhelper.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycbzhelper
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python library for creating CBZ files with metadata.
 Home-page: https://github.com/hyugogirubato/pycbzhelper
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: metadata,manga,comics,ebooks,cbz
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyCBZHelper
 
-[![License](https://img.shields.io/github/license/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pycbzhelper)](https://github.com/hyugogirubato/pycbzhelper/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pycbzhelper)](https://pypi.org/project/pycbzhelper/)
 
 PyCBZHelper is a Python library for creating CBZ (Comic Book Zip) files with metadata. It provides functionality to
 generate a CBZ file from a list of image pages and associated comic book metadata.
 
 ## Features
@@ -77,12 +77,21 @@
     helper = Helper(metadata)
 
     # Create the CBZ file
     helper.create_cbz(output_path)
 ````
 
 For more information on how to use PyCBZHelper, please refer to
-the [documentation](https://github.com/hyugogirubato/pycbzhelper/blob/master/docs/schema).
+the [documentation](https://github.com/hyugogirubato/pycbzhelper/blob/main/docs/schema).
+
+### Exceptions
+
+The following exceptions can be raised by PyCBZHelper:
+
+- `InvalidKeyValue`: Raised when a key value is invalid.
+- `MissingPageFile`: Raised when no page files are available.
+- `InvalidFileExtension`: Raised when an invalid file extension is used.
+- `FileNotFound`: Raised when the specified source file is not found.
 
 ### License
 
-This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pycbzhelper/blob/master/LICENSE).
+This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pycbzhelper/blob/main/LICENSE).
```

### Comparing `pycbzhelper-3.1.0/setup.py` & `pycbzhelper-3.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pycbzhelper",
-    version="3.1.0",
+    version="3.1.1",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for creating CBZ files with metadata.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pycbzhelper",
     packages=find_packages(),
```

