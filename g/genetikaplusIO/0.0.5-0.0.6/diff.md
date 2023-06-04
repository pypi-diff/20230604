# Comparing `tmp/genetikaplusIO-0.0.5.tar.gz` & `tmp/genetikaplusIO-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetikaplusIO-0.0.5.tar", last modified: Sun Jun  4 13:04:42 2023, max compression
+gzip compressed data, was "genetikaplusIO-0.0.6.tar", last modified: Sun Jun  4 13:50:05 2023, max compression
```

## Comparing `genetikaplusIO-0.0.5.tar` & `genetikaplusIO-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 13:04:42.879801 genetikaplusIO-0.0.5/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusIO-0.0.5/LICENSE.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     5200 2023-06-04 13:04:42.879631 genetikaplusIO-0.0.5/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3700 2023-06-04 12:46:28.000000 genetikaplusIO-0.0.5/README.md
--rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-04 13:04:42.879848 genetikaplusIO-0.0.5/setup.cfg
--rw-r--r--   0 alonbentzion   (501) staff       (20)      762 2023-06-04 13:03:58.000000 genetikaplusIO-0.0.5/setup.py
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 13:04:42.878773 genetikaplusIO-0.0.5/src/
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 13:04:42.879445 genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     5200 2023-06-04 13:04:42.000000 genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-04 13:04:42.000000 genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/SOURCES.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-04 13:04:42.000000 genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/dependency_links.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-04 13:04:42.000000 genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/requires.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-04 13:04:42.000000 genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/top_level.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     6906 2023-06-04 12:43:30.000000 genetikaplusIO-0.0.5/src/gp_db_io.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     2000 2023-06-01 15:07:22.000000 genetikaplusIO-0.0.5/src/gp_sqlconnection.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-04 13:04:01.000000 genetikaplusIO-0.0.5/src/gp_storage_io.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 13:50:05.377459 genetikaplusIO-0.0.6/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusIO-0.0.6/LICENSE.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     5200 2023-06-04 13:50:05.377290 genetikaplusIO-0.0.6/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     3700 2023-06-04 12:46:28.000000 genetikaplusIO-0.0.6/README.md
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-04 13:50:05.377503 genetikaplusIO-0.0.6/setup.cfg
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      762 2023-06-04 13:48:44.000000 genetikaplusIO-0.0.6/setup.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 13:50:05.375942 genetikaplusIO-0.0.6/src/
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 13:50:05.377099 genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     5200 2023-06-04 13:50:05.000000 genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      239 2023-06-04 13:50:05.000000 genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/SOURCES.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-04 13:50:05.000000 genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/dependency_links.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-04 13:50:05.000000 genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/requires.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-04 13:50:05.000000 genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/top_level.txt
```

### Comparing `genetikaplusIO-0.0.5/LICENSE.txt` & `genetikaplusIO-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.5/PKG-INFO` & `genetikaplusIO-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusIO
-Version: 0.0.5
+Version: 0.0.6
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `genetikaplusIO-0.0.5/README.md` & `genetikaplusIO-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.5/setup.py` & `genetikaplusIO-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     requirements = r.read().splitlines()
 
 with open("LICENSE.txt", 'r') as l:
     license = l.read()
 
 setup(
     name="genetikaplusIO",
-    version="0.0.5",
+    version="0.0.6",
     author="Alon Ben Zion",
     author_email="alon@genetikaplus.com",
     license=license,
     description="IO for database",
     py_modules=["gp_db_io", "gp_storage_io", "gp_sqlconnection"],
     package_dir={"": "src"},
     classifiers=[
```

### Comparing `genetikaplusIO-0.0.5/src/genetikaplusIO.egg-info/PKG-INFO` & `genetikaplusIO-0.0.6/src/genetikaplusIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusIO
-Version: 0.0.5
+Version: 0.0.6
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

