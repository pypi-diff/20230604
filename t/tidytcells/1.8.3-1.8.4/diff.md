# Comparing `tmp/tidytcells-1.8.3.tar.gz` & `tmp/tidytcells-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.8.3.tar", last modified: Sat Jun  3 17:33:19 2023, max compression
+gzip compressed data, was "tidytcells-1.8.4.tar", last modified: Sun Jun  4 12:51:01 2023, max compression
```

## Comparing `tidytcells-1.8.3.tar` & `tidytcells-1.8.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.794156 tidytcells-1.8.3/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.8.3/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.8.3/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-03 17:33:19.794156 tidytcells-1.8.3/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-03 13:18:28.000000 tidytcells-1.8.3/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-03 17:28:40.000000 tidytcells-1.8.3/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-03 17:33:19.794156 tidytcells-1.8.3/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-03 13:18:28.000000 tidytcells-1.8.3/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.788156 tidytcells-1.8.3/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.789156 tidytcells-1.8.3/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 19:32:17.000000 tidytcells-1.8.3/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.791156 tidytcells-1.8.3/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-06-03 17:26:57.000000 tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-06-03 17:26:58.000000 tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-06-03 17:26:58.000000 tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-06-03 17:26:58.000000 tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.792156 tidytcells-1.8.3/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.8.3/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4092 2023-06-03 16:23:43.000000 tidytcells-1.8.3/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.8.3/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-03 17:26:54.000000 tidytcells-1.8.3/src/tidytcells/_utils/gene_standardizers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.792156 tidytcells-1.8.3/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1290 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.793156 tidytcells-1.8.3/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2671 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.793156 tidytcells-1.8.3/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10302 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.793156 tidytcells-1.8.3/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8597 2023-06-03 13:18:28.000000 tidytcells-1.8.3/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.790156 tidytcells-1.8.3/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-03 17:33:19.000000 tidytcells-1.8.3/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-03 17:33:19.794156 tidytcells-1.8.3/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1231 2023-03-11 19:32:17.000000 tidytcells-1.8.3/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2021 2023-03-11 19:32:17.000000 tidytcells-1.8.3/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9153 2023-06-03 15:14:45.000000 tidytcells-1.8.3/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8447 2023-06-03 17:26:54.000000 tidytcells-1.8.3/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.441820 tidytcells-1.8.4/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.8.4/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.8.4/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 12:51:01.441820 tidytcells-1.8.4/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-04 12:40:43.000000 tidytcells-1.8.4/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-04 12:40:51.000000 tidytcells-1.8.4/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-04 12:51:01.441820 tidytcells-1.8.4/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-04 12:40:43.000000 tidytcells-1.8.4/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.431820 tidytcells-1.8.4/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.433820 tidytcells-1.8.4/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 19:32:17.000000 tidytcells-1.8.4/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.437820 tidytcells-1.8.4/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-06-04 12:41:24.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-06-04 12:41:24.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.438820 tidytcells-1.8.4/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.8.4/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4926 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.8.4/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/_utils/gene_standardizers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.438820 tidytcells-1.8.4/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1607 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.438820 tidytcells-1.8.4/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3144 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.439820 tidytcells-1.8.4/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10549 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.439820 tidytcells-1.8.4/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8842 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.434820 tidytcells-1.8.4/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.440820 tidytcells-1.8.4/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1403 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2199 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9326 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8620 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_tcr.py
```

### Comparing `tidytcells-1.8.3/LICENSE.txt` & `tidytcells-1.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/PKG-INFO` & `tidytcells-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.3
+Version: 1.8.4
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.3/README.md` & `tidytcells-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/setup.py` & `tidytcells-1.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/__init__.py` & `tidytcells-1.8.4/src/tidytcells/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json` & `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.4/src/tidytcells/_utils/abstract_functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 def standardize_template(
     gene: str,
     gene_type: str,
     species: str,
     enforce_functional: bool,
     precision: str,
+    on_fail: str,
     suppress_warnings: bool,
     standardizer_dict: Dict[str, GeneStandardizer],
     allowed_precision: set,
 ) -> str:
     if type(gene) != str:
         raise TypeError(f"gene_name must be type str, got {gene} ({type(gene)}).")
     if type(species) != str:
