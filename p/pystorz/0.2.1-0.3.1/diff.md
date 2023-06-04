# Comparing `tmp/pystorz-0.2.1.tar.gz` & `tmp/pystorz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystorz-0.2.1.tar", last modified: Wed May 31 04:18:32 2023, max compression
+gzip compressed data, was "dist/pystorz-0.3.1.tar", last modified: Sun Jun  4 18:46:53 2023, max compression
```

## Comparing `pystorz-0.2.1.tar` & `pystorz-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.632314 pystorz-0.2.1/
--rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.2.1/LICENSE
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-31 04:18:32.632111 pystorz-0.2.1/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)     2558 2023-04-26 01:57:49.000000 pystorz-0.2.1/README.md
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.627784 pystorz-0.2.1/pystorz/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.2.1/pystorz/__init__.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.628843 pystorz-0.2.1/pystorz/internal/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.2.1/pystorz/internal/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)      334 2023-04-29 21:02:22.000000 pystorz-0.2.1/pystorz/internal/constants.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.629597 pystorz-0.2.1/pystorz/mgen/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.2.1/pystorz/mgen/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     3892 2023-04-24 17:22:07.000000 pystorz-0.2.1/pystorz/mgen/builder.py
--rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.2.1/pystorz/mgen/loader.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.630790 pystorz-0.2.1/pystorz/mgen/templates/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.2.1/pystorz/mgen/templates/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/imports.py
--rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.2.1/pystorz/mgen/templates/interface.py
--rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/schema.py
--rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/templates/specinternal.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.2.1/pystorz/mgen/templates/structure.py
--rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.2.1/pystorz/mgen/templates/unmarshall.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.2.1/pystorz/mgen/test.py
--rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.2.1/pystorz/mgen/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.631080 pystorz-0.2.1/pystorz/sql/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.2.1/pystorz/sql/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)    15702 2023-05-31 04:07:15.000000 pystorz-0.2.1/pystorz/sql/store.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.631872 pystorz-0.2.1/pystorz/store/
--rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.2.1/pystorz/store/__init__.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.2.1/pystorz/store/meta.py
--rw-r--r--   0 wazofski   (501) staff       (20)     8681 2023-05-30 20:25:45.000000 pystorz-0.2.1/pystorz/store/options.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2997 2023-05-30 20:27:50.000000 pystorz-0.2.1/pystorz/store/store.py
--rw-r--r--   0 wazofski   (501) staff       (20)     2869 2023-04-29 00:20:58.000000 pystorz-0.2.1/pystorz/store/utils.py
-drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-05-31 04:18:32.628555 pystorz-0.2.1/pystorz.egg-info/
--rw-r--r--   0 wazofski   (501) staff       (20)     2915 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/PKG-INFO
--rw-r--r--   0 wazofski   (501) staff       (20)      819 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/SOURCES.txt
--rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/dependency_links.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       36 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/requires.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       87 2023-05-31 04:18:32.000000 pystorz-0.2.1/pystorz.egg-info/top_level.txt
--rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-05-31 04:18:32.632365 pystorz-0.2.1/setup.cfg
--rw-r--r--   0 wazofski   (501) staff       (20)      963 2023-05-31 04:08:02.000000 pystorz-0.2.1/setup.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.053105 pystorz-0.3.1/
+-rw-r--r--   0 wazofski   (501) staff       (20)     1086 2023-04-24 05:31:47.000000 pystorz-0.3.1/LICENSE
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-04 18:46:53.052918 pystorz-0.3.1/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)     2615 2023-06-04 18:42:13.000000 pystorz-0.3.1/README.md
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.045306 pystorz-0.3.1/pystorz/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:48.000000 pystorz-0.3.1/pystorz/__init__.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.046282 pystorz-0.3.1/pystorz/internal/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:44.000000 pystorz-0.3.1/pystorz/internal/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      380 2023-06-04 14:02:51.000000 pystorz-0.3.1/pystorz/internal/constants.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.046560 pystorz-0.3.1/pystorz/meta/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2630 2023-06-04 14:02:51.000000 pystorz-0.3.1/pystorz/meta/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.047869 pystorz-0.3.1/pystorz/mgen/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:41.000000 pystorz-0.3.1/pystorz/mgen/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     4161 2023-06-03 19:10:23.000000 pystorz-0.3.1/pystorz/mgen/builder.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     7119 2023-05-02 17:05:13.000000 pystorz-0.3.1/pystorz/mgen/loader.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.049465 pystorz-0.3.1/pystorz/mgen/templates/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:21:36.000000 pystorz-0.3.1/pystorz/mgen/templates/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)       56 2023-04-24 14:15:03.000000 pystorz-0.3.1/pystorz/mgen/templates/imports.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      225 2023-04-24 14:24:31.000000 pystorz-0.3.1/pystorz/mgen/templates/interface.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      331 2023-04-24 14:15:03.000000 pystorz-0.3.1/pystorz/mgen/templates/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      473 2023-04-24 14:15:03.000000 pystorz-0.3.1/pystorz/mgen/templates/schema.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      110 2023-04-24 14:15:03.000000 pystorz-0.3.1/pystorz/mgen/templates/specinternal.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1123 2023-05-01 01:21:35.000000 pystorz-0.3.1/pystorz/mgen/templates/structure.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1772 2023-05-02 17:04:18.000000 pystorz-0.3.1/pystorz/mgen/templates/unmarshall.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2808 2023-04-24 15:47:15.000000 pystorz-0.3.1/pystorz/mgen/test.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      611 2023-04-24 14:15:03.000000 pystorz-0.3.1/pystorz/mgen/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.050422 pystorz-0.3.1/pystorz/rest/
+-rw-r--r--   0 wazofski   (501) staff       (20)     8259 2023-06-04 14:02:51.000000 pystorz-0.3.1/pystorz/rest/client.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     1099 2023-06-03 19:10:23.000000 pystorz-0.3.1/pystorz/rest/headers.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2462 2023-06-04 14:02:51.000000 pystorz-0.3.1/pystorz/rest/internals.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     9691 2023-06-04 15:53:12.000000 pystorz-0.3.1/pystorz/rest/server.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.051450 pystorz-0.3.1/pystorz/sql/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:39.000000 pystorz-0.3.1/pystorz/sql/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2617 2023-06-04 18:13:23.000000 pystorz-0.3.1/pystorz/sql/mysql.py
+-rw-r--r--   0 wazofski   (501) staff       (20)      192 2023-06-04 16:07:46.000000 pystorz-0.3.1/pystorz/sql/sqlite.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    15373 2023-06-04 18:21:14.000000 pystorz-0.3.1/pystorz/sql/store.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.052666 pystorz-0.3.1/pystorz/store/
+-rw-r--r--   0 wazofski   (501) staff       (20)        0 2023-04-24 14:17:33.000000 pystorz-0.3.1/pystorz/store/__init__.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2667 2023-04-26 20:36:31.000000 pystorz-0.3.1/pystorz/store/meta.py
+-rw-r--r--   0 wazofski   (501) staff       (20)    10450 2023-06-04 14:02:51.000000 pystorz-0.3.1/pystorz/store/options.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     2974 2023-06-03 19:10:23.000000 pystorz-0.3.1/pystorz/store/store.py
+-rw-r--r--   0 wazofski   (501) staff       (20)     3505 2023-06-04 14:02:51.000000 pystorz-0.3.1/pystorz/store/utils.py
+drwxr-xr-x   0 wazofski   (501) staff       (20)        0 2023-06-04 18:46:53.046029 pystorz-0.3.1/pystorz.egg-info/
+-rw-r--r--   0 wazofski   (501) staff       (20)     2992 2023-06-04 18:46:53.000000 pystorz-0.3.1/pystorz.egg-info/PKG-INFO
+-rw-r--r--   0 wazofski   (501) staff       (20)      980 2023-06-04 18:46:53.000000 pystorz-0.3.1/pystorz.egg-info/SOURCES.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)        1 2023-06-04 18:46:53.000000 pystorz-0.3.1/pystorz.egg-info/dependency_links.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       93 2023-06-04 18:46:53.000000 pystorz-0.3.1/pystorz.egg-info/requires.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)      113 2023-06-04 18:46:53.000000 pystorz-0.3.1/pystorz.egg-info/top_level.txt
+-rw-r--r--   0 wazofski   (501) staff       (20)       38 2023-06-04 18:46:53.053152 pystorz-0.3.1/setup.cfg
+-rw-r--r--   0 wazofski   (501) staff       (20)     1290 2023-06-04 18:46:27.000000 pystorz-0.3.1/setup.py
```

### Comparing `pystorz-0.2.1/LICENSE` & `pystorz-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/PKG-INFO` & `pystorz-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
-<img src="logo.png" width="300" alt="storz" />
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
 </p>
 
 **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
 
 **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
 
 Original storz was written in go. You can check it out here:
