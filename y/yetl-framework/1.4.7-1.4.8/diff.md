# Comparing `tmp/yetl-framework-1.4.7.tar.gz` & `tmp/yetl-framework-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.4.7.tar", last modified: Sat Jun  3 19:38:20 2023, max compression
+gzip compressed data, was "yetl-framework-1.4.8.tar", last modified: Sun Jun  4 04:43:06 2023, max compression
```

## Comparing `yetl-framework-1.4.7.tar` & `yetl-framework-1.4.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.949183 yetl-framework-1.4.7/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-03 19:38:20.949183 yetl-framework-1.4.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-03 19:38:20.949183 yetl-framework-1.4.7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.945183 yetl-framework-1.4.7/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.945183 yetl-framework-1.4.7/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.945183 yetl-framework-1.4.7/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.945183 yetl-framework-1.4.7/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.949183 yetl-framework-1.4.7/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.949183 yetl-framework-1.4.7/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2931 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-03 19:37:25.000000 yetl-framework-1.4.7/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-03 19:38:20.949183 yetl-framework-1.4.7/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-03 19:38:20.000000 yetl-framework-1.4.7/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-03 19:38:20.000000 yetl-framework-1.4.7/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-03 19:38:20.000000 yetl-framework-1.4.7/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-03 19:38:20.000000 yetl-framework-1.4.7/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-03 19:38:20.000000 yetl-framework-1.4.7/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-03 19:38:20.000000 yetl-framework-1.4.7/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.406257 yetl-framework-1.4.8/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-04 04:43:06.406257 yetl-framework-1.4.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-04 04:43:06.406257 yetl-framework-1.4.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.402257 yetl-framework-1.4.8/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.402257 yetl-framework-1.4.8/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.402257 yetl-framework-1.4.8/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16007 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.402257 yetl-framework-1.4.8/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16262 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.406257 yetl-framework-1.4.8/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3991 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.406257 yetl-framework-1.4.8/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-04 04:42:17.000000 yetl-framework-1.4.8/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-04 04:43:06.406257 yetl-framework-1.4.8/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-04 04:43:06.000000 yetl-framework-1.4.8/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-04 04:43:06.000000 yetl-framework-1.4.8/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-04 04:43:06.000000 yetl-framework-1.4.8/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-04 04:43:06.000000 yetl-framework-1.4.8/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-04 04:43:06.000000 yetl-framework-1.4.8/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-04 04:43:06.000000 yetl-framework-1.4.8/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.4.7/PKG-INFO` & `yetl-framework-1.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.7
+Version: 1.4.8
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.7/README.md` & `yetl-framework-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/setup.py` & `yetl-framework-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.4.7",
+    version="1.4.8",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.4.7/yetl/__main__.py` & `yetl-framework-1.4.8/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/cli/_init.py` & `yetl-framework-1.4.8/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.4.8/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/__init__.py` & `yetl-framework-1.4.8/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_config.py` & `yetl-framework-1.4.8/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_decorators.py` & `yetl-framework-1.4.8/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_logging_config.py` & `yetl-framework-1.4.8/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_project.py` & `yetl-framework-1.4.8/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_spark_context.py` & `yetl-framework-1.4.8/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_tables.py` & `yetl-framework-1.4.8/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_timeslice.py` & `yetl-framework-1.4.8/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/_utils.py` & `yetl-framework-1.4.8/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/deltalake.py` & `yetl-framework-1.4.8/yetl/config/deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,20 +206,15 @@
             predicates.append(p)
 
         predicate = " and ".join(predicates)
 
         return predicate
 
     def table_exists(self, database: str, table: str):
-        table_exists = (
-            self.spark.sql(f"SHOW TABLES in {database};")
-            .where(f"tableName='{table}' AND !isTemporary")
-            .count()
-            == 1
-        )
+        table_exists = self.spark.catalog.tableExists(f"`{database}`.`{table}`")
         return table_exists
 
     def get_delta_properties_sql(self, delta_properties: Dict[str, Union[str, bool]]):
         sql_properties = [
             f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
         ]
         sql_properties = ", ".join(sql_properties)
@@ -230,15 +225,14 @@
         database: str,
         table: str,
         path: str = None,
         delta_properties: List[str] = None,
         sql: str = None,
     ):
         _logger.debug(f"Creating table if not exists {database}.{table} at {path}")
-
         if not sql:
             sql = f"CREATE TABLE IF NOT EXISTS `{database}`.`{table}`"
 
             # add in the delta properties if there are any
             sql_properties = ""
             if delta_properties:
                 sql_properties = self.get_delta_properties_sql(delta_properties)
