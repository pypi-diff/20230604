# Comparing `tmp/mlplatformutils-0.4.tar.gz` & `tmp/mlplatformutils-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.4.tar", last modified: Sun Jun  4 21:18:09 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.5.tar", last modified: Sun Jun  4 21:21:08 2023, max compression
```

## Comparing `mlplatformutils-0.4.tar` & `mlplatformutils-0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 21:18:09.785901 mlplatformutils-0.4/
--rw-rw-rw-   0        0        0     2782 2023-06-04 21:18:09.785901 mlplatformutils-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-04 02:08:17.000000 mlplatformutils-0.4/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-04 21:18:09.790907 mlplatformutils-0.4/setup.cfg
--rw-rw-rw-   0        0        0      640 2023-06-04 21:18:02.000000 mlplatformutils-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:18:09.689585 mlplatformutils-0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 21:18:09.707599 mlplatformutils-0.4/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.4/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:18:09.781905 mlplatformutils-0.4/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.4/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.4/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.4/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.4/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.4/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.4/src/mlplatformutils/core/sparkutils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 21:18:09.752901 mlplatformutils-0.4/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     2782 2023-06-04 21:18:09.000000 mlplatformutils-0.4/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-04 21:18:09.000000 mlplatformutils-0.4/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 21:18:09.000000 mlplatformutils-0.4/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 21:18:09.000000 mlplatformutils-0.4/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 21:18:09.000000 mlplatformutils-0.4/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.186158 mlplatformutils-0.5/
+-rw-rw-rw-   0        0        0     3046 2023-06-04 21:21:08.187156 mlplatformutils-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-04 02:08:17.000000 mlplatformutils-0.5/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-04 21:21:08.192152 mlplatformutils-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-06-04 21:21:04.000000 mlplatformutils-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.084007 mlplatformutils-0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.105603 mlplatformutils-0.5/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.5/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.182153 mlplatformutils-0.5/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.5/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.5/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.5/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.5/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.5/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.5/src/mlplatformutils/core/sparkutils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:21:08.150152 mlplatformutils-0.5/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3046 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 21:21:07.000000 mlplatformutils-0.5/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.4/PKG-INFO` & `mlplatformutils-0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,63 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.4
+Version: 0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Description: # mlplatformutils
+        
+        <br />
          mlplatformutils for observability
         
         ## Structure
-        .
-        |-- LICENSE.txt
-        |-- README.rst
-        |-- setup.cfg
-        |-- setup.py
-        |-- src
-        |   |-- mlplatformutils
-        |   |   |-- __init__.py
-        |   |   |-- core
-        |   |   |-- |-- __init__.py
-        |   |   |-- |-- sparkutils.py
-        |   |   |-- |-- platformutils.py
-        |   |   |-- |-- pandasutils.py
-        |   |   |-- |-- lineagegraph.py
-        |   |   |-- |-- app_insights_logger.py
-        |-- tests
-        |   |-- __init__.py
-        |   |-- core
-        |   |-- |--__init__.py
-        |   |-- |-- sparkutils.py
-        |   |-- |-- platformutils.py
-        |   |-- |-- pandasutils.py
-        |   |-- |-- lineagegraph.py
-        |   |-- |-- app_insights_logger.py
+        
+        <br />
+        .<br />
+        |-- LICENSE.txt<br />
+        |-- README.rst<br />
+        |-- setup.cfg<br />
+        |-- setup.py<br />
+        |-- src<br />
+        |   |-- mlplatformutils<br />
+        |   |   |-- __init__.py<br />
+        |   |   |-- core<br />
+        |   |   |-- |-- __init__.py<br />
+        |   |   |-- |-- sparkutils.py<br />
+        |   |   |-- |-- platformutils.py<br />
+        |   |   |-- |-- pandasutils.py<br />
+        |   |   |-- |-- lineagegraph.py<br />
+        |   |   |-- |-- app_insights_logger.py<br />
+        |-- tests<br />
+        |   |-- __init__.py<br />
+        |   |-- core<br />
+        |   |-- |--__init__.py<br />
+        |   |-- |-- sparkutils.py<br />
+        |   |-- |-- platformutils.py<br />
+        |   |-- |-- pandasutils.py<br />
+        |   |-- |-- lineagegraph.py<br />
+        |   |-- |-- app_insights_logger.py<br />
+        <br />
         
         ## Instructions
         
