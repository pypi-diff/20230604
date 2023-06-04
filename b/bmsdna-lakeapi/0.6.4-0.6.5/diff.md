# Comparing `tmp/bmsdna_lakeapi-0.6.4.tar.gz` & `tmp/bmsdna_lakeapi-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.6.4.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.6.5.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.6.4.tar` & `bmsdna_lakeapi-0.6.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1081 2023-06-03 09:25:26.935517 bmsdna_lakeapi-0.6.4/LICENSE
--rw-r--r--   0        0        0     8929 2023-06-03 09:25:26.935517 bmsdna_lakeapi-0.6.4/README.md
--rw-r--r--   0        0        0      337 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1185 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      566 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     6595 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     9409 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6030 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11077 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12618 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15456 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6754 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1452 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6408 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4291 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3763 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3109 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2478 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     1998 2023-06-03 09:25:26.939517 bmsdna_lakeapi-0.6.4/pyproject.toml
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-03 15:00:14.685430 bmsdna_lakeapi-0.6.5/LICENSE
+-rw-r--r--   0        0        0     8929 2023-06-03 15:00:14.685430 bmsdna_lakeapi-0.6.5/README.md
+-rw-r--r--   0        0        0      337 2023-06-03 15:00:14.685430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:00:14.685430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-03 15:00:14.685430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      566 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     6595 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     9383 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6030 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11077 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12618 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15557 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6754 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1452 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6467 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4291 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3763 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3109 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2478 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     1998 2023-06-03 15:00:14.689430 bmsdna_lakeapi-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.6.5/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.6.4/LICENSE` & `bmsdna_lakeapi-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/README.md` & `bmsdna_lakeapi-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 import pypika.functions
 import pypika.enums
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 
-
 ENABLE_COPY_TO = os.environ.get("ENABLE_COPY_TO", "0") == "1"
-#ENABLE_COPY_TO = True
 
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
     ) -> None:
```

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,16 +280,15 @@
     ):  # type: ignore
         logger.info(f"{params.dict(exclude_unset=True) if params else None}Union[ ,  ]{request.url.path}")
 
         engine = engine or basic_config.default_engine
 
         logger.info(f"Engine: {engine}")
 
-
-        with  get_context_by_engine(engine) as context:
+        with get_context_by_engine(engine) as context:
             realdataframe = Dataframe(
                 config.version_str, config.tag, config.name, config.datasource, context, basic_config=basic_config
             )
             parts = await get_partitions(realdataframe, params, config)
             df = realdataframe.get_df(parts or None)
 
             expr = await get_params_filter_expr(df.columns(), config, params)
@@ -337,15 +336,14 @@
                 assert len(columns) <= 3  # reduce complexity here
                 new_query = new_query.distinct()
 
             if not (limit == -1 and config.allow_get_all_pages):
                 limit = 1000 if limit == -1 else limit
                 new_query = new_query.offset(offset or 0).limit(limit)
 
-
             if len(searches) > 0 and config.search is not None:
                 import pypika.queries
                 import pypika.terms
 
                 source_view = realdataframe.tablename
                 context.init_search(source_view, config.search)
                 score_sum = None
@@ -363,12 +361,17 @@
 
             logger.info(f"Query: {get_sql(new_query)}")
 
             df2 = context.execute_sql(new_query)
 
             try:
                 return await create_response(
-                    request.url, format or request.headers["Accept"], df2, context, basic_config=basic_config, close_context=True
+                    request.url,
+                    format or request.headers["Accept"],
+                    df2,
+                    context,
+                    basic_config=basic_config,
+                    close_context=True,
                 )
             except Exception as err:
                 logger.error("Error in creating response", exc_info=err)
                 raise HTTPException(status_code=500)
```

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
 class FileResponseWCharset(FileResponse):
     def __init__(self, *args, **kwargs):
         if "charset" in kwargs:
             self.charset = kwargs.pop("charset")
         super().__init__(*args, **kwargs)
 
 
-
 async def create_response(
     url: URL,
     accept: str,
     content: ResultData,
     context: ExecutionContext,
     basic_config: BasicConfig,
     close_context=False,
@@ -153,22 +152,26 @@
         OutputFormats.CSV,
         OutputFormats.SEMI_CSV,
         OutputFormats.CSV4EXCEL,
     ]:
         content_dispositiont_type = "inline"
         filename = None
 
-    temp_file = tempfile.NamedTemporaryFile(delete=False, suffix=extension)
+    temp_file = tempfile.NamedTemporaryFile(delete=True, suffix=extension)
     media_type = "text/csv" if extension == ".csv" else mimetypes.guess_type("file" + extension)[0]
-    additional_files = write_frame(url=url, content=content, format=format, out=temp_file.name, basic_config=basic_config)
+    additional_files = write_frame(
+        url=url, content=content, format=format, out=temp_file.name, basic_config=basic_config
+    )
 
     def clean_up():
         if close_context:
             context.close()
+            logger.debug("closed context")
         temp_file.close()
+
         for f in additional_files:
             os.remove(f)
 
     fr = FileResponseWCharset(
         path=temp_file.name,
         headers=headers,
         media_type=media_type,
```

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.6.5/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.6.4/pyproject.toml` & `bmsdna_lakeapi-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.6.4/PKG-INFO` & `bmsdna_lakeapi-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

