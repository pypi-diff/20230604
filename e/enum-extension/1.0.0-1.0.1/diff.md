# Comparing `tmp/enum-extension-1.0.0.tar.gz` & `tmp/enum-extension-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/enum-extension/enum-extension/dist/.tmp-forqox0x/enum-extension-1.0.0.tar", last modified: Tue May 23 20:16:14 2023, max compression
+gzip compressed data, was "/home/runner/work/enum-extension/enum-extension/dist/.tmp-w_i190cr/enum-extension-1.0.1.tar", last modified: Sun Jun  4 16:50:41 2023, max compression
```

## Comparing `enum-extension-1.0.0.tar` & `enum-extension-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:14.000000 enum-extension-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:14.000000 enum-extension-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:14.000000 enum-extension-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-23 20:16:02.000000 enum-extension-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-23 20:16:02.000000 enum-extension-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-23 20:16:02.000000 enum-extension-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-23 20:16:02.000000 enum-extension-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-23 20:16:02.000000 enum-extension-1.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 20:16:02.000000 enum-extension-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-23 20:16:14.000000 enum-extension-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-23 20:16:02.000000 enum-extension-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:14.000000 enum-extension-1.0.0/enum_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-23 20:16:14.000000 enum-extension-1.0.0/enum_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 20:16:14.000000 enum-extension-1.0.0/enum_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:16:14.000000 enum-extension-1.0.0/enum_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 20:16:14.000000 enum-extension-1.0.0/enum_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:14.000000 enum-extension-1.0.0/enum_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-23 20:16:02.000000 enum-extension-1.0.0/enum_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-05-23 20:16:02.000000 enum-extension-1.0.0/enum_extensions/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-23 20:16:02.000000 enum-extension-1.0.0/enum_extensions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-23 20:16:02.000000 enum-extension-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 20:16:02.000000 enum-extension-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-23 20:16:14.000000 enum-extension-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:14.000000 enum-extension-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 20:16:02.000000 enum-extension-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 20:16:02.000000 enum-extension-1.0.0/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-23 20:16:02.000000 enum-extension-1.0.0/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:41.000000 enum-extension-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:41.000000 enum-extension-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:41.000000 enum-extension-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-04 16:50:27.000000 enum-extension-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 16:50:27.000000 enum-extension-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-04 16:50:27.000000 enum-extension-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-04 16:50:27.000000 enum-extension-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-04 16:50:27.000000 enum-extension-1.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-04 16:50:27.000000 enum-extension-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-04 16:50:41.000000 enum-extension-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-04 16:50:27.000000 enum-extension-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:41.000000 enum-extension-1.0.1/enum_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-04 16:50:41.000000 enum-extension-1.0.1/enum_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-04 16:50:41.000000 enum-extension-1.0.1/enum_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:50:41.000000 enum-extension-1.0.1/enum_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 16:50:41.000000 enum-extension-1.0.1/enum_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:41.000000 enum-extension-1.0.1/enum_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 16:50:27.000000 enum-extension-1.0.1/enum_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-04 16:50:27.000000 enum-extension-1.0.1/enum_extensions/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-04 16:50:27.000000 enum-extension-1.0.1/enum_extensions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-04 16:50:27.000000 enum-extension-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 16:50:27.000000 enum-extension-1.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-04 16:50:41.000000 enum-extension-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:41.000000 enum-extension-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:50:27.000000 enum-extension-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-04 16:50:27.000000 enum-extension-1.0.1/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-04 16:50:27.000000 enum-extension-1.0.1/tests/tests.py
```

### Comparing `enum-extension-1.0.0/.github/workflows/ci.yml` & `enum-extension-1.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/.github/workflows/python-publish.yml` & `enum-extension-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/.gitignore` & `enum-extension-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/.pre-commit-config.yaml` & `enum-extension-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/LICENSE` & `enum-extension-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/PKG-INFO` & `enum-extension-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-extension
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library that extends the functionality of the built-in enum module,
 Author-email: MuhammadAli <usermalikhan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Muhammad Ali
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,19 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: repository, https://github.com/m-ali-ubit/enum-extension
+Project-URL: homepage, https://github.com/m-ali-ubit/enum-extension
+Keywords: enum,extension,python,enhancements,utilities,advanced,capabilities
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enum-extension-1.0.0/README.md` & `enum-extension-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/enum_extension.egg-info/PKG-INFO` & `enum-extension-1.0.1/enum_extension.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-extension
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python library that extends the functionality of the built-in enum module,
 Author-email: MuhammadAli <usermalikhan@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Muhammad Ali
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,14 +21,19 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: repository, https://github.com/m-ali-ubit/enum-extension
+Project-URL: homepage, https://github.com/m-ali-ubit/enum-extension
+Keywords: enum,extension,python,enhancements,utilities,advanced,capabilities
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `enum-extension-1.0.0/enum_extensions/enum.py` & `enum-extension-1.0.1/enum_extensions/enum.py`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/tests/factories.py` & `enum-extension-1.0.1/tests/factories.py`

 * *Files identical despite different names*

### Comparing `enum-extension-1.0.0/tests/tests.py` & `enum-extension-1.0.1/tests/tests.py`

 * *Files identical despite different names*

