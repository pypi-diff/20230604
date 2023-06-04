# Comparing `tmp/vegafusion-1.3.0rc3.tar.gz` & `tmp/vegafusion-1.3.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegafusion-1.3.0rc3.tar", last modified: Tue May 23 21:55:31 2023, max compression
+gzip compressed data, was "vegafusion-1.3.0rc4.tar", last modified: Tue May 30 22:42:34 2023, max compression
```

## Comparing `vegafusion-1.3.0rc3.tar` & `vegafusion-1.3.0rc4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.041258 vegafusion-1.3.0rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_conext_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_input_utc.py
--rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_pretransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_pretransform_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_row_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_transformed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/vegafusion/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/compilers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/vegafusion/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/connection/duckdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/local_tz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-23 21:54:18.000000 vegafusion-1.3.0rc3/vegafusion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:55:31.045259 vegafusion-1.3.0rc3/vegafusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 21:55:31.000000 vegafusion-1.3.0rc3/vegafusion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.369663 vegafusion-1.3.0rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_conext_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18632 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_input_utc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38103 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_pretransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_pretransform_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_row_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13990 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_transformed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.369663 vegafusion-1.3.0rc4/vegafusion/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/compilers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/vegafusion/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/connection/duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/local_tz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-30 22:41:13.000000 vegafusion-1.3.0rc4/vegafusion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:42:34.373663 vegafusion-1.3.0rc4/vegafusion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 22:42:34.000000 vegafusion-1.3.0rc4/vegafusion.egg-info/top_level.txt
```

### Comparing `vegafusion-1.3.0rc3/LICENSE.txt` & `vegafusion-1.3.0rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/PKG-INFO` & `vegafusion-1.3.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.3.0rc3
+Version: 1.3.0rc4
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.3.0rc3/README.md` & `vegafusion-1.3.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/setup.cfg` & `vegafusion-1.3.0rc4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = vegafusion
 description = Core tools for using VegaFusion from Python
-version = 1.3.0-rc3
+version = 1.3.0-rc4
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = vega, altair, vegafusion, arrow
 license = BSD-3-Clause
 license_file = LICENSE.txt
 python = "^3.7"
 homepage = "https://vegafusion.io"
@@ -30,14 +30,14 @@
 	altair>=4.2.0
 	pyarrow>=5
 	pandas
 	psutil
 
 [options.extras_require]
 embed = 
-	vegafusion-python-embed==1.3.0-rc3
+	vegafusion-python-embed==1.3.0-rc4
 	vl-convert-python>=0.7.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vegafusion-1.3.0rc3/tests/test_conext_manager.py` & `vegafusion-1.3.0rc4/tests/test_conext_manager.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/tests/test_input_utc.py` & `vegafusion-1.3.0rc4/tests/test_input_utc.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/tests/test_pretransform.py` & `vegafusion-1.3.0rc4/tests/test_pretransform.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/tests/test_pretransform_specs.py` & `vegafusion-1.3.0rc4/tests/test_pretransform_specs.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/tests/test_row_limit.py` & `vegafusion-1.3.0rc4/tests/test_row_limit.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/tests/test_save.py` & `vegafusion-1.3.0rc4/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/tests/test_transformed_data.py` & `vegafusion-1.3.0rc4/tests/test_transformed_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
     # Check that the expected columns are present
     assert set(expected_cols).issubset(set(df.columns))
 
     # Check that datetime columns have local timezone
     for dtype in df.dtypes.values:
         if dtype.kind == "M":
