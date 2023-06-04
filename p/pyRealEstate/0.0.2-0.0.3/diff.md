# Comparing `tmp/pyRealEstate-0.0.2.tar.gz` & `tmp/pyRealEstate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.2.tar", last modified: Fri Jun  2 21:53:20 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.3.tar", last modified: Sun Jun  4 11:35:38 2023, max compression
```

## Comparing `pyRealEstate-0.0.2.tar` & `pyRealEstate-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 21:53:20.000000 pyRealEstate-0.0.2/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-02 21:53:11.000000 pyRealEstate-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-02 21:53:20.865359 pyRealEstate-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:35:38.535899 pyRealEstate-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 11:35:38.539899 pyRealEstate-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:35:38.535899 pyRealEstate-0.0.3/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:35:38.535899 pyRealEstate-0.0.3/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 11:35:38.000000 pyRealEstate-0.0.3/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-04 11:35:21.000000 pyRealEstate-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-04 11:35:38.539899 pyRealEstate-0.0.3/setup.cfg
```

### Comparing `pyRealEstate-0.0.2/LICENSE` & `pyRealEstate-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.2/PKG-INFO` & `pyRealEstate-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.2
+Version: 0.0.3
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
-Author-email: joshua.j.jorgensen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyRealEstate
 
-pyRealEstate is a library designed for data scientists working in the real estate industry. pyRealEstate is still currently under development but is aimed at providing functions to assist in the development and evaluation of AVM's. 
+pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
+of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
+but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
 
-## Instructions
-
-1. Install:
+## Instilation
 
+Simply run:
 ```
 pip3 install pyRealEstate
 ```
-## Tutorial on how to test AVM  Performance 
-
-pyRealEstate can calculate the COD (Coefficient of Dispersion) and PRD (Price Related Differential) as shown below 
-
-```
-import numpy as np 
-from pyRealEstate import RealEstateMetrics
-appr = np.array([25500,57000,39000,90000,51000,93000,49500])
-sale = np.array([75000,150000,90000,180000,90000,150000,75000])
-RealEstateMetrics.COD(appr,sale)
-```
```

### Comparing `pyRealEstate-0.0.2/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.0.3/pyRealEstate.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.2
+Version: 0.0.3
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
-Author-email: joshua.j.jorgensen@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyRealEstate
 
-pyRealEstate is a library designed for data scientists working in the real estate industry. pyRealEstate is still currently under development but is aimed at providing functions to assist in the development and evaluation of AVM's. 
+pyRealEstate is a package designed for data scientists working in the real estate industry.  This Library aims to provide tools to help in the preprocessing of data, feature engineering and evaluation 
+of AVM's (Automated valuation models). Some of metrics provided in this library are the COD ( coeficient of Disspersion), PRD ( Price Relted Differential) and weighted mean for example. pyRealEstate is still currently under development 
+but is aimed at providing functions to assist in the development and evaluation of AVM's sp please continually check for updates . 
 
-## Instructions
-
-1. Install:
+## Instilation
 
+Simply run:
 ```
 pip3 install pyRealEstate
 ```
-## Tutorial on how to test AVM  Performance 
-
-pyRealEstate can calculate the COD (Coefficient of Dispersion) and PRD (Price Related Differential) as shown below 
-
-```
-import numpy as np 
-from pyRealEstate import RealEstateMetrics
-appr = np.array([25500,57000,39000,90000,51000,93000,49500])
-sale = np.array([75000,150000,90000,180000,90000,150000,75000])
-RealEstateMetrics.COD(appr,sale)
-```
```

