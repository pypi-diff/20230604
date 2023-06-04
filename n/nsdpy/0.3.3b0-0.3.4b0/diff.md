# Comparing `tmp/nsdpy-0.3.3b0.tar.gz` & `tmp/nsdpy-0.3.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.3.3b0.tar", max compression
+gzip compressed data, was "nsdpy-0.3.4b0.tar", max compression
```

## Comparing `nsdpy-0.3.3b0.tar` & `nsdpy-0.3.4b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.3b0/LICENSE
--rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.3b0/README.md
--rw-r--r--   0        0        0    34776 2023-06-04 14:34:07.888380 nsdpy-0.3.3b0/functions.py
--rw-r--r--   0        0        0    12984 2023-06-04 14:35:43.213733 nsdpy-0.3.3b0/nsdpy.py
--rw-r--r--   0        0        0      841 2023-06-04 14:35:46.358656 nsdpy-0.3.3b0/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.3b0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.4b0/LICENSE
+-rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.4b0/README.md
+-rw-r--r--   0        0        0    34766 2023-06-04 14:44:25.311303 nsdpy-0.3.4b0/functions.py
+-rw-r--r--   0        0        0    12975 2023-06-04 14:46:25.455939 nsdpy-0.3.4b0/nsdpy.py
+-rw-r--r--   0        0        0      841 2023-06-04 14:46:34.741645 nsdpy-0.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.4b0/PKG-INFO
```

### Comparing `nsdpy-0.3.3b0/LICENSE` & `nsdpy-0.3.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.3b0/README.md` & `nsdpy-0.3.4b0/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.3b0/functions.py` & `nsdpy-0.3.4b0/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
  #import from standard library
 import os
 import re
 import csv
 from collections import Counter
-from constants.constants import *
+from constants import *
 #third party imports
 import requests             #https://requests.readthedocs.io/en/master/
 
     
 def countDown(iteration, total, message=''):
     """
     Take the number of iteration, the range of a forloop and a message and output a message with the percent of job done
```

### Comparing `nsdpy-0.3.3b0/nsdpy.py` & `nsdpy-0.3.4b0/nsdpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 __version__ = '0.3.3-beta'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
+# local imports
+from constants import *
+from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
+
 import sys
 import os
 import argparse                     #parsing command line arguments
 from datetime import datetime    
 
-# local imports
-from constants.constants import *
-from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
 
 
 def main():
 ############################################
 ###### CHECK COMMAND LINE ARGUMENTS ########
 ############################################
```

### Comparing `nsdpy-0.3.3b0/pyproject.toml` & `nsdpy-0.3.4b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = "0.3.3-beta"
+version = '0.3.4-beta'
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.3.3b0/PKG-INFO` & `nsdpy-0.3.4b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdpy
-Version: 0.3.3b0
+Version: 0.3.4b0
 Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
 Home-page: https://github.com/RaphaelHebert/nsdpy
 License: MIT
 Keywords: NCBI,Taxonomy,DNA
 Author: RaphaelHebert
 Author-email: raphaelhebert18@gmail.com
 Requires-Python: >=3.8,<4.0
```

