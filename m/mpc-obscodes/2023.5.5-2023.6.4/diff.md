# Comparing `tmp/mpc_obscodes-2023.5.5.tar.gz` & `tmp/mpc_obscodes-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.5.5.tar", last modified: Fri May  5 02:26:46 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.6.4.tar", last modified: Sun Jun  4 02:51:16 2023, max compression
```

## Comparing `mpc_obscodes-2023.5.5.tar` & `mpc_obscodes-2023.6.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245386 2023-05-05 02:26:35.000000 mpc_obscodes-2023.5.5/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 02:26:35.000000 mpc_obscodes-2023.5.5/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 02:26:35.000000 mpc_obscodes-2023.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.248063 mpc_obscodes-2023.6.4/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245714 2023-06-04 02:51:05.000000 mpc_obscodes-2023.6.4/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-04 02:51:05.000000 mpc_obscodes-2023.6.4/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-04 02:51:01.000000 mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:51:16.248063 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-04 02:51:16.000000 mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-04 02:51:05.000000 mpc_obscodes-2023.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:51:16.252063 mpc_obscodes-2023.6.4/setup.cfg
```

### Comparing `mpc_obscodes-2023.5.5/PKG-INFO` & `mpc_obscodes-2023.6.4/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mpc_obscodes
-Version: 2023.5.5
+Name: mpc-obscodes
+Version: 2023.6.4
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.5.5/README.md` & `mpc_obscodes-2023.6.4/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes/compare.py` & `mpc_obscodes-2023.6.4/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.6.4/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.6.4/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987674609695973%*

 * *Differences: {"'M55'": "OrderedDict([('Longitude', 19.987), ('cos', 0.656685), ('sin', 0.751814), ('Name', "*

 * *          "'Luckystar Observatory, Vazec')])",*

 * * "'P63'": "OrderedDict([('Longitude', 126.8475), ('cos', 0.817778), ('sin', 0.573621), ('Name', "*

 * *          "'GSA Observatory, Gwangju')])",*

 * * "'Y05'": "OrderedDict([('Longitude', 316.31), ('cos', 0.941254), ('sin', -0.337051), ('Name', "*

 * *          "'SONEAR Wykrota-CEAMIG, Serra da Piedade')])"}*

```diff
@@ -12085,14 +12085,20 @@
     },
     "M54": {
         "Longitude": 7.07781,
         "Name": "Observatoire Albireo de Biot",
         "cos": 0.72514,
         "sin": 0.686335
     },
+    "M55": {
+        "Longitude": 19.987,
+        "Name": "Luckystar Observatory, Vazec",
+        "cos": 0.656685,
+        "sin": 0.751814
+    },
     "M90": {
         "Longitude": 65.4286,
         "Name": "Chervishevo",
         "cos": 0.54672,
         "sin": 0.83452
     },
     "N27": {
@@ -12349,14 +12355,20 @@
     },
     "P48": {
         "Longitude": 123.32403,
         "Name": "ASTEP, Concordia Station",
         "cos": 0.258064,
         "sin": -0.963413
     },
+    "P63": {
+        "Longitude": 126.8475,
+        "Name": "GSA Observatory, Gwangju",
+        "cos": 0.817778,
+        "sin": 0.573621
+    },
     "P64": {
         "Longitude": 127.00489,
         "Name": "GSHS Observatory, Suwon",
         "cos": 0.796371,
         "sin": 0.602805
     },
     "P65": {
@@ -13867,14 +13879,20 @@
     },
     "Y01": {
         "Longitude": 316.0158,
         "Name": "SONEAR 2 Observatory, Belo Horizonte",
         "cos": 0.94089,
         "sin": -0.337985
     },
+    "Y05": {
+        "Longitude": 316.31,
+        "Name": "SONEAR Wykrota-CEAMIG, Serra da Piedade",
+        "cos": 0.941254,
+        "sin": -0.337051
+    },
     "Y16": {
         "Longitude": 318.68794,
         "Name": "ROCG, Campos dos Goytacazes",
         "cos": 0.929268,
         "sin": -0.36817
     },
     "Y28": {
```

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.6.4/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mpc-obscodes
-Version: 2023.5.5
+Name: mpc_obscodes
+Version: 2023.6.4
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.5.5/pyproject.toml` & `mpc_obscodes-2023.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.05.05"
+version = "2023.06.04"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