@@ -24,22 +25,26 @@
             "enforce_functional must be type bool, got "
             f"{enforce_functional} ({type(enforce_functional)})."
         )
     if type(precision) != str:
         raise TypeError(
             f"precision must be type str, got {precision} ({type(precision)})."
         )
+    if type(on_fail) != str:
+        raise TypeError(f"on_fail must be type str, got {on_fail} ({type(on_fail)}).")
     if type(suppress_warnings) != bool:
         raise TypeError(
             "suppress_warnings must be type bool, got "
             f"{suppress_warnings} ({type(suppress_warnings)})."
         )
 
     if not precision in allowed_precision:
         raise ValueError(f"precision must be in {allowed_precision}, got {precision}.")
+    if not on_fail in ("reject", "keep"):
+        raise ValueError(f'on_fail must be "reject" or "keep", got {on_fail}.')
 
     # For backward compatibility, fix CamelCased species
     species = "".join(species.split()).lower()
 
     if not species in standardizer_dict:
         if not suppress_warnings:
             warn_unsupported_species(species, gene_type)
@@ -52,15 +57,17 @@
         if not suppress_warnings:
             warn_failure(
                 reason_for_failure=invalid_reason,
                 original_input=gene,
                 attempted_fix=standardized.compile("allele"),
                 species=species,
             )
