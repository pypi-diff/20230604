# Comparing `tmp/only_train_once-2.0.8.tar.gz` & `tmp/only_train_once-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "only_train_once-2.0.8.tar", last modified: Sat Apr  1 05:15:35 2023, max compression
+gzip compressed data, was "only_train_once-2.0.9.tar", last modified: Mon Apr  3 03:56:08 2023, max compression
```

## Comparing `only_train_once-2.0.8.tar` & `only_train_once-2.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.067956 only_train_once-2.0.8/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1068 2023-03-28 15:38:06.000000 only_train_once-2.0.8/LICENSE
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      665 2023-04-01 05:15:35.067956 only_train_once-2.0.8/PKG-INFO
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     6225 2023-04-01 05:12:28.000000 only_train_once-2.0.8/README.md
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.063956 only_train_once-2.0.8/only_train_once/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3965 2023-03-28 19:20:18.000000 only_train_once-2.0.8/only_train_once/__init__.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.063956 only_train_once-2.0.8/only_train_once/assets/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       47 2023-03-09 04:56:08.000000 only_train_once-2.0.8/only_train_once/assets/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      136 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/assets/group_types.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      288 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/assets/theme.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.063956 only_train_once-2.0.8/only_train_once/compression/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       26 2023-03-09 04:55:12.000000 only_train_once-2.0.8/only_train_once/compression/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3322 2023-03-11 21:17:31.000000 only_train_once-2.0.8/only_train_once/compression/compression.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.063956 only_train_once-2.0.8/only_train_once/flops/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       20 2023-03-09 04:56:39.000000 only_train_once-2.0.8/only_train_once/flops/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     2438 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/flops/flops.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.063956 only_train_once-2.0.8/only_train_once/graph/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       75 2023-03-09 01:52:14.000000 only_train_once-2.0.8/only_train_once/graph/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     4237 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/graph/connected_component.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)    28362 2023-04-01 05:13:41.000000 only_train_once-2.0.8/only_train_once/graph/graph.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3337 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/graph/node.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.067956 only_train_once-2.0.8/only_train_once/operation/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       53 2023-03-09 04:58:03.000000 only_train_once-2.0.8/only_train_once/operation/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1667 2023-03-09 05:16:20.000000 only_train_once-2.0.8/only_train_once/operation/operator.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3269 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/operation/operators_dict.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.067956 only_train_once-2.0.8/only_train_once/optimizer/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       24 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/optimizer/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)    27476 2023-04-01 05:12:28.000000 only_train_once-2.0.8/only_train_once/optimizer/dhspg.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      743 2023-03-28 19:24:08.000000 only_train_once-2.0.8/only_train_once/optimizer/hyperparameter.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.067956 only_train_once-2.0.8/only_train_once/transform/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       35 2023-03-09 05:11:59.000000 only_train_once-2.0.8/only_train_once/transform/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     4988 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/transform/ge.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      287 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/transform/onnx_graph_transform.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3081 2023-03-09 05:24:18.000000 only_train_once-2.0.8/only_train_once/transform/transforms.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.067956 only_train_once-2.0.8/only_train_once/zig/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       18 2023-03-09 04:59:38.000000 only_train_once-2.0.8/only_train_once/zig/__init__.py
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     4763 2023-03-09 00:37:43.000000 only_train_once-2.0.8/only_train_once/zig/zig.py
-drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-01 05:15:35.063956 only_train_once-2.0.8/only_train_once.egg-info/
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      665 2023-04-01 05:15:34.000000 only_train_once-2.0.8/only_train_once.egg-info/PKG-INFO
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1097 2023-04-01 05:15:35.000000 only_train_once-2.0.8/only_train_once.egg-info/SOURCES.txt
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)        1 2023-04-01 05:15:34.000000 only_train_once-2.0.8/only_train_once.egg-info/dependency_links.txt
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       53 2023-04-01 05:15:34.000000 only_train_once-2.0.8/only_train_once.egg-info/requires.txt
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       16 2023-04-01 05:15:34.000000 only_train_once-2.0.8/only_train_once.egg-info/top_level.txt
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       38 2023-04-01 05:15:35.067956 only_train_once-2.0.8/setup.cfg
--rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1101 2023-04-01 05:15:25.000000 only_train_once-2.0.8/setup.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.378003 only_train_once-2.0.9/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1068 2023-03-28 15:38:06.000000 only_train_once-2.0.9/LICENSE
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      665 2023-04-03 03:56:08.378003 only_train_once-2.0.9/PKG-INFO
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     6225 2023-04-01 05:12:28.000000 only_train_once-2.0.9/README.md
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.374003 only_train_once-2.0.9/only_train_once/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3965 2023-03-28 19:20:18.000000 only_train_once-2.0.9/only_train_once/__init__.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.374003 only_train_once-2.0.9/only_train_once/assets/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       47 2023-03-09 04:56:08.000000 only_train_once-2.0.9/only_train_once/assets/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      136 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/assets/group_types.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      288 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/assets/theme.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.374003 only_train_once-2.0.9/only_train_once/compression/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       26 2023-03-09 04:55:12.000000 only_train_once-2.0.9/only_train_once/compression/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3322 2023-03-11 21:17:31.000000 only_train_once-2.0.9/only_train_once/compression/compression.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.374003 only_train_once-2.0.9/only_train_once/flops/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       20 2023-03-09 04:56:39.000000 only_train_once-2.0.9/only_train_once/flops/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     2438 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/flops/flops.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.374003 only_train_once-2.0.9/only_train_once/graph/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       75 2023-03-09 01:52:14.000000 only_train_once-2.0.9/only_train_once/graph/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     4237 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/graph/connected_component.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)    28362 2023-04-01 05:20:45.000000 only_train_once-2.0.9/only_train_once/graph/graph.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3337 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/graph/node.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.378003 only_train_once-2.0.9/only_train_once/operation/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       53 2023-03-09 04:58:03.000000 only_train_once-2.0.9/only_train_once/operation/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1667 2023-03-09 05:16:20.000000 only_train_once-2.0.9/only_train_once/operation/operator.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3269 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/operation/operators_dict.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.378003 only_train_once-2.0.9/only_train_once/optimizer/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       24 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/optimizer/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)    27476 2023-04-01 05:12:28.000000 only_train_once-2.0.9/only_train_once/optimizer/dhspg.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      743 2023-03-28 19:24:08.000000 only_train_once-2.0.9/only_train_once/optimizer/hyperparameter.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.378003 only_train_once-2.0.9/only_train_once/transform/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       35 2023-03-09 05:11:59.000000 only_train_once-2.0.9/only_train_once/transform/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     4988 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/transform/ge.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      287 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/transform/onnx_graph_transform.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     3081 2023-03-09 05:24:18.000000 only_train_once-2.0.9/only_train_once/transform/transforms.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.378003 only_train_once-2.0.9/only_train_once/zig/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       18 2023-03-09 04:59:38.000000 only_train_once-2.0.9/only_train_once/zig/__init__.py
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     4763 2023-03-09 00:37:43.000000 only_train_once-2.0.9/only_train_once/zig/zig.py
+drwxrwxr-x   0 tianyi    (1005) tianyi    (1005)        0 2023-04-03 03:56:08.374003 only_train_once-2.0.9/only_train_once.egg-info/
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)      665 2023-04-03 03:56:08.000000 only_train_once-2.0.9/only_train_once.egg-info/PKG-INFO
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1097 2023-04-03 03:56:08.000000 only_train_once-2.0.9/only_train_once.egg-info/SOURCES.txt
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)        1 2023-04-03 03:56:08.000000 only_train_once-2.0.9/only_train_once.egg-info/dependency_links.txt
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       53 2023-04-03 03:56:08.000000 only_train_once-2.0.9/only_train_once.egg-info/requires.txt
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       16 2023-04-03 03:56:08.000000 only_train_once-2.0.9/only_train_once.egg-info/top_level.txt
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)       38 2023-04-03 03:56:08.378003 only_train_once-2.0.9/setup.cfg
+-rw-rw-r--   0 tianyi    (1005) tianyi    (1005)     1101 2023-04-03 03:55:27.000000 only_train_once-2.0.9/setup.py
```

### Comparing `only_train_once-2.0.8/LICENSE` & `only_train_once-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/PKG-INFO` & `only_train_once-2.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: only_train_once
-Version: 2.0.8
+Version: 2.0.9
 Summary: Only Train Once (OTO): Automatic One-Shot General DNN Training and Compression Framework
 Home-page: https://github.com/tianyic/only_train_once
 Author: Tianyi Chen
 Author-email: tiachen@microsoft.com
 License: MIT
 Keywords: automatic,one-shot,structure pruning,sparse optimization
 Platform: UNKNOWN
