# Comparing `tmp/mlplatformutils-0.2.tar.gz` & `tmp/mlplatformutils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.2.tar", last modified: Sun Jun  4 02:06:17 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.3.tar", last modified: Sun Jun  4 21:12:54 2023, max compression
```

## Comparing `mlplatformutils-0.2.tar` & `mlplatformutils-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.298859 mlplatformutils-0.2/
--rw-rw-rw-   0        0        0      242 2023-06-04 02:06:17.299860 mlplatformutils-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-04 02:05:42.000000 mlplatformutils-0.2/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-04 02:06:17.308860 mlplatformutils-0.2/setup.cfg
--rw-rw-rw-   0        0        0      466 2023-06-04 02:05:51.000000 mlplatformutils-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.053238 mlplatformutils-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.071267 mlplatformutils-0.2/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.2/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.293859 mlplatformutils-0.2/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.2/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.2/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.2/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3549 2023-06-04 01:58:38.000000 mlplatformutils-0.2/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     2815 2023-06-04 01:59:57.000000 mlplatformutils-0.2/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.2/src/mlplatformutils/core/sparkutils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.131775 mlplatformutils-0.2/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0      242 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 21:12:54.773355 mlplatformutils-0.3/
+-rw-rw-rw-   0        0        0     3441 2023-06-04 21:12:54.774357 mlplatformutils-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-04 02:08:17.000000 mlplatformutils-0.3/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-04 21:12:54.780360 mlplatformutils-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-06-04 21:12:30.000000 mlplatformutils-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:12:54.532052 mlplatformutils-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 21:12:54.574274 mlplatformutils-0.3/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.3/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:12:54.769823 mlplatformutils-0.3/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.3/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.3/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.3/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3583 2023-06-04 21:11:12.000000 mlplatformutils-0.3/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.3/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.3/src/mlplatformutils/core/sparkutils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:12:54.639269 mlplatformutils-0.3/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3441 2023-06-04 21:12:54.000000 mlplatformutils-0.3/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-04 21:12:54.000000 mlplatformutils-0.3/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:12:54.000000 mlplatformutils-0.3/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 21:12:54.000000 mlplatformutils-0.3/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 21:12:54.000000 mlplatformutils-0.3/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.2/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.3/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.2/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.3/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.2/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.3/src/mlplatformutils/core/pandasutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,8 @@
 import json
-from deltalake import DeltaTable
-from adlfs import AzureBlobFileSystem
-from azure.identity import ClientSecretCredential
-import pyarrow.fs
-import pyarrowfs_adlgen2
-import pandas as pd
-
 def get_max_properties_starting_with(id, prefix,LineageLogger):
 
     document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
@@ -24,14 +17,18 @@
                               SOURCE_READ_SPN_VALUE,\
                               SOURCE_READ_SPNKEY_VALUE,\
                               tenant_id,\
                               AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH,\
                               RUN_ID,\
                               PIPELINE_STEP_NAME,\
                               LineageLogger):
+    
+    from deltalake import DeltaTable
+    from adlfs import AzureBlobFileSystem
+
     fs = AzureBlobFileSystem(
         account_name=SOURCE_STORAGE_ACCOUNT_VALUE,\
         client_id=SOURCE_READ_SPN_VALUE,\
         client_secret=SOURCE_READ_SPNKEY_VALUE,\
         tenant_id=tenant_id
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
@@ -47,14 +44,19 @@
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
                                 RUN_ID,\
                                 PIPELINE_STEP_NAME,\
                                 LineageLogger):
+    
+    from azure.identity import ClientSecretCredential
+    import pyarrow.fs
+    import pyarrowfs_adlgen2
+    import pandas as pd
 
     credential = ClientSecretCredential(
     tenant_id=tenant_id,
     client_id=SOURCE_READ_SPN_VALUE,
     client_secret=SOURCE_READ_SPNKEY_VALUE)
     
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
```

### Comparing `mlplatformutils-0.2/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.3/src/mlplatformutils/core/platformutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,7 +74,16 @@
                 subprocess.check_call(["pip", "install", pkg])
                 print(f"Successfully installed {pkg}!")
             else:
                 print(f"{pkg} is already installed.")
         except subprocess.CalledProcessError:
             print(f"Failed to install {pkg}.")
     return
+
+def upgrade_pip(package_name):
+    for pkg in package_name:
+        try:
+            subprocess.check_call(["pip", "install","--upgrade", pkg])
+            print(f"Successfully upgraded and installed {pkg}!")
+        except subprocess.CalledProcessError:
+            print(f"Failed to install {pkg}.")
+    return
```

### Comparing `mlplatformutils-0.2/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.3/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.2/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.3/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

