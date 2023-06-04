# Comparing `tmp/tidytcells-1.8.4.tar.gz` & `tmp/tidytcells-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidytcells-1.8.4.tar", last modified: Sun Jun  4 12:51:01 2023, max compression
+gzip compressed data, was "tidytcells-1.8.5.tar", last modified: Sun Jun  4 14:01:03 2023, max compression
```

## Comparing `tidytcells-1.8.4.tar` & `tidytcells-1.8.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.441820 tidytcells-1.8.4/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.8.4/LICENSE.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.8.4/MANIFEST.in
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 12:51:01.441820 tidytcells-1.8.4/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-04 12:40:43.000000 tidytcells-1.8.4/README.md
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-04 12:40:51.000000 tidytcells-1.8.4/VERSION.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-04 12:51:01.441820 tidytcells-1.8.4/setup.cfg
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-04 12:40:43.000000 tidytcells-1.8.4/setup.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.431820 tidytcells-1.8.4/src/
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.433820 tidytcells-1.8.4/src/tidytcells/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-03-11 19:32:17.000000 tidytcells-1.8.4/src/tidytcells/__init__.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.437820 tidytcells-1.8.4/src/tidytcells/_resources/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/_resources/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-06-04 12:41:24.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-06-04 12:41:24.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-06-04 12:41:25.000000 tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_tcr.json
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.438820 tidytcells-1.8.4/src/tidytcells/_utils/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-02-24 16:40:58.000000 tidytcells-1.8.4/src/tidytcells/_utils/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4926 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/_utils/abstract_functions.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-03-05 13:54:54.000000 tidytcells-1.8.4/src/tidytcells/_utils/gene_query_engines.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/_utils/gene_standardizers.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/_utils/warnings.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.438820 tidytcells-1.8.4/src/tidytcells/aa/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/aa/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1607 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/aa/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.438820 tidytcells-1.8.4/src/tidytcells/junction/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/junction/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3144 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/junction/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.439820 tidytcells-1.8.4/src/tidytcells/mhc/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/mhc/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10549 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/mhc/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.439820 tidytcells-1.8.4/src/tidytcells/tcr/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-04 12:40:43.000000 tidytcells-1.8.4/src/tidytcells/tcr/__init__.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8842 2023-06-04 12:40:51.000000 tidytcells-1.8.4/src/tidytcells/tcr/_main.py
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.434820 tidytcells-1.8.4/src/tidytcells.egg-info/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/PKG-INFO
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/SOURCES.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/dependency_links.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/requires.txt
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-04 12:51:01.000000 tidytcells-1.8.4/src/tidytcells.egg-info/top_level.txt
-drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 12:51:01.440820 tidytcells-1.8.4/tests/
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1403 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_aa.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2199 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_junction.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9326 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_mhc.py
--rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8620 2023-06-04 12:40:51.000000 tidytcells-1.8.4/tests/test_tcr.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.990591 tidytcells-1.8.5/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1068 2022-11-05 19:14:55.000000 tidytcells-1.8.5/LICENSE.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       19 2022-11-06 20:07:03.000000 tidytcells-1.8.5/MANIFEST.in
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 14:01:03.990591 tidytcells-1.8.5/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1504 2023-06-04 13:01:59.000000 tidytcells-1.8.5/README.md
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        5 2023-06-04 13:54:37.000000 tidytcells-1.8.5/VERSION.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       38 2023-06-04 14:01:03.990591 tidytcells-1.8.5/setup.cfg
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1321 2023-06-04 13:01:59.000000 tidytcells-1.8.5/setup.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.982591 tidytcells-1.8.5/src/
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.983591 tidytcells-1.8.5/src/tidytcells/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       90 2023-06-04 13:01:43.000000 tidytcells-1.8.5/src/tidytcells/__init__.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.986591 tidytcells-1.8.5/src/tidytcells/_resources/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1258 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_resources/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)   620328 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1295 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    14382 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    88302 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     6476 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1031 2023-06-04 13:01:15.000000 tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     5344 2023-06-04 13:01:15.000000 tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc_synonyms.json
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    16802 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_tcr.json
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.987591 tidytcells-1.8.5/src/tidytcells/_utils/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 13:01:06.000000 tidytcells-1.8.5/src/tidytcells/_utils/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     4921 2023-06-04 13:51:59.000000 tidytcells-1.8.5/src/tidytcells/_utils/abstract_functions.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3081 2023-06-04 13:01:37.000000 tidytcells-1.8.5/src/tidytcells/_utils/gene_query_engines.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    12709 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_utils/gene_standardizers.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      479 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/_utils/warnings.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.988592 tidytcells-1.8.5/src/tidytcells/aa/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      246 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/aa/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1607 2023-06-04 13:02:14.000000 tidytcells-1.8.5/src/tidytcells/aa/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.988592 tidytcells-1.8.5/src/tidytcells/junction/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      248 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/junction/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     3139 2023-06-04 13:52:39.000000 tidytcells-1.8.5/src/tidytcells/junction/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.988592 tidytcells-1.8.5/src/tidytcells/mhc/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      625 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/mhc/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)    10549 2023-06-04 13:02:14.000000 tidytcells-1.8.5/src/tidytcells/mhc/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.989591 tidytcells-1.8.5/src/tidytcells/tcr/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)      260 2023-06-04 13:01:59.000000 tidytcells-1.8.5/src/tidytcells/tcr/__init__.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8842 2023-06-04 13:02:14.000000 tidytcells-1.8.5/src/tidytcells/tcr/_main.py
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.984591 tidytcells-1.8.5/src/tidytcells.egg-info/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2136 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/PKG-INFO
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1244 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/SOURCES.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)        1 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/dependency_links.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       95 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/requires.txt
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)       11 2023-06-04 14:01:03.000000 tidytcells-1.8.5/src/tidytcells.egg-info/top_level.txt
+drwxr-xr-x   0 yutanagano  (1000) yutanagano  (1000)        0 2023-06-04 14:01:03.990591 tidytcells-1.8.5/tests/
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     1400 2023-06-04 13:52:56.000000 tidytcells-1.8.5/tests/test_aa.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     2193 2023-06-04 13:53:42.000000 tidytcells-1.8.5/tests/test_junction.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     9326 2023-06-04 13:02:14.000000 tidytcells-1.8.5/tests/test_mhc.py
+-rw-r--r--   0 yutanagano  (1000) yutanagano  (1000)     8620 2023-06-04 13:02:14.000000 tidytcells-1.8.5/tests/test_tcr.py
```

### Comparing `tidytcells-1.8.4/LICENSE.txt` & `tidytcells-1.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/PKG-INFO` & `tidytcells-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.4
+Version: 1.8.5
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.4/README.md` & `tidytcells-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/setup.py` & `tidytcells-1.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/__init__.py` & `tidytcells-1.8.5/src/tidytcells/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc.json` & `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_mhc_synonyms.json` & `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr.json` & `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json` & `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_aa_sequences.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/homosapiens_tcr_synonyms.json` & `tidytcells-1.8.5/src/tidytcells/_resources/homosapiens_tcr_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc.json` & `tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_mhc_synonyms.json` & `tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_mhc_synonyms.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_resources/musmusculus_tcr.json` & `tidytcells-1.8.5/src/tidytcells/_resources/musmusculus_tcr.json`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_utils/abstract_functions.py` & `tidytcells-1.8.5/src/tidytcells/_utils/abstract_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,14 @@
 
     seq = seq.upper()
 
     for char in seq:
         if not char in AMINO_ACIDS:
             if not suppress_warnings:
                 warn(
-                    f"Input {original_input} was rejected as it is not a valid amino acid sequence."
+                    f"Failed to standardize {original_input}: not a valid amino acid sequence."
                 )
             if on_fail == "reject":
                 return None
             return original_input
 
     return seq
```

