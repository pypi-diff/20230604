# Comparing `tmp/types-cffi-1.15.1.8.tar.gz` & `tmp/types-cffi-1.15.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-cffi-1.15.1.8.tar", last modified: Thu Mar 23 12:32:01 2023, max compression
+gzip compressed data, was "types-cffi-1.15.1.9.tar", last modified: Mon Mar 27 15:17:45 2023, max compression
```

## Comparing `types-cffi-1.15.1.8.tar` & `types-cffi-1.15.1.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:32:01.861726 types-cffi-1.15.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-23 12:32:00.000000 types-cffi-1.15.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 12:32:00.000000 types-cffi-1.15.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-23 12:32:01.861726 types-cffi-1.15.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:32:01.861726 types-cffi-1.15.1.8/_cffi_backend-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-23 12:32:00.000000 types-cffi-1.15.1.8/_cffi_backend-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-03-23 12:32:00.000000 types-cffi-1.15.1.8/_cffi_backend-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:32:01.861726 types-cffi-1.15.1.8/cffi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-23 12:32:00.000000 types-cffi-1.15.1.8/cffi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/backend_ctypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/cffi_opcode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/commontypes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/cparser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/ffiplatform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/pkgconfig.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/recompiler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/setuptools_ext.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/vengine_cpy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/vengine_gen.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-23 12:31:50.000000 types-cffi-1.15.1.8/cffi-stubs/verifier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 12:32:01.861726 types-cffi-1.15.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-23 12:32:00.000000 types-cffi-1.15.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 12:32:01.861726 types-cffi-1.15.1.8/types_cffi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-23 12:32:01.000000 types-cffi-1.15.1.8/types_cffi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-23 12:32:01.000000 types-cffi-1.15.1.8/types_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 12:32:01.000000 types-cffi-1.15.1.8/types_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-23 12:32:01.000000 types-cffi-1.15.1.8/types_cffi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:17:45.238616 types-cffi-1.15.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-27 15:17:42.000000 types-cffi-1.15.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 15:17:42.000000 types-cffi-1.15.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-27 15:17:45.238616 types-cffi-1.15.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:17:45.234616 types-cffi-1.15.1.9/_cffi_backend-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-27 15:17:42.000000 types-cffi-1.15.1.9/_cffi_backend-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-03-27 15:17:42.000000 types-cffi-1.15.1.9/_cffi_backend-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:17:45.238616 types-cffi-1.15.1.9/cffi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-27 15:17:42.000000 types-cffi-1.15.1.9/cffi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/backend_ctypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/cffi_opcode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/commontypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/cparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/ffiplatform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/pkgconfig.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/recompiler.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/setuptools_ext.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/vengine_cpy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/vengine_gen.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-27 15:17:24.000000 types-cffi-1.15.1.9/cffi-stubs/verifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 15:17:45.238616 types-cffi-1.15.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-27 15:17:42.000000 types-cffi-1.15.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:17:45.238616 types-cffi-1.15.1.9/types_cffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-27 15:17:45.000000 types-cffi-1.15.1.9/types_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-27 15:17:45.000000 types-cffi-1.15.1.9/types_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:17:45.000000 types-cffi-1.15.1.9/types_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-27 15:17:45.000000 types-cffi-1.15.1.9/types_cffi.egg-info/top_level.txt
```

### Comparing `types-cffi-1.15.1.8/CHANGELOG.md` & `types-cffi-1.15.1.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.15.1.9 (2023-03-27)
+
+[cffi] add some return types (#9949)
+
 ## 1.15.1.8 (2023-03-23)
 
 [cffi] cast source can be an int too  (#9930)
 
 [cffi] cast source can be an int too
 
 Co-authored-by: Francesc Elies <francesc.elies@mbbm-ast.com>
```

### Comparing `types-cffi-1.15.1.8/PKG-INFO` & `types-cffi-1.15.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-cffi
-Version: 1.15.1.8
+Version: 1.15.1.9
 Summary: Typing stubs for cffi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/cffi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `cffi`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/cffi. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a34da859660cdad9ab6cd427093a6cde9df09565`.
+This package was generated from typeshed commit `ce5f02fcdc11d8c8888290b79a70e3b034a46569`.
```

### Comparing `types-cffi-1.15.1.8/_cffi_backend-stubs/__init__.pyi` & `types-cffi-1.15.1.9/_cffi_backend-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-cffi-1.15.1.8/cffi-stubs/api.pyi` & `types-cffi-1.15.1.9/cffi-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-cffi-1.15.1.8/cffi-stubs/backend_ctypes.pyi` & `types-cffi-1.15.1.9/cffi-stubs/backend_ctypes.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     ): ...
     def new_function_type(self, BArgs, BResult, has_varargs): ...
     def new_enum_type(self, name, enumerators, enumvalues, CTypesInt): ...
     def get_errno(self): ...
     def set_errno(self, value) -> None: ...
     def string(self, b, maxlen: int = ...): ...
     def buffer(self, bptr, size: int = ...) -> None: ...
-    def sizeof(self, cdata_or_BType): ...
-    def alignof(self, BType): ...
+    def sizeof(self, cdata_or_BType) -> int: ...
+    def alignof(self, BType) -> int: ...
     def newp(self, BType, source): ...
     def cast(self, BType, source): ...
     def callback(self, BType, source, error, onerror): ...
     def gcp(self, cdata, destructor, size: int = ...): ...
     typeof: Incomplete
     def getcname(self, BType, replace_with): ...
     def typeoffsetof(self, BType, fieldname, num: int = ...): ...
```

### Comparing `types-cffi-1.15.1.8/cffi-stubs/cffi_opcode.pyi` & `types-cffi-1.15.1.9/cffi-stubs/cffi_opcode.pyi`

 * *Files identical despite different names*

### Comparing `types-cffi-1.15.1.8/cffi-stubs/model.pyi` & `types-cffi-1.15.1.9/cffi-stubs/model.pyi`

 * *Files identical despite different names*

### Comparing `types-cffi-1.15.1.8/cffi-stubs/recompiler.pyi` & `types-cffi-1.15.1.9/cffi-stubs/recompiler.pyi`

 * *Files identical despite different names*

### Comparing `types-cffi-1.15.1.8/cffi-stubs/verifier.pyi` & `types-cffi-1.15.1.9/cffi-stubs/verifier.pyi`

 * *Files identical despite different names*

### Comparing `types-cffi-1.15.1.8/setup.py` & `types-cffi-1.15.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `cffi`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/cffi. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a34da859660cdad9ab6cd427093a6cde9df09565`.
+This package was generated from typeshed commit `ce5f02fcdc11d8c8888290b79a70e3b034a46569`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.15.1.8",
+      version="1.15.1.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/cffi.md",
```

### Comparing `types-cffi-1.15.1.8/types_cffi.egg-info/PKG-INFO` & `types-cffi-1.15.1.9/types_cffi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-cffi
-Version: 1.15.1.8
+Version: 1.15.1.9
 Summary: Typing stubs for cffi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/cffi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `cffi`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/cffi. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a34da859660cdad9ab6cd427093a6cde9df09565`.
+This package was generated from typeshed commit `ce5f02fcdc11d8c8888290b79a70e3b034a46569`.
```

### Comparing `types-cffi-1.15.1.8/types_cffi.egg-info/SOURCES.txt` & `types-cffi-1.15.1.9/types_cffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

