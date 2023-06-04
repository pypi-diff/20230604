# Comparing `tmp/pydash2hls-2.1.1.tar.gz` & `tmp/pydash2hls-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash2hls-2.1.1.tar", last modified: Sun Jun  4 12:03:50 2023, max compression
+gzip compressed data, was "pydash2hls-2.1.2.tar", last modified: Sun Jun  4 14:12:12 2023, max compression
```

## Comparing `pydash2hls-2.1.1.tar` & `pydash2hls-2.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/
--rw-rw-rw-   0        0        0    35823 2023-06-03 12:20:09.000000 pydash2hls-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     3128 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2202 2023-06-03 14:21:01.000000 pydash2hls-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 12:03:50.583502 pydash2hls-2.1.1/pydash2hls/
--rw-rw-rw-   0        0        0       51 2023-06-04 12:00:32.000000 pydash2hls-2.1.1/pydash2hls/__init__.py
--rw-rw-rw-   0        0        0     7234 2023-06-04 11:59:35.000000 pydash2hls-2.1.1/pydash2hls/converter.py
--rw-rw-rw-   0        0        0      469 2023-06-03 13:17:40.000000 pydash2hls-2.1.1/pydash2hls/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/pydash2hls.egg-info/
--rw-rw-rw-   0        0        0     3128 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-04 12:00:32.000000 pydash2hls-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:12:12.689725 pydash2hls-2.1.2/
+-rw-rw-rw-   0        0        0    35823 2023-06-03 12:20:09.000000 pydash2hls-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3387 2023-06-04 14:12:12.688723 pydash2hls-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2461 2023-06-04 14:04:17.000000 pydash2hls-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 14:12:12.669157 pydash2hls-2.1.2/pydash2hls/
+-rw-rw-rw-   0        0        0       51 2023-06-04 14:10:39.000000 pydash2hls-2.1.2/pydash2hls/__init__.py
+-rw-rw-rw-   0        0        0     7234 2023-06-04 11:59:35.000000 pydash2hls-2.1.2/pydash2hls/converter.py
+-rw-rw-rw-   0        0        0      469 2023-06-03 13:17:40.000000 pydash2hls-2.1.2/pydash2hls/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:12:12.687732 pydash2hls-2.1.2/pydash2hls.egg-info/
+-rw-rw-rw-   0        0        0     3387 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 14:12:12.000000 pydash2hls-2.1.2/pydash2hls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 14:12:12.689725 pydash2hls-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-06-04 14:10:39.000000 pydash2hls-2.1.2/setup.py
```

### Comparing `pydash2hls-2.1.1/LICENSE` & `pydash2hls-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.1/PKG-INFO` & `pydash2hls-2.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,21 +20,28 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyDash2HLS
 
-[![License](https://img.shields.io/github/license/hyugogirubato/PyDash2HLS)](https://github.com/hyugogirubato/PyDash2HLS/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
+## Features
+
+- Convert MPD files to HLS format
+- Support for remote and local MPD files
+- Retrieve media URLs for a specific profile
+- Handle DRM (Digital Rights Management) information in MPD files
+
 ## Installation
 
 You can install PyDash2HLS using pip:
 
 ````shell
 pip install pydash2hls
 ````
@@ -93,9 +100,9 @@
 - `InvalidPath`: Raised when the file path is invalid.
 - `InvalidFileContent`: Raised when the contents of the file are not in DASH format or are incompatible.
 - `InvalidProfile`: Raised when the selected profile is invalid.
 - `MissingRemoteUrl`: Raised when a remote file URL is required but not provided.
 
 ### License
 
-This project is licensed under the [GPL v3 License](LICENSE).
+This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE).
```

### Comparing `pydash2hls-2.1.1/README.md` & `pydash2hls-2.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # PyDash2HLS
 
-[![License](https://img.shields.io/github/license/hyugogirubato/PyDash2HLS)](https://github.com/hyugogirubato/PyDash2HLS/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
+## Features
+
+- Convert MPD files to HLS format
+- Support for remote and local MPD files
+- Retrieve media URLs for a specific profile
+- Handle DRM (Digital Rights Management) information in MPD files
+
 ## Installation
 
 You can install PyDash2HLS using pip:
 
 ````shell
 pip install pydash2hls
 ````
@@ -69,9 +76,9 @@
 - `InvalidPath`: Raised when the file path is invalid.
 - `InvalidFileContent`: Raised when the contents of the file are not in DASH format or are incompatible.
 - `InvalidProfile`: Raised when the selected profile is invalid.
 - `MissingRemoteUrl`: Raised when a remote file URL is required but not provided.
 
 ### License
 
-This project is licensed under the [GPL v3 License](LICENSE).
+This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE).
```

### Comparing `pydash2hls-2.1.1/pydash2hls/converter.py` & `pydash2hls-2.1.2/pydash2hls/converter.py`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.1/pydash2hls.egg-info/PKG-INFO` & `pydash2hls-2.1.2/pydash2hls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,21 +20,28 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyDash2HLS
 
-[![License](https://img.shields.io/github/license/hyugogirubato/PyDash2HLS)](https://github.com/hyugogirubato/PyDash2HLS/blob/master/LICENSE)
+[![License](https://img.shields.io/github/license/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/releases)
 [![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
+## Features
+
+- Convert MPD files to HLS format
+- Support for remote and local MPD files
+- Retrieve media URLs for a specific profile
+- Handle DRM (Digital Rights Management) information in MPD files
+
 ## Installation
 
 You can install PyDash2HLS using pip:
 
 ````shell
 pip install pydash2hls
 ````
@@ -93,9 +100,9 @@
 - `InvalidPath`: Raised when the file path is invalid.
 - `InvalidFileContent`: Raised when the contents of the file are not in DASH format or are incompatible.
 - `InvalidProfile`: Raised when the selected profile is invalid.
 - `MissingRemoteUrl`: Raised when a remote file URL is required but not provided.
 
 ### License
 
-This project is licensed under the [GPL v3 License](LICENSE).
+This project is licensed under the [GPL v3 License](https://github.com/hyugogirubato/pydash2hls/blob/main/LICENSE).
```

### Comparing `pydash2hls-2.1.1/setup.py` & `pydash2hls-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pydash2hls",
-    version="2.1.1",
+    version="2.1.2",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for converting DASH manifest files to HLS format.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pydash2hls",
     packages=find_packages(),
```

