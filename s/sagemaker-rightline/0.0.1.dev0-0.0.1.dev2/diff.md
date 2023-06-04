# Comparing `tmp/sagemaker-rightline-0.0.1.dev0.tar.gz` & `tmp/sagemaker-rightline-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.0.1.dev0.tar", last modified: Sun Jun  4 09:28:19 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.0.1.dev2.tar", last modified: Sun Jun  4 09:45:42 2023, max compression
```

## Comparing `sagemaker-rightline-0.0.1.dev0.tar` & `sagemaker-rightline-0.0.1.dev2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:28:19.405647 sagemaker-rightline-0.0.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-04 09:28:19.405647 sagemaker-rightline-0.0.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-04 09:28:12.000000 sagemaker-rightline-0.0.1.dev0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:28:19.401647 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 09:28:12.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:28:19.405647 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-04 09:28:19.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-04 09:28:19.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:28:19.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 09:28:19.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 09:28:19.000000 sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:28:19.405647 sagemaker-rightline-0.0.1.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:28:19.405647 sagemaker-rightline-0.0.1.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-04 09:28:08.000000 sagemaker-rightline-0.0.1.dev0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:45:42.511468 sagemaker-rightline-0.0.1.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-04 09:45:42.511468 sagemaker-rightline-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:45:42.507468 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 09:45:33.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:45:42.511468 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-04 09:45:42.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-04 09:45:42.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:45:42.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 09:45:42.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-04 09:45:42.000000 sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:45:42.511468 sagemaker-rightline-0.0.1.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:45:42.511468 sagemaker-rightline-0.0.1.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-04 09:45:28.000000 sagemaker-rightline-0.0.1.dev2/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.0.1.dev0/LICENSE` & `sagemaker-rightline-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/PKG-INFO` & `sagemaker-rightline-0.0.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.0.1.dev0
+Version: 0.0.1.dev2
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sagemaker-rightline-0.0.1.dev0/README.md` & `sagemaker-rightline-0.0.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/pyproject.toml` & `sagemaker-rightline-0.0.1.dev2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "sagemaker-rightline"
 requires-python = ">=3.8"
-version = "0.0.1dev0"
+dynamic = ["version"]
 description = "Python package to easily validate properties of a SageMaker Pipeline."
 authors = [
     {name = "stiebels", email = "stiebels@github.com"},
     {name = "dipanjank", email = "dipanjank@github.com"},
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
@@ -49,14 +49,17 @@
 
 [build-system]
 # These are the assumed default build requirements from pip:
 # https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.dynamic]
+version = {attr = "sagemaker_rightline.__version__"}
+
 [tool.black]
 line-length = 100
 
 [tool.flake8]
 max-line-length = 100
 per-file-ignores = [
     'tests/*:F401,F811',
```

### Comparing `sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/model.py` & `sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.0.1.dev2/sagemaker_rightline/validations.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.0.1.dev2/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.0.1.dev0
+Version: 0.0.1.dev2
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sagemaker-rightline-0.0.1.dev0/tests/test_model.py` & `sagemaker-rightline-0.0.1.dev2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/tests/test_rules.py` & `sagemaker-rightline-0.0.1.dev2/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.0.1.dev0/tests/test_validations.py` & `sagemaker-rightline-0.0.1.dev2/tests/test_validations.py`

 * *Files identical despite different names*

