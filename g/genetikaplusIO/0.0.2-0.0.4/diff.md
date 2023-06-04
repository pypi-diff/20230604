# Comparing `tmp/genetikaplusIO-0.0.2.tar.gz` & `tmp/genetikaplusIO-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetikaplusIO-0.0.2.tar", last modified: Sun Jun  4 12:22:50 2023, max compression
+gzip compressed data, was "genetikaplusIO-0.0.4.tar", last modified: Sun Jun  4 12:47:10 2023, max compression
```

## Comparing `genetikaplusIO-0.0.2.tar` & `genetikaplusIO-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:22:50.161462 genetikaplusIO-0.0.2/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusIO-0.0.2/LICENSE.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     5085 2023-06-04 12:22:50.161229 genetikaplusIO-0.0.2/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3585 2023-06-01 15:07:25.000000 genetikaplusIO-0.0.2/README.md
--rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-04 12:22:50.161512 genetikaplusIO-0.0.2/setup.cfg
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1167 2023-06-04 12:12:26.000000 genetikaplusIO-0.0.2/setup.py
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:22:50.159995 genetikaplusIO-0.0.2/src/
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:22:50.160962 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     5085 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/SOURCES.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/dependency_links.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/requires.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/top_level.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     6906 2023-06-04 12:06:23.000000 genetikaplusIO-0.0.2/src/gp_db_io.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     2000 2023-06-01 15:07:22.000000 genetikaplusIO-0.0.2/src/gp_sqlconnection.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-01 15:07:24.000000 genetikaplusIO-0.0.2/src/gp_storage_io.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:47:10.320967 genetikaplusIO-0.0.4/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusIO-0.0.4/LICENSE.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     5200 2023-06-04 12:47:10.320788 genetikaplusIO-0.0.4/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     3700 2023-06-04 12:46:28.000000 genetikaplusIO-0.0.4/README.md
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-04 12:47:10.321011 genetikaplusIO-0.0.4/setup.cfg
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      762 2023-06-04 12:46:46.000000 genetikaplusIO-0.0.4/setup.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:47:10.316002 genetikaplusIO-0.0.4/src/
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:47:10.320568 genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     5200 2023-06-04 12:47:10.000000 genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-04 12:47:10.000000 genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/SOURCES.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-04 12:47:10.000000 genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/dependency_links.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-04 12:47:10.000000 genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/requires.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-04 12:47:10.000000 genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/top_level.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     6906 2023-06-04 12:43:30.000000 genetikaplusIO-0.0.4/src/gp_db_io.py
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     2000 2023-06-01 15:07:22.000000 genetikaplusIO-0.0.4/src/gp_sqlconnection.py
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-01 15:07:24.000000 genetikaplusIO-0.0.4/src/gp_storage_io.py
```

### Comparing `genetikaplusIO-0.0.2/LICENSE.txt` & `genetikaplusIO-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.2/PKG-INFO` & `genetikaplusIO-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusIO
-Version: 0.0.2
+Version: 0.0.4
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -29,15 +29,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # **GPIO Package**
 
 The GPIO package is a Python package that provides functionality for managing input/output operations related to
 Postgres databases and file storage.
-It consists of two modules: db and storage.
+It consists of three modules: dgp_db_io, gp_storage_io, gp_sqlconnection.
+Before you download this package you need to have an env file in your root directory
 
 ## **Installation**
 
 To install the genetikaplusIO package, you can use pip:
 
 `pip install genetikaplusIO`
```

### Comparing `genetikaplusIO-0.0.2/README.md` & `genetikaplusIO-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # **GPIO Package**
 
 The GPIO package is a Python package that provides functionality for managing input/output operations related to
 Postgres databases and file storage.
-It consists of two modules: db and storage.
+It consists of three modules: dgp_db_io, gp_storage_io, gp_sqlconnection.
+Before you download this package you need to have an env file in your root directory
 
 ## **Installation**
 
 To install the genetikaplusIO package, you can use pip:
 
 `pip install genetikaplusIO`
```

### Comparing `genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/PKG-INFO` & `genetikaplusIO-0.0.4/src/genetikaplusIO.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusIO
-Version: 0.0.2
+Version: 0.0.4
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -29,15 +29,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # **GPIO Package**
 
 The GPIO package is a Python package that provides functionality for managing input/output operations related to
 Postgres databases and file storage.
-It consists of two modules: db and storage.
+It consists of three modules: dgp_db_io, gp_storage_io, gp_sqlconnection.
+Before you download this package you need to have an env file in your root directory
 
 ## **Installation**
 
 To install the genetikaplusIO package, you can use pip:
 
 `pip install genetikaplusIO`
```

### Comparing `genetikaplusIO-0.0.2/src/gp_db_io.py` & `genetikaplusIO-0.0.4/src/gp_db_io.py`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.2/src/gp_sqlconnection.py` & `genetikaplusIO-0.0.4/src/gp_sqlconnection.py`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.2/src/gp_storage_io.py` & `genetikaplusIO-0.0.4/src/gp_storage_io.py`

 * *Files identical despite different names*

