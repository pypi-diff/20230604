# Comparing `tmp/paux-1.0.8.tar.gz` & `tmp/paux-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paux-1.0.8.tar", last modified: Tue Feb 21 14:03:54 2023, max compression
+gzip compressed data, was "dist/paux-1.0.9.tar", last modified: Wed Mar  1 03:30:43 2023, max compression
```

## Comparing `paux-1.0.8.tar` & `paux-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-02-21 14:03:54.189530 paux-1.0.8/
--rw-r--r--   0 kzlknight   (501) staff       (20)      594 2023-02-21 14:03:54.189078 paux-1.0.8/PKG-INFO
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-02-21 14:03:54.185228 paux-1.0.8/paux/
--rw-r--r--   0 kzlknight   (501) staff       (20)      232 2023-02-21 14:03:18.000000 paux-1.0.8/paux/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    12493 2023-01-14 21:57:07.000000 paux-1.0.8/paux/date.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      338 2023-01-14 21:53:10.000000 paux-1.0.8/paux/digit.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-02-21 14:03:54.188441 paux-1.0.8/paux/exception/
--rw-r--r--   0 kzlknight   (501) staff       (20)       71 2023-01-14 21:57:07.000000 paux-1.0.8/paux/exception/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      103 2023-01-14 08:47:16.000000 paux-1.0.8/paux/exception/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      143 2023-01-14 21:57:07.000000 paux-1.0.8/paux/exception/execute.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1354 2023-01-14 21:57:07.000000 paux-1.0.8/paux/exception/param.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1437 2023-01-14 21:53:18.000000 paux-1.0.8/paux/filter.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     3927 2023-01-28 08:49:55.000000 paux-1.0.8/paux/log.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     9092 2023-02-21 14:03:04.000000 paux-1.0.8/paux/order.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1924 2023-01-14 21:53:55.000000 paux-1.0.8/paux/param.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     3778 2023-01-14 21:57:07.000000 paux-1.0.8/paux/process.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1054 2023-01-26 07:18:44.000000 paux-1.0.8/paux/system.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      816 2023-01-14 21:54:26.000000 paux-1.0.8/paux/thread.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-02-21 14:03:54.186767 paux-1.0.8/paux.egg-info/
--rw-r--r--   0 kzlknight   (501) staff       (20)      594 2023-02-21 14:03:54.000000 paux-1.0.8/paux.egg-info/PKG-INFO
--rw-r--r--   0 kzlknight   (501) staff       (20)      393 2023-02-21 14:03:54.000000 paux-1.0.8/paux.egg-info/SOURCES.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-02-21 14:03:54.000000 paux-1.0.8/paux.egg-info/dependency_links.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       28 2023-02-21 14:03:54.000000 paux-1.0.8/paux.egg-info/requires.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)        5 2023-02-21 14:03:54.000000 paux-1.0.8/paux.egg-info/top_level.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-02-21 14:03:54.189638 paux-1.0.8/setup.cfg
--rw-r--r--   0 kzlknight   (501) staff       (20)     2744 2023-02-21 14:03:08.000000 paux-1.0.8/setup.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-01 03:30:43.250825 paux-1.0.9/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      594 2023-03-01 03:30:43.250323 paux-1.0.9/PKG-INFO
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-01 03:30:43.246207 paux-1.0.9/paux/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      232 2023-03-01 03:30:23.000000 paux-1.0.9/paux/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    12493 2023-01-14 21:57:07.000000 paux-1.0.9/paux/date.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      338 2023-01-14 21:53:10.000000 paux-1.0.9/paux/digit.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-01 03:30:43.249659 paux-1.0.9/paux/exception/
+-rw-r--r--   0 kzlknight   (501) staff       (20)       71 2023-01-14 21:57:07.000000 paux-1.0.9/paux/exception/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      103 2023-01-14 08:47:16.000000 paux-1.0.9/paux/exception/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      143 2023-01-14 21:57:07.000000 paux-1.0.9/paux/exception/execute.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1354 2023-01-14 21:57:07.000000 paux-1.0.9/paux/exception/param.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1437 2023-01-14 21:53:18.000000 paux-1.0.9/paux/filter.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     3927 2023-01-28 08:49:55.000000 paux-1.0.9/paux/log.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     9132 2023-03-01 03:29:13.000000 paux-1.0.9/paux/order.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1924 2023-01-14 21:53:55.000000 paux-1.0.9/paux/param.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     3778 2023-01-14 21:57:07.000000 paux-1.0.9/paux/process.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1054 2023-01-26 07:18:44.000000 paux-1.0.9/paux/system.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      816 2023-01-14 21:54:26.000000 paux-1.0.9/paux/thread.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-03-01 03:30:43.248022 paux-1.0.9/paux.egg-info/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      594 2023-03-01 03:30:43.000000 paux-1.0.9/paux.egg-info/PKG-INFO
+-rw-r--r--   0 kzlknight   (501) staff       (20)      393 2023-03-01 03:30:43.000000 paux-1.0.9/paux.egg-info/SOURCES.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-03-01 03:30:43.000000 paux-1.0.9/paux.egg-info/dependency_links.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       28 2023-03-01 03:30:43.000000 paux-1.0.9/paux.egg-info/requires.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)        5 2023-03-01 03:30:43.000000 paux-1.0.9/paux.egg-info/top_level.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-03-01 03:30:43.250976 paux-1.0.9/setup.cfg
+-rw-r--r--   0 kzlknight   (501) staff       (20)     2744 2023-03-01 03:30:15.000000 paux-1.0.9/setup.py
```

### Comparing `paux-1.0.8/PKG-INFO` & `paux-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paux
-Version: 1.0.8
+Version: 1.0.9
 Summary: finance trade tool
 Home-page: https://github.com/pyted/paux
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `paux-1.0.8/paux/date.py` & `paux-1.0.9/paux/date.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/exception/param.py` & `paux-1.0.9/paux/exception/param.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/filter.py` & `paux-1.0.9/paux/filter.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/log.py` & `paux-1.0.9/paux/log.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/order.py` & `paux-1.0.9/paux/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 # 用于模拟交易中的的价格圆整，保证圆整后的价格与圆整前相差不超过0.001%
 def round_simulate(price) -> float:
     '''
     :param price: 价格
     '''
     if isinstance(price, int):
         return price
+    if price == 0:
+        return price
     price_0_00001 = 0.00001 * price
     if price_0_00001 < 1:
         ndigits = len(str(int(1 / price_0_00001)))
         price_round = round(price, ndigits)
     else:
         price_round = round(price, 1)
     if abs((price_round - price) / price) >= 0.00001:
```

### Comparing `paux-1.0.8/paux/param.py` & `paux-1.0.9/paux/param.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/process.py` & `paux-1.0.9/paux/process.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/system.py` & `paux-1.0.9/paux/system.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux/thread.py` & `paux-1.0.9/paux/thread.py`

 * *Files identical despite different names*

### Comparing `paux-1.0.8/paux.egg-info/PKG-INFO` & `paux-1.0.9/paux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paux
-Version: 1.0.8
+Version: 1.0.9
 Summary: finance trade tool
 Home-page: https://github.com/pyted/paux
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `paux-1.0.8/setup.py` & `paux-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'paux'
 DESCRIPTION = "finance trade tool"
 URL = "https://github.com/pyted/paux"
 EMAIL = 'pyted@outlook.com'
 AUTHOR = 'pyted'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 REQUIRED = [
     'numpy',
     'pandas',
     'pendulum',
     'redis'
 ]
```