### Comparing `tidytcells-1.8.4/src/tidytcells/_utils/gene_query_engines.py` & `tidytcells-1.8.5/src/tidytcells/_utils/gene_query_engines.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/_utils/gene_standardizers.py` & `tidytcells-1.8.5/src/tidytcells/_utils/gene_standardizers.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/aa/_main.py` & `tidytcells-1.8.5/src/tidytcells/aa/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/junction/_main.py` & `tidytcells-1.8.5/src/tidytcells/junction/_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             return None
         return original_input
 
     if not re.match(f"^C[A-Z]*[FW]$", seq):
         if strict:
             if not suppress_warnings:
                 warn(
-                    f"Input {original_input} was rejected as it is not a valid junction sequence."
+                    f"Failed to standardize {original_input}: not a valid junction sequence."
                 )
             if on_fail == "reject":
                 return None
             return original_input
         seq = "C" + seq + "F"
 
     return seq
```

### Comparing `tidytcells-1.8.4/src/tidytcells/mhc/__init__.py` & `tidytcells-1.8.5/src/tidytcells/mhc/__init__.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/mhc/_main.py` & `tidytcells-1.8.5/src/tidytcells/mhc/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells/tcr/_main.py` & `tidytcells-1.8.5/src/tidytcells/tcr/_main.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/src/tidytcells.egg-info/PKG-INFO` & `tidytcells-1.8.5/src/tidytcells.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidytcells
-Version: 1.8.4
+Version: 1.8.5
 Summary: Standardise TCR/MHC data.
 Author: Yuta Nagano
 Author-email: yutanagano51@proton.me
 Keywords: immunology,bioinformatics,TCR,MHC,HLA,T cell,IMGT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidytcells-1.8.4/src/tidytcells.egg-info/SOURCES.txt` & `tidytcells-1.8.5/src/tidytcells.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/tests/test_aa.py` & `tidytcells-1.8.5/tests/test_aa.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def test_alreadY_correct(self, seq):
         result = aa.standardize(seq=seq)
 
         assert result == seq
 
     @pytest.mark.parametrize("seq", ("123456", "ASDFGHJKL", "A?AAAA", "AAAXAA"))
     def test_various_rejections(self, seq):