+        <br />
          install twine - twine is a utility package that is used for publishing Python packages on PyPI
          python -m pip install twine 
          Build Package - create the source distribution of the package
          python setup.py sdist 
          Upload Package to PyPI
          python -m twine upload dist/*
         
         ## Description
+        
+        <br />
+        
         **app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights
         **lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin
         
         **platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute
         
         * is_package_installed
         * install_pip
```

### Comparing `mlplatformutils-0.4/setup.py` & `mlplatformutils-0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.4',
+    version='0.5',
     license='MIT',
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     keywords='mlplatformutils',
     install_requires=[
```

### Comparing `mlplatformutils-0.4/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.5/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.4/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.5/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.4/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.5/src/mlplatformutils/core/pandasutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.4/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.5/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.4/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.5/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.4/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.5/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,63 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.4
+Version: 0.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Description: # mlplatformutils
+        
+        <br />
          mlplatformutils for observability
         
         ## Structure
-        .
-        |-- LICENSE.txt
-        |-- README.rst
-        |-- setup.cfg
-        |-- setup.py
-        |-- src
-        |   |-- mlplatformutils
-        |   |   |-- __init__.py
-        |   |   |-- core
-        |   |   |-- |-- __init__.py
-        |   |   |-- |-- sparkutils.py
-        |   |   |-- |-- platformutils.py
-        |   |   |-- |-- pandasutils.py
-        |   |   |-- |-- lineagegraph.py
-        |   |   |-- |-- app_insights_logger.py
-        |-- tests
-        |   |-- __init__.py
-        |   |-- core
-        |   |-- |--__init__.py
-        |   |-- |-- sparkutils.py
-        |   |-- |-- platformutils.py
-        |   |-- |-- pandasutils.py
-        |   |-- |-- lineagegraph.py
-        |   |-- |-- app_insights_logger.py
+        
+        <br />
+        .<br />
+        |-- LICENSE.txt<br />
+        |-- README.rst<br />
+        |-- setup.cfg<br />
+        |-- setup.py<br />
+        |-- src<br />
+        |   |-- mlplatformutils<br />
+        |   |   |-- __init__.py<br />
+        |   |   |-- core<br />
+        |   |   |-- |-- __init__.py<br />
+        |   |   |-- |-- sparkutils.py<br />
+        |   |   |-- |-- platformutils.py<br />
+        |   |   |-- |-- pandasutils.py<br />
+        |   |   |-- |-- lineagegraph.py<br />
+        |   |   |-- |-- app_insights_logger.py<br />
+        |-- tests<br />
+        |   |-- __init__.py<br />
+        |   |-- core<br />
+        |   |-- |--__init__.py<br />
+        |   |-- |-- sparkutils.py<br />
+        |   |-- |-- platformutils.py<br />
+        |   |-- |-- pandasutils.py<br />
+        |   |-- |-- lineagegraph.py<br />
+        |   |-- |-- app_insights_logger.py<br />
+        <br />
         
         ## Instructions
         
+        <br />
          install twine - twine is a utility package that is used for publishing Python packages on PyPI
          python -m pip install twine 
          Build Package - create the source distribution of the package
          python setup.py sdist 
          Upload Package to PyPI
          python -m twine upload dist/*
         
         ## Description
+        
+        <br />
+        
         **app_insights_logger** - Constains **telemetrylogger** Class with Functions to Manage and Log Telemetry into Azure Application Insights
         **lineagegraph** - Contains **LineageGraph** Class with functions to manage Graph on Azure Cosmos DB enabled with Gremlin
         
         **platformutils** - Contains platform utility functions to check, install depedencies, check Azure ML Compute
         
         * is_package_installed
         * install_pip
```

### Comparing `mlplatformutils-0.4/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.5/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

