# Comparing `tmp/static-frame-pyodide-0.1.3.tar.gz` & `tmp/static-frame-pyodide-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-pyodide-0.1.3.tar", last modified: Sat Jun  3 22:54:40 2023, max compression
+gzip compressed data, was "static-frame-pyodide-0.1.4.tar", last modified: Sun Jun  4 21:51:32 2023, max compression
```

## Comparing `static-frame-pyodide-0.1.3.tar` & `static-frame-pyodide-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.3/LICENSE
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.3/README.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.3/pyproject.toml
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/setup.cfg
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:54:40.261634 static-frame-pyodide-0.1.3/static_frame_pyodide/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      975 2023-06-03 22:54:24.000000 static-frame-pyodide-0.1.3/static_frame_pyodide/__init__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-04 21:51:32.938228 static-frame-pyodide-0.1.4/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.4/LICENSE
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-04 21:51:32.934228 static-frame-pyodide-0.1.4/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.4/README.md
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.4/pyproject.toml
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-04 21:51:32.938228 static-frame-pyodide-0.1.4/setup.cfg
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-04 21:51:32.934228 static-frame-pyodide-0.1.4/static_frame_pyodide/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1188 2023-06-04 21:49:45.000000 static-frame-pyodide-0.1.4/static_frame_pyodide/__init__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-04 21:51:32.934228 static-frame-pyodide-0.1.4/static_frame_pyodide.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-04 21:51:32.000000 static-frame-pyodide-0.1.4/static_frame_pyodide.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-04 21:51:32.000000 static-frame-pyodide-0.1.4/static_frame_pyodide.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-04 21:51:32.000000 static-frame-pyodide-0.1.4/static_frame_pyodide.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-04 21:51:32.000000 static-frame-pyodide-0.1.4/static_frame_pyodide.egg-info/top_level.txt
```

### Comparing `static-frame-pyodide-0.1.3/LICENSE` & `static-frame-pyodide-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.3/PKG-INFO` & `static-frame-pyodide-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.3
+Version: 0.1.4
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `static-frame-pyodide-0.1.3/pyproject.toml` & `static-frame-pyodide-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/PKG-INFO` & `static-frame-pyodide-0.1.4/static_frame_pyodide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.3
+Version: 0.1.4
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

