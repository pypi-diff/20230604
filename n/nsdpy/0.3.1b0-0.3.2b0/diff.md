# Comparing `tmp/nsdpy-0.3.1b0.tar.gz` & `tmp/nsdpy-0.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.3.1b0.tar", max compression
+gzip compressed data, was "nsdpy-0.3.2b0.tar", max compression
```

## Comparing `nsdpy-0.3.1b0.tar` & `nsdpy-0.3.2b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.1b0/LICENSE
--rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.1b0/README.md
--rw-r--r--   0        0        0    34827 2023-06-03 12:39:19.745531 nsdpy-0.3.1b0/functions.py
--rw-r--r--   0        0        0    12986 2023-06-04 14:17:13.448073 nsdpy-0.3.1b0/nsdpy.py
--rw-r--r--   0        0        0      841 2023-06-04 14:17:11.345858 nsdpy-0.3.1b0/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.1b0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.2b0/LICENSE
+-rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.2b0/README.md
+-rw-r--r--   0        0        0    34827 2023-06-04 14:22:11.687233 nsdpy-0.3.2b0/functions.py
+-rw-r--r--   0        0        0    12977 2023-06-04 14:23:30.688097 nsdpy-0.3.2b0/nsdpy.py
+-rw-r--r--   0        0        0      841 2023-06-04 14:23:45.879269 nsdpy-0.3.2b0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.2b0/PKG-INFO
```

### Comparing `nsdpy-0.3.1b0/LICENSE` & `nsdpy-0.3.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.1b0/README.md` & `nsdpy-0.3.2b0/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.1b0/functions.py` & `nsdpy-0.3.2b0/functions.py`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.1b0/nsdpy.py` & `nsdpy-0.3.2b0/nsdpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-__version__ = '0.3.1-beta'
+__version__ = '0.3.2-beta'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
 import sys
 import os
 import argparse                     #parsing command line arguments
 from datetime import datetime    
 
 # local imports
-from .constants import ESEARCH_URL
-from .functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
+import constants
+from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
 
 
 def main():
 ############################################
 ###### CHECK COMMAND LINE ARGUMENTS ########
 ############################################
 
@@ -147,15 +147,15 @@
             with open(file, "r") as data:
                 taxa_list = taxa_list + data.read().splitlines()
         
         # Add the taxa to the query
         taxa_list = [ taxon + "[ORGN] OR " for taxon in taxa_list]
 
         # Base URL with params
-        esearch_address = ESEARCH_URL
+        esearch_address = constants.ESEARCH_URL
         base_URL_length = len(esearch_address) + 100 # Keep 100 chars for params
 
         # Base query
         base_query = args.request + " AND ("
         
         # Remaining space for the taxa list 
         taxa_max_length = 2048 - ( len(base_query) + base_URL_length )
```

### Comparing `nsdpy-0.3.1b0/pyproject.toml` & `nsdpy-0.3.2b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = "0.3.1-beta"
+version = "0.3.2-beta"
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.3.1b0/PKG-INFO` & `nsdpy-0.3.2b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdpy
-Version: 0.3.1b0
+Version: 0.3.2b0
 Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
 Home-page: https://github.com/RaphaelHebert/nsdpy
 License: MIT
 Keywords: NCBI,Taxonomy,DNA
 Author: RaphaelHebert
 Author-email: raphaelhebert18@gmail.com
 Requires-Python: >=3.8,<4.0
```

