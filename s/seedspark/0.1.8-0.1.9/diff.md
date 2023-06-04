# Comparing `tmp/seedspark-0.1.8.tar.gz` & `tmp/seedspark-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedspark-0.1.8.tar", max compression
+gzip compressed data, was "seedspark-0.1.9.tar", max compression
```

## Comparing `seedspark-0.1.8.tar` & `seedspark-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     2621 2022-03-15 11:53:17.875443 seedspark-0.1.8/README.md
--rw-r--r--   0        0        0     3844 2022-03-15 15:34:42.556564 seedspark-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       46 2022-03-09 19:30:08.417780 seedspark-0.1.8/seedspark/__init__.py
--rw-r--r--   0        0        0       93 2022-03-09 19:56:17.611401 seedspark-0.1.8/seedspark/configs/__init__.py
--rw-r--r--   0        0        0     1173 2022-03-09 19:56:17.612094 seedspark-0.1.8/seedspark/configs/configs.py
--rw-r--r--   0        0        0      118 2022-03-09 19:59:04.777353 seedspark-0.1.8/seedspark/contrib/__init__.py
--rw-r--r--   0        0        0      212 2022-03-09 19:56:17.627892 seedspark-0.1.8/seedspark/contrib/test/__init__.py
--rw-r--r--   0        0        0     3361 2022-03-09 19:56:17.628283 seedspark-0.1.8/seedspark/contrib/test/base_airflow_test.py
--rw-r--r--   0        0        0     6639 2022-03-09 19:56:17.628663 seedspark-0.1.8/seedspark/contrib/test/base_spark_test.py
--rw-r--r--   0        0        0      110 2022-03-09 19:56:17.638675 seedspark-0.1.8/seedspark/dataquality/__init__.py
--rw-r--r--   0        0        0     1145 2022-03-09 19:56:17.638958 seedspark-0.1.8/seedspark/dataquality/ge.py
--rw-r--r--   0        0        0        0 2022-03-09 19:56:17.639246 seedspark-0.1.8/seedspark/dataquality/service.py
--rw-r--r--   0        0        0      215 2022-03-09 19:56:17.654600 seedspark-0.1.8/seedspark/spark/__init__.py
--rw-r--r--   0        0        0        0 2022-03-09 19:56:17.654927 seedspark-0.1.8/seedspark/spark/dataframe/__init__.py
--rw-r--r--   0        0        0        0 2022-03-09 19:56:17.655297 seedspark-0.1.8/seedspark/spark/dataframe/compare/__init__.py
--rw-r--r--   0        0        0    17096 2022-03-09 20:05:21.798404 seedspark-0.1.8/seedspark/spark/dataframe/compare/df_compare.py
--rw-r--r--   0        0        0     9456 2022-03-09 19:56:17.655912 seedspark-0.1.8/seedspark/spark/dataframe/compare/schema_comparer.py
--rw-r--r--   0        0        0     2351 2022-03-09 19:56:17.656256 seedspark-0.1.8/seedspark/spark/dataframe/utils.py
--rw-r--r--   0        0        0     7817 2022-03-09 19:56:17.656514 seedspark-0.1.8/seedspark/spark/sparkapp.py
--rw-r--r--   0        0        0      100 2022-03-09 19:56:17.665124 seedspark-0.1.8/seedspark/utils/__init__.py
--rw-r--r--   0        0        0     2989 2022-03-09 19:56:17.665383 seedspark-0.1.8/seedspark/utils/_datetime.py
--rw-r--r--   0        0        0     1719 2022-03-09 19:56:17.665642 seedspark-0.1.8/seedspark/utils/json.py
--rw-r--r--   0        0        0     3689 2022-03-15 15:34:45.440925 seedspark-0.1.8/setup.py
--rw-r--r--   0        0        0     4125 2022-03-15 15:34:45.441344 seedspark-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2621 2023-06-04 17:57:38.018059 seedspark-0.1.9/README.MD
+-rw-r--r--   0        0        0     3941 2023-06-04 17:59:22.668079 seedspark-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/__init__.py
+-rw-r--r--   0        0        0       93 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/configs/__init__.py
+-rw-r--r--   0        0        0     1173 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/configs/configs.py
+-rw-r--r--   0        0        0      118 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/test/__init__.py
+-rw-r--r--   0        0        0     3361 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/test/base_airflow_test.py
+-rw-r--r--   0        0        0     6639 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/test/base_spark_test.py
+-rw-r--r--   0        0        0      110 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/dataquality/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/dataquality/ge.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/dataquality/service.py
+-rw-r--r--   0        0        0      215 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/spark/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/spark/dataframe/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/compare/__init__.py
+-rw-r--r--   0        0        0    17049 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/compare/df_compare.py
+-rw-r--r--   0        0        0     9456 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/compare/schema_comparer.py
+-rw-r--r--   0        0        0     2338 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/utils.py
+-rw-r--r--   0        0        0     7924 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/sparkapp.py
+-rw-r--r--   0        0        0      100 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/utils/__init__.py
+-rw-r--r--   0        0        0     2989 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/utils/_datetime.py
+-rw-r--r--   0        0        0     1719 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/utils/json.py
+-rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 seedspark-0.1.9/PKG-INFO
```

### Comparing `seedspark-0.1.8/README.md` & `seedspark-0.1.9/README.MD`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/pyproject.toml` & `seedspark-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "seedspark"
-version = "0.1.8"
+version = "0.1.9"
 description = "SeedSpark is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments"
 authors = ["ChethanUK <chethanuk@outlook.com>"]
 maintainers = ["ChethanUK <chethanuk@outlook.com>"]
 license = "Apache-2.0"
-readme = "README.md"
+readme = "README.MD"
 homepage = "https://github.com/ChethanUK/"
 repository = "https://github.com/ChethanUK/seedspark"
 documentation = "https://github.com/ChethanUK/seedspark#readme"
 keywords = [
     "PySpark",
     "data-ops",
     "data-engineering",
@@ -29,54 +29,57 @@
     "Programming Language :: Python :: 3",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Testing"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
-pyspark = { version = ">=2.4.0, <=3.1.2", extras = ["sql"], optional = true }
+python = ">=3.8,<4.0"
+pyspark = { version = ">=2.4.7", extras = ["sql"], optional = true }
 pyarrow = { version = ">=2.0.0", optional = true }  # "^4.0.1"
-lognub = "^0.1.4"
+lognub = "^0.1.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.2"
-mypy = "^0.812"
-black = "^20.8b1"
-flake8 = "^3.9.0"
-pre-commit = "^2.12.0"
-testcontainers = "^3.4.0"
-pytest-docker-tools = "^1.0.3"
-pytest-timeout = "^1.4.2"
 pytest-lazy-fixture = "^0.6.3"
 pytest-ordering = "^0.6"
-pytest-mock = "^3.5.1"
 pytest-tldr = "^0.2.4"
 pytest-picked = "^0.4.6"
 pytest-instafail = "^0.4.2"
 pytest-deadfixtures = "^2.2.1"
 pytest-helpers-namespace = "^2021.3.24"
 pytest-icdiff = "^0.5"
 pytest-runner = "^5.3.0"
 pytest-xdist = "^2.2.1"
 pytest-rerunfailures = "^10.0"
 flake8-docstrings = "^1.6.0"
-pytest-flake8 = "^1.0.7"
 hypothesis = "^6.9.1"
 pydantic = "^1.8.1"
-great-expectations = "^0.13.19"
 #pydeequ3 = { file = "/Users/chethanuk/Work/Github/deequ/pydeequ3/dist/pydeequ3-0.1.7-py3-none-any.whl" }
 pydeequ3 = "^0.1.8"
 flaky = "^3.7.0"
-coverage = "^5.5"
+flake8 = "5"
+pre-commit = "^2.21.0"
+great-expectations = "^0.15.44"
+pytest-docker-tools = "^3.1.3"
+testcontainers = "^3.7.1"
+black = "^22.12.0"
+mypy = "^0.991"
+pytest-flake8 = "^1.1.1"
+pytest-timeout = "^2.1.0"
+pytest = "^7.2.1"
+coverage = "^7.0.5"
+pytest-mock = "^3.10.0"
+lognub = "^0.1.4"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 ## Black
```

