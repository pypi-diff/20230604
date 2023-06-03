# Comparing `tmp/fgdb_to_gpkg-0.1.4.tar.gz` & `tmp/fgdb_to_gpkg-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgdb_to_gpkg-0.1.4.tar", max compression
+gzip compressed data, was "fgdb_to_gpkg-0.1.6.tar", max compression
```

## Comparing `fgdb_to_gpkg-0.1.4.tar` & `fgdb_to_gpkg-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-03-27 05:13:52.237334 fgdb_to_gpkg-0.1.4/LICENSE
--rw-r--r--   0        0        0     2571 2023-03-30 16:37:52.130877 fgdb_to_gpkg-0.1.4/README.md
--rw-r--r--   0        0        0       74 2023-03-22 01:50:55.132497 fgdb_to_gpkg-0.1.4/fgdb_to_gpkg/__init__.py
--rw-r--r--   0        0        0     2584 2023-03-27 05:17:45.387926 fgdb_to_gpkg-0.1.4/fgdb_to_gpkg/fgdb_to_gpkg.py
--rw-r--r--   0        0        0      826 2023-03-30 16:38:01.948718 fgdb_to_gpkg-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 fgdb_to_gpkg-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-03 23:27:08.943283 fgdb_to_gpkg-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2601 2023-06-03 23:27:08.943283 fgdb_to_gpkg-0.1.6/README.md
+-rw-r--r--   0        0        0       74 2023-06-03 23:27:08.943283 fgdb_to_gpkg-0.1.6/fgdb_to_gpkg/__init__.py
+-rw-r--r--   0        0        0     2584 2023-06-03 23:27:08.943283 fgdb_to_gpkg-0.1.6/fgdb_to_gpkg/fgdb_to_gpkg.py
+-rw-r--r--   0        0        0      870 2023-06-03 23:27:08.943283 fgdb_to_gpkg-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 fgdb_to_gpkg-0.1.6/PKG-INFO
```

### Comparing `fgdb_to_gpkg-0.1.4/LICENSE` & `fgdb_to_gpkg-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fgdb_to_gpkg-0.1.4/README.md` & `fgdb_to_gpkg-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pip install fgdb-to-gpkg
 ```
 
 #### Installing the development version of this package
 
 1. Clone the repository: `git clone https://github.com/philiporlando/fgdb_to_gdb.git`
 2. Navigate to the repository directory: `cd fgdb_to_gdb`
-3. Install the package and its dependencies with poetry: `poetry install`
+3. Install the package and its dependencies with [poetry](https://python-poetry.org/): `poetry install`
 
 ## Usage
 
 ### Command Line Usage
 
 To use `fgdb_to_gpkg` from the command line, simply call the `fgdb_to_gpkg` command with the path to the input File GeoDatabase and the path to the output GeoPackage:
```

### Comparing `fgdb_to_gpkg-0.1.4/fgdb_to_gpkg/fgdb_to_gpkg.py` & `fgdb_to_gpkg-0.1.6/fgdb_to_gpkg/fgdb_to_gpkg.py`

 * *Files identical despite different names*

### Comparing `fgdb_to_gpkg-0.1.4/pyproject.toml` & `fgdb_to_gpkg-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "fgdb-to-gpkg"
-version = "0.1.4"
+version = "0.1.6"
 description = "A lightweight Python package that converts Esri File GeoDataBases into OGC GeoPackages"
 authors = [
     {name = "Philip Orlando", email = "phlp.orlando@gmail.com"},
     ]
 
 [project.dependencies]
 fiona = "1.9.2"
 geopandas = "0.12.2"
 [tool.poetry]
 name = "fgdb-to-gpkg"
-version = "0.1.4"
+version = "0.1.6"
 description = "A lightweight Python package that converts Esri File GeoDataBases into OGC GeoPackages"
 authors = ["Philip Orlando <phlp.orlando@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 geopandas = "^0.12.2"
@@ -23,11 +23,13 @@
 tqdm = "^4.65.0"
 argparse = "^1.4.0"
 fiona = "^1.9.2"
 gdal = "^3.6.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
+pytest-cov = "^4.0.0"
+ipykernel = "^6.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fgdb_to_gpkg-0.1.4/PKG-INFO` & `fgdb_to_gpkg-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgdb-to-gpkg
-Version: 0.1.4
+Version: 0.1.6
 Summary: A lightweight Python package that converts Esri File GeoDataBases into OGC GeoPackages
 Author: Philip Orlando
 Author-email: phlp.orlando@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,15 +30,15 @@
 pip install fgdb-to-gpkg
 ```
 
 #### Installing the development version of this package
 
 1. Clone the repository: `git clone https://github.com/philiporlando/fgdb_to_gdb.git`
 2. Navigate to the repository directory: `cd fgdb_to_gdb`
-3. Install the package and its dependencies with poetry: `poetry install`
+3. Install the package and its dependencies with [poetry](https://python-poetry.org/): `poetry install`
 
 ## Usage
 
 ### Command Line Usage
 
 To use `fgdb_to_gpkg` from the command line, simply call the `fgdb_to_gpkg` command with the path to the input File GeoDatabase and the path to the output GeoPackage:
```

