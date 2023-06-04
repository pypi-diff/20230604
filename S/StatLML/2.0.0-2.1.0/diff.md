# Comparing `tmp/StatLML-2.0.0.tar.gz` & `tmp/StatLML-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StatLML-2.0.0.tar", last modified: Fri Jun  2 03:12:00 2023, max compression
+gzip compressed data, was "StatLML-2.1.0.tar", last modified: Sun Jun  4 03:45:39 2023, max compression
```

## Comparing `StatLML-2.0.0.tar` & `StatLML-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 03:12:00.636906 StatLML-2.0.0/
--rw-rw-rw-   0        0        0    27030 2023-02-05 08:35:17.000000 StatLML-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1211 2023-06-02 03:12:00.637406 StatLML-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-02-05 08:35:17.000000 StatLML-2.0.0/README.md
--rw-rw-rw-   0        0        0      517 2023-05-30 02:09:30.000000 StatLML-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1159 2023-06-02 03:12:00.638407 StatLML-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-06-02 03:11:28.000000 StatLML-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:12:00.620908 StatLML-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 03:12:00.628908 StatLML-2.0.0/src/SLML/
--rw-rw-rw-   0        0        0    83715 2023-05-30 02:35:41.000000 StatLML-2.0.0/src/SLML/SLML.py
--rw-rw-rw-   0        0        0      346 2023-02-05 08:35:17.000000 StatLML-2.0.0/src/SLML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 03:12:00.635908 StatLML-2.0.0/src/StatLML.egg-info/
--rw-rw-rw-   0        0        0     1211 2023-06-02 03:12:00.000000 StatLML-2.0.0/src/StatLML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-02 03:12:00.000000 StatLML-2.0.0/src/StatLML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 03:12:00.000000 StatLML-2.0.0/src/StatLML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      172 2023-06-02 03:12:00.000000 StatLML-2.0.0/src/StatLML.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-02 03:12:00.000000 StatLML-2.0.0/src/StatLML.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 03:45:39.604279 StatLML-2.1.0/
+-rw-rw-rw-   0        0        0    27030 2023-02-05 08:35:17.000000 StatLML-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1252 2023-06-04 03:45:39.604784 StatLML-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-02-05 08:35:17.000000 StatLML-2.1.0/README.md
+-rw-rw-rw-   0        0        0      517 2023-05-30 02:09:30.000000 StatLML-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1159 2023-06-04 03:45:39.605780 StatLML-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2023-06-04 03:39:31.000000 StatLML-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 03:45:39.586774 StatLML-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 03:45:39.596280 StatLML-2.1.0/src/SLML/
+-rw-rw-rw-   0        0        0    83739 2023-06-04 03:20:42.000000 StatLML-2.1.0/src/SLML/SLML.py
+-rw-rw-rw-   0        0        0      356 2023-06-04 03:45:09.000000 StatLML-2.1.0/src/SLML/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 03:45:39.603279 StatLML-2.1.0/src/StatLML.egg-info/
+-rw-rw-rw-   0        0        0     1252 2023-06-04 03:45:39.000000 StatLML-2.1.0/src/StatLML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-04 03:45:39.000000 StatLML-2.1.0/src/StatLML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 03:45:39.000000 StatLML-2.1.0/src/StatLML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      172 2023-06-04 03:45:39.000000 StatLML-2.1.0/src/StatLML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-04 03:45:39.000000 StatLML-2.1.0/src/StatLML.egg-info/top_level.txt
```

### Comparing `StatLML-2.0.0/LICENSE` & `StatLML-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `StatLML-2.0.0/PKG-INFO` & `StatLML-2.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: StatLML
-Version: 2.0.0
+Version: 2.1.0
 Summary: Statistical Learning Models Library
 Home-page: https://github.com/Ahmed-Bayoumy/SLML
 Author: Ahmed H. Bayoumy
 Author-email: ahmed.bayoumy@mail.mcgill.ca
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Ahmed-Bayoumy/SLML/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -32,7 +34,9 @@
 ## How to use SLML package
 
 After installing the `SLML` package, the functions and classes of `SLML` module can be imported directly into the python script as follows:
 
 ```pycon
 from SLML import *
 ```
+
+
```

### Comparing `StatLML-2.0.0/pyproject.toml` & `StatLML-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `StatLML-2.0.0/setup.cfg` & `StatLML-2.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7461 744c 4d4c 0d0a 7665 7273   = StatLML..vers
-00000020: 696f 6e20 3d20 322e 302e 300d 0a64 6573  ion = 2.0.0..des
+00000020: 696f 6e20 3d20 322e 312e 300d 0a64 6573  ion = 2.1.0..des
 00000030: 6372 6970 7469 6f6e 203d 2022 5374 6174  cription = "Stat
 00000040: 6973 7469 6361 6c20 4c65 6172 6e69 6e67  istical Learning
 00000050: 204d 6f64 656c 7320 6c69 6272 6172 7922   Models library"
 00000060: 0d0a 6175 7468 6f72 203d 2041 686d 6564  ..author = Ahmed
 00000070: 2048 2e20 4261 796f 756d 790d 0a61 7574   H. Bayoumy..aut
 00000080: 686f 725f 656d 6169 6c20 3d20 6168 6d65  hor_email = ahme
 00000090: 642e 6261 796f 756d 7940 6d61 696c 2e6d  d.bayoumy@mail.m
