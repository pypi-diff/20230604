# Comparing `tmp/ipttrace-0.1.0.tar.gz` & `tmp/ipttrace-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipttrace-0.1.0.tar", max compression
+gzip compressed data, was "ipttrace-0.1.1.tar", max compression
```

## Comparing `ipttrace-0.1.0.tar` & `ipttrace-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2302 2023-06-04 05:56:31.434312 ipttrace-0.1.0/ipttrace/main.py
--rw-r--r--   0        0        0      560 2023-06-04 07:44:12.436789 ipttrace-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      863 2023-06-04 07:47:13.978096 ipttrace-0.1.0/setup.py
--rw-r--r--   0        0        0      571 2023-06-04 07:47:13.978323 ipttrace-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2302 2023-06-04 05:56:31.434312 ipttrace-0.1.1/ipttrace/main.py
+-rw-r--r--   0        0        0      615 2023-06-04 07:59:37.941898 ipttrace-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      900 2023-06-04 07:59:52.954564 ipttrace-0.1.1/setup.py
+-rw-r--r--   0        0        0      687 2023-06-04 07:59:52.954787 ipttrace-0.1.1/PKG-INFO
```

### Comparing `ipttrace-0.1.0/ipttrace/main.py` & `ipttrace-0.1.1/ipttrace/main.py`

 * *Files identical despite different names*

### Comparing `ipttrace-0.1.0/pyproject.toml` & `ipttrace-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "ipttrace"
-version = "0.1.0"
+version = "0.1.1"
 description = "trace iptables rules with ease"
 authors = ["sieginglion <sieginglion@gmail.com>"]
+repository = "https://github.com/sieginglion/ipttrace"
 
 [tool.poetry.dependencies]
 python = "^3.6.3"
 dataclasses = { version = "^0.8", python = "<3.7" }
 rich = "^12.6.0"
 typer = "^0.9.0"
```

### Comparing `ipttrace-0.1.0/setup.py` & `ipttrace-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 {':python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 entry_points = \
 {'console_scripts': ['ipttrace = ipttrace.main:app']}
 
 setup_kwargs = {
     'name': 'ipttrace',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'trace iptables rules with ease',
     'long_description': None,
     'author': 'sieginglion',
     'author_email': 'sieginglion@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
-    'url': None,
+    'url': 'https://github.com/sieginglion/ipttrace',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.6.3,<4.0.0',
 }
```

### Comparing `ipttrace-0.1.0/PKG-INFO` & `ipttrace-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: ipttrace
-Version: 0.1.0
+Version: 0.1.1
 Summary: trace iptables rules with ease
+Home-page: https://github.com/sieginglion/ipttrace
 Author: sieginglion
 Author-email: sieginglion@gmail.com
 Requires-Python: >=3.6.3,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: dataclasses (>=0.8,<0.9); python_version < "3.7"
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
+Project-URL: Repository, https://github.com/sieginglion/ipttrace
```

