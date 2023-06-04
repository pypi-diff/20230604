# Comparing `tmp/nsdpy-0.3.4b0.tar.gz` & `tmp/nsdpy-0.3.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.3.4b0.tar", max compression
+gzip compressed data, was "nsdpy-0.3.5b0.tar", max compression
```

## Comparing `nsdpy-0.3.4b0.tar` & `nsdpy-0.3.5b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.4b0/LICENSE
--rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.4b0/README.md
--rw-r--r--   0        0        0    34766 2023-06-04 14:44:25.311303 nsdpy-0.3.4b0/functions.py
--rw-r--r--   0        0        0    12975 2023-06-04 14:46:25.455939 nsdpy-0.3.4b0/nsdpy.py
--rw-r--r--   0        0        0      841 2023-06-04 14:46:34.741645 nsdpy-0.3.4b0/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.4b0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.5b0/LICENSE
+-rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.5b0/README.md
+-rw-r--r--   0        0        0    35941 2023-06-04 14:52:45.584025 nsdpy-0.3.5b0/functions.py
+-rw-r--r--   0        0        0    13024 2023-06-04 14:53:26.111581 nsdpy-0.3.5b0/nsdpy.py
+-rw-r--r--   0        0        0      841 2023-06-04 14:53:27.677228 nsdpy-0.3.5b0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.5b0/PKG-INFO
```

### Comparing `nsdpy-0.3.4b0/LICENSE` & `nsdpy-0.3.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.4b0/README.md` & `nsdpy-0.3.5b0/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.4b0/functions.py` & `nsdpy-0.3.5b0/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,31 @@
  #import from standard library
 import os
 import re
 import csv
 from collections import Counter
-from constants import *
 #third party imports
 import requests             #https://requests.readthedocs.io/en/master/
 
+ESEARCH_URL = 'https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi'
+ESUMMARY_URL = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esummary.fcgi"
+EFETCH_URL = "https://eutils.ncbi.nlm.nih.gov/entrez/eutils/efetch.fcgi"
+
+PLANTAE = ['Chlorophyta', 'Charophyta', 'Bryophyta', 'Marchantiophyta', 'Lycopodiophyta', 'Ophioglossophyta', 'Pteridophyta',\
+    'Cycadophyta', 'Ginkgophyta', 'Gnetophyta', 'Pinophyta', 'Magnoliophyta', 'Equisetidae', 'Psilophyta', 'Bacillariophyta',\
+    'Cyanidiophyta', 'Glaucophyta', 'Prasinophyceae','Rhodophyta']
+
+FUNGI = ['Chytridiomycota', 'Zygomycota', 'Ascomycota', 'Basidiomycota', 'Glomeromycota']
+
+METAZOA = ['Acanthocephala', 'Acoelomorpha', 'Annelida', 'Arthropoda', 'Brachiopoda', 'Ectoprocta', 'Bryozoa', 'Chaetognatha',\
+    'Chordata', 'Cnidaria', 'Ctenophora', 'Cycliophora', 'Echinodermata', 'Echiura', 'Entoprocta', 'Gastrotricha', 'Gnathostomulida',\
+    'Hemichordata', 'Kinorhyncha', 'Loricifera', 'Micrognathozoa', 'Mollusca', 'Nematoda', 'Nematomorpha', 'Nemertea', 'Onychophora'\
+    'Orthonectida', 'Phoronida', 'Placozoa', 'Plathelminthes', 'Porifera', 'Priapulida', 'Rhombozoa', 'Rotifera', 'Sipuncula',\
+    'Tardigrada', 'Xenoturbella']
+
     
 def countDown(iteration, total, message=''):
     """
     Take the number of iteration, the range of a forloop and a message and output a message with the percent of job done
 
     INPUTS: countDown(iteration, total, message='')
     iteration:  positive INT
```

### Comparing `nsdpy-0.3.4b0/nsdpy.py` & `nsdpy-0.3.5b0/nsdpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-__version__ = '0.3.3-beta'
+__version__ = '0.3.5-beta'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
-# local imports
-from constants import *
-from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
-
 import sys
 import os
 import argparse                     #parsing command line arguments
 from datetime import datetime    
 
+# local imports
+
+from functions import esearchquery, completetaxo, taxids, cds_fasta, taxo, fasta, duplicates
 
+ESEARCH_URL='https://eutils.ncbi.nlm.nih.gov/entrez/eutils/esearch.fcgi'
 
 def main():
 ############################################
 ###### CHECK COMMAND LINE ARGUMENTS ########
 ############################################
 
     parser = argparse.ArgumentParser()
```

### Comparing `nsdpy-0.3.4b0/pyproject.toml` & `nsdpy-0.3.5b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = '0.3.4-beta'
+version = "0.3.5-beta"
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.3.4b0/PKG-INFO` & `nsdpy-0.3.5b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdpy
-Version: 0.3.4b0
+Version: 0.3.5b0
 Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
 Home-page: https://github.com/RaphaelHebert/nsdpy
 License: MIT
 Keywords: NCBI,Taxonomy,DNA
 Author: RaphaelHebert
 Author-email: raphaelhebert18@gmail.com
 Requires-Python: >=3.8,<4.0
```

