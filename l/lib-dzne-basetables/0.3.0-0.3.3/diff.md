# Comparing `tmp/lib-dzne-basetables-0.3.0.tar.gz` & `tmp/lib-dzne-basetables-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-basetables-0.3.0.tar", last modified: Fri Jun  2 22:17:33 2023, max compression
+gzip compressed data, was "lib-dzne-basetables-0.3.3.tar", last modified: Sun Jun  4 21:16:45 2023, max compression
```

## Comparing `lib-dzne-basetables-0.3.0.tar` & `lib-dzne-basetables-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.3.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       22 2023-05-29 09:10:54.000000 lib-dzne-basetables-0.3.0/README.md
--rw-r--r--   0 base      (1001) base      (1001)      528 2023-06-02 22:16:56.000000 lib-dzne-basetables-0.3.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/
--rw-r--r--   0 base      (1001) base      (1001)       88 2023-06-02 22:16:04.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/__init__.py
--rw-rw-r--   0 base      (1001) base      (1001)     1732 2023-06-02 22:17:06.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/_data.py
--rw-r--r--   0 base      (1001) base      (1001)     2363 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/baseconv.py
--rw-r--r--   0 base      (1001) base      (1001)      675 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/common.py
--rw-r--r--   0 base      (1001) base      (1001)     1524 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/pattern.py
--rw-r--r--   0 base      (1001) base      (1001)     7732 2023-05-29 12:54:58.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/table.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-02 22:17:33.155144 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      483 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-06-02 22:17:33.000000 lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 21:16:45.925114 lib-dzne-basetables-0.3.3/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.3.3/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-04 21:16:45.925114 lib-dzne-basetables-0.3.3/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       22 2023-05-29 09:10:54.000000 lib-dzne-basetables-0.3.3/README.md
+-rw-r--r--   0 base      (1001) base      (1001)      528 2023-06-04 21:16:36.000000 lib-dzne-basetables-0.3.3/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-04 21:16:45.925114 lib-dzne-basetables-0.3.3/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 21:16:45.925114 lib-dzne-basetables-0.3.3/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 21:16:45.925114 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables/
+-rw-r--r--   0 base      (1001) base      (1001)    10385 2023-06-04 21:14:50.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     1524 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables/_pattern.py
+-rw-rw-r--   0 base      (1001) base      (1001)     1858 2023-06-04 21:07:25.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables/_utils.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-04 21:16:45.925114 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-06-04 21:16:45.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      382 2023-06-04 21:16:45.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-04 21:16:45.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-06-04 21:16:45.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-06-04 21:16:45.000000 lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/top_level.txt
```

### Comparing `lib-dzne-basetables-0.3.0/LICENSE` & `lib-dzne-basetables-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.3.0/PKG-INFO` & `lib-dzne-basetables-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-basetables
-Version: 0.3.0
+Version: 0.3.3
 Summary: Libary for basetables. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-basetables-0.3.0/pyproject.toml` & `lib-dzne-basetables-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-basetables"
-version = "0.3.0"
+version = "0.3.3"
 description = "Libary for basetables. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables/pattern.py` & `lib-dzne-basetables-0.3.3/src/lib_dzne_basetables/_pattern.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.3.0/src/lib_dzne_basetables.egg-info/PKG-INFO` & `lib-dzne-basetables-0.3.3/src/lib_dzne_basetables.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-basetables
-Version: 0.3.0
+Version: 0.3.3
 Summary: Libary for basetables. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

