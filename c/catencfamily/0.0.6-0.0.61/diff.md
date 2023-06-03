# Comparing `tmp/catencfamily-0.0.6.tar.gz` & `tmp/catencfamily-0.0.61.tar.gz`

## Comparing `catencfamily-0.0.6.tar` & `catencfamily-0.0.61.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.6/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.6/src/catencfamily/cef.py
--rw-r--r--   0        0        0    44680 2020-02-02 00:00:00.000000 catencfamily-0.0.6/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.6/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.6/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 catencfamily-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.61/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    88962 2020-02-02 00:00:00.000000 catencfamily-0.0.61/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 catencfamily-0.0.61/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.61/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.61/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.61/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.61/PKG-INFO
```

### Comparing `catencfamily-0.0.6/src/catencfamily/cef.py` & `catencfamily-0.0.61/src/catencfamily/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# 3rd June, 2023
+"""
+References:
+Coding standard:
+    https://gist.github.com/nateGeorge/5455d2c57fb33c1ae04706f2dc4fee01
+    
+Developing sklearn estimators:
+    https://scikit-learn.org/stable/developers/develop.html 
+    
+Project template:
+    https://github.com/scikit-learn-contrib/project-template/    
+    
+"""
+
+
+
 # 1.0 Libraries
 import pandas as pd
 import numpy as np
 
 
 # 1.01 For networks and centrality measures
 import networkx as nx
@@ -289,21 +305,37 @@
         """
         assert self.n_iter > 0, "n_iter can not be 0. Default is 1."
         assert len(self.cat_cols) > 0, "cat_cols can not be empty"
 
         # Check cat_cols names. These must not contain
         # any char other than a-zA-Z and _. Else, exception 
         # is raised
+        # https://stackoverflow.com/a/3301453
+        a = [ i for i in self.cat_cols if ' ' in i ]
+        if (len(a) > 0) :
+            raise Exception(f"Column names have spaces {a}. Remove spaces first.")
+        
+        a = [ i  for i in self.cat_cols if bool(re.search(r'\d', i))] 
+        if (len(a) > 0) :
+            raise Exception(f"Column names have digits; {a}. Rename cols to remove digits.")
+
         # https://stackoverflow.com/a/336220/3282777
-        a = [not re.search("^[a-zA-Z_]+$", i)  for i in self.cat_cols]
-        if (sum(a) > 0) :
-            raise Exception("Column names in cat_cols/data must be alphabets and may have underscore. No other char or digit etc allowed")
+        a = [ i for i in self.cat_cols       if not bool(re.search("^[a-zA-Z_]+$", i)) ]
+        if (len(a) > 0) :
+            raise Exception(f"Col names in cat_cols/data may only have alphabets/underscore: {a}. Rename cols appropriately.")
 
         msg = "No of interactingCatCols can not exceed cat_cols"
         assert (len(self.interactingCatCols) < len(self.cat_cols)) or (len(self.interactingCatCols) == len(self.cat_cols)), msg 
+        
+        if (len(self.interactingCatCols) > 0):
+            a = [ i for i in self.interactingCatCols if i not in self.cat_cols]
+            if len(a) > 0:
+                raise Exception("interactingCatCols can not have any col not included in cat_col.")
+                
+        
         assert self.noOfColsToConcat == 2,"In this ver noOfColsToConcat can only be 2"
         assert self.sampsize < 1, "sampsize be < 1. Ignored when n_iter is 1"
         assert self.verbose > 0, "verbose should minimum 1"
         if (self.saveGraph) or (self.n_iter > 1):
             assert self.modelsPath is not None, "modelsPath can not be None when n_iter > 1 as maps are saved to folder."
         u = sum(self.cMeasures[:4]) + sum(self.cMeasures[5:])
         if self.cMeasures[4] is None:   # No function object specified
```

### Comparing `catencfamily-0.0.6/LICENSE` & `catencfamily-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.6/README.md` & `catencfamily-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.6/pyproject.toml` & `catencfamily-0.0.61/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.6"
+version = "0.0.61"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.6/PKG-INFO` & `catencfamily-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.6
+Version: 0.0.61
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