-            assert dtype.tz == pytz.timezone(vf.get_local_tz())
+            assert str(dtype.tz) == vf.get_local_tz()
 
     # Check expected length
     assert len(df) == expected_len
 
 
 @pytest.mark.parametrize(
     "mock_name,expected_lens,all_expected_cols", [
@@ -189,15 +189,15 @@
 
         # Check that the expected columns are present
         assert set(expected_cols).issubset(set(df.columns))
 
         # Check that datetime columns have local timezone
         for dtype in df.dtypes.values:
             if dtype.kind == "M":
-                assert dtype.tz == pytz.timezone(vf.get_local_tz())
+                assert str(dtype.tz) == vf.get_local_tz()
 
         # Check expected length
         assert len(df) == expected_len
 
 
 def test_transformed_data_exclude():
     source = data.wheat()
```

### Comparing `vegafusion-1.3.0rc3/tests/test_transformer.py` & `vegafusion-1.3.0rc4/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/__init__.py` & `vegafusion-1.3.0rc4/vegafusion/__init__.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/compilers.py` & `vegafusion-1.3.0rc4/vegafusion/compilers.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/connection/__init__.py` & `vegafusion-1.3.0rc4/vegafusion/connection/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,24 @@
         :param name: Table name
         :param path: Path to parquet file
         :param temporary: Whether table is considered temporary,
             and should be removed by unregister_temporary_tables
         """
         raise ValueError("Connection does not support registration of parquet datasets")
 
+    def register_arrow_file(self, name: str, path: str, temporary: bool = False):
+        """
+        Register the Arrow file at the provided path as a table with the provided name
+        :param name: Table name
+        :param path: Path to arrow file (aka feather file)
+        :param temporary: Whether table is considered temporary,
+            and should be removed by unregister_temporary_tables
+        """
+        raise ValueError("Connection does not support registration of arrow file datasets")
+
     def unregister(self, name: str):
         """
         Unregister a table (temporary or otherwise) by name
         :param name: Table name
         """
         raise ValueError("Connection does not support unregistration")
```

### Comparing `vegafusion-1.3.0rc3/vegafusion/connection/duckdb.py` & `vegafusion-1.3.0rc4/vegafusion/connection/duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from . import SqlConnection, CsvReadOptions
 
 from typing import Dict, Optional
 from distutils.version import LooseVersion
 
 import duckdb
 import pyarrow as pa
+import pyarrow.feather
 import pandas as pd
 import logging
 import uuid
 
 # Table suffix name to use for raw registered table
 RAW_PREFIX = "_vf_raw_"
 
 
 def duckdb_type_name_to_pyarrow_type(duckdb_type: str) -> pa.DataType:
-    if duckdb_type in ("VARCHAR", "JSON", "CHAR"):
+    duckdb_type = str(duckdb_type).upper()
+    if duckdb_type in ("VARCHAR", "JSON", "CHAR", "CATEGORICAL"):
         return pa.string()
     elif duckdb_type in ("REAL", "FLOAT4", "FLOAT"):
         return pa.float32()
     elif duckdb_type in ("DOUBLE", "FLOAT8"):
         return pa.float64()
     elif duckdb_type in ("TINYINT", "INT1"):
         return pa.int8()
@@ -184,15 +186,15 @@
         for col, type_name in zip(rel.columns, rel.dtypes):
             quoted_col_name = quote_column(col)
             try:
                 duckdb_type_name_to_pyarrow_type(type_name)
                 # Skip columns with supported types
             except ValueError:
                 # Convert unsupported types to strings (except struct)
-                if not type_name.startswith("STRUCT"):
+                if not str(type_name).startswith("STRUCT"):
                     replaces.append(f"{quoted_col_name}::varchar as {quoted_col_name}")
 
         if replaces:
             replace_csv = ", ".join(replaces)
             return f"SELECT * REPLACE({replace_csv}) FROM {table_name}"
         else:
             return f"SELECT * FROM {table_name}"
@@ -316,14 +318,18 @@
         # then convert unsupported columns and register result as name
         replace_query = self._replace_query_for_table(raw_name)
         self.conn.query(replace_query).to_view(name)
 
         self._update_temp_names(name, temporary)
         self._registered_table_schemas[name] = self._schema_for_table(name)
 
+    def register_arrow_file(self, name: str, path: str, temporary: bool = False):
+        arrow_table = pa.feather.read_table(path)
+        self.register_arrow(name, arrow_table, temporary)
+
     def unregister(self, name: str):
         for view_name in [name, RAW_PREFIX + name]:
             self.conn.unregister(view_name)
             if view_name in self._temp_tables:
                 self._temp_tables.remove(view_name)
             self._registered_table_schemas.pop(view_name, None)
```

### Comparing `vegafusion-1.3.0rc3/vegafusion/evaluation.py` & `vegafusion-1.3.0rc4/vegafusion/evaluation.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/local_tz.py` & `vegafusion-1.3.0rc4/vegafusion/local_tz.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/renderer.py` & `vegafusion-1.3.0rc4/vegafusion/renderer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/runtime.py` & `vegafusion-1.3.0rc4/vegafusion/runtime.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/save.py` & `vegafusion-1.3.0rc4/vegafusion/save.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/transformer.py` & `vegafusion-1.3.0rc4/vegafusion/transformer.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion/utils.py` & `vegafusion-1.3.0rc4/vegafusion/utils.py`

 * *Files identical despite different names*

### Comparing `vegafusion-1.3.0rc3/vegafusion.egg-info/PKG-INFO` & `vegafusion-1.3.0rc4/vegafusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegafusion
-Version: 1.3.0rc3
+Version: 1.3.0rc4
 Summary: Core tools for using VegaFusion from Python
 License: BSD-3-Clause
 Keywords: vega,altair,vegafusion,arrow
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vegafusion-1.3.0rc3/vegafusion.egg-info/SOURCES.txt` & `vegafusion-1.3.0rc4/vegafusion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

