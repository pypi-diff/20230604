# Comparing `tmp/mlplatformutils-0.1.tar.gz` & `tmp/mlplatformutils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.1.tar", last modified: Sat Jun  3 21:13:53 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.2.tar", last modified: Sun Jun  4 02:06:17 2023, max compression
```

## Comparing `mlplatformutils-0.1.tar` & `mlplatformutils-0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 21:13:53.548273 mlplatformutils-0.1/
--rw-rw-rw-   0        0        0      242 2023-06-03 21:13:53.549275 mlplatformutils-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-06-03 21:03:57.000000 mlplatformutils-0.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-03 21:13:53.553276 mlplatformutils-0.1/setup.cfg
--rw-rw-rw-   0        0        0      440 2023-06-03 21:11:44.000000 mlplatformutils-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:13:53.328144 mlplatformutils-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 21:13:53.394203 mlplatformutils-0.1/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.1/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:13:53.535275 mlplatformutils-0.1/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.1/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.1/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.1/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3260 2023-06-03 20:48:56.000000 mlplatformutils-0.1/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     2823 2023-06-03 20:50:22.000000 mlplatformutils-0.1/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     6799 2023-06-03 20:47:25.000000 mlplatformutils-0.1/src/mlplatformutils/core/sparkutils.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:13:53.480733 mlplatformutils-0.1/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0      242 2023-06-03 21:13:53.000000 mlplatformutils-0.1/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-06-03 21:13:53.000000 mlplatformutils-0.1/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 21:13:53.000000 mlplatformutils-0.1/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-06-03 21:13:53.000000 mlplatformutils-0.1/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-03 21:13:53.000000 mlplatformutils-0.1/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.298859 mlplatformutils-0.2/
+-rw-rw-rw-   0        0        0      242 2023-06-04 02:06:17.299860 mlplatformutils-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-04 02:05:42.000000 mlplatformutils-0.2/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-04 02:06:17.308860 mlplatformutils-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      466 2023-06-04 02:05:51.000000 mlplatformutils-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.053238 mlplatformutils-0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.071267 mlplatformutils-0.2/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.2/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.293859 mlplatformutils-0.2/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.2/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.2/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     7150 2023-06-03 20:43:14.000000 mlplatformutils-0.2/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     3549 2023-06-04 01:58:38.000000 mlplatformutils-0.2/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     2815 2023-06-04 01:59:57.000000 mlplatformutils-0.2/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7035 2023-06-04 02:03:44.000000 mlplatformutils-0.2/src/mlplatformutils/core/sparkutils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 02:06:17.131775 mlplatformutils-0.2/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 02:06:16.000000 mlplatformutils-0.2/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.1/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.2/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.1/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.2/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.1/src/mlplatformutils/core/pandasutils.py` & `mlplatformutils-0.2/src/mlplatformutils/core/pandasutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 import json
-def get_max_properties_starting_with(id, prefix):
+from deltalake import DeltaTable
+from adlfs import AzureBlobFileSystem
+from azure.identity import ClientSecretCredential
+import pyarrow.fs
+import pyarrowfs_adlgen2
+import pandas as pd
+
+def get_max_properties_starting_with(id, prefix,LineageLogger):
+
     document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
@@ -14,15 +22,16 @@
 
 def read_from_delta_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                               SOURCE_READ_SPN_VALUE,\
                               SOURCE_READ_SPNKEY_VALUE,\
                               tenant_id,\
                               AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH,\
                               RUN_ID,\
-                              PIPELINE_STEP_NAME):
+                              PIPELINE_STEP_NAME,\
+                              LineageLogger):
     fs = AzureBlobFileSystem(
         account_name=SOURCE_STORAGE_ACCOUNT_VALUE,\
         client_id=SOURCE_READ_SPN_VALUE,\
         client_secret=SOURCE_READ_SPNKEY_VALUE,\
         tenant_id=tenant_id
     )
     pandas_df = DeltaTable(AML_STORAGE_EXPERIMENT_DELTA_ROOT_PATH, file_system=fs).to_pandas()