@@ -55,15 +56,15 @@
 
     # you can then import the generated model
     from generated import model
 
     # initialize a store
     stor = SqliteStore(
         Schema(),
-        SqliteConnection("path/to/your/sqlite3.db"))
+        SqliteConnector("path/to/your/sqlite3.db"))
 
     world = model.WorldFactory()
     world.External().SetName("hello")
 
     created_world = stor.Create(world)
     world.External().SetDescription("hello world")
     updated_world = stor.Update(world.Metadata().Identity(), world)
```

### Comparing `pystorz-0.2.1/README.md` & `pystorz-0.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-<img src="logo.png" width="300" alt="storz" />
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
 </p>
 
 **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
 
 **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
 
 Original storz was written in go. You can check it out here:
@@ -43,15 +43,15 @@
 
     # you can then import the generated model
     from generated import model
 
     # initialize a store
     stor = SqliteStore(
         Schema(),
-        SqliteConnection("path/to/your/sqlite3.db"))
+        SqliteConnector("path/to/your/sqlite3.db"))
 
     world = model.WorldFactory()
     world.External().SetName("hello")
 
     created_world = stor.Create(world)
     world.External().SetDescription("hello world")
     updated_world = stor.Update(world.Metadata().Identity(), world)
```

### Comparing `pystorz-0.2.1/pystorz/mgen/builder.py` & `pystorz-0.3.1/pystorz/mgen/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import os
 import shutil
 import black
 import logging
-from typing import List
 from io import StringIO
 
 from jinja2 import Template
 
 from pystorz.mgen.loader import load_model, Resource, Struct, Prop, typeDefault
 from pystorz.store import utils
 
 log = logging.getLogger(__name__)
 log.debug('loading builder.py...')
 
 