@@ -246,16 +240,15 @@
 
             sql_path = ""
             if path:
                 sql_path = f"USING DELTA LOCATION '{path}'"
 
                 sql = f"{sql}\n{sql_path}\n{sql_properties};"
 
-        _logger.debug(f"{sql}")
-        print(sql)
+        _logger.info(f"{sql}")
         self.spark.sql(sql)
 
         return sql
 
     def create_database(self, database: str):
         _logger.debug(f"Creating database if not exists `{database}`")
         sql = f"CREATE DATABASE IF NOT EXISTS {database}"
```

### Comparing `yetl-framework-1.4.7/yetl/config/table/_deltalake.py` & `yetl-framework-1.4.8/yetl/config/table/_deltalake.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 class DeltaLake(Table):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._spark = DeltaLakeFn(project=self.project)
         self._render()
+        self._spark.create_database(self.database)
 
     @classmethod
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
@@ -81,24 +82,26 @@
                     if isinstance(value, str):
                         self.options[option] = render_jinja(value, self._replacements)
 
         self._rendered = True
 
     # TODO: Create or alter table
     def create_table(self):
-        self._spark.create_database(self.database)
-
-        if self.managed:
-            self._spark.create_table(
-                database=self.database,
-                table=self.table,
-                delta_properties=self.delta_properties,
-                sql=self.sql,
-            )
+        if self._spark.table_exists(database=self.database, table=self.table):
+            pass
+            # TODO: alter table
         else:
-            self._spark.create_table(
-                database=self.database,
-                table=self.table,
-                delta_properties=self.delta_properties,
-                path=self.location,
-                sql=self.sql,
-            )
+            if self.managed:
+                self._spark.create_table(
+                    database=self.database,
+                    table=self.table,
+                    delta_properties=self.delta_properties,
+                    sql=self.sql,
+                )
+            else:
+                self._spark.create_table(
+                    database=self.database,
+                    table=self.table,
+                    delta_properties=self.delta_properties,
+                    path=self.location,
+                    sql=self.sql,
+                )
```

### Comparing `yetl-framework-1.4.7/yetl/config/table/_factory.py` & `yetl-framework-1.4.8/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/table/_read.py` & `yetl-framework-1.4.8/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/config/table/_table.py` & `yetl-framework-1.4.8/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.7/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.4.8/yetl/workflow/_multi_threaded.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,59 +2,48 @@
 from ._notebook import Notebook
 from typing import List
 
 
 # execute a notebook using databricks workflows
 def _execute_notebook(notebook: Notebook, dbutils):
     """Execute a notebookd using databricks workflows"""
-    job_id = (
-        dbutils.notebook.entry_point.getDbutils()
-        .notebook()
-        .getContext()
-        .jobId()
-        .toString()
-    )
     msg = {
-        "_message": f"Executing notebook {notebook.path} parameters {notebook.parameters} job_id {job_id}",
+        "_message": f"Executing notebook {notebook.path} parameters {notebook.parameters}",
         "status": "executing",
         "notebook": notebook.path,
-        "job_id": job_id,
     }
     print(msg["_message"], flush=True)
 
     try:
         result = dbutils.notebook.run(
             notebook.path, notebook.timeout, notebook.parameters
         )
         msg = {
-            "_message": f"Succeeded notebook {notebook.path} job_id {job_id}",
+            "_message": f"Succeeded notebook {notebook.path}",
             "status": "succeeded",
             "notebook": notebook.path,
-            "job_id": job_id,
         }
         print(msg["_message"], flush=True)
         return result
 
     except Exception as e:
         if notebook.retry < 1:
             msg = {
-                "_message": f"notebook {notebook.path}  job_id {job_id} failed.",
+                "_message": f"notebook {notebook.path} failed.",
                 "status": "failed",
                 "error": str(e),
                 "notebook": notebook.path,
-                "job_id": job_id,
             }
             print(msg["_message"], flush=True)
             raise Exception(msg["_message"])
 
         msg = {
-            "_message": f"Retrying notebook {notebook.path} job_id {job_id}",
+            "_message": f"Retrying notebook {notebook.path}",
             "status": "executing",
             "notebook": notebook.path,
-            "job_id": job_id,
         }
         print(msg["_message"], flush=True)
         notebook.retry -= 1
 
 
 def _try_future(future: Future, catch=False):
     return future.result()
```

### Comparing `yetl-framework-1.4.7/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.4.8/yetl_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.7
+Version: 1.4.8
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.7/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.4.8/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

