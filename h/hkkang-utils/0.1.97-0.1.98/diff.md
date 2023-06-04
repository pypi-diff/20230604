# Comparing `tmp/hkkang_utils-0.1.97.tar.gz` & `tmp/hkkang_utils-0.1.98.tar.gz`

## Comparing `hkkang_utils-0.1.97.tar` & `hkkang_utils-0.1.98.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/.vscode/settings.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/docs/make.bat
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/docs/source/conf.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/docs/source/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_concurrent.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_misc.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_string.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_testing.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_tensor/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_tensor/test_tensor.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/tests/test_tensor/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/pyproject.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.97/PKG-INFO
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/source/conf.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/docs/source/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_string.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_testing.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_tensor/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_tensor/test_tensor.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/tests/test_tensor/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/pyproject.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.98/PKG-INFO
```

### Comparing `hkkang_utils-0.1.97/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.1.98/.github/workflows/deploy_doc.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/.github/workflows/unittest.yml` & `hkkang_utils-0.1.98/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/docs/Makefile` & `hkkang_utils-0.1.98/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/docs/make.bat` & `hkkang_utils-0.1.98/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/docs/source/conf.py` & `hkkang_utils-0.1.98/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/__init__.py` & `hkkang_utils-0.1.98/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.1.98/src/hkkang_utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/file.py` & `hkkang_utils-0.1.98/src/hkkang_utils/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,52 +73,60 @@
     file_path_of_caller = inspect.stack()[1].filename
     dir_path_of_caller = os.path.dirname(file_path_of_caller)
     full_path = os.path.join(dir_path_of_caller, relative_path)
     return os.path.normpath(full_path)
 
 
 # Related to json files
-def read_json_file(file_path: str, auto_detect_extension: bool = False) -> Dict:
+def read_json_file(
+    file_path: str,
+    auto_detect_extension: bool = False,
+    encoding: Optional[str] = None,
+) -> Dict:
     """Read a json file
 
     :param file_path: json file path
     :type file_path: str
     :return: json data
     :rtype: dict
     """
     if auto_detect_extension and file_path.endswith(".jsonl"):
-        return read_jsonl_file(file_path)
+        return read_jsonl_file(file_path, encoding=encoding)
     else:
-        with open(file_path, "r") as f:
+        with open(file_path, "r", encoding=encoding) as f:
             return ujson.load(f)
 
 
-def read_jsonl_file(file_path: str) -> Dict:
-    with open(file_path, "r") as f:
+def read_jsonl_file(file_path: str, encoding: Optional[str] = None) -> Dict:
+    with open(file_path, "r", encoding=encoding) as f:
         return [ujson.loads(line) for line in f.readlines()]
 
 
 def write_json_file(
     dict_object: Dict,
     file_path: str,
     indent: int = 4,
     auto_detect_extension: bool = False,
+    encoding: Optional[str] = None,
 ) -> None:
     if auto_detect_extension and file_path.endswith(".jsonl"):
-        return write_jsonl_file(file_path)
+        return write_jsonl_file(
+            dict_object=dict_object, file_path=file_path, encoding=encoding
+        )
     else:
-        with open(file_path, "w") as f:
+        with open(file_path, "w", encoding=encoding) as f:
             ujson.dump(dict_object, f, indent=indent)
 
 
 def write_jsonl_file(
     dict_object: Dict,
     file_path: str,
+    encoding: Optional[str] = None,
 ):
-    with open(file_path, "w") as f:
+    with open(file_path, "w", encoding=encoding) as f:
         for line in dict_object:
             f.write(f"{ujson.dumps(line)}\n")
 
 
 # Related to yaml files
 def read_yaml_file(file_path: str) -> Dict:
     """Read a yaml file
```

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/list.py` & `hkkang_utils-0.1.98/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/metrics.py` & `hkkang_utils-0.1.98/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/misc.py` & `hkkang_utils-0.1.98/src/hkkang_utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/ml.py` & `hkkang_utils-0.1.98/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/pattern.py` & `hkkang_utils-0.1.98/src/hkkang_utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/pg.py` & `hkkang_utils-0.1.98/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/slack.py` & `hkkang_utils-0.1.98/src/hkkang_utils/slack.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.98/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/string.py` & `hkkang_utils-0.1.98/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.98/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/src/hkkang_utils/time.py` & `hkkang_utils-0.1.98/src/hkkang_utils/time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_concurrent.py` & `hkkang_utils-0.1.98/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_file.py` & `hkkang_utils-0.1.98/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_io.py` & `hkkang_utils-0.1.98/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_list.py` & `hkkang_utils-0.1.98/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_metrics.py` & `hkkang_utils-0.1.98/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_misc.py` & `hkkang_utils-0.1.98/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_pattern.py` & `hkkang_utils-0.1.98/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_string.py` & `hkkang_utils-0.1.98/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_testing.py` & `hkkang_utils-0.1.98/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_time.py` & `hkkang_utils-0.1.98/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_tensor/test_tensor.py` & `hkkang_utils-0.1.98/tests/test_tensor/test_tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/tests/test_tensor/utils.py` & `hkkang_utils-0.1.98/tests/test_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/.gitignore` & `hkkang_utils-0.1.98/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/LICENSE` & `hkkang_utils-0.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.97/pyproject.toml` & `hkkang_utils-0.1.98/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.97"
+version = "0.1.98"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.97/PKG-INFO` & `hkkang_utils-0.1.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.97
+Version: 0.1.98
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

