# Comparing `tmp/bmsdna_lakeapi-0.6.6.tar.gz` & `tmp/bmsdna_lakeapi-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.6.6.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.6.7.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.6.6.tar` & `bmsdna_lakeapi-0.6.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-04 11:03:20.729902 bmsdna_lakeapi-0.6.6/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-04 11:03:20.729902 bmsdna_lakeapi-0.6.6/README.md
--rw-r--r--   0        0        0      337 2023-06-04 11:03:20.729902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 11:03:20.729902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-04 11:03:20.729902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-04 11:03:20.729902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6595 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9383 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6030 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11077 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12618 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15557 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6754 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1452 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6470 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4291 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3763 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1998 2023-06-04 11:03:20.733902 bmsdna_lakeapi-0.6.6/pyproject.toml
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/README.md
+-rw-r--r--   0        0        0      337 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6595 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9383 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6030 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11077 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12618 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15559 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6754 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1452 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6470 2023-06-04 18:21:15.904085 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4291 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3763 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1998 2023-06-04 18:21:15.908086 bmsdna_lakeapi-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.7/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.6.6/LICENSE` & `bmsdna_lakeapi-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/README.md` & `bmsdna_lakeapi-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
                 columns = [c for c in columns if c in select.split(",")]
             if config.datasource.exclude and len(config.datasource.exclude) > 0:
                 columns = [c for c in columns if c not in config.datasource.exclude]
             if config.datasource.sortby and len(searches) == 0:
                 for s in config.datasource.sortby:
                     new_query = new_query.orderby(
                         s.by,
-                        ord=pypika.Order.desc if s.direction and s.direction.lower() == "desc" else pypika.Order.asc,
+                        order=pypika.Order.desc if s.direction and s.direction.lower() == "desc" else pypika.Order.asc,
                     )
             if has_complex and format in ["csv", "excel", "scsv", "csv4excel"]:
                 jsonify_complex = True
             if jsonify_complex:
                 new_query = new_query.select(
                     *[
                         pypika.Field(c)
```

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.6.7/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.6/pyproject.toml` & `bmsdna_lakeapi-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.6.6"
+version = "0.6.7"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.6.6/PKG-INFO` & `bmsdna_lakeapi-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.6.6
+Version: 0.6.7
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