@@ -36,24 +45,24 @@
 
 def read_from_parquet_as_pandas(SOURCE_STORAGE_ACCOUNT_VALUE,\
                                 SOURCE_READ_SPN_VALUE,\
                                 SOURCE_READ_SPNKEY_VALUE,\
                                 tenant_id,\
                                 AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH,\
                                 RUN_ID,\
-                                PIPELINE_STEP_NAME):
+                                PIPELINE_STEP_NAME,\
+                                LineageLogger):
 
     credential = ClientSecretCredential(
     tenant_id=tenant_id,
     client_id=SOURCE_READ_SPN_VALUE,
     client_secret=SOURCE_READ_SPNKEY_VALUE)
     
     handler=pyarrowfs_adlgen2.AccountHandler.from_account_name(SOURCE_STORAGE_ACCOUNT_VALUE,credential=credential)
     fs = pyarrow.fs.PyFileSystem(handler)
-    
     pandas_df = pd.read_parquet(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH, filesystem=fs)
 
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
     LineageLogger.update_vertex(documentId, {"DataReadSource_"+sourcePostfix: str(AML_STORAGE_EXPERIMENT_PARQUET_ROOT_PATH),\
                                              "FileFormat_"+sourcePostfix:str("parquet"),\
                                              "DataReadSourceColumns_"+sourcePostfix:"["+",".join(pandas_df.columns.tolist())+"]"})
```

### Comparing `mlplatformutils-0.1/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.2/src/mlplatformutils/core/platformutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #Defining all Utility Functions
 import os
 import subprocess
 import configparser
+from azureml.core.compute import ComputeInstance
+from azureml.core.compute_target import ComputeTargetException
 
 def is_package_installed(package_name, package_version=None):
     try:
         output = subprocess.check_output(['pip', 'show', package_name])
         output = output.decode('utf-8')
         if package_version is None:
             return True
@@ -30,16 +32,14 @@
         print(f"Error: section '{section_name}' not found in setup.ini")
         return None
     except configparser.NoOptionError:
         print(f"Error: key '{key_name}' not found in section '{section_name}' in setup.ini")
         return None
 
 def assert_amlcompute(workspace, compute_name):
-    from azureml.core.compute import ComputeInstance
-    from azureml.core.compute_target import ComputeTargetException
     try:
         compute_instance = ComputeInstance(workspace=workspace, name=compute_name)
         print(f"Found existing compute instance: {compute_name}")
     except ComputeTargetException:
         print(f"Not Found compute instance: {compute_name}")
 
 def get_environment(env_yaml_file_path):
```

### Comparing `mlplatformutils-0.1/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.2/src/mlplatformutils/core/sparkutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-def get_max_properties_starting_with(id, prefix):
+def get_max_properties_starting_with(id, prefix,LineageLogger):
     document=LineageLogger.query_graph("g.V().hasLabel('amlrun').has('id', '"+id+"')")
     jsondump = json.dumps(document)
     jsonload = json.loads(jsondump)
     for item in jsonload:
         properties = item.get('properties')
     if properties:
         matching_props = [prop[-1] for prop in properties.keys() if prop.startswith(prefix)]