-def Generate(model: str) -> None:
-    structs, resources = load_model(model)
+def Generate(*models) -> None:
+    structs = []
+    resources = []
+
+    for model in models:
+        log.debug(f"Loading model {model}...")
+        
+        s, r = load_model(model)
+        
+        structs.extend(s)
+        resources.extend(r)
 
     imports = [
         "import json",
         "from pystorz.store import utils",
         "from pystorz.store import store",
         "from pystorz.store import meta",
     ]
@@ -40,15 +48,15 @@
     if os.path.exists(targetDir):
         # delete the directory with contents
         shutil.rmtree(targetDir)
 
     utils.export_file(targetDir, "model.py", res)
 
 
-def compileResources(resources: List[Resource]) -> str:
+def compileResources(resources: list[Resource]) -> str:
     b = StringIO()
 
     for r in resources:
         log.debug(f"Compiling resource {r.name}...")
 
         props = [
             Prop(
@@ -80,15 +88,15 @@
         b.write(render("mgen/templates/meta.py", r))
 
     b.write(render("mgen/templates/schema.py", {"resources": resources}))
 
     return b.getvalue()
 
 
-def compileStructs(structs: List[Struct]) -> str:
+def compileStructs(structs: list[Struct]) -> str:
     b = StringIO()
 
     for s in structs:
         b.write(compileStruct(s))
 
     return b.getvalue()
 
@@ -97,28 +105,35 @@
     log.debug(f"Compiling struct {s.name}...")
 
     b = StringIO()
     methods = []
 
     s.properties = addDefaultPropValues(s.properties)
 
+    parent = "store.Object"
+
     for p in s.properties:
         if p.name != "Meta":
             # methods.append(f"{p.name}(self) -> {p.StrippedType()}")
             methods.append(f"{p.name}(self)")
 
         if p.name != "Meta" and p.name != "External" and p.name != "Internal":
             # methods.append(f"Set{p.name}(self, val: {p.StrippedType()})")
             methods.append(f"Set{p.name}(self, val)")
 
-    b.write(render("mgen/templates/interface.py",
+        if p.name == "External":
+            parent = "store.ExternalHolder"
+    
+    b.write(
+        render(
+            "mgen/templates/interface.py",
             {
                 'name': s.name,
                 'methods': methods,
-                'implements': "store.Object"
+                'implements': parent
             }))
 
     for p in s.properties:
         if p.name == "External":
             b.write(render("mgen/templates/specinternal.py", None))
 
     b.write(render("mgen/templates/structure.py", s))
@@ -133,15 +148,15 @@
     with open(path, 'r') as f:
         content = f.read()
 
     t = Template(content)
     return t.render(data=data)
 
 
-def addDefaultPropValues(props: List[Prop]) -> List[Prop]:
+def addDefaultPropValues(props: list[Prop]) -> list[Prop]:
     res = []
 
     for p in props:
         if len(p.default) > 0:
             res.append(p)
             continue
```

### Comparing `pystorz-0.2.1/pystorz/mgen/loader.py` & `pystorz-0.3.1/pystorz/mgen/loader.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/pystorz/mgen/templates/structure.py` & `pystorz-0.3.1/pystorz/mgen/templates/structure.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/pystorz/mgen/templates/unmarshall.py` & `pystorz-0.3.1/pystorz/mgen/templates/unmarshall.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/pystorz/mgen/test.py` & `pystorz-0.3.1/pystorz/mgen/test.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/pystorz/mgen/utils.py` & `pystorz-0.3.1/pystorz/mgen/utils.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/pystorz/sql/store.py` & `pystorz-0.3.1/pystorz/sql/store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,93 @@
 import logging
-import sqlite3
+import threading
+import sqlparse
+
 from pystorz.internal import constants
 from pystorz.store import store, options, utils
-from datetime import datetime
 
 log = logging.getLogger(__name__)
 
 
-def SqliteConnection(path):
-    def func():
-        return sqlite3.connect(path)
-
-    return func
-
-
-# def MySqlConnection(path):
-#     def __call__():
-#         log.Printf("mysql connection %s", path)
-#         return mysql.connect(path)
-
+class SqlStore(store.Store):
+    def __init__(self, Schema, connector):
+        self._schema = Schema
+        self._makeConnection = connector
+        self._connection_cache = {}
+
+    def _connection(self):
+        tid = threading.get_ident()
+        if tid not in self._connection_cache:
+            self._connection_cache[tid] = self._makeConnection()
+            self._prepareTables(self._connection_cache[tid])
 
-class SqliteStore:
-    def __init__(self, Schema, MakeConnection):
-        self.Schema = Schema
-        self.MakeConnection = MakeConnection
-        self.DB = None
+        return self._connection_cache[tid]
 
-    def TestConnection(self):
-        if self.DB is not None:
-            return
-
-        self.DB = self.MakeConnection()
-        self._prepareTables()
-
-        return self.DB.cursor()
-
-    def Create(self, obj, opt=[]):
+    def Create(self, obj, *opt):
         if obj is None:
             raise Exception(constants.ErrObjectNil)
 
-        log.info("create {}".format(obj.PrimaryKey()))
-
-        copt = options.CommonOptionHolderFactory()
-        for o in opt:
-            o.ApplyFunction()(copt)
+        log.info("create {} {}".format(
+            obj.Metadata().Kind(),
+            obj.PrimaryKey()))
+
+        # copt = options.CommonOptionHolderFactory()
+        # for o in opt:
+        #     o.ApplyFunction()(copt)
 
         lk = obj.Metadata().Kind().lower()
         path = "{}/{}".format(lk, obj.PrimaryKey())
         existing = None
         try:
             existing = self.Get(store.ObjectIdentity(path))
         except Exception as e:
             pass
+
         if existing is not None:
             raise Exception(constants.ErrObjectExists)
 
-        self.TestConnection()
-
-        obj.Metadata().SetCreated(datetime.now())
-        obj.Metadata().SetUpdated(obj.Metadata().Created())
-        obj.Metadata().SetRevision(1)
+        db = self._connection()
 
         try:
             # Start a transaction
-            self.DB.execute("BEGIN")
-            cursor = self.DB.cursor()
+            db.execute("BEGIN")
+            cursor = db.cursor()
 
             self._setIdentity(
                 cursor,
                 obj.Metadata().Identity().Path(),
                 obj.PrimaryKey(),
                 obj.Metadata().Kind(),
             )
 
             self._setObject(cursor, obj.PrimaryKey(), obj.Metadata().Kind(), obj)
 
             # Commit the transaction
-            self.DB.commit()
+            db.commit()
             return obj.Clone()
         except Exception as e:
-            self.DB.rollback()
+            db.rollback()
             raise e
 
     def Update(self, identity, obj, *opt):
-        log.info("update {}".format(identity.Path()))
-
-        copt = options.CommonOptionHolderFactory()
+        # copt = options.CommonOptionHolderFactory()
+        # for o in opt:
+        #     o.ApplyFunction()(copt)
 
-        for o in opt:
-            o.ApplyFunction()(copt)
+        if identity is None:
+            raise Exception(constants.ErrInvalidPath)
 
         if obj is None:
             raise Exception(constants.ErrObjectNil)
 
+        log.info("update {}".format(identity.Path()))
+
         existing = self.Get(identity)
-        if existing is None:
-            raise Exception(constants.ErrNoSuchObject)
+        if existing.Metadata().Kind() != obj.Metadata().Kind():
+            raise Exception(constants.ErrObjectIdentityMismatch)
 
         if existing.PrimaryKey() != obj.PrimaryKey():
             # log.info("primary key changed from {} to {}".format(
             #     existing.PrimaryKey(), obj.PrimaryKey())
             # )
 
             if (
@@ -118,20 +106,20 @@
                 target = self.Get(target_identity)
             except Exception as e:
                 pass
 
             if target is not None:
                 raise Exception(constants.ErrObjectExists)
 
-        self.TestConnection()
+        db = self._connection()
 
         try:
             # Start a transaction
-            self.DB.execute("BEGIN")
-            cursor = self.DB.cursor()
+            db.execute("BEGIN")
+            cursor = db.cursor()
 
             self._removeIdentity(cursor, existing.Metadata().Identity().Path())
 
             obj.Metadata().SetIdentity(existing.Metadata().Identity())
 
             self._setIdentity(
                 cursor,
@@ -140,103 +128,94 @@
                 obj.Metadata().Kind(),
             )
 
             self._removeObject(
                 cursor, existing.PrimaryKey(), existing.Metadata().Kind()
             )
 
-            obj.Metadata().SetCreated(existing.Metadata().Created())
-            obj.Metadata().SetUpdated(datetime.now())
-            obj.Metadata().SetRevision(existing.Metadata().Revision() + 1)
-
             self._setObject(cursor, obj.PrimaryKey(), obj.Metadata().Kind(), obj)
 
-            self.DB.commit()
+            db.commit()
             return obj.Clone()
         except Exception as e:
-            self.DB.rollback()
+            db.rollback()
             raise e
 
     def Delete(self, identity, *opt):
+        if identity is None:
+            raise Exception(constants.ErrInvalidPath)
+
         log.info("delete {}".format(identity.Path()))
         copt = options.CommonOptionHolderFactory()
-
         for o in opt:
             o.ApplyFunction()(copt)
 
         existing = None
         if copt.filter is None:
             existing = self.Get(identity)
-            if existing is None:
-                raise Exception(constants.ErrNoSuchObject)
 
-        self.TestConnection()
+        db = self._connection()
 
-        try:
-            # Start a transaction
-            self.DB.execute("BEGIN")
-            cursor = self.DB.cursor()
+        # try:
+        # Start a transaction
+        db.execute("BEGIN")
+        cursor = db.cursor()
 
-            if copt.filter is None:
-                self._removeIdentity(cursor, existing.Metadata().Identity().Path())
-                self._removeObject(
-                    cursor, existing.PrimaryKey(), existing.Metadata().Kind()
-                )
-            else:
-                clause = self._buildFilterClause(copt, identity)
-                keys = self._getObjectKeys(
-                    cursor,
-                    identity.Type(),
-                    clause)
-                
-                self._removeObjects(
-                    cursor,
-                    identity.Type(),
-                    clause)
-                
-                self._removeIdentities(
-                    cursor,
-                    identity.Type(),
-                    keys)
+        if copt.filter is None:
+            self._removeIdentity(cursor, existing.Metadata().Identity().Path())
+            self._removeObject(
+                cursor, existing.PrimaryKey(), existing.Metadata().Kind()
+            )
+        else:
+            clause = self._buildFilterClause(copt, identity)
+            keys = self._getObjectKeys(cursor, identity.Type(), clause)
 
-            self.DB.commit()
-        except Exception as e:
-            self.DB.rollback()
-            raise e
+            self._removeObjects(cursor, identity.Type(), clause)
+            self._removeIdentities(cursor, identity.Type(), keys)
+
+        db.commit()
+        # except Exception as e:
+        #     db.rollback()
+        #     raise e
 
     def Get(self, identity, *opt):
+        if identity is None:
+            raise Exception(constants.ErrInvalidPath)
+
         log.info("get {}".format(identity.Path()))
 
         copt = options.CommonOptionHolderFactory()
         for o in opt:
             o.ApplyFunction()(copt)
 
-        self.TestConnection()
-
-        cursor = self.DB.cursor()
+        db = self._connection()
+        cursor = db.cursor()
 
         if identity.IsId():
             pkey, typ = self._getIdentity(cursor, identity.Path())
             return self._getObject(cursor, pkey, typ)
 
         return self._getObject(cursor, identity.Key(), identity.Type())
 
-    def List(self, identity, *opt):
-        log.info("list {}".format(identity))
+    def List(self, identity, *opt: list[options.ListOption]):
+        if identity is None:
+            raise Exception(constants.ErrInvalidPath)
+
+        log.info("list {}".format(identity.Path()))
 
         if len(identity.Key()) > 0:
             raise Exception(constants.ErrInvalidPath)
 
         copt = options.CommonOptionHolderFactory()
+
         for o in opt:
             o.ApplyFunction()(copt)
 
-        self.TestConnection()
-
-        cursor = self.DB.cursor()
+        db = self._connection()
+        cursor = db.cursor()
 
         query = """SELECT Object FROM Objects 
         WHERE Type = '{}'""".format(
             identity.Type()
         )
 
         query += self._buildFilterClause(copt, identity)
@@ -253,42 +232,42 @@
 
         if copt.page_size is not None and copt.page_size > 0:
             query = query + " LIMIT {}".format(copt.page_size)
 
         if copt.page_offset is not None and copt.page_offset > 0:
             query = query + " OFFSET {}".format(copt.page_offset)
 
-        cursor = self.DB.cursor()
         self._do_query(cursor, query)
         rows = cursor.fetchall()
 
         return self._parseObjectRows(rows, identity.Type())
 
-    def _prepareTables(self):
+    def _prepareTables(self, db):
         create = """
         CREATE TABLE IF NOT EXISTS IdIndex (
-            Path VARCHAR(25) NOT NULL PRIMARY KEY,
+            Path VARCHAR(75) NOT NULL PRIMARY KEY,
             Pkey NVARCHAR(50) NOT NULL,
             Type VARCHAR(25) NOT NULL);
         """
 
-        cursor = self.DB.cursor()
+        cursor = db.cursor()
         self._do_query(cursor, create)
 
         create = """
         CREATE TABLE IF NOT EXISTS Objects (
             Pkey NVARCHAR(50) NOT NULL,
             Type VARCHAR(25) NOT NULL,
             Object JSON,
             PRIMARY KEY (Pkey,Type));
         """
 
         cursor.execute(create)
         cursor.close()
-        self.DB.commit()
+
+        db.commit()
 
     def _getIdentity(self, cursor, path):
         query = """SELECT Pkey, Type FROM IdIndex 
         WHERE Path='{}'""".format(
             path
         )
 
@@ -298,32 +277,32 @@
         if result is not None:
             pkey, typ = result
             return pkey, typ
         else:
             raise Exception(constants.ErrNoSuchObject)
 
     def _setIdentity(self, cursor, path, pkey, typ):
-        existing_pkey, existing_typ = None, None
+        # existing_pkey, existing_typ = None, None
 
-        try:
-            existing_pkey, existing_typ = self._getIdentity(cursor, path)
-        except Exception as e:
-            log.debug("identity get failed: {}".format(e))
-
-        query = ""
-        if existing_pkey is not None and existing_typ is not None:
-            query = """UPDATE IdIndex SET Pkey='{}', Type='{}'
-            WHERE Path='{}'""".format(
-                pkey, typ.lower(), path
-            )
-        else:
-            query = """INSERT INTO IdIndex (Pkey, Type, Path)
-            VALUES ('{}', '{}', '{}')""".format(
-                pkey, typ.lower(), path
-            )
+        # try:
+        #     existing_pkey, existing_typ = self._getIdentity(cursor, path)
+        # except Exception as e:
+        #     log.debug("identity get failed: {}".format(e))
+
+        # query = ""
+        # if existing_pkey is not None and existing_typ is not None:
+        #     query = """UPDATE IdIndex SET Pkey='{}', Type='{}'
+        #     WHERE Path='{}'""".format(
+        #         pkey, typ.lower(), path
+        #     )
+        # else:
+        query = """INSERT INTO IdIndex (Pkey, Type, Path)
+        VALUES ('{}', '{}', '{}')""".format(
+            pkey, typ.lower(), path
+        )
 
         self._do_query(cursor, query)
 
     def _removeIdentity(self, cursor, path):
         query = """DELETE FROM IdIndex
         WHERE Path = '{}'""".format(
             path
@@ -345,46 +324,46 @@
             data = utils.decode_string(data)
             return self._parseObjectRow(data, typ)
         else:
             raise Exception(constants.ErrNoSuchObject)
 
     def _setObject(self, cursor, pkey, typ, obj):
         query = ""
-        existing_obj = None
+        # existing_obj = None
 
-        try:
-            existing_obj = self._getObject(cursor, pkey, typ)
-        except Exception as e:
-            log.debug("object get failed: {}".format(e))
+        # try:
+        #     existing_obj = self._getObject(cursor, pkey, typ)
+        # except Exception as e:
+        #     log.debug("object get failed: {}".format(e))
 
         data = obj.ToJson()
         # encode the data so it doesn't contain any SQL unfriendly characters
         data = utils.encode_string(data)
 
-        if existing_obj is not None:
-            query = """UPDATE Objects SET Object='{}'
-            WHERE Pkey = '{}' AND Type = '{}'""".format(
-                data, pkey, typ.lower()
-            )
-        else:
-            query = """INSERT INTO Objects (Object, Pkey, Type)
-            VALUES ('{}', '{}', '{}')""".format(
-                data, pkey, typ.lower()
-            )
+        # if existing_obj is not None:
+        #     query = """UPDATE Objects SET Object='{}'
+        #     WHERE Pkey = '{}' AND Type = '{}'""".format(
+        #         data, pkey, typ.lower()
+        #     )
+        # else:
+        query = """INSERT INTO Objects (Object, Pkey, Type)
+        VALUES ('{}', '{}', '{}')""".format(
+            data, pkey, typ.lower()
+        )
 
         self._do_query(cursor, query)
 
     def _removeObject(self, cursor, pkey, typ):
         query = """DELETE FROM Objects
         WHERE Pkey = '{}' AND Type = '{}'""".format(
             pkey, typ.lower()
         )
 
         self._do_query(cursor, query)
-    
+
     def _getObjectKeys(self, cursor, typ, clause):
         query = """SELECT Pkey FROM Objects
         WHERE Type = '{}' {}""".format(
             typ.lower(),
             clause,
         )
 
@@ -394,129 +373,130 @@
         for row in rows:
             res.append(row[0])
         return res
 
     def _removeIdentities(self, cursor, typ, keys):
         batch_size = 100
         for i in range(0, len(keys), batch_size):
-            batch = keys[i:i+batch_size]
-            clause = "Pkey IN ({})".format(
-                ",".join(["'{}'".format(k) for k in batch])
-            )
+            batch = keys[i : i + batch_size]
+            clause = "Pkey IN ({})".format(",".join(["'{}'".format(k) for k in batch]))
 
             query = """DELETE FROM IdIndex
                 WHERE Type = '{}' AND {}""".format(
-                    typ.lower(),
-                    clause,
-                )
+                typ.lower(),
+                clause,
+            )
 
             self._do_query(cursor, query)
 
     def _removeObjects(self, cursor, typ, clause):
         query = """DELETE FROM Objects
         WHERE Type = '{}' {}""".format(
             typ.lower(),
             clause,
         )
 
         self._do_query(cursor, query)
 
     def _parseObjectRow(self, data, typ):
-        return utils.unmarshal_object(data, self.Schema, typ)
+        return utils.unmarshal_object(data, self._schema, typ)
 
     def _parseObjectRows(self, rows, typ):
         res = []
         for row in rows:
             data = utils.decode_string(row[0])
             res.append(self._parseObjectRow(data, typ))
         return res
 
     def _do_query(self, cursor, query):
         log.debug("running query: {}".format(query))
 
+        statements = sqlparse.parse(query)
+        if len(statements) > 1:
+            raise Exception(constants.ErrInvalidRequest)
+
         cursor.execute(query)
 
     def _buildFilterClause(self, copt, identity):
         if copt.filter is None:
             return ""
 
-        sample = self.Schema.ObjectForKind(identity.Type())
-        if sample is None:
-            raise Exception(constants.ErrNoSuchObject)
+        sample = self._schema.ObjectForKind(identity.Type())
+        # if sample is None:
+        #     raise Exception(constants.ErrInvalidPath)
 
         return """
             AND ({})
             """.format(
             self._convertFilter(copt.filter, sample)
         )
 
-    def _convertFilter(self, filterSetting, sample):
-        if isinstance(filterSetting, options._ListDeleteOption):
+    def _convertFilter(self, filterOption, sample):
+        if isinstance(filterOption, options._ListDeleteOption):
             copt = options.CommonOptionHolderFactory()
-            filterSetting.ApplyFunction()(copt)
-            filterSetting = copt.filter
+            filterOption.ApplyFunction()(copt)
+            filterOption = copt.filter
 
-        if isinstance(filterSetting, options.AndSetting):
+        if isinstance(filterOption, options.AndOption):
             return "( {} )".format(
                 " AND ".join(
-                    [self._convertFilter(f, sample) for f in filterSetting.filters]
+                    [self._convertFilter(f, sample) for f in filterOption.filters]
                 )
             )
 
-        if isinstance(filterSetting, options.OrSetting):
+        if isinstance(filterOption, options.OrOption):
             return "( {} )".format(
                 " OR ".join(
-                    [self._convertFilter(f, sample) for f in filterSetting.filters]
+                    [self._convertFilter(f, sample) for f in filterOption.filters]
                 )
             )
 
-        if isinstance(filterSetting, options.NotSetting):
+        if isinstance(filterOption, options.NotOption):
             return "( NOT {} )".format(
-                self._convertFilter(filterSetting.filter, sample)
+                self._convertFilter(filterOption.filter, sample)
             )
 
-        if utils.object_path(sample, filterSetting.key) is None:
+        if utils.object_path(sample, filterOption.key) is None:
             raise Exception(constants.ErrInvalidFilter)
 
-        if isinstance(filterSetting, options.InSetting):
-
-            def convert_value(v):
-                # return "'{}'".format(v)
-                if isinstance(v, str):
-                    return "'{}'".format(v)
-                elif isinstance(v, bool):
-                    return str(v).lower()
-                else:
-                    return str(v)
-
-            values = ", ".join([convert_value(v) for v in filterSetting.values])
+        def convert_value(v):
+            # return "'{}'".format(v)
+            if isinstance(v, str):
+                return "'{}'".format(utils.encode_string(v))
+            elif isinstance(v, bool):
+                return str(v).lower()
+            else:
+                return str(v)
+        
+        if isinstance(filterOption, options.InOption):
+            values = ", ".join([convert_value(v) for v in filterOption.values])
 
             return " json_extract(Object, '$.{}') IN ({})".format(
-                filterSetting.key, values
+                filterOption.key, values
             )
 
-        if isinstance(filterSetting, options.EqSetting):
+        if isinstance(filterOption, options.EqOption):
             return " json_extract(Object, '$.{}') = {} ".format(
-                filterSetting.key, filterSetting.value
+                filterOption.key, convert_value(filterOption.value)
             )
 
-        if isinstance(filterSetting, options.LtSetting):
+        if isinstance(filterOption, options.LtOption):
             return " json_extract(Object, '$.{}') < {} ".format(
-                filterSetting.key, filterSetting.value
+                filterOption.key, convert_value(filterOption.value)
             )
 
-        if isinstance(filterSetting, options.GtSetting):
+        if isinstance(filterOption, options.GtOption):
             return " json_extract(Object, '$.{}') > {} ".format(
-                filterSetting.key, filterSetting.value
+                filterOption.key, convert_value(filterOption.value)
             )
 
-        if isinstance(filterSetting, options.LteSetting):
+        if isinstance(filterOption, options.LteOption):
             return " json_extract(Object, '$.{}') <= {} ".format(
-                filterSetting.key, filterSetting.value
+                filterOption.key, convert_value(filterOption.value)
             )
 
-        if isinstance(filterSetting, options.GteSetting):
+        if isinstance(filterOption, options.GteOption):
             return " json_extract(Object, '$.{}') >= {} ".format(
-                filterSetting.key, filterSetting.value
+                filterOption.key, convert_value(filterOption.value)
             )
 
         raise Exception(constants.ErrInvalidFilter)
```

### Comparing `pystorz-0.2.1/pystorz/store/meta.py` & `pystorz-0.3.1/pystorz/store/meta.py`

 * *Files identical despite different names*

### Comparing `pystorz-0.2.1/pystorz/store/store.py` & `pystorz-0.3.1/pystorz/store/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import uuid
 import json
-from typing import List
 
 
 class Object:
 
     def __init__(self):
         raise Exception("Object is an interface")
 
-    # def MetaHolder(self):
-    #     pass
+    def Metadata(self):
+        pass
 
     def Clone(self):
         pass
 
     def ToJson(self) -> str:
         pass
 
@@ -26,24 +25,23 @@
     def ToDict(self) -> dict:
         pass
 
     def PrimaryKey(self) -> str:
         pass
 
 
-class ExternalHolder:
+class ExternalHolder(Object):
     def ExternalInternalSet(self, obj: object):
         pass
 
     def ExternalInternal(self) -> object:
         pass
 
 
-class ObjectList(List[Object]):
-
+class ObjectList(list[Object]):
     pass
 
 
 class ObjectIdentity:
     def __init__(self, id: str):
         self.id_ = id
 
@@ -113,15 +111,15 @@
         pass
 
 
 class SchemaHolder:
     def ObjectForKind(self, kind: str) -> Object:
         pass
 
-    def Types(self) -> List[str]:
+    def Types(self) -> list[str]:
         pass
 
 
 class Factory:
     def __call__(self, schema: SchemaHolder) -> Store:
         pass
```

### Comparing `pystorz-0.2.1/pystorz/store/utils.py` & `pystorz-0.3.1/pystorz/store/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import json
 import time
 import logging
 import pathlib
+import base64
+
+from urllib.parse import quote, unquote
 
 from jsonpath import JSONPath
 from datetime import datetime
 
 log = logging.getLogger(__name__)
 
 # import gabs
@@ -26,44 +29,44 @@
     ret = schema.ObjectForKind(obj.Metadata().Kind())
     jsn = obj.ToJson()
     ret.FromJson(jsn)
     return ret
 
 
 def unmarshal_object(
-    body: bytes, schema: store.SchemaHolder, kind: str
+    body: str, schema: store.SchemaHolder, kind: str
 ) -> store.Object:
     resource = schema.ObjectForKind(kind)
     resource.FromJson(body)
     return resource
 
 
-# def object_kind(response: bytes) -> str:
-#     obj = _MetaHolder()
-#     err = json.loads(response, object_hook=lambda d: obj.__dict__.update(d))
-#     if err:
-#         return ""
-#     if obj.Metadata is None:
-#         return ""
-#     return obj.Metadata['kind']
+def object_kind(data) -> str:
+    if "metadata" not in data:
+        return None
+    
+    if "kind" not in data["metadata"]:
+        return None
+    
+    return data["metadata"]["kind"]
 
 
 def pps(string: str) -> str:
     return pp(json.loads(string))
 
 
 def pp(obj) -> str:
     return json.dumps(obj, indent=4)
 
 
 def timestamp() -> str:
     return time.strftime("%Y-%m-%dT%H:%M:%S.%fZ", time.gmtime())
 
 
-def serialize(mo: store.Object) -> bytes:
+def serialize(mo: store.Object) -> str:
     if mo is None:
         raise constants.ErrObjectNil
     return json.dumps(mo, default=lambda x: x.to_dict())
 
 
 def object_path(obj: store.Object, path: str) -> str:
     # print("object_path: {} {}".format(obj, path))
@@ -106,7 +109,21 @@
     # return str(encoded_message, 'utf-8')  # Convert the bytes to a string
 
 
 def decode_string(soup):
     return soup.replace("$%#", "'")
     # encoded_message = bytes(soup, 'utf-8')  # Convert the soup to bytes
     # return base64.b64decode(encoded_message).decode('utf-8')  # Decode the base64 bytes and convert to string
+
+
+# encoding = 'ascii'
+encoding = 'utf-8'
+def base64_encode_string(string):
+    # encoded_message = base64.b64encode(string.encode('utf-8'))  # Encode the message as base64 bytes
+    # return str(encoded_message, 'utf-8')  # Convert the bytes to a string
+    encoded_message = base64.b64encode(string.encode(encoding))  # Encode the message as base64 bytes
+    return quote(str(encoded_message, encoding))  # Convert the bytes to a string
+
+
+def base64_decode_string(soup):
+    encoded_message = bytes(unquote(soup), encoding)  # Convert the soup to bytes
+    return base64.b64decode(encoded_message).decode(encoding)  # Decode the base64 bytes and convert to string
```

### Comparing `pystorz-0.2.1/pystorz.egg-info/PKG-INFO` & `pystorz-0.3.1/pystorz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pystorz
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python package for the Storz object store framework.
 Home-page: https://github.com/wazofski/pystorz
 Author: wazofski
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
-<img src="logo.png" width="300" alt="storz" />
+<img src="https://raw.githubusercontent.com/wazofski/pystorz/master/logo.png" width="300" alt="storz" />
 </p>
 
 **pystorz** is an *object store framework* built in python. It consists of a set of modules implementing the [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface and features a simple [object modeling language](https://github.com/wazofski/pystorz/tree/master/pystorz/mgen) used to generate golang object class meta for interacting with `Store` APIs.
 
 **pystorz** modules provide functionality to store, modify and retrieve modeled objects from various sources (TBD). Such modules can be composed together to chain `Store` functionality into more complex logical modules. Combining modules allows handling object changes and manipulating data in complex ways *within or across* services, making multi-level server complexity achievable with ease. The Store modules are fully compatible with each other and can be composed in any combination since they all implement or expose the same [Store](https://github.com/wazofski/pystorz/tree/master/pystorz/store) interface.
 
 Original storz was written in go. You can check it out here:
@@ -55,15 +56,15 @@
 
     # you can then import the generated model
     from generated import model
 
     # initialize a store
     stor = SqliteStore(
         Schema(),
-        SqliteConnection("path/to/your/sqlite3.db"))
+        SqliteConnector("path/to/your/sqlite3.db"))
 
     world = model.WorldFactory()
     world.External().SetName("hello")
 
     created_world = stor.Create(world)
     world.External().SetDescription("hello world")
     updated_world = stor.Update(world.Metadata().Identity(), world)
```

### Comparing `pystorz-0.2.1/pystorz.egg-info/SOURCES.txt` & `pystorz-0.3.1/pystorz.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,34 @@
 pystorz.egg-info/PKG-INFO
 pystorz.egg-info/SOURCES.txt
 pystorz.egg-info/dependency_links.txt
 pystorz.egg-info/requires.txt
 pystorz.egg-info/top_level.txt
 pystorz/internal/__init__.py
 pystorz/internal/constants.py
+pystorz/meta/store.py
 pystorz/mgen/__init__.py
 pystorz/mgen/builder.py
 pystorz/mgen/loader.py
 pystorz/mgen/test.py
 pystorz/mgen/utils.py
 pystorz/mgen/templates/__init__.py
 pystorz/mgen/templates/imports.py
 pystorz/mgen/templates/interface.py
 pystorz/mgen/templates/meta.py
 pystorz/mgen/templates/schema.py
 pystorz/mgen/templates/specinternal.py
 pystorz/mgen/templates/structure.py
 pystorz/mgen/templates/unmarshall.py
+pystorz/rest/client.py
+pystorz/rest/headers.py
+pystorz/rest/internals.py
+pystorz/rest/server.py
 pystorz/sql/__init__.py
+pystorz/sql/mysql.py
+pystorz/sql/sqlite.py
 pystorz/sql/store.py
 pystorz/store/__init__.py
 pystorz/store/meta.py
 pystorz/store/options.py
 pystorz/store/store.py
 pystorz/store/utils.py
```

