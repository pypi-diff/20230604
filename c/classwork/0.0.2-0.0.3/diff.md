# Comparing `tmp/classwork-0.0.2.tar.gz` & `tmp/classwork-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classwork-0.0.2.tar", last modified: Sat Jun  3 18:53:04 2023, max compression
+gzip compressed data, was "classwork-0.0.3.tar", max compression
```

## Comparing `classwork-0.0.2.tar` & `classwork-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 18:53:04.188561 classwork-0.0.2/
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     1072 2023-06-03 17:09:04.000000 classwork-0.0.2/LICENSE.md
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     4766 2023-06-03 18:53:04.188561 classwork-0.0.2/PKG-INFO
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     4193 2023-06-03 16:54:31.000000 classwork-0.0.2/README.md
-drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 18:53:04.184561 classwork-0.0.2/classwork/
--rw-rw-r--   0 mugz      (1000) mugz      (1000)      161 2023-06-03 15:43:24.000000 classwork-0.0.2/classwork/__init__.py
--rw-rw-r--   0 mugz      (1000) mugz      (1000)    11866 2023-06-03 16:13:53.000000 classwork-0.0.2/classwork/main.py
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     3086 2023-06-03 15:08:39.000000 classwork-0.0.2/classwork/utils.py
-drwxrwxr-x   0 mugz      (1000) mugz      (1000)        0 2023-06-03 18:53:04.188561 classwork-0.0.2/classwork.egg-info/
--rw-rw-r--   0 mugz      (1000) mugz      (1000)     4766 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/PKG-INFO
--rw-rw-r--   0 mugz      (1000) mugz      (1000)      258 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/SOURCES.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)        1 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/dependency_links.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)       75 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/requires.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)       10 2023-06-03 18:53:04.000000 classwork-0.0.2/classwork.egg-info/top_level.txt
--rw-rw-r--   0 mugz      (1000) mugz      (1000)      759 2023-06-03 18:08:27.000000 classwork-0.0.2/pyproject.toml
--rw-rw-r--   0 mugz      (1000) mugz      (1000)       38 2023-06-03 18:53:04.188561 classwork-0.0.2/setup.cfg
+-rw-r--r--   0        0        0     1072 2023-06-03 17:09:04.784909 classwork-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     4193 2023-06-03 16:54:31.476439 classwork-0.0.3/README.md
+-rw-r--r--   0        0        0      161 2023-06-03 15:43:24.017838 classwork-0.0.3/classwork/__init__.py
+-rw-r--r--   0        0        0    11060 2023-06-03 22:43:17.833105 classwork-0.0.3/classwork/main.py
+-rw-r--r--   0        0        0     3086 2023-06-03 15:08:39.227871 classwork-0.0.3/classwork/utils.py
+-rw-r--r--   0        0        0      451 2023-06-03 22:35:53.120516 classwork-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 classwork-0.0.3/PKG-INFO
```

### Comparing `classwork-0.0.2/LICENSE.md` & `classwork-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.2/PKG-INFO` & `classwork-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: classwork
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python module to help distribute you tasks across multiple brokers as microservices
-Author-email: Anthony Mugendi <ngurumugz@gmail.com>
-Project-URL: Bug Tracker, https://github.com/mugendi/classwork/issues
-Project-URL: Homepage, https://github.com/mugendi/classwork
-Classifier: Programming Language :: Python :: 3
+License: MIT
+Author: Anthony Mugendi
+Author-email: ngurumugz@gmail.com
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: hashids (==1.3.1)
+Requires-Dist: nats-py (==2.2.0)
+Requires-Dist: numpy (==1.23.5)
+Requires-Dist: typjson (==0.0.32)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
 
 <!--
  Copyright (c) 2023 Anthony Mugendi
  
  This software is released under the MIT License.
  https://opensource.org/licenses/MIT
 -->
```

### Comparing `classwork-0.0.2/README.md` & `classwork-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `classwork-0.0.2/classwork/main.py` & `classwork-0.0.3/classwork/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import uuid
 import nats
 
 from time import perf_counter as pc
 from typ import json as safe_json
 from nats.aio.client import Client as NATS
 from nats.aio.errors import ErrNoServers, ErrTimeout
-from yachalk import chalk
 
-from .utils import hash_str, precision_format_time, importing_script, sanitize_name, get_class_props, RaisingThread, trace_caller
+from .utils import hash_str, precision_format_time, importing_script, sanitize_name, get_class_props, RaisingThread
 
 app_name = "classwork"
 
 
 class ClassWork:
     def __init__(self, nats_url) -> None:
         self.nats_url = nats_url
@@ -30,39 +29,14 @@
 
     async def __setup(self):
         mac_id = hex(uuid.getnode())
         exec_file = importing_script()
         hashid = hash_str(f"{exec_file}")
         self.id = f"{app_name}_{mac_id}_{str(hashid)}"
 
-    def __log(self, level="info", *args):
-        id = self.id.replace(f"{app_name}_", "")
-
-        level = level.upper()
-
-        prefix = f"[{level}][{id}]"
-        clr = chalk.gray
-
-        if level in ["SUCCESS"]:
-            clr = chalk.green
-            prefix = chalk.bold.green("✔ " + prefix)
-        if level in ["ERROR"]:
-            clr = chalk.red
-            prefix = chalk.bold.red("✘ " + prefix)
-        if level in ["WARNING"]:
-            clr = chalk.yellow
-            prefix = chalk.bold.yellow("⚠ " + prefix)
-        elif level in ["INFO"]:
-            clr = chalk.blue
-            prefix = chalk.bold.blue(prefix)
-
-        args = list(map(lambda arg: clr(str(arg)), args))
-
-        print("", prefix, *args)
-
     async def __connect(self):       
         
         # trace_caller()
     
         # Setup pool of servers from a NATS cluster.
         options = {
             "servers": self.nats_url
@@ -106,16 +80,15 @@
             nc = await nats.connect(**options)
         except ErrNoServers as e:
             # Could not connect to any server in the cluster.
             # print(e)
             return
 
         if nc.is_connected:
-            # print(nc.connected_url)
-            self.__log("info", f"Successfully connected : {nc.connected_url.netloc}")
+            print(f" >> Connection to NATS server [{nc.connected_url.netloc}] established.")
             self.nc = nc
             self.js = nc.jetstream()
 
             return self.nc, self.js
         
 
     async def __add_stream(self, stream_name, subjects):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `classwork-0.0.2/classwork/utils.py` & `classwork-0.0.3/classwork/utils.py`

 * *Files identical despite different names*

