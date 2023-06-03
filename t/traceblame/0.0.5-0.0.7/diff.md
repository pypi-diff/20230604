# Comparing `tmp/traceblame-0.0.5.tar.gz` & `tmp/traceblame-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceblame-0.0.5.tar", last modified: Sat Jun  3 22:17:45 2023, max compression
+gzip compressed data, was "traceblame-0.0.7.tar", last modified: Sat Jun  3 22:19:33 2023, max compression
```

## Comparing `traceblame-0.0.5.tar` & `traceblame-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:17:45.066165 traceblame-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 22:17:35.000000 traceblame-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-03 22:17:45.066165 traceblame-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-03 22:17:35.000000 traceblame-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:17:45.066165 traceblame-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:17:45.062165 traceblame-0.0.5/traceblame/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-03 22:17:35.000000 traceblame-0.0.5/traceblame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-03 22:17:35.000000 traceblame-0.0.5/traceblame/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:17:45.062165 traceblame-0.0.5/traceblame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-03 22:17:45.000000 traceblame-0.0.5/traceblame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-03 22:17:45.000000 traceblame-0.0.5/traceblame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:17:45.000000 traceblame-0.0.5/traceblame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 22:17:45.000000 traceblame-0.0.5/traceblame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 22:17:45.000000 traceblame-0.0.5/traceblame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:19:33.286489 traceblame-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 22:19:27.000000 traceblame-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-03 22:19:33.286489 traceblame-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-03 22:19:27.000000 traceblame-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:19:33.286489 traceblame-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:19:33.282489 traceblame-0.0.7/traceblame/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-03 22:19:27.000000 traceblame-0.0.7/traceblame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-03 22:19:27.000000 traceblame-0.0.7/traceblame/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:19:33.282489 traceblame-0.0.7/traceblame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-03 22:19:33.000000 traceblame-0.0.7/traceblame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-03 22:19:33.000000 traceblame-0.0.7/traceblame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:19:33.000000 traceblame-0.0.7/traceblame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 22:19:33.000000 traceblame-0.0.7/traceblame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 22:19:33.000000 traceblame-0.0.7/traceblame.egg-info/top_level.txt
```

### Comparing `traceblame-0.0.5/LICENSE` & `traceblame-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `traceblame-0.0.5/PKG-INFO` & `traceblame-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceblame
-Version: 0.0.5
+Version: 0.0.7
 Summary: Tool to extend locals variables in stacktrace by git blame information for python projects
 Home-page: https://github.com/ncopiy/traceblame
 Author: ncopiy
 Author-email: ncopiy@yandex.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `traceblame-0.0.5/traceblame/main.py` & `traceblame-0.0.7/traceblame/main.py`

 * *Files identical despite different names*

### Comparing `traceblame-0.0.5/traceblame.egg-info/PKG-INFO` & `traceblame-0.0.7/traceblame.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceblame
-Version: 0.0.5
+Version: 0.0.7
 Summary: Tool to extend locals variables in stacktrace by git blame information for python projects
 Home-page: https://github.com/ncopiy/traceblame
 Author: ncopiy
 Author-email: ncopiy@yandex.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

