# Comparing `tmp/godto-0.0.2.tar.gz` & `tmp/godto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godto-0.0.2.tar", last modified: Sun Jun  4 21:20:28 2023, max compression
+gzip compressed data, was "godto-0.0.3.tar", last modified: Sun Jun  4 21:36:43 2023, max compression
```

## Comparing `godto-0.0.2.tar` & `godto-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.327596 godto-0.0.2/
--rw-rw-r--   0 louis     (1000) louis     (1000)      145 2023-06-03 11:01:33.000000 godto-0.0.2/.gitignore
--rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-06-02 22:46:58.000000 godto-0.0.2/LICENSE
--rw-rw-r--   0 louis     (1000) louis     (1000)     1950 2023-06-04 21:20:28.327596 godto-0.0.2/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      843 2023-06-04 20:58:51.000000 godto-0.0.2/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)      100 2023-06-04 21:17:59.000000 godto-0.0.2/direct_dependency_requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       24 2023-06-04 21:15:51.000000 godto-0.0.2/requirements.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-06-04 21:20:28.327596 godto-0.0.2/setup.cfg
--rw-rw-r--   0 louis     (1000) louis     (1000)     3273 2023-06-04 21:16:42.000000 godto-0.0.2/setup.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.319596 godto-0.0.2/src/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.323596 godto-0.0.2/src/godto/
--rw-rw-r--   0 louis     (1000) louis     (1000)      457 2023-06-04 20:47:16.000000 godto-0.0.2/src/godto/__init__.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.319596 godto-0.0.2/src/godto/data/
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.323596 godto-0.0.2/src/godto/data/openapi/
--rw-rw-r--   0 louis     (1000) louis     (1000)       94 2023-06-02 23:16:49.000000 godto-0.0.2/src/godto/data/openapi/README.md
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.323596 godto-0.0.2/src/godto/data/openapi/v2.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      248 2023-06-02 23:13:14.000000 godto-0.0.2/src/godto/data/openapi/v2.0/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    40247 2023-06-02 23:13:14.000000 godto-0.0.2/src/godto/data/openapi/v2.0/schema.json
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.327596 godto-0.0.2/src/godto/data/openapi/v3.0/
--rw-rw-r--   0 louis     (1000) louis     (1000)      890 2023-06-02 23:13:14.000000 godto-0.0.2/src/godto/data/openapi/v3.0/README.md
--rw-rw-r--   0 louis     (1000) louis     (1000)    35817 2023-06-02 23:13:14.000000 godto-0.0.2/src/godto/data/openapi/v3.0/schema.json
--rw-rw-r--   0 louis     (1000) louis     (1000)    22670 2023-06-02 23:13:14.000000 godto-0.0.2/src/godto/data/openapi/v3.0/schema.yaml
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.327596 godto-0.0.2/src/godto/generated/
--rw-rw-r--   0 louis     (1000) louis     (1000)    14214 2023-06-04 20:46:08.000000 godto-0.0.2/src/godto/generated/openapi_v3.py
-drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:20:28.323596 godto-0.0.2/src/godto.egg-info/
--rw-rw-r--   0 louis     (1000) louis     (1000)     1950 2023-06-04 21:20:28.000000 godto-0.0.2/src/godto.egg-info/PKG-INFO
--rw-rw-r--   0 louis     (1000) louis     (1000)      570 2023-06-04 21:20:28.000000 godto-0.0.2/src/godto.egg-info/SOURCES.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)      100 2023-06-04 21:20:28.000000 godto-0.0.2/src/godto.egg-info/dependency_links.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-04 21:20:28.000000 godto-0.0.2/src/godto.egg-info/not-zip-safe
--rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-06-04 21:20:28.000000 godto-0.0.2/src/godto.egg-info/requires.txt
--rw-rw-r--   0 louis     (1000) louis     (1000)        6 2023-06-04 21:20:28.000000 godto-0.0.2/src/godto.egg-info/top_level.txt
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.496627 godto-0.0.3/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      145 2023-06-03 11:01:33.000000 godto-0.0.3/.gitignore
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1069 2023-06-02 22:46:58.000000 godto-0.0.3/LICENSE
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1950 2023-06-04 21:36:43.496627 godto-0.0.3/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      843 2023-06-04 21:34:04.000000 godto-0.0.3/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)      100 2023-06-04 21:17:59.000000 godto-0.0.3/direct_dependency_requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       24 2023-06-04 21:15:51.000000 godto-0.0.3/requirements.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)       38 2023-06-04 21:36:43.496627 godto-0.0.3/setup.cfg
+-rw-rw-r--   0 louis     (1000) louis     (1000)     3273 2023-06-04 21:16:42.000000 godto-0.0.3/setup.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.484627 godto-0.0.3/src/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      442 2023-06-04 21:34:38.000000 godto-0.0.3/src/godto/__init__.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.484627 godto-0.0.3/src/godto/data/
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto/data/openapi/
+-rw-rw-r--   0 louis     (1000) louis     (1000)       94 2023-06-02 23:16:49.000000 godto-0.0.3/src/godto/data/openapi/README.md
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto/data/openapi/v2.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      248 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v2.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    40247 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v2.0/schema.json
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.492627 godto-0.0.3/src/godto/data/openapi/v3.0/
+-rw-rw-r--   0 louis     (1000) louis     (1000)      890 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v3.0/README.md
+-rw-rw-r--   0 louis     (1000) louis     (1000)    35817 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v3.0/schema.json
+-rw-rw-r--   0 louis     (1000) louis     (1000)    22670 2023-06-02 23:13:14.000000 godto-0.0.3/src/godto/data/openapi/v3.0/schema.yaml
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.492627 godto-0.0.3/src/godto/openapi/
+-rw-rw-r--   0 louis     (1000) louis     (1000)    14214 2023-06-04 20:46:08.000000 godto-0.0.3/src/godto/openapi/v3.py
+drwxrwxr-x   0 louis     (1000) louis     (1000)        0 2023-06-04 21:36:43.488627 godto-0.0.3/src/godto.egg-info/
+-rw-rw-r--   0 louis     (1000) louis     (1000)     1950 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/PKG-INFO
+-rw-rw-r--   0 louis     (1000) louis     (1000)      560 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/SOURCES.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)      100 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/dependency_links.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        1 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/not-zip-safe
+-rw-rw-r--   0 louis     (1000) louis     (1000)      113 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/requires.txt
+-rw-rw-r--   0 louis     (1000) louis     (1000)        6 2023-06-04 21:36:43.000000 godto-0.0.3/src/godto.egg-info/top_level.txt
```

### Comparing `godto-0.0.2/LICENSE` & `godto-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/PKG-INFO` & `godto-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godto
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Transfer Object (DTO) codegen from JSON schemas following the OpenAPI spec
 Home-page: https://github.com/lmmx/godto
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
@@ -34,15 +34,15 @@
 
 ## Usage
 
 To work with an OpenAPI schema, load it with the `Model` class,
 which is a [Dataclass Wizard](https://github.com/rnag/dataclass-wizard/) deserialiser.
 
 ```py
-from godto.openapi_v3 import Model
+from godto.openapi.v3 import Model
 
 model = Model.from_json(schema_json)
 ```
 
 For example the Transport for London `StopPoint` API schema
 is [shipped as package data][StopPoint_schema] in `tubeulator`.
```

### Comparing `godto-0.0.2/README.md` & `godto-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Usage
 
 To work with an OpenAPI schema, load it with the `Model` class,
 which is a [Dataclass Wizard](https://github.com/rnag/dataclass-wizard/) deserialiser.
 
 ```py
-from godto.openapi_v3 import Model
+from godto.openapi.v3 import Model
 
 model = Model.from_json(schema_json)
 ```
 
 For example the Transport for London `StopPoint` API schema
 is [shipped as package data][StopPoint_schema] in `tubeulator`.
```

### Comparing `godto-0.0.2/setup.py` & `godto-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/src/godto/data/openapi/v2.0/schema.json` & `godto-0.0.3/src/godto/data/openapi/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/src/godto/data/openapi/v3.0/README.md` & `godto-0.0.3/src/godto/data/openapi/v3.0/README.md`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/src/godto/data/openapi/v3.0/schema.json` & `godto-0.0.3/src/godto/data/openapi/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/src/godto/data/openapi/v3.0/schema.yaml` & `godto-0.0.3/src/godto/data/openapi/v3.0/schema.yaml`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/src/godto/generated/openapi_v3.py` & `godto-0.0.3/src/godto/openapi/v3.py`

 * *Files identical despite different names*

### Comparing `godto-0.0.2/src/godto.egg-info/PKG-INFO` & `godto-0.0.3/src/godto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godto
-Version: 0.0.2
+Version: 0.0.3
 Summary: Data Transfer Object (DTO) codegen from JSON schemas following the OpenAPI spec
 Home-page: https://github.com/lmmx/godto
 Author: Louis Maddox
 Author-email: louismmx@gmail.com
 Maintainer: Louis Maddox
 Maintainer-email: louismmx@gmail.com
 License: MIT
@@ -34,15 +34,15 @@
 
 ## Usage
 
 To work with an OpenAPI schema, load it with the `Model` class,
 which is a [Dataclass Wizard](https://github.com/rnag/dataclass-wizard/) deserialiser.
 
 ```py
-from godto.openapi_v3 import Model
+from godto.openapi.v3 import Model
 
 model = Model.from_json(schema_json)
 ```
 
 For example the Transport for London `StopPoint` API schema
 is [shipped as package data][StopPoint_schema] in `tubeulator`.
```

### Comparing `godto-0.0.2/src/godto.egg-info/SOURCES.txt` & `godto-0.0.3/src/godto.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 src/godto.egg-info/top_level.txt
 src/godto/data/openapi/README.md
 src/godto/data/openapi/v2.0/README.md
 src/godto/data/openapi/v2.0/schema.json
 src/godto/data/openapi/v3.0/README.md
 src/godto/data/openapi/v3.0/schema.json
 src/godto/data/openapi/v3.0/schema.yaml
-src/godto/generated/openapi_v3.py
+src/godto/openapi/v3.py
```

