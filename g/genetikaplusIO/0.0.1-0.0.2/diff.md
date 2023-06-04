# Comparing `tmp/genetikaplusIO-0.0.1.tar.gz` & `tmp/genetikaplusIO-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetikaplusIO-0.0.1.tar", last modified: Thu Jun  1 15:08:23 2023, max compression
+gzip compressed data, was "genetikaplusIO-0.0.2.tar", last modified: Sun Jun  4 12:22:50 2023, max compression
```

## Comparing `genetikaplusIO-0.0.1.tar` & `genetikaplusIO-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 15:08:23.482534 genetikaplusIO-0.0.1/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusIO-0.0.1/LICENSE.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     5085 2023-06-01 15:08:23.482371 genetikaplusIO-0.0.1/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3585 2023-06-01 15:07:25.000000 genetikaplusIO-0.0.1/README.md
--rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-01 15:08:23.482580 genetikaplusIO-0.0.1/setup.cfg
--rw-r--r--   0 alonbentzion   (501) staff       (20)     1167 2023-06-01 15:08:03.000000 genetikaplusIO-0.0.1/setup.py
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 15:08:23.481495 genetikaplusIO-0.0.1/src/
-drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-01 15:08:23.482170 genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/
--rw-r--r--   0 alonbentzion   (501) staff       (20)     5085 2023-06-01 15:08:23.000000 genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/PKG-INFO
--rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-01 15:08:23.000000 genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/SOURCES.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-01 15:08:23.000000 genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/dependency_links.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-01 15:08:23.000000 genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/requires.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-01 15:08:23.000000 genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/top_level.txt
--rw-r--r--   0 alonbentzion   (501) staff       (20)     6913 2023-06-01 15:07:21.000000 genetikaplusIO-0.0.1/src/gp_db_io.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     2000 2023-06-01 15:07:22.000000 genetikaplusIO-0.0.1/src/gp_sqlconnection.py
--rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-01 15:07:24.000000 genetikaplusIO-0.0.1/src/gp_storage_io.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:22:50.161462 genetikaplusIO-0.0.2/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1035 2023-06-01 14:13:50.000000 genetikaplusIO-0.0.2/LICENSE.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     5085 2023-06-04 12:22:50.161229 genetikaplusIO-0.0.2/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     3585 2023-06-01 15:07:25.000000 genetikaplusIO-0.0.2/README.md
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       38 2023-06-04 12:22:50.161512 genetikaplusIO-0.0.2/setup.cfg
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     1167 2023-06-04 12:12:26.000000 genetikaplusIO-0.0.2/setup.py
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:22:50.159995 genetikaplusIO-0.0.2/src/
+drwxr-xr-x   0 alonbentzion   (501) staff       (20)        0 2023-06-04 12:22:50.160962 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     5085 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/PKG-INFO
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      300 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/SOURCES.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)        1 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/dependency_links.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)      318 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/requires.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)       40 2023-06-04 12:22:50.000000 genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/top_level.txt
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     6906 2023-06-04 12:06:23.000000 genetikaplusIO-0.0.2/src/gp_db_io.py
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     2000 2023-06-01 15:07:22.000000 genetikaplusIO-0.0.2/src/gp_sqlconnection.py
+-rw-r--r--   0 alonbentzion   (501) staff       (20)     3034 2023-06-01 15:07:24.000000 genetikaplusIO-0.0.2/src/gp_storage_io.py
```

### Comparing `genetikaplusIO-0.0.1/LICENSE.txt` & `genetikaplusIO-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.1/PKG-INFO` & `genetikaplusIO-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusIO
-Version: 0.0.1
+Version: 0.0.2
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `genetikaplusIO-0.0.1/README.md` & `genetikaplusIO-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.1/setup.py` & `genetikaplusIO-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     requirements = r.read().splitlines()
 
 with open("LICENSE.txt", 'r') as l:
     license = l.read()
 
 setup(
     name="genetikaplusIO",
-    version="0.0.1",
+    version="0.0.2",
     author="Alon Ben Zion",
     author_email="alon@genetikaplus.com",
     license=license,
     description="IO for database",
     py_modules=["gp_db_io", "gp_storage_io", "gp_sqlconnection"],
     package_dir={"": "src"},
     classifiers=[
```

### Comparing `genetikaplusIO-0.0.1/src/genetikaplusIO.egg-info/PKG-INFO` & `genetikaplusIO-0.0.2/src/genetikaplusIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetikaplusIO
-Version: 0.0.1
+Version: 0.0.2
 Summary: IO for database
 Author: Alon Ben Zion
 Author-email: alon@genetikaplus.com
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `genetikaplusIO-0.0.1/src/gp_db_io.py` & `genetikaplusIO-0.0.2/src/gp_db_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 import pandas as pd
-from . import gp_sqlconnection as sqlConnection
+import gp_sqlconnection as sqlConnection
 from psycopg2.errors import OperationalError, UndefinedTable
 import sqlalchemy
 from sqlalchemy.sql.expression import text
 
 
 def dbReadQuery(query: str, database: str = "gbase", **kwargs):
     """
```

### Comparing `genetikaplusIO-0.0.1/src/gp_sqlconnection.py` & `genetikaplusIO-0.0.2/src/gp_sqlconnection.py`

 * *Files identical despite different names*

### Comparing `genetikaplusIO-0.0.1/src/gp_storage_io.py` & `genetikaplusIO-0.0.2/src/gp_storage_io.py`

 * *Files identical despite different names*