-        return None
+        if on_fail == "reject":
+            return None
+        return gene
 
     return standardized.compile(precision)
 
 
 def query_template(
     species: str,
     precision: str,
@@ -104,24 +111,36 @@
 
     if contains is None:
         return result
 
     return frozenset([i for i in result if re.search(contains, i)])
 
 
-def standardize_aa_template(seq: str, suppress_warnings: bool):
+def standardize_aa_template(seq: str, on_fail: str, suppress_warnings: bool):
     if type(seq) != str:
         raise TypeError(f"seq must be type str, got {seq} ({type(seq)}).")
+    if type(on_fail) != str:
+        raise TypeError(f"on_fail must be type str, got {on_fail} ({type(on_fail)}).")
+    if type(suppress_warnings) != bool:
+        raise TypeError(
+            "suppress_warnings must be type bool, got "
+            f"{suppress_warnings} ({type(suppress_warnings)})."
+        )
+
+    if not on_fail in ("reject", "keep"):
+        raise ValueError(f'on_fail must be "reject" or "keep", got {on_fail}.')
 
     original_input = seq
 
     seq = seq.upper()
 
     for char in seq:
         if not char in AMINO_ACIDS:
             if not suppress_warnings:
                 warn(
                     f"Input {original_input} was rejected as it is not a valid amino acid sequence."
                 )
-            return None
+            if on_fail == "reject":
+                return None
+            return original_input
 
     return seq
```

### Comparing `tidytcells-1.8.3/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.4/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/_utils/gene_standardizers.py` & `tidytcells-1.8.4/src/tidytcells/_utils/gene_standardizers.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/aa/_main.py` & `tidytcells-1.8.4/src/tidytcells/aa/_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from .._utils.abstract_functions import standardize_aa_template
 
 
-def standardize(seq: str, suppress_warnings: bool = False):
+def standardize(seq: str, on_fail: str = "reject", suppress_warnings: bool = False):
     """
     Ensures that a string value looks like a valid amino acid sequence.
 
     :param seq:
         String value representing an amino acid sequence.
     :type seq:
-        ``str``
+        str
+    :param on_fail:
+        Behaviour when standardization fails.
+        If set to ``"reject"``, returns ``None`` on failure.
+        If set to ``"keep"``, returns the original input.
+        Defaults to ``"reject"``.
+    :type on_fail:
+        str
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
-        ``bool``
+        bool
 
     :return:
         Capitalised version of ``seq``, if seq is a valid amino acid sequence.
         Otherwise the input is rejected and ``None`` is returned.
     :rtype:
-        ``str`` or ``None``
+        Union[str, None]
 
     .. topic:: Example usage
 
         Strings that look like amino acid sequences will be accepted, and returned in capitalised form.
 
         >>> tt.aa.standardize("sqllnakyl")
         'SQLLNAKYL'
@@ -32,8 +39,10 @@
 
         >>> result = tt.aa.standardize("sqll?akyl")
         UserWarning: Input sqll?akyl was rejected as it is not a valid amino acid sequence.
         >>> print(result)
         None
     """
 
-    return standardize_aa_template(seq, suppress_warnings)
+    return standardize_aa_template(
+        seq=seq, on_fail=on_fail, suppress_warnings=suppress_warnings
+    )
```

### Comparing `tidytcells-1.8.3/src/tidytcells/junction/_main.py` & `tidytcells-1.8.4/src/tidytcells/junction/_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import re
 from .._utils.abstract_functions import standardize_aa_template
 from warnings import warn
 
 
-def standardize(seq: str, strict: bool = False, suppress_warnings: bool = False):
+def standardize(
+    seq: str,
+    strict: bool = False,
+    on_fail: str = "reject",
+    suppress_warnings: bool = False,
+):
     """
     Ensures that a string value looks like a valid junction (CDR3) amino acid sequence.
     This function is a special variant of :py:func:`tidytcells.aa.standardize`.
 
     A valid junction sequence must:
 
     1. Be a valid amino acid sequence
     2. Begin with a cysteine (C)
     3. End with a phenylalanine (F) or a tryptophan (W)
 
     :param seq:
         String value representing a junction sequence.
     :type seq:
-        ``str``
+        str
     :param strict:
         If ``True``, any string that does not look like a junction sequence is rejected.
         If ``False``, any inputs that are valid amino acid sequences but do not start with C and end with F/W are not rejected and instead are corrected by having a C appended to the beginning and an F appended at the end.
         Defaults to ``False``.
     :type strict:
-        ``bool``
+        bool
+    :param on_fail:
+        Behaviour when standardization fails.
+        If set to ``"reject"``, returns ``None`` on failure.
+        If set to ``"keep"``, returns the original input.
+        Defaults to ``"reject"``.
+    :type on_fail:
+        str
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
-        ``bool``
+        bool
 
     :return:
         If possible, a standardized version of the input string is returned.
         If the input string cannot be standardized, it is rejected and ``None`` is returned.
     :rtype:
-        ``str`` or ``None``
+        Union[str, None]
 
     .. topic:: Example usage
 
         Strings that look like junction sequences will be accepted, and returned in capitalised form.
 
         >>> tt.junction.standardize("csadaff")
         'CSADAFF'
@@ -55,22 +67,28 @@
         >>> print(result)
         None
     """
 
     # take note of original input
     original_input = seq
 
-    seq = standardize_aa_template(seq, suppress_warnings)
+    seq = standardize_aa_template(
+        seq=seq, on_fail="reject", suppress_warnings=suppress_warnings
+    )
 
     if seq is None:  # not a valid amino acid sequence
-        return None
+        if on_fail == "reject":
+            return None
+        return original_input
 
     if not re.match(f"^C[A-Z]*[FW]$", seq):
         if strict:
             if not suppress_warnings:
                 warn(
                     f"Input {original_input} was rejected as it is not a valid junction sequence."
                 )
-            return None
+            if on_fail == "reject":
+                return None
+            return original_input
         seq = "C" + seq + "F"
 
     return seq
```

### Comparing `tidytcells-1.8.3/src/tidytcells/mhc/__init__.py` & `tidytcells-1.8.4/src/tidytcells/mhc/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.4/src/tidytcells/mhc/_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 }
 
 
 def standardize(
     gene: Optional[str] = None,
     species: str = "homosapiens",
     precision: str = "allele",
+    on_fail: str = "reject",
     suppress_warnings: bool = False,
     gene_name: Optional[str] = None,
 ) -> tuple:
     """
     Attempt to standardize an MHC gene name to be IMGT-compliant.
 
     .. topic:: Supported species
@@ -52,45 +53,52 @@
         This function will only verify the validity of an MHC gene/allele up to the level of the protein.
         Any further precise allele designations will not be verified, apart from the requirement that the format (colon-separated numbers) look valid.
         The reasons for this is firstly because new alleles at that level are added to the IMGT list quite often and so accurate verification is difficult, secondly because people rarely need verification to such a precise level, and finally because such verification costs more computational effort with diminishing returns.
 
     :param gene:
         Potentially non-standardized MHC gene name.
     :type gene:
-        ``str``
+        str
     :param species:
         Species to which the MHC gene belongs (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
-        ``str``
+        str
     :param precision:
         The maximum level of precision to standardize to.
         ``'allele'`` standardizes to the maximum precision possible.
         ``'protein'`` keeps allele designators up to the level of the protein.
         ``'gene'`` standardizes only to the level of the gene.
         Defaults to ``'allele'``.
     :type precision:
-        ``str``
+        str
+    :param on_fail:
+        Behaviour when standardization fails.
+        If set to ``"reject"``, returns ``None`` on failure.
+        If set to ``"keep"``, returns the original input.
+        Defaults to ``"reject"``.
+    :type on_fail:
+        str
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
-        ``bool``
+        bool
 
     :param gene_name:
         Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
-        ``str``
+        str
 
     :return:
         If the specified ``species`` is supported, and ``gene`` could be standardized, then return the standardized gene name.
         If ``species`` is unsupported, then the function does not attempt to standardize, and returns the unaltered ``gene`` string.
         Else returns ``None``.
     :rtype:
-        ``str`` or ``None``
+        Union[str, None]
 
     .. topic:: Example usage
 
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
         >>> tt.mhc.standardize("A1")
         'HLA-A*01'
@@ -115,14 +123,15 @@
 
     return standardize_template(
         gene=gene,
         gene_type="MHC",
         species=species,
         enforce_functional=True,
         precision=precision,
+        on_fail=on_fail,
         suppress_warnings=suppress_warnings,
         standardizer_dict=STANDARDIZERS,
         allowed_precision={"allele", "protein", "gene"},
     )
 
 
 def query(
@@ -136,41 +145,41 @@
     .. topic:: Supported species
 
         - ``'homosapiens'``
         - ``'musmusculus'``
 
     .. note::
 
-        ``tidytcells``' knowledge of MHC alleles is limited, especially outside of humans.
-        ``tidytcells`` will allow you to query HLA alleles up to the level of the protein (first two allele designators), but that is the highest resolution available.
+        :py:mod:`tidytcells`' knowledge of MHC alleles is limited, especially outside of humans.
+        :py:mod:`tidytcells` will allow you to query HLA alleles up to the level of the protein (first two allele designators), but that is the highest resolution available.
         For Mus musculus, there is currently only support for gene-level querying.
 
     :param species:
         Species to query (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
-        ``str``
+        str
     :param precision:
         The level of precision to query.
         ``allele`` will query from the set of all possible alleles.
         ``gene`` will query from the set of all possible genes.
         Defaults to ``allele``.
     :type precision:
-        ``str``
+        str
     :param contains:
         An optional **regular expression** string which will be used to filter the query result.
         If supplied, only genes/alleles which contain the regular expression will be returned.
         Defaults to ``None``.
     :type contains:
-        ``str``
+        str
 
     :return:
         The set of all genes/alleles that satisfy the given constraints.
     :rtype:
-        ``FrozenSet[str]``
+        FrozenSet[str]
 
     .. topic:: Example usage
 
         List all known HLA-G variants.
 
         >>> tt.mhc.query(species="homosapiens", contains="HLA-G")
         frozenset({'HLA-TAP1*03:01', 'HLA-TAP1*01:02', 'HLA-TAP1*06:01', 'HLA-TAP1*04:01', 'HLA-TAP1*02:01', 'HLA-TAP1*05:01', 'HLA-TAP1*01:01'})
@@ -201,30 +210,30 @@
     .. note::
 
         This function currently only recognises HLAs, and not MHCs from other species.
 
     :param gene:
         Standardized MHC gene name
     :type gene:
-        ``str``
+        str
     :param suppress_warnings:
         Disable warnings that are usually emitted when chain classification fails.
         Defaults to ``False``.
     :type suppress_warnings:
-        ``bool``
+        bool
 
     :param gene_name:
         Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
-        ``str``
+        str
 
     :return:
         ``'alpha'`` or ``'beta'`` if ``gene`` is recognised and its chain is known, else ``None``.
     :rtype:
-        ``str`` or ``None``
+        Union[str, None]
 
     .. topic:: Example usage
 
         >>> tt.mhc.get_chain("HLA-A")
         'alpha'
         >>> tt.mhc.get_chain("HLA-DRB2")
         'beta'
@@ -273,30 +282,30 @@
     .. note::
 
         This function currently only recognises HLAs, and not MHCs from other species.
 
     :param gene:
         Standardized MHC gene name
     :type gene:
-        ``str``
+        str
     :param suppress_warnings:
         Disable warnings that are usually emitted when classification fails.
         Defaults to ``False``.
     :type suppress_warnings:
-        ``bool``
+        bool
 
     :param gene_name:
         Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
-        ``str``
+        str
 
     :return:
         ``1`` or ``2`` if ``gene`` is recognised and its class is known, else ``None``.
     :rtype:
-        ``int`` or ``None``
+        Union[int, None]
 
     .. topic:: Example usage
 
         >>> tt.mhc.get_class("HLA-A")
         1
         >>> tt.mhc.get_class("HLA-DRB2")
         2
```

### Comparing `tidytcells-1.8.3/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.4/src/tidytcells/tcr/_main.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,63 +29,71 @@
 
 
 def standardize(
     gene: Optional[str] = None,
     species: str = "homosapiens",
     enforce_functional: bool = False,
     precision: str = "allele",
+    on_fail: str = "reject",
     suppress_warnings: bool = False,
     gene_name: Optional[str] = None,
 ) -> str:
     """
     Attempt to standardize a TCR gene name to be IMGT-compliant.
 
     .. topic:: Supported species
 
         - ``'homosapiens'``
         - ``'musmusculus'``
 
     :param gene:
         Potentially non-standardized TCR gene name.
     :type gene:
