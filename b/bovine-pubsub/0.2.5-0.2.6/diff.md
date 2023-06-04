# Comparing `tmp/bovine_pubsub-0.2.5.tar.gz` & `tmp/bovine_pubsub-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_pubsub-0.2.5.tar", max compression
+gzip compressed data, was "bovine_pubsub-0.2.6.tar", max compression
```

## Comparing `bovine_pubsub-0.2.5.tar` & `bovine_pubsub-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       68 2023-05-28 14:23:45.592439 bovine_pubsub-0.2.5/README.md
--rw-r--r--   0        0        0      279 2023-05-28 14:23:45.592439 bovine_pubsub-0.2.5/bovine_pubsub/__init__.py
--rw-r--r--   0        0        0      868 2023-05-28 14:23:45.592439 bovine_pubsub-0.2.5/bovine_pubsub/queue.py
--rw-r--r--   0        0        0     1091 2023-05-28 14:23:45.592439 bovine_pubsub-0.2.5/bovine_pubsub/redis.py
--rw-r--r--   0        0        0      258 2023-05-28 14:23:45.592439 bovine_pubsub-0.2.5/bovine_pubsub/test_app.py
--rw-r--r--   0        0        0      632 2023-05-28 14:23:45.592439 bovine_pubsub-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.5/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/README.md
+-rw-r--r--   0        0        0      279 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/__init__.py
+-rw-r--r--   0        0        0      868 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/queue.py
+-rw-r--r--   0        0        0     1091 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/redis.py
+-rw-r--r--   0        0        0      258 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/test_app.py
+-rw-r--r--   0        0        0      632 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.6/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.6/PKG-INFO
```

### Comparing `bovine_pubsub-0.2.5/bovine_pubsub/queue.py` & `bovine_pubsub-0.2.6/bovine_pubsub/queue.py`

 * *Files identical despite different names*

### Comparing `bovine_pubsub-0.2.5/bovine_pubsub/redis.py` & `bovine_pubsub-0.2.6/bovine_pubsub/redis.py`

 * *Files identical despite different names*

### Comparing `bovine_pubsub-0.2.5/pyproject.toml` & `bovine_pubsub-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-pubsub"
-version = "0.2.5"
+version = "0.2.6"
 description = "A Quart Redis thing to handle pubsub tasks in particular the event source"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://codeberg.org/bovine/bovine"
 packages = [{include = "bovine_pubsub"}]
```

### Comparing `bovine_pubsub-0.2.5/setup.py` & `bovine_pubsub-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['quart-redis>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bovine-pubsub',
-    'version': '0.2.5',
+    'version': '0.2.6',
     'description': 'A Quart Redis thing to handle pubsub tasks in particular the event source',
     'long_description': '# bovine_pubsub\n\nRequires redis. Usage see `examples/basic_app.py`.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine_pubsub-0.2.5/PKG-INFO` & `bovine_pubsub-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine-pubsub
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Quart Redis thing to handle pubsub tasks in particular the event source
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

