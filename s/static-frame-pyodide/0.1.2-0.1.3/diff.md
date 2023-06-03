# Comparing `tmp/static-frame-pyodide-0.1.2.tar.gz` & `tmp/static-frame-pyodide-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-pyodide-0.1.2.tar", last modified: Sat Jun  3 22:29:46 2023, max compression
+gzip compressed data, was "static-frame-pyodide-0.1.3.tar", last modified: Sat Jun  3 22:54:40 2023, max compression
```

## Comparing `static-frame-pyodide-0.1.2.tar` & `static-frame-pyodide-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:29:46.691456 static-frame-pyodide-0.1.2/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.2/LICENSE
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 22:29:46.691456 static-frame-pyodide-0.1.2/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.2/README.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.2/pyproject.toml
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-03 22:29:46.691456 static-frame-pyodide-0.1.2/setup.cfg
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:29:46.687456 static-frame-pyodide-0.1.2/static_frame_pyodide/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      616 2023-06-03 22:29:17.000000 static-frame-pyodide-0.1.2/static_frame_pyodide/__init__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:29:46.691456 static-frame-pyodide-0.1.2/static_frame_pyodide.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 22:29:46.000000 static-frame-pyodide-0.1.2/static_frame_pyodide.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-03 22:29:46.000000 static-frame-pyodide-0.1.2/static_frame_pyodide.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-03 22:29:46.000000 static-frame-pyodide-0.1.2/static_frame_pyodide.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-03 22:29:46.000000 static-frame-pyodide-0.1.2/static_frame_pyodide.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.3/LICENSE
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.3/README.md
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.3/pyproject.toml
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/setup.cfg
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:54:40.261634 static-frame-pyodide-0.1.3/static_frame_pyodide/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      975 2023-06-03 22:54:24.000000 static-frame-pyodide-0.1.3/static_frame_pyodide/__init__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-03 22:54:40.265633 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-03 22:54:40.000000 static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/top_level.txt
```

### Comparing `static-frame-pyodide-0.1.2/LICENSE` & `static-frame-pyodide-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.2/PKG-INFO` & `static-frame-pyodide-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.2
+Version: 0.1.3
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `static-frame-pyodide-0.1.2/pyproject.toml` & `static-frame-pyodide-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.2/static_frame_pyodide.egg-info/PKG-INFO` & `static-frame-pyodide-0.1.3/static_frame_pyodide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.2
+Version: 0.1.3
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

