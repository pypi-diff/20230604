# Comparing `tmp/segytools-0.1.1.tar.gz` & `tmp/segytools-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segytools-0.1.1.tar", max compression
+gzip compressed data, was "segytools-0.2.0.tar", max compression
```

## Comparing `segytools-0.1.1.tar` & `segytools-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.1.1/LICENSE
--rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.1.1/README.md
--rw-r--r--   0        0        0      786 2023-06-02 08:15:34.847622 segytools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      215 2023-02-04 10:18:01.553258 segytools-0.1.1/src/segytools/__init__.py
--rw-r--r--   0        0        0     1165 2023-01-29 16:40:13.789248 segytools-0.1.1/src/segytools/datatypes.py
--rw-r--r--   0        0        0     4192 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_abstract_header.py
--rw-r--r--   0        0        0    13599 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_file_header.py
--rw-r--r--   0        0        0     8542 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_header_item.py
--rw-r--r--   0        0        0    35111 2023-06-02 08:15:34.847622 segytools-0.1.1/src/segytools/segy_trace_header.py
--rw-r--r--   0        0        0      497 2023-01-29 16:40:13.789248 segytools-0.1.1/src/segytools/toolkit.py
--rw-r--r--   0        0        0       95 2023-01-29 16:40:13.789248 segytools-0.1.1/src/segytools/utils.py
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 segytools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2022-06-22 10:42:33.628006 segytools-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1020 2023-02-02 11:46:01.496827 segytools-0.2.0/README.md
+-rw-r--r--   0        0        0      870 2023-06-04 20:39:52.857422 segytools-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-02-04 10:18:01.553258 segytools-0.2.0/src/segytools/__init__.py
+-rw-r--r--   0        0        0     1165 2023-01-29 16:40:13.789248 segytools-0.2.0/src/segytools/datatypes.py
+-rw-r--r--   0        0        0     4192 2023-06-02 08:15:34.847622 segytools-0.2.0/src/segytools/segy_abstract_header.py
+-rw-r--r--   0        0        0    14741 2023-06-04 20:39:52.857422 segytools-0.2.0/src/segytools/segy_file_header.py
+-rw-r--r--   0        0        0     8540 2023-06-04 20:39:52.857422 segytools-0.2.0/src/segytools/segy_header_item.py
+-rw-r--r--   0        0        0    35111 2023-06-02 08:15:34.847622 segytools-0.2.0/src/segytools/segy_trace_header.py
+-rw-r--r--   0        0        0     2543 2023-06-04 20:39:52.857422 segytools-0.2.0/src/segytools/toolkit.py
+-rw-r--r--   0        0        0       95 2023-01-29 16:40:13.789248 segytools-0.2.0/src/segytools/utils.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 segytools-0.2.0/PKG-INFO
```

### Comparing `segytools-0.1.1/LICENSE` & `segytools-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segytools-0.1.1/README.md` & `segytools-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `segytools-0.1.1/pyproject.toml` & `segytools-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "segytools"
-version = "0.1.1"
+version = "0.2.0"
 description = "low level toolkit for manipulating and analyzing segy formatted data"
 authors = ["anthonytorlucci <anthonytorlucci@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -23,10 +23,15 @@
 myst-nb = {version = "^0.17.1", python = "^3.9"}
 sphinx-autoapi = "^2.0.0"
 sphinx-rtd-theme = "^1.1.1"
 flake8 = "^6.0.0"
 black = "^22.12.0"
 isort = "^5.12.0"
 
+
+[tool.poetry.group.examples.dependencies]
+pandas = "^2.0.2"
+matplotlib = "^3.7.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `segytools-0.1.1/src/segytools/datatypes.py` & `segytools-0.2.0/src/segytools/datatypes.py`

 * *Files identical despite different names*

### Comparing `segytools-0.1.1/src/segytools/segy_abstract_header.py` & `segytools-0.2.0/src/segytools/segy_abstract_header.py`

 * *Files identical despite different names*

### Comparing `segytools-0.1.1/src/segytools/segy_file_header.py` & `segytools-0.2.0/src/segytools/segy_file_header.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 '''
 
 # import python standard modules
 
 # import 3rd party libraries
 
 # import local python
-from segytools.datatypes import (DATA_SAMPLE_FORMAT_INT16,
-                                 DATA_SAMPLE_FORMAT_INT32)
+from segytools.datatypes import (DataSampleFormat,
+                                 DATA_SAMPLE_FORMAT_INT8,
+                                 DATA_SAMPLE_FORMAT_INT16,
+                                 DATA_SAMPLE_FORMAT_INT32,
+                                 DATA_SAMPLE_FORMAT_FLOAT32,
+                                 DATA_SAMPLE_FORMAT_IBM)
 from segytools.segy_abstract_header import SegyAbstractHeader
 from segytools.segy_header_item import SegyHeaderItem
 
 # --- Mappings
 # bytes 25-26
 DATA_SAMPLE_FORMAT_CODE = {
     0: "undefined",
@@ -402,12 +406,33 @@
             raise ValueError(
                 "Unable to determine sample format size in bytes \
                 as sample format is undefined."
             )
         # self.segy_logger.debug(f'sample format {fmt} size in bytes is {byte_size}')
         return byte_size
 
+    def sample_format_datatype(self) -> DataSampleFormat:
+        """Return the DataSampleFormat datatype from the data_sample_format_code member variable."""
+        fmt = self.data_sample_format_code._mapped_value
+        sample_format = DATA_SAMPLE_FORMAT_FLOAT32  # default
+        if fmt == "ibm":
+            sample_format = DATA_SAMPLE_FORMAT_IBM
+        elif fmt == "float32":
+            sample_format = DATA_SAMPLE_FORMAT_FLOAT32
+        elif fmt == "int32":
+            sample_format = DATA_SAMPLE_FORMAT_INT32
+        elif fmt == "int16":
+            sample_format = DATA_SAMPLE_FORMAT_INT16
+        elif fmt == "int8":
+            sample_format = DATA_SAMPLE_FORMAT_INT8
+        else:
+            raise ValueError(
+                "Unable to determine sample format."
+            )
+        # self.segy_logger.debug(f'sample format {fmt} size in bytes is {byte_size}')
+        return sample_format
+    
     # TODO: def is_fixed_length(self):
     #     if self.fixedlen == ??:
     #         return True
     #     else:
     #         return False
```

### Comparing `segytools-0.1.1/src/segytools/segy_header_item.py` & `segytools-0.2.0/src/segytools/segy_header_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
             either '<' for little or '>' for big endian
         sample_format : DataSampleFormat
             data sample format used for interpreting bytes object.
         """
         if sample_format.format == 'ibm':
             # NOTE: only 32-bit ibm floats currently tested and supported
             fmt = ''.join([endianess, 'u4'])
-            val = ibm2float32(numpy.frombuffer(buffer=buf, dtype='>u4'))
+            val = ibm2float32(numpy.frombuffer(buffer=buf, dtype=fmt))
         else:
             fmt = ''.join([endianess, sample_format.format])
             val = struct.unpack(fmt, buf)
             val = val[0]  # unpack always returns a tuple
         return val
 
     @classmethod
```

### Comparing `segytools-0.1.1/src/segytools/segy_trace_header.py` & `segytools-0.2.0/src/segytools/segy_trace_header.py`

 * *Files identical despite different names*

### Comparing `segytools-0.1.1/PKG-INFO` & `segytools-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segytools
-Version: 0.1.1
+Version: 0.2.0
 Summary: low level toolkit for manipulating and analyzing segy formatted data
 License: MIT
 Author: anthonytorlucci
 Author-email: anthonytorlucci@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

