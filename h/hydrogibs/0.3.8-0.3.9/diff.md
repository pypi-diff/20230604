# Comparing `tmp/hydrogibs-0.3.8.tar.gz` & `tmp/hydrogibs-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.3.8.tar", last modified: Sat Jun  3 17:09:21 2023, max compression
+gzip compressed data, was "hydrogibs-0.3.9.tar", last modified: Sat Jun  3 17:29:29 2023, max compression
```

## Comparing `hydrogibs-0.3.8.tar` & `hydrogibs-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:09:21.517545 hydrogibs-0.3.8/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.8/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)     1615 2023-06-03 17:09:21.517545 hydrogibs-0.3.8/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.3.8/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:09:21.513545 hydrogibs-0.3.8/hydrogibs/
--rwxrwxr-x   0 axel      (1000) axel      (1000)    14055 2023-06-03 17:07:49.000000 hydrogibs-0.3.8/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-06-03 17:06:24.000000 hydrogibs-0.3.8/hydrogibs/ModelApp.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.8/hydrogibs/ModelTemplate.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     7892 2023-06-03 17:08:00.000000 hydrogibs-0.3.8/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.8/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-05-24 13:52:28.000000 hydrogibs-0.3.8/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      121 2023-06-03 17:06:41.000000 hydrogibs-0.3.8/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.8/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:09:21.513545 hydrogibs-0.3.8/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1615 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-06-03 17:09:21.000000 hydrogibs-0.3.8/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      592 2023-06-03 17:05:24.000000 hydrogibs-0.3.8/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-06-03 17:09:21.517545 hydrogibs-0.3.8/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:29:29.362735 hydrogibs-0.3.9/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.3.9/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1615 2023-06-03 17:29:29.358735 hydrogibs-0.3.9/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1008 2023-05-23 16:56:32.000000 hydrogibs-0.3.9/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:29:29.358735 hydrogibs-0.3.9/hydrogibs/
+-rwxrwxr-x   0 axel      (1000) axel      (1000)    14093 2023-06-03 17:28:28.000000 hydrogibs-0.3.9/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     5176 2023-06-03 17:06:24.000000 hydrogibs-0.3.9/hydrogibs/ModelApp.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1084 2023-04-29 08:59:49.000000 hydrogibs-0.3.9/hydrogibs/ModelTemplate.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     7930 2023-06-03 17:28:28.000000 hydrogibs-0.3.9/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1022 2023-05-14 09:41:57.000000 hydrogibs-0.3.9/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-05-24 13:52:28.000000 hydrogibs-0.3.9/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      121 2023-06-03 17:06:41.000000 hydrogibs-0.3.9/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4751 2023-05-01 00:17:18.000000 hydrogibs-0.3.9/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-06-03 17:29:29.358735 hydrogibs-0.3.9/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1615 2023-06-03 17:29:29.000000 hydrogibs-0.3.9/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      335 2023-06-03 17:29:29.000000 hydrogibs-0.3.9/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-06-03 17:29:29.000000 hydrogibs-0.3.9/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-06-03 17:29:29.000000 hydrogibs-0.3.9/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      592 2023-06-03 17:29:14.000000 hydrogibs-0.3.9/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-06-03 17:29:29.362735 hydrogibs-0.3.9/setup.cfg
```

### Comparing `hydrogibs-0.3.8/LICENSE` & `hydrogibs-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/PKG-INFO` & `hydrogibs-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.8
+Version: 0.3.9
 Summary: A small hydrology package created for a class project with Christophe Ancey: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.3.8/README.md` & `hydrogibs-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/hydrogibs/GR4.py` & `hydrogibs-0.3.9/hydrogibs/GR4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from matplotlib import pyplot as plt
 from typing import Callable, Literal
 from hydrogibs.ModelApp import ModelApp, Entry
 import hydrogibs.ModelTemplate as ModelTemplate
 from warnings import warn
+from os.path import dirname
 
 
 def _transfer_func(X4: float, num: int) -> np.ndarray:
     """
     This function will make the transition between the
     water flow and the discharge through a convolution
 
@@ -157,19 +158,18 @@
 
     def __matmul__(self, rain):
         return rain @ self
 
 
 def _read_presets():
 
-    presets = dict()
-
-    with open("hydrogibs/data/GR4presets.csv") as file:
+    with open(f"{dirname(__file__)}/data/GR4presets.csv") as file:
         lines = file.readlines()
 
+    presets = dict()
     for line in lines[2:]:
         line = line.replace('\n', '')
         data = [
             float(d) if d.replace('.', '', 1).isdigit()
             else d
             for d in line.split(',')
         ]
```

### Comparing `hydrogibs-0.3.8/hydrogibs/ModelApp.py` & `hydrogibs-0.3.9/hydrogibs/ModelApp.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/hydrogibs/ModelTemplate.py` & `hydrogibs-0.3.9/hydrogibs/ModelTemplate.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/hydrogibs/QDF.py` & `hydrogibs-0.3.9/hydrogibs/QDF.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 from hydrogibs.misc import Turraza
 from typing import Literal, Union
 from matplotlib import pyplot as plt
 from hydrogibs.ModelApp import ModelApp, Entry
 from warnings import warn
 from scipy.optimize import least_squares
+from os.path import dirname
 
 
 def _read_coeficients(kind="mean"):
 
-    with open(f"hydrogibs/data/QDFcoefs_{kind}.csv") as file:
+    with open(f"{dirname(__file__)}/data/QDFcoefs_{kind}.csv") as file:
         lines = file.readlines()
 
     coefs = dict()
     for line in lines[2:]:
         name, *values = line.split(',')
         values = [float(v) for v in values]
         coefs[name] = dict(
```

### Comparing `hydrogibs-0.3.8/hydrogibs/RationalMethod.py` & `hydrogibs-0.3.9/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/hydrogibs/SoCoSe.py` & `hydrogibs-0.3.9/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/hydrogibs/misc.py` & `hydrogibs-0.3.9/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.3.8/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.3.9/hydrogibs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.3.8
+Version: 0.3.9
 Summary: A small hydrology package created for a class project with Christophe Ancey: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.3.8/pyproject.toml` & `hydrogibs-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hydrogibs"
-version = "0.3.8"
+version = "0.3.9"
 authors = [
   { name="axel Giboulot", email="axel.giboulot@epfl.ch" },
 ]
 description = "A small hydrology package created for a class project with Christophe Ancey: http://fr.ancey.ch/cours/masterGC/cours-hydraulique.pdf"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