-        with pytest.warns(UserWarning, match="is not a valid amino acid"):
+        with pytest.warns(UserWarning, match="not a valid amino acid"):
             result = aa.standardize(seq=seq)
 
         assert result == None
 
     @pytest.mark.parametrize(("seq", "expected"), (("klgak", "KLGAK"),))
     def test_various_corrections(self, seq, expected):
         result = aa.standardize(seq=seq)
```

### Comparing `tidytcells-1.8.4/tests/test_junction.py` & `tidytcells-1.8.5/tests/test_junction.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def test_already_correct(self, seq):
         result = junction.standardise(seq=seq)
 
         assert result == seq
 
     @pytest.mark.parametrize("seq", ("123456", "ASDFGHJKL", "A?AAAA", "AAAXAA"))
     def test_various_rejections(self, seq):
-        with pytest.warns(UserWarning, match="is not a valid amino acid sequence"):
+        with pytest.warns(UserWarning, match="not a valid amino acid sequence"):
             result = junction.standardise(seq=seq)
 
         assert result is None
 
     @pytest.mark.parametrize(
         ("seq", "expected"),
         (
@@ -50,15 +50,15 @@
     @pytest.mark.parametrize("seq", (None, 1, True, 5.4))
     def test_bad_input_type(self, seq):
         with pytest.raises(TypeError):
             junction.standardise(seq=seq)
 
     @pytest.mark.parametrize("seq", ("ASQY", "CASQY", "ASQYF", "ASQYW"))
     def test_strict(self, seq):
-        with pytest.warns(UserWarning, match="is not a valid junction"):
+        with pytest.warns(UserWarning, match="not a valid junction"):
             result = junction.standardise(seq=seq, strict=True)
 
         assert result is None
 
     def test_standardize(self):
         result = junction.standardize(seq="CASSPGGADRRIDGYTF")
```

### Comparing `tidytcells-1.8.4/tests/test_mhc.py` & `tidytcells-1.8.5/tests/test_mhc.py`

 * *Files identical despite different names*

### Comparing `tidytcells-1.8.4/tests/test_tcr.py` & `tidytcells-1.8.5/tests/test_tcr.py`

 * *Files identical despite different names*