### Comparing `seedspark-0.1.8/seedspark/configs/configs.py` & `seedspark-0.1.9/seedspark/configs/configs.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/seedspark/contrib/test/base_airflow_test.py` & `seedspark-0.1.9/seedspark/contrib/test/base_airflow_test.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/seedspark/contrib/test/base_spark_test.py` & `seedspark-0.1.9/seedspark/contrib/test/base_spark_test.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/seedspark/dataquality/ge.py` & `seedspark-0.1.9/seedspark/dataquality/ge.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/seedspark/spark/dataframe/compare/df_compare.py` & `seedspark-0.1.9/seedspark/spark/dataframe/compare/df_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,20 +126,17 @@
             compare_path=compare_sh_path,
             message="Columns not matched",
             additional_info=additional_info,
             func_path_modifier=func_path_modifier,
         )
 
     # compare the types
-    result_columns: List[Tuple[str, str]] = list(
-        map(lambda t: (t.name, t.dataType.typeName()), result_df.schema)
-    )
-    expected_columns: List[Tuple[str, str]] = list(
-        map(lambda t: (t.name, t.dataType.typeName()), expected_df.schema)
-    )
+    result_columns: List[Tuple[str, str]] = [(t.name, t.dataType.typeName()) for t in result_df.schema]
+    expected_columns: List[Tuple[str, str]] = [(t.name, t.dataType.typeName()) for t in expected_df.schema]
+
     number_of_mismatched_columns: int = 0
     mismatched_column_errors: List[str] = []
     for i in range(0, len(result_columns)):
         result_column = result_columns[i]
         expected_column = expected_columns[i]
         if result_column != expected_column:
             mismatched_column_errors.append(
@@ -297,15 +294,15 @@
         if result_value is None and expected_value is None:
             return error_count, []
         if result_value is None or expected_value is None:
             return error_count + 1, [
                 f"Expected array in row:{row_num}, col:{column_num} to be {expected_value} "
                 f"but actual is {result_value}"
             ]
-        array_item: Row
+        # array_item: Row
         for array_item_index in range(0, len(result_value)):
             element_type: StructField = data_type_for_column.elementType
             result_array_item = result_value[array_item_index]
             if len(expected_value) < array_item_index + 1:
                 return error_count + 1, [
                     f"Expected row:{row_num}, col:{column_num} has only {len(expected_value)} "
                     f"items but Actual has > {array_item_index + 1}"
```

### Comparing `seedspark-0.1.8/seedspark/spark/dataframe/compare/schema_comparer.py` & `seedspark-0.1.9/seedspark/spark/dataframe/compare/schema_comparer.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/seedspark/spark/dataframe/utils.py` & `seedspark-0.1.9/seedspark/spark/dataframe/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,20 +41,18 @@
                     f"posexplode_outer({field_name}) as ({field_name}_pos, {field_name})"
                 ]
                 array_df = nested_df.selectExpr(*field_names_and_explode)
                 return DataFrameUtils.flatten_data_frame(array_df)
 
             elif isinstance(field_data_type, StructType):
                 child_fieldnames = field_data_type.names
-                struct_field_names = list(
-                    map(lambda childname: f"{field_name}.{childname}", child_fieldnames)
-                )
+                struct_field_names = [f"{field_name}.{childname}" for childname in child_fieldnames]
                 new_field_names = (
                     list(filter(lambda col_name: col_name != field_name, field_names)) + struct_field_names
                 )
-                renamed_cols = map(lambda x: x.replace(".", "_"), new_field_names)
-                zip_alias_col_names = zip(new_field_names, renamed_cols)
-                alias_col_names = map(lambda y: col(y[0]).alias(y[1]), zip_alias_col_names)
+                renamed_cols = map(lambda x: x.replace(".", "_"), new_field_names)  # noqa: C417
+                zip_alias_col_names = zip(new_field_names, renamed_cols)  # noqa: B905
+                alias_col_names = map(lambda y: col(y[0]).alias(y[1]), zip_alias_col_names)  # noqa
                 struct_df = nested_df.select(*alias_col_names)
                 return DataFrameUtils.flatten_data_frame(struct_df)
 
         return nested_df
```

### Comparing `seedspark-0.1.8/seedspark/spark/sparkapp.py` & `seedspark-0.1.9/seedspark/spark/sparkapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,24 @@
         """
         quiet_py4j Reuce the spark py4j log level
         Check more at
         spark.apache.org/docs/latest/api/python/reference/api/pyspark.SparkContext.setLogLevel.html
         """
         import logging
 
-        if level is not None and level is ["ALL", "DEBUG", "ERROR", "FATAL", "INFO", "OFF", "TRACE", "WARN"]:
+        if level is not None and level is [
+            "ALL",
+            "DEBUG",
+            "ERROR",
+            "FATAL",
+            "INFO",
+            "OFF",
+            "TRACE",
+            "WARN",
+        ]:
             sc.setLogLevel(level)
         else:
             log.info(f"Error, Wrong Py4j Log level: {level} is passed")
         log4j = logging.getLogger("py4j")
         log4j.setLevel(logging.ERROR)
         logger = sc._jvm.org.apache.log4j  # pylint: disable=W0212
         logger.LogManager.getLogger("offer").setLevel(logger.Level.DEBUG)
```

### Comparing `seedspark-0.1.8/seedspark/utils/_datetime.py` & `seedspark-0.1.9/seedspark/utils/_datetime.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/seedspark/utils/json.py` & `seedspark-0.1.9/seedspark/utils/json.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.8/PKG-INFO` & `seedspark-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: seedspark
-Version: 0.1.8
+Version: 0.1.9
 Summary: SeedSpark is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments
 Home-page: https://github.com/ChethanUK/
 License: Apache-2.0
 Keywords: PySpark,data-ops,data-engineering,data-quality,data-profiling,dataquality,dataunittest,data-unit-tests,data-profilers,data-engineer,best-practices,big-data
 Author: ChethanUK
 Author-email: chethanuk@outlook.com
 Maintainer: ChethanUK
 Maintainer-email: chethanuk@outlook.com
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: lognub (>=0.1.4,<0.2.0)
+Requires-Dist: lognub (>=0.1.3,<0.2.0)
 Requires-Dist: pyarrow (>=2.0.0)
-Requires-Dist: pyspark[sql] (>=2.4.0,<=3.1.2)
+Requires-Dist: pyspark[sql] (>=2.4.7)
 Project-URL: Documentation, https://github.com/ChethanUK/seedspark#readme
 Project-URL: Repository, https://github.com/ChethanUK/seedspark
-Description-Content-Type: text/markdown
+Description-Content-Type: text/plain
 
 # SeedSpark
 
 **SeedSpark** is an open-source is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments or to perform end to end tests. The goal is to enable rapid development of Spark pipelines via PySpark on Spark clusters and locally test the pipeline by using various utilities.
 
 ## TODO
```

