# Comparing `tmp/pydisort-0.0.3.tar.gz` & `tmp/pydisort-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisort-0.0.3.tar", last modified: Sun Jun  4 15:20:24 2023, max compression
+gzip compressed data, was "pydisort-0.0.4.tar", last modified: Sun Jun  4 16:28:07 2023, max compression
```

## Comparing `pydisort-0.0.3.tar` & `pydisort-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 15:20:24.828760 pydisort-0.0.3/
--rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-04 15:20:24.828336 pydisort-0.0.3/PKG-INFO
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 15:20:24.822666 pydisort-0.0.3/pydisort/
--rw-r--r--   0 zyhu       (502) staff       (20)       24 2023-06-04 01:28:16.000000 pydisort-0.0.3/pydisort/__init__.py
--rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 00:45:04.000000 pydisort-0.0.3/pydisort/pydisort.cpython-311-darwin.so
--rw-r--r--   0 zyhu       (502) staff       (20)   656160 2023-06-04 04:41:55.000000 pydisort-0.0.3/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so
--rw-r--r--   0 zyhu       (502) staff       (20)   547920 2023-06-04 14:55:32.000000 pydisort-0.0.3/pydisort/pydisort.cpython-38-darwin.so
--rwxr-xr-x   0 zyhu       (502) staff       (20)   652096 2023-06-04 01:53:08.000000 pydisort-0.0.3/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 15:20:24.827742 pydisort-0.0.3/pydisort.egg-info/
--rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-04 15:20:24.000000 pydisort-0.0.3/pydisort.egg-info/PKG-INFO
--rw-r--r--   0 zyhu       (502) staff       (20)      335 2023-06-04 15:20:24.000000 pydisort-0.0.3/pydisort.egg-info/SOURCES.txt
--rw-r--r--   0 zyhu       (502) staff       (20)        1 2023-06-04 15:20:24.000000 pydisort-0.0.3/pydisort.egg-info/dependency_links.txt
--rw-r--r--   0 zyhu       (502) staff       (20)        9 2023-06-04 15:20:24.000000 pydisort-0.0.3/pydisort.egg-info/top_level.txt
--rw-r--r--   0 zyhu       (502) staff       (20)       38 2023-06-04 15:20:24.828893 pydisort-0.0.3/setup.cfg
--rw-r--r--   0 zyhu       (502) staff       (20)      193 2023-06-04 15:20:13.000000 pydisort-0.0.3/setup.py
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 16:28:07.991413 pydisort-0.0.4/
+-rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-04 16:28:07.990613 pydisort-0.0.4/PKG-INFO
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 16:28:07.982846 pydisort-0.0.4/pydisort/
+-rw-r--r--   0 zyhu       (502) staff       (20)       24 2023-06-04 01:28:16.000000 pydisort-0.0.4/pydisort/__init__.py
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 16:24:51.000000 pydisort-0.0.4/pydisort/pydisort.cpython-310-darwin.so
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 00:45:04.000000 pydisort-0.0.4/pydisort/pydisort.cpython-311-darwin.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   656160 2023-06-04 04:41:55.000000 pydisort-0.0.4/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so
+-rw-r--r--   0 zyhu       (502) staff       (20)   547920 2023-06-04 14:55:32.000000 pydisort-0.0.4/pydisort/pydisort.cpython-38-darwin.so
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 16:19:20.000000 pydisort-0.0.4/pydisort/pydisort.cpython-39-darwin.so
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   652096 2023-06-04 01:53:08.000000 pydisort-0.0.4/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 16:28:07.989755 pydisort-0.0.4/pydisort.egg-info/
+-rw-r--r--   0 zyhu       (502) staff       (20)       52 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/PKG-INFO
+-rw-r--r--   0 zyhu       (502) staff       (20)      414 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/SOURCES.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)        1 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/dependency_links.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)        9 2023-06-04 16:28:07.000000 pydisort-0.0.4/pydisort.egg-info/top_level.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)       38 2023-06-04 16:28:07.992008 pydisort-0.0.4/setup.cfg
+-rw-r--r--   0 zyhu       (502) staff       (20)      193 2023-06-04 16:27:37.000000 pydisort-0.0.4/setup.py
```

### Comparing `pydisort-0.0.3/pydisort/pydisort.cpython-311-darwin.so` & `pydisort-0.0.4/pydisort/pydisort.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.3/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so` & `pydisort-0.0.4/pydisort/pydisort.cpython-36m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.3/pydisort/pydisort.cpython-38-darwin.so` & `pydisort-0.0.4/pydisort/pydisort.cpython-38-darwin.so`

 * *Files identical despite different names*

### Comparing `pydisort-0.0.3/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so` & `pydisort-0.0.4/pydisort/pydisort.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