```

### Comparing `only_train_once-2.0.8/README.md` & `only_train_once-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/__init__.py` & `only_train_once-2.0.9/only_train_once/__init__.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/compression/compression.py` & `only_train_once-2.0.9/only_train_once/compression/compression.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/flops/flops.py` & `only_train_once-2.0.9/only_train_once/flops/flops.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/graph/connected_component.py` & `only_train_once-2.0.9/only_train_once/graph/connected_component.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/graph/graph.py` & `only_train_once-2.0.9/only_train_once/graph/graph.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/graph/node.py` & `only_train_once-2.0.9/only_train_once/graph/node.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/operation/operator.py` & `only_train_once-2.0.9/only_train_once/operation/operator.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/operation/operators_dict.py` & `only_train_once-2.0.9/only_train_once/operation/operators_dict.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/optimizer/dhspg.py` & `only_train_once-2.0.9/only_train_once/optimizer/dhspg.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/optimizer/hyperparameter.py` & `only_train_once-2.0.9/only_train_once/optimizer/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/transform/ge.py` & `only_train_once-2.0.9/only_train_once/transform/ge.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/transform/transforms.py` & `only_train_once-2.0.9/only_train_once/transform/transforms.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once/zig/zig.py` & `only_train_once-2.0.9/only_train_once/zig/zig.py`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/only_train_once.egg-info/PKG-INFO` & `only_train_once-2.0.9/only_train_once.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: only-train-once
-Version: 2.0.8
+Version: 2.0.9
 Summary: Only Train Once (OTO): Automatic One-Shot General DNN Training and Compression Framework
 Home-page: https://github.com/tianyic/only_train_once
 Author: Tianyi Chen
 Author-email: tiachen@microsoft.com
 License: MIT
 Keywords: automatic,one-shot,structure pruning,sparse optimization
 Platform: UNKNOWN
```

### Comparing `only_train_once-2.0.8/only_train_once.egg-info/SOURCES.txt` & `only_train_once-2.0.9/only_train_once.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `only_train_once-2.0.8/setup.py` & `only_train_once-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def parse_requirements(filename):
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 reqs = parse_requirements('requirements.txt')
 
-VERSION = '2.0.8'
+VERSION = '2.0.9'
 DESCRIPTION = 'Only Train Once (OTO): Automatic One-Shot General DNN Training and Compression Framework'
 LONG_DESCRIPTION = 'Only Train Once (OTO): Automatic One-Shot General DNN Training and Compression Framework'
 
 setup(
     name="only_train_once",
     version=VERSION,
     description=DESCRIPTION,
```

