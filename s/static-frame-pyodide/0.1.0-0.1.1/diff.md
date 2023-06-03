# Comparing `tmp/static-frame-pyodide-0.1.0.tar.gz` & `tmp/static-frame-pyodide-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-pyodide-0.1.0.tar", last modified: Fri Jun  2 23:59:41 2023, max compression
+gzip compressed data, was "static-frame-pyodide-0.1.1.tar", last modified: Sat Jun  3 16:51:47 2023, max compression
```

## Comparing `static-frame-pyodide-0.1.0.tar` & `static-frame-pyodide-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 23:59:41.318626 static-frame-pyodide-0.1.0/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.0/LICENSE
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-02 23:59:41.318626 static-frame-pyodide-0.1.0/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.0/README.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.0/pyproject.toml
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-02 23:59:41.318626 static-frame-pyodide-0.1.0/setup.cfg
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 23:59:41.318626 static-frame-pyodide-0.1.0/static_frame_pyodide/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       97 2023-06-02 15:04:23.000000 static-frame-pyodide-0.1.0/static_frame_pyodide/__init__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-02 23:59:41.318626 static-frame-pyodide-0.1.0/static_frame_pyodide.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-02 23:59:41.000000 static-frame-pyodide-0.1.0/static_frame_pyodide.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-02 23:59:41.000000 static-frame-pyodide-0.1.0/static_frame_pyodide.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-02 23:59:41.000000 static-frame-pyodide-0.1.0/static_frame_pyodide.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-02 23:59:41.000000 static-frame-pyodide-0.1.0/static_frame_pyodide.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 16:51:47.254877 static-frame-pyodide-0.1.1/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.1/LICENSE
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 16:51:47.250877 static-frame-pyodide-0.1.1/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.1/README.md
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.1/pyproject.toml
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-03 16:51:47.254877 static-frame-pyodide-0.1.1/setup.cfg
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 16:51:47.246877 static-frame-pyodide-0.1.1/static_frame_pyodide/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      555 2023-06-03 16:51:22.000000 static-frame-pyodide-0.1.1/static_frame_pyodide/__init__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 16:51:47.250877 static-frame-pyodide-0.1.1/static_frame_pyodide.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 16:51:47.000000 static-frame-pyodide-0.1.1/static_frame_pyodide.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-03 16:51:47.000000 static-frame-pyodide-0.1.1/static_frame_pyodide.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-03 16:51:47.000000 static-frame-pyodide-0.1.1/static_frame_pyodide.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-03 16:51:47.000000 static-frame-pyodide-0.1.1/static_frame_pyodide.egg-info/top_level.txt
```

### Comparing `static-frame-pyodide-0.1.0/LICENSE` & `static-frame-pyodide-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.0/PKG-INFO` & `static-frame-pyodide-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.0
+Version: 0.1.1
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `static-frame-pyodide-0.1.0/pyproject.toml` & `static-frame-pyodide-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.0/static_frame_pyodide.egg-info/PKG-INFO` & `static-frame-pyodide-0.1.1/static_frame_pyodide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.0
+Version: 0.1.1
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

