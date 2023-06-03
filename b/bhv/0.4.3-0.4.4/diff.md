# Comparing `tmp/bhv-0.4.3.tar.gz` & `tmp/bhv-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.4.3.tar", last modified: Thu May 25 00:19:32 2023, max compression
+gzip compressed data, was "bhv-0.4.4.tar", last modified: Sat Jun  3 22:42:21 2023, max compression
```

## Comparing `bhv-0.4.3.tar` & `bhv-0.4.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-25 00:19:32.799492 bhv-0.4.3/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.4.3/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-05-25 00:19:32.799492 bhv-0.4.3/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3846 2023-05-23 17:55:24.000000 bhv-0.4.3/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-25 00:19:32.796158 bhv-0.4.3/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.4.3/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    14714 2023-05-24 23:52:24.000000 bhv-0.4.3/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.4.3/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11951 2023-05-24 23:29:38.000000 bhv-0.4.3/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.4.3/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.4.3/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.4.3/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.4.3/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.4.3/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    26226 2023-05-25 00:18:10.000000 bhv-0.4.3/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.4.3/bhv/unification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3456 2023-05-24 13:05:15.000000 bhv-0.4.3/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.4.3/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-25 00:19:32.799492 bhv-0.4.3/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      363 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-25 00:19:32.000000 bhv-0.4.3/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-25 00:19:32.799492 bhv-0.4.3/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1343 2023-05-24 23:58:58.000000 bhv-0.4.3/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-03 22:42:21.837169 bhv-0.4.4/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.4.4/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-06-03 22:42:21.837169 bhv-0.4.4/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3846 2023-05-23 17:55:24.000000 bhv-0.4.4/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-03 22:42:21.833835 bhv-0.4.4/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.4.4/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    14829 2023-06-03 22:37:33.000000 bhv-0.4.4/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.4.4/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     4220 2023-06-03 22:38:22.000000 bhv-0.4.4/bhv/lookup.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11951 2023-06-03 22:37:20.000000 bhv-0.4.4/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-05-27 17:35:51.000000 bhv-0.4.4/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.4.4/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.4.4/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.4.4/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.4.4/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    26226 2023-05-25 00:18:10.000000 bhv-0.4.4/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.4.4/bhv/unification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3456 2023-05-24 13:05:15.000000 bhv-0.4.4/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.4.4/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-06-03 22:42:21.833835 bhv-0.4.4/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1055 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      377 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-06-03 22:42:21.000000 bhv-0.4.4/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-06-03 22:42:21.837169 bhv-0.4.4/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1343 2023-06-03 22:40:59.000000 bhv-0.4.4/setup.py
```

### Comparing `bhv-0.4.3/LICENSE` & `bhv-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/PKG-INFO` & `bhv-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.4.3
+Version: 0.4.4
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bhv-0.4.3/README.md` & `bhv-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/abstract.py` & `bhv-0.4.4/bhv/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from statistics import NormalDist
 from itertools import accumulate
 from functools import cache
 from operator import or_, and_
+from math import comb
 
 from .shared import *
 
 
 class AbstractBHV:
     # recall
     # information_entropy(p) = -p*log2(p) - (1 - p)*log2(1 - p)
@@ -191,14 +192,18 @@
         return self.frac_to_std(self.bit_error_rate(other), invert)
 
     @staticmethod
     def normal(mean=0., p=.5):
         return NormalDist(mean, (DIMENSION*p*(1 - p))**.5)
 
     @staticmethod
+    def maj_ber(n):
+        return comb(n - 1, (n - 1)//2)/2**n
+
+    @staticmethod
     def frac_to_std(frac, invert=False):
         n = AbstractBHV.normal(0.0)
         estdvs = n.zscore(0.5*DIMENSION)
         stdvs = n.zscore(frac*DIMENSION)
         return estdvs - stdvs if invert else stdvs
 
     @staticmethod
@@ -213,22 +218,22 @@
 
     def pvalue(self) -> float:
         n = AbstractBHV.normal(0.5*DIMENSION)
         s = n.cdf(self.active())
         return 2.*min(s, 1. - s)
 
     def related(self, other: Self, stdvs=6) -> bool:
-        return abs(self.std_apart(other)) < stdvs
+        return abs(self.std_apart(other)) <= stdvs
 
     def unrelated(self, other: Self, stdvs=6) -> bool:
-        return abs(self.std_apart(other, invert=True)) < stdvs
+        return abs(self.std_apart(other, invert=True)) <= stdvs
 
     def bias_rel(self, other: Self, rel: Self) -> float:
-        rel_l = rel.hamming(self)
-        rel_r = rel.hamming(other)
+        rel_l = (rel & self).active()
+        rel_r = (rel & other).active()
         return rel_l/(rel_l + rel_r)
 
     # Alternative implementations
 
     @classmethod
     def _majority3_select(cls, a: Self, b: Self, c: Self) -> Self:
         # C:  1 0 0 1 0 1 1
```

### Comparing `bhv-0.4.3/bhv/embedding.py` & `bhv-0.4.4/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/np.py` & `bhv-0.4.4/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/poibin.py` & `bhv-0.4.4/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/positions.py` & `bhv-0.4.4/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/pytorch.py` & `bhv-0.4.4/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/shared.py` & `bhv-0.4.4/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/slice.py` & `bhv-0.4.4/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/symbolic.py` & `bhv-0.4.4/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/unification.py` & `bhv-0.4.4/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/vanilla.py` & `bhv-0.4.4/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv/visualization.py` & `bhv-0.4.4/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.4.3/bhv.egg-info/PKG-INFO` & `bhv-0.4.4/bhv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.4.3
+Version: 0.4.4
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bhv-0.4.3/setup.py` & `bhv-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.3'
+VERSION = '0.4.4'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