-        ``str``
+        str
     :param species:
         Species to which the TCR gene belongs (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
-        ``str``
+        str
     :param enforce_functional:
         If ``True``, disallows TCR genes that are recognised by IMGT but are marked as non-functional (ORF or pseudogene).
         Defaults to ``False``.
     :type enforce_functional:
-        ``bool``
+        bool
     :param precision:
         The maximum level of precision to standardize to.
         ``'allele'`` standardizes to the maximum precision possible.
         ``'gene'`` standardizes only to the level of the gene.
         Defaults to ``'allele'``.
     :type precision:
-        ``str``
+        str
+    :param on_fail:
+        Behaviour when standardization fails.
+        If set to ``"reject"``, returns ``None`` on failure.
+        If set to ``"keep"``, returns the original input.
+        Defaults to ``"reject"``.
+    :type on_fail:
+        str
     :param suppress_warnings:
         Disable warnings that are usually emitted when standardisation fails.
         Defaults to ``False``.
     :type suppress_warnings:
-        ``bool``
+        bool
 
     :param gene_name:
         Alias for the parameter ``gene``. This will be deprecated soon.
     :type gene_name:
-        ``str``
+        str
 
     :return:
         If the specified ``species`` is supported, and ``gene`` could be standardized, then return the standardized gene name.
         If ``species`` is unsupported, then the function does not attempt to standardize , and returns the unaltered ``gene`` string.
         Else returns ``None``.
     :rtype:
-        ``str`` or ``None``
+        Union[str, None]
 
     .. topic:: Example usage
 
         Input strings will intelligently be corrected to IMGT-compliant gene symbols.
 
         >>> tt.tcr.standardize("aj1")
         'TRAJ1'
@@ -117,14 +125,15 @@
 
     return standardize_template(
         gene=gene,
         gene_type="TCR",
         species=species,
         enforce_functional=enforce_functional,
         precision=precision,
+        on_fail=on_fail,
         suppress_warnings=suppress_warnings,
         standardizer_dict=STANDARDIZERS,
         allowed_precision={"allele", "gene"},
     )
 
 
 def query(
@@ -141,45 +150,45 @@
         - ``'homosapiens'``
         - ``'musmusculus'``
 
     :param species:
         Species to query (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
-        ``str``
+        str
     :param precision:
         The level of precision to query.
         ``allele`` will query from the set of all possible alleles.
         ``gene`` will query from the set of all possible genes.
         Defaults to ``allele``.
     :type precision:
-        ``str``
+        str
     :param functionality:
         Gene/allele functionality to subset by.
         ``"any"`` queries from all possible genes/alleles.
         ``"F"`` queries from functional genes/alleles.
         ``"NF"`` queries from psuedogenes and ORFs.
         ``"P"`` queries from pseudogenes.
         ``"ORF"`` queries from ORFs.
         An allele is considered queriable if its functionality label matches the description.
         A gene is considered queriable if at least one of its alleles' functionality label matches the description.
         Defaults to ``"any"``.
     :type functionality:
-        ``str``
+        str
     :param contains:
         An optional regular expression string which will be used to filter the query result.
         If supplied, only genes/alleles which contain the regular expression will be returned.
         Defaults to ``None``.
     :type contains:
-        ``str``
+        str
 
     :return:
         The set of all genes/alleles that satisfy the given constraints.
     :rtype:
-        ``FrozenSet[str]``
+        FrozenSet[str]
 
     .. topic:: Example usage
 
         List all known variants for the human TCR gene TRBV6-1.
 
         >>> tt.tcr.query(species="homosapiens", contains="TRBV6-1")
         frozenset({'TRBV6-1*01'})
@@ -213,25 +222,25 @@
         Support for J genes is planned for the future.
 
     :param gene:
         Standardized gene name.
         The gene must be specified to the level of the allele.
         Note that some genes, notably the non-functional ones, will not have resolvable amino acid sequences.
     :type gene:
-        ``str``
+        str
     :param species:
         Species to which the TCR gene in question belongs (see above for supported species).
         Defaults to ``'homosapiens'``.
     :type species:
-        ``str``
+        str
 
     :return:
         A dictionary with keys corresponding to names of different sequence regions within the gene, and values corresponding to their amino acid sequences.
     :rtype:
-        ``Dict[str, str]``
+        Dict[str, str]
 
     .. topic:: Example usage
 
         Get amino acid sequence information about the human V gene TRBV2*01.
 
         >>> tt.tcr.get_aa_sequence(gene="TRBV2*01", species="homosapiens")
         {'CDR1-IMGT': 'SNHLY', 'CDR2-IMGT': 'FYNNEI', 'FR1-IMGT': 'EPEVTQTPSHQVTQMGQEVILRCVPI', 'FR2-IMGT': 'FYWYRQILGQKVEFLVS', 'FR3-IMGT': 'SEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFC', 'V-REGION': 'EPEVTQTPSHQVTQMGQEVILRCVPISNHLYFYWYRQILGQKVEFLVSFYNNEISEKSEIFDDQFSVERPDGSNFTLKIRSTKLEDSAMYFCASSE'}
```

### Comparing `tidytcells-1.8.3/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.4/src/tidytcells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.3
+Version: 1.8.4
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.3/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.4/src/tidytcells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.3/tests/test_aa.py` & `tidytcells-1.8.4/tests/test_aa.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,44 @@
 from tidytcells import aa
 import warnings
 
 
 class TestStandardise:
     @pytest.mark.parametrize("seq", ("KLGGALQAK", "LLQTGIHVRVSQPSL", "SQLLNAKYL"))
     def test_alreadY_correct(self, seq):
-        result = aa.standardise(seq=seq)
+        result = aa.standardize(seq=seq)
 
         assert result == seq
 
     @pytest.mark.parametrize("seq", ("123456", "ASDFGHJKL", "A?AAAA", "AAAXAA"))
     def test_various_rejections(self, seq):
         with pytest.warns(UserWarning, match="is not a valid amino acid"):
-            result = aa.standardise(seq=seq)
+            result = aa.standardize(seq=seq)
 
         assert result == None
 
     @pytest.mark.parametrize(("seq", "expected"), (("klgak", "KLGAK"),))
     def test_various_corrections(self, seq, expected):
-        result = aa.standardise(seq=seq)
+        result = aa.standardize(seq=seq)
 
         assert result == expected
 
     @pytest.mark.parametrize("seq", (None, 1, True, 5.4))
     def test_bad_input_type(self, seq):
         with pytest.raises(TypeError):
-            aa.standardise(seq=seq)
+            aa.standardize(seq=seq)
 
-    def test_standardize(self):
-        result = aa.standardize(seq="KLGAK")
+    def test_standardise(self):
+        result = aa.standardise(seq="KLGAK")
 
         assert result == "KLGAK"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
-            aa.standardise(seq="123456", suppress_warnings=True)
+            aa.standardize(seq="123456", suppress_warnings=True)
+
+    def test_on_fail(self):
+        with pytest.warns(UserWarning):
+            result = aa.standardize("foobarbaz", on_fail="keep")
+
+        assert result == "foobarbaz"
```

### Comparing `tidytcells-1.8.3/tests/test_junction.py` & `tidytcells-1.8.4/tests/test_junction.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,7 +64,13 @@
 
         assert result == "CASSPGGADRRIDGYTF"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
             junction.standardise(seq="123456", suppress_warnings=True)
+
+    def test_on_fail(self):
+        with pytest.warns(UserWarning):
+            result = junction.standardize("foobarbaz", on_fail="keep")
+
+        assert result == "foobarbaz"
```

### Comparing `tidytcells-1.8.3/tests/test_mhc.py` & `tidytcells-1.8.4/tests/test_mhc.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,20 @@
         assert result == "HLA-B*07"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
             mhc.standardize("foobarbaz", suppress_warnings=True)
 
+    def test_on_fail(self):
+        with pytest.warns(UserWarning):
+            result = mhc.standardize("foobarbaz", on_fail="keep")
+
+        assert result == "foobarbaz"
+
 
 class TestStandardizeHomoSapiens:
     @pytest.mark.parametrize("gene", [*HOMOSAPIENS_MHC, "B2M"])
     def test_already_correctly_formatted(self, gene):
         result = mhc.standardize(gene=gene, species="homosapiens")
 
         assert result == gene
```

### Comparing `tidytcells-1.8.3/tests/test_tcr.py` & `tidytcells-1.8.4/tests/test_tcr.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,20 @@
         assert result == "TRBV20/OR9-2*01"
 
     def test_suppress_warnings(self):
         with warnings.catch_warnings():
             warnings.simplefilter("error")
             tcr.standardize("foobarbaz", suppress_warnings=True)
 
+    def test_on_fail(self):
+        with pytest.warns(UserWarning):
+            result = tcr.standardize("foobarbaz", on_fail="keep")
+
+        assert result == "foobarbaz"
+
 
 class TestStandardizeHomoSapiens:
     @pytest.mark.parametrize("gene", HOMOSAPIENS_TCR)
     def test_already_correctly_formatted(self, gene):
         result = tcr.standardize(gene=gene, species="homosapiens")
 
         assert result == gene
```