```

### Comparing `StatLML-2.0.0/setup.py` & `StatLML-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 if __name__ == "__main__":
   setup(
     name="StatLML",
     author="Ahmed H. Bayoumy",
     author_email="ahmed.bayoumy@mail.mcgill.ca",
-    version='2.0.0',
+    version='2.1.0',
     packages=find_packages(include=['SLML', 'SLML.*']),
     description="Statistical Learning Models Library",
     install_requires=[
       'numpy>=1.22.4',
       'OMADS>=1.5.0',
       'pandas>=1.4.2',
       'pyDOE2>=1.3.0',
```

### Comparing `StatLML-2.0.0/src/SLML/SLML.py` & `StatLML-2.1.0/src/SLML/SLML.py`

 * *Files 0% similar despite different names*

```diff
@@ -2313,17 +2313,18 @@
     self.sm.store_model()
 
     self.sm1 = RBF(x=xt, y=yt)
     self.sm1.model_db = os.path.join(os.getcwd(), f"tests/models_db/{self.sm.name}")
 
     self.sm1.load_model()
 
-    lower, yp, upper = self.sm.bootstrap()
+    
     # Visualization
     if display:
+      lower, yp, upper = self.sm.bootstrap()
       Xm, Ym, Z = self.RB2d(x=None, isSurf=True)
       vis = visualize(xsurf=Xm, ysurf=Ym, zsurf=Z, residuals= self.sm.metrics.residuals,xs=self.sm.xtest.points, yp=yp, ys=self.sm.ytest.points, lower=lower, upper=upper, RMSE=self.sm.metrics.RMSE, PRESS=self.sm.metrics.PRESS, R2_pred=self.sm.metrics.R2_PRED, R2=self.sm.metrics.R2, style="deeplearning.mplstyle")
       vis.accuracy_metrics()
       vis.plot3d_surf_and_scatter()
       plt.show()
 
   def RB_kriging(self, display=True):
@@ -2348,17 +2349,18 @@
     self.sm.model_db = os.path.join(os.getcwd(), f"tests/models_db/{self.sm.name}")
     self.sm.store_model()
 
     self.sm1 = Kriging(x=xt, y=yt)
     self.sm1.model_db = os.path.join(os.getcwd(), f"tests/models_db/{self.sm.name}")
     self.sm1.load_model()
 
-    lower, yp, upper = self.sm.bootstrap()
+    
     # Visualization
     if display:
+      lower, yp, upper = self.sm.bootstrap()
       Xm, Ym, Z = self.RB2d(x=None, isSurf=True)
       vis = visualize(xsurf=Xm, ysurf=Ym, zsurf=Z, residuals= self.sm.metrics.residuals,xs=self.sm.xtest.points, yp=yp, ys=self.sm.ytest.points, lower=lower, upper=upper, RMSE=self.sm.metrics.RMSE, PRESS=self.sm.metrics.PRESS, R2_pred=self.sm.metrics.R2_PRED, R2=self.sm.metrics.R2, style="deeplearning.mplstyle")
       vis.accuracy_metrics()
       vis.plot3d_surf_and_scatter()
       plt.show()
 
   def RB_LS(self, display=True):
@@ -2384,16 +2386,17 @@
     self.sm.store_model()
 
     self.sm1 = LS(x=xt, y=yt)
     self.sm1.model_db = os.path.join(os.getcwd(), f"tests/models_db/{self.sm.name}")
 
     self.sm1.load_model()
 
-    lower, yp, upper = self.sm.bootstrap()
+    
     if display:
+      lower, yp, upper = self.sm.bootstrap()
     # Visualization
       Xm, Ym, Z = self.RB2d(x=None, isSurf=True)
       vis = visualize(xsurf=Xm, ysurf=Ym, zsurf=Z, residuals= self.sm.metrics.residuals,xs=self.sm.xtest.points, yp=yp, ys=self.sm.ytest.points, lower=lower, upper=upper, RMSE=self.sm.metrics.RMSE, PRESS=self.sm.metrics.PRESS, R2_pred=self.sm.metrics.R2_PRED, R2=self.sm.metrics.R2, style="deeplearning.mplstyle")
       vis.accuracy_metrics()
       vis.plot3d_surf_and_scatter()
       plt.show()
```

### Comparing `StatLML-2.0.0/src/StatLML.egg-info/PKG-INFO` & `StatLML-2.1.0/src/StatLML.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: StatLML
-Version: 2.0.0
+Version: 2.1.0
 Summary: Statistical Learning Models Library
 Home-page: https://github.com/Ahmed-Bayoumy/SLML
 Author: Ahmed H. Bayoumy
 Author-email: ahmed.bayoumy@mail.mcgill.ca
+License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Ahmed-Bayoumy/SLML/issues
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -32,7 +34,9 @@
 ## How to use SLML package
 
 After installing the `SLML` package, the functions and classes of `SLML` module can be imported directly into the python script as follows:
 
 ```pycon
 from SLML import *
 ```
+
+
```