@@ -15,15 +15,16 @@
 def read_from_adls_gen2(SOURCE_STORAGE_ACCOUNT_VALUE,\
                         AZURE_TENANT_ID,\
                         file_path,\
                         file_format,\
                         SOURCE_READ_SPN_VALUE,\
                         SOURCE_READ_SPNKEY_VALUE,\
                         RUN_ID,\
-                        PIPELINE_STEP_NAME):
+                        PIPELINE_STEP_NAME,\
+                        LineageLogger):
 
     spark = SparkSession.builder.appName("Read from ADLS Gen2").getOrCreate()
     spark.conf.set("fs.azure.account.auth.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "OAuth")
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_READ_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
@@ -42,56 +43,58 @@
                        file_path,\
                        file_format,\
                        repartition,\
                        df,\
                        SOURCE_WRITE_SPN_VALUE,\
                        SOURCE_WRITE_SPNKEY_VALUE,\
                        RUN_ID,\
-                       PIPELINE_STEP_NAME):
+                       PIPELINE_STEP_NAME,\
+                       LineageLogger):
                        
     spark = SparkSession.builder.appName("Read from ADLS Gen2").getOrCreate()
     spark.conf.set("fs.azure.account.auth.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "OAuth")
     spark.conf.set("fs.azure.account.oauth.provider.type."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net",  "org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
     spark.conf.set("fs.azure.account.oauth2.client.id."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_WRITE_SPN_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.secret."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", SOURCE_WRITE_SPNKEY_VALUE)
     spark.conf.set("fs.azure.account.oauth2.client.endpoint."+SOURCE_STORAGE_ACCOUNT_VALUE+".dfs.core.windows.net", "https://login.microsoftonline.com/"+AZURE_TENANT_ID+"/oauth2/token")
+    
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     targetPostfix=get_max_properties_starting_with(documentId,"DataWriteColumns")
     LineageLogger.update_vertex(documentId, {"DataWriteTarget_"+targetPostfix: str(file_path),\
                                         "FileFormat_"+targetPostfix:file_format,\
                                         "DataWriteColumns_"+targetPostfix:"["+",".join(df.columns)+"]"})
-
-    df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
-
+    if repartition is None:
+        df.write.format(file_format).mode('overwrite').save(file_path)
+    else:
+        df.repartition(repartition).write.format(file_format).mode('overwrite').save(file_path)
     return
 
-def read_from_kusto(kustoOptions,RUN_ID,PIPELINE_STEP_NAME):
+def read_from_kusto(kustoOptions,RUN_ID,PIPELINE_STEP_NAME,LineageLogger):
     pyKusto = SparkSession.builder.appName("kustoPySpark").getOrCreate()
-
     kustoDf  = pyKusto.read. \
                 format("com.microsoft.kusto.spark.datasource"). \
                 option("kustoCluster", kustoOptions["kustoCluster"]). \
                 option("kustoDatabase", kustoOptions["kustoDatabase"]). \
                 option("kustoQuery", kustoOptions["kustoTable"]). \
                 option("kustoAadAppId", kustoOptions["kustoAADClientID"]). \
                 option("kustoAadAppSecret", kustoOptions["kustoClientAADClientPassword"]). \
                 option("kustoAadAuthorityID", kustoOptions["kustoAADAuthorityID"]). \
                 load()
+    
     documentId = LineageLogger.query_graph("g.V().hasLabel('amlrun').has('RUN_ID', '"+RUN_ID+"').has('PIPELINE_STEP_NAME', '"+PIPELINE_STEP_NAME+"').values('id')")[0]
     sourcePostfix=get_max_properties_starting_with(documentId,"DataReadSourceColumns")
     LineageLogger.update_vertex(documentId, {"KustoDataReadCluster_"+sourcePostfix: str(kustoOptions["kustoCluster"]),\
                                         "KustoDataReadDatabase_"+sourcePostfix: str(kustoOptions["kustoDatabase"]),\
                                         "KustoDataReadQuery_"+sourcePostfix: str(kustoOptions["kustoTable"]),\
                                         "DataReadSourceColumns_"+sourcePostfix:"["+",".join(kustoDf.columns)+"]"})                
     return kustoDf
 
-def read_from_azsql(SQL_SERVER_INSTANCE,access_token,Query,RUN_ID,PIPELINE_STEP_NAME):
+def read_from_azsql(SQL_SERVER_INSTANCE,access_token,Query,RUN_ID,PIPELINE_STEP_NAME,LineageLogger):
 
     pySql = SparkSession.builder.appName("AzSQLPySpark").getOrCreate()
-    
     df = pySql.read \
         .format("com.microsoft.sqlserver.jdbc.spark") \
         .option("url", SQL_SERVER_INSTANCE) \
         .option("query", Query) \
         .option("accessToken", access_token) \
         .option("encrypt", "true") \
         .option("hostNameInCertificate", "*.database.windows.net") \
```

### Comparing `mlplatformutils-0.1/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.2/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

