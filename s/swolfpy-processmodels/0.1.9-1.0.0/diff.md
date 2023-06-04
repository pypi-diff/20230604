# Comparing `tmp/swolfpy_processmodels-0.1.9.tar.gz` & `tmp/swolfpy_processmodels-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\swolfpy_processmodels-0.1.9.tar", last modified: Wed Apr  6 04:09:07 2022, max compression
+gzip compressed data, was "swolfpy_processmodels-1.0.0.tar", last modified: Sun Jun  4 18:01:52 2023, max compression
```

## Comparing `swolfpy_processmodels-0.1.9.tar` & `swolfpy_processmodels-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-04-06 04:09:07.000000 swolfpy_processmodels-0.1.9/
--rw-rw-rw-   0        0        0      749 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     1674 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      676 2022-04-06 04:08:36.000000 swolfpy_processmodels-0.1.9/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/LICENSE.md
--rw-rw-rw-   0        0        0      273 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     8587 2022-04-06 04:09:07.000000 swolfpy_processmodels-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     5370 2022-04-06 03:54:56.000000 swolfpy_processmodels-0.1.9/README.rst
--rw-rw-rw-   0        0        0       42 2022-04-06 04:09:07.000000 swolfpy_processmodels-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     2118 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-06 04:09:06.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/
--rw-rw-rw-   0        0        0    23021 2021-11-25 12:14:16.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/AD.py
--rw-rw-rw-   0        0        0    26822 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/AD_subprocess.py
--rw-rw-rw-   0        0        0     8726 2022-02-10 18:17:25.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/AnF.py
--rw-rw-rw-   0        0        0    36943 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/COM_Col.py
--rw-rw-rw-   0        0        0    13596 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/Common_subprocess.py
--rw-rw-rw-   0        0        0    14367 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/Comp.py
--rw-rw-rw-   0        0        0    13981 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/Comp_subprocess.py
--rw-rw-rw-   0        0        0     3422 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/Distance.py
--rw-rw-rw-   0        0        0    26110 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/GC.py
--rw-rw-rw-   0        0        0     6113 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/HC.py
--rw-rw-rw-   0        0        0     4173 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/HC_subprocess.py
--rw-rw-rw-   0        0        0    41739 2021-11-25 12:14:16.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/LF.py
--rw-rw-rw-   0        0        0    36842 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/MF_Col.py
--rw-rw-rw-   0        0        0    29451 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/MRF_subprocess.py
--rw-rw-rw-   0        0        0      923 2021-10-02 16:43:47.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/ProcessModel.py
--rw-rw-rw-   0        0        0     4342 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/ProcessModelsMetaData.py
--rw-rw-rw-   0        0        0    11182 2021-10-02 16:35:14.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/RDF.py
--rw-rw-rw-   0        0        0     1910 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/Reproc.py
--rw-rw-rw-   0        0        0    40433 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/SF_Col.py
--rw-rw-rw-   0        0        0    12426 2022-03-04 22:06:33.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/SS_MRF.py
--rw-rw-rw-   0        0        0     4836 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/TS.py
--rw-rw-rw-   0        0        0     4840 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/TS_subprocess.py
--rw-rw-rw-   0        0        0    16711 2022-02-10 00:51:06.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/WTE.py
--rw-rw-rw-   0        0        0      887 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-06 04:09:07.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/
--rw-rw-rw-   0        0        0     8587 2022-04-06 04:09:02.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1209 2022-04-06 04:09:03.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-06 04:09:02.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-04-06 04:09:02.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       82 2022-04-06 04:09:02.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2022-04-06 04:09:02.000000 swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-06 04:09:07.000000 swolfpy_processmodels-0.1.9/tests/
--rw-rw-rw-   0        0        0      149 2021-08-24 20:24:04.000000 swolfpy_processmodels-0.1.9/tests/__init__.py
--rw-rw-rw-   0        0        0     4864 2022-02-03 21:42:35.000000 swolfpy_processmodels-0.1.9/tests/test_processmodels.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.603304 swolfpy_processmodels-1.0.0/
+-rw-rw-rw-   0        0        0      748 2023-06-04 17:34:44.000000 swolfpy_processmodels-1.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1674 2022-11-25 05:39:51.000000 swolfpy_processmodels-1.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      768 2023-06-04 17:34:44.000000 swolfpy_processmodels-1.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    18431 2022-11-25 05:03:08.000000 swolfpy_processmodels-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0      273 2023-02-26 03:37:23.000000 swolfpy_processmodels-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7498 2023-06-04 18:01:52.602305 swolfpy_processmodels-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5365 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/README.rst
+-rw-rw-rw-   0        0        0    10501 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      124 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:01:52.604305 swolfpy_processmodels-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.529304 swolfpy_processmodels-1.0.0/swolfpy_processmodels/
+-rw-rw-rw-   0        0        0    24138 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD.py
+-rw-rw-rw-   0        0        0    26334 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD_subprocess.py
+-rw-rw-rw-   0        0        0     8517 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/AnF.py
+-rw-rw-rw-   0        0        0    38421 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/COM_Col.py
+-rw-rw-rw-   0        0        0    14792 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Common_subprocess.py
+-rw-rw-rw-   0        0        0    14479 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Comp.py
+-rw-rw-rw-   0        0        0    14643 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Comp_subprocess.py
+-rw-rw-rw-   0        0        0     3388 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Distance.py
+-rw-rw-rw-   0        0        0    26389 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/GC.py
+-rw-rw-rw-   0        0        0     6748 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC.py
+-rw-rw-rw-   0        0        0     3998 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC_subprocess.py
+-rw-rw-rw-   0        0        0    44003 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/LF.py
+-rw-rw-rw-   0        0        0    37798 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/MF_Col.py
+-rw-rw-rw-   0        0        0    30289 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/MRF_subprocess.py
+-rw-rw-rw-   0        0        0      858 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModel.py
+-rw-rw-rw-   0        0        0     4335 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModelsMetaData.py
+-rw-rw-rw-   0        0        0    10116 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/RDF.py
+-rw-rw-rw-   0        0        0     1848 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/Reproc.py
+-rw-rw-rw-   0        0        0    42618 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/SF_Col.py
+-rw-rw-rw-   0        0        0    14816 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/SS_MRF.py
+-rw-rw-rw-   0        0        0     5203 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS.py
+-rw-rw-rw-   0        0        0     5036 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS_subprocess.py
+-rw-rw-rw-   0        0        0    17518 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/WTE.py
+-rw-rw-rw-   0        0        0      744 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.571304 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/
+-rw-rw-rw-   0        0        0     7498 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1188 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-04 18:01:51.000000 swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 18:01:52.597305 swolfpy_processmodels-1.0.0/tests/
+-rw-rw-rw-   0        0        0       79 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4801 2023-06-04 17:34:45.000000 swolfpy_processmodels-1.0.0/tests/test_processmodels.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swolfpy_processmodels-0.1.9/AUTHORS.rst` & `swolfpy_processmodels-1.0.0/AUTHORS.rst`

 * *Files 14% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 * Prof. Ranji Ranjithan <ranji@ncsu.edu>
 * Dr. Joe DeCarolis <jfdecaro@ncsu.edu>
 
 
 
 Acknowledgements
 ----------------
-This work was supported by the National Science Foundation(Awards Numbers: `CBET-1437498`_ and  `CBET-1034059`_) and  Environmental Research and Educational Foundation (`EREF`_). 
+This work was supported by the National Science Foundation(Awards Numbers: `CBET-1437498`_ and  `CBET-1034059`_) and  Environmental Research and Educational Foundation (`EREF`_).
 
 .. _CBET-1437498: https://nsf.gov/awardsearch/showAward?AWD_ID=1437498
 .. _CBET-1034059: https://nsf.gov/awardsearch/showAward?AWD_ID=1034059
 .. _EREF: https://erefdn.org/
```

### Comparing `swolfpy_processmodels-0.1.9/CONTRIBUTING.rst` & `swolfpy_processmodels-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-0.1.9/HISTORY.rst` & `swolfpy_processmodels-1.0.0/HISTORY.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 =======
 History
 =======
 
+1.0.0 (2023-06-03)
+------------------
+
+* Upgrade to Python 3.10
+* Add PreCommit
+
+
 0.1.9 (2022-04-06)
 ------------------
+
 * Add Multi-family and commercial Waste collection
 * Add Animal feed production
 * Refactor SF-collection model
 
 
 0.1.8 (2021-11-25)
 ------------------
@@ -22,15 +30,15 @@
 * Add Gasification & Syngas combustion (GC)
 * Add Refuse-derived fuel (RDF)
 
 
 0.1.4 (2021-05-10)
 ------------------
 
-* New Life-cyle model: TS
+* New Life-cycle model: TS
 * Add Cost calculations
 
 
 
 0.1.0 (2020-05-06)
 ------------------
```

### Comparing `swolfpy_processmodels-0.1.9/LICENSE.md` & `swolfpy_processmodels-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swolfpy_processmodels-0.1.9/PKG-INFO` & `swolfpy_processmodels-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,201 +1,210 @@
 Metadata-Version: 2.1
 Name: swolfpy_processmodels
-Version: 0.1.9
-Summary: Life-Cylce Process Models for swolfpy (swolfpy_processmodels)
-Home-page: https://github.com/SwolfPy-Project/swolfpy-processmodels
-Author: Mojtaba Sardarmehni
-Author-email: msardar2@ncsu.edu
+Version: 1.0.0
+Summary: Life-Cylce Process Models for swolfpy (swolfpy_processmodels).
+Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
+Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
-Description: .. General
-        
-        ==============================================================
-        Life-Cycle Process Models for SwolfPy (swolfpy_processmodels)
-        ==============================================================
-        
-        .. image:: https://img.shields.io/pypi/v/swolfpy_processmodels.svg
-                :target: https://pypi.python.org/pypi/swolfpy_processmodels
-                
-        .. image:: https://img.shields.io/pypi/pyversions/swolfpy_processmodels.svg
-            :target: https://pypi.org/project/swolfpy_processmodels/
-            :alt: Supported Python Versions
-        
-        .. image:: https://img.shields.io/pypi/l/swolfpy_processmodels.svg
-            :target: https://pypi.org/project/swolfpy_processmodels/
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/dm/swolfpy-processmodels.svg?label=Pypi%20downloads
-            :target: https://pypi.org/project/swolfpy-processmodels/
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/format/swolfpy_processmodels.svg
-            :target: https://pypi.org/project/swolfpy_processmodels/
-            :alt: Format
-        
-        .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
-                :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml/badge.svg?branch=master
-                :target: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml
-                :alt: Test
-        
-        .. image:: https://zenodo.org/badge/395802174.svg
-                :target: https://zenodo.org/badge/latestdoi/395802174
-                :alt: DOI
-        
-        .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
-           :target: https://doi.org/10.1111/jiec.13236
-           :alt: JIE DOI
-        
-        
-        * Free software: GNU GENERAL PUBLIC LICENSE V2
-        * Website: https://swolfpy-project.github.io
-        * Documentation: https://swolfpy.readthedocs.io.
-        * Repository: https://github.com/SwolfPy-Project/swolfpy-processmodels
-        
-        
-        Features
-        --------
-        * Life-cycle process models for solid waste management (SWM) processes.
-        * Built-in Monte Carlo simulation
-        
-        .. list-table:: **Life-cycle process models**
-           :widths: auto
-           :header-rows: 1
-        
-           * - 
-             - Process model 
-             - Description
-           * - 1
-             - Landfill (**LF**)
-             - Calculates emissions, material use, and energy use associated with construction, operations, 
-               closure and post-closure activities, landfill gas and leachate management, and carbon storage.
-           * - 2
-             - Waste-to-Energy (**WTE**)
-             - Calculates emissions, mass flows, and resource use and recovery for the mass burn WTE process.
-           * - 3
-             - Gasification & Syngas Combustion (**GC**)
-             - Calculates emissions, mass flows, and resource use and recovery for the GC process (Produced syngas from
-               gasification is combusted to produce electricity by steam turbine). 
-           * - 4
-             - Composting (**Comp**)
-             - Calculates emissions, mass flows, and resource use and recovery for aerobic composting process and final use of compost.
-           * - 5
-             - Home Composting (**HC**)
-             - Calculates emissions, mass flows, and resource use and recovery for home composting process and final use of compost.
-           * - 6
-             - Anaerobic Digestion (**AD**)
-             - Calculates emissions, mass flows, and resource use and recovery for anaerobic digestion process and final use of compost.
-           * - 7
-             - Single-Stream Material Recovery facility (**SS_MRF**)
-             - Calculates cost, emissions, and energy use associated with material recovery facilities.
-           * - 8
-             - Refuse-Derived Fuel (**RDF**)
-             - Calculates cost, emissions, and energy use associated with RDF production facilities.
-           * - 9
-             - Reprocessing (**Reproc**)
-             - Calculates emissions, mass flows, and resource use and recovery associated with recycling materials.	 
-           * - 10
-             - Transfer Station (**TS**)
-             - Calculates cost, emissions, and energy use associated with Transfer Stations.
-           * - 11
-             - Single Family Collection (**SF_Col**)
-             - Calculates cost, emissions, and fossil fuel use associated with MSW collection from single family sector.
-           * - 12
-             - Multi Family Collection (**MF_Col**)
-             - Calculates cost, emissions, and fossil fuel use associated with MSW collection from multi-family sector.
-           * - 13
-             - Collection (**COM_Col**)
-             - Calculates cost, emissions, and fossil fuel use associated with MSW collection from commercial sector.
-           * - 14
-             - Animal Feed (**AnF**)
-             - Calculates cost, emissions, and energy use associated with conversion of food waste to animal feed and final use of produced feed.
-          
-        .. Installation
-        
-        Installation
-        ------------
-        1- Download and install miniconda from:  https://docs.conda.io/en/latest/miniconda.html
-        
-        2- Update conda in a terminal window or anaconda prompt::
-        
-                conda update conda
-        
-        3- Create a new environment for swolfpy::
-        
-                conda create --name swolfpy python=3.7
-        
-        4- Activate the environment::
-        
-                conda activate swolfpy
-        
-        5- Install swolfpy_processmodels in the environment::
-        
-                pip install swolfpy_processmodels
-        
-        6- Use in python (e.g., Landfill model)::
-        
-                import swolfpy_processmodels as sppm 
-                model = sppm.LF()
-                model.calc()
-                LCI_report = model.report()
-                LCI_report
-        
-        .. endInstallation
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.9 (2022-04-06)
-        ------------------
-        * Add Multi-family and commercial Waste collection
-        * Add Animal feed production
-        * Refactor SF-collection model
-        
-        
-        0.1.8 (2021-11-25)
-        ------------------
-        
-        * Update Landfill model.
-        
-        
-        0.1.6 (2021-10-02)
-        ------------------
-        
-        * Add Home Composting (HC)
-        * Add Gasification & Syngas combustion (GC)
-        * Add Refuse-derived fuel (RDF)
-        
-        
-        0.1.4 (2021-05-10)
-        ------------------
-        
-        * New Life-cyle model: TS
-        * Add Cost calculations
-        
-        
-        
-        0.1.0 (2020-05-06)
-        ------------------
-        
-        * First release on PyPI. Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
-        
-Keywords: swolfpy_processmodels
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://swolfpy-project.github.io/
+Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-processmodels
+Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE.md
+License-File: AUTHORS.rst
+
+.. General
+
+==============================================================
+Life-Cycle Process Models for SwolfPy (swolfpy_processmodels)
+==============================================================
+
+.. image:: https://img.shields.io/pypi/v/swolfpy_processmodels.svg
+        :target: https://pypi.python.org/pypi/swolfpy_processmodels
+
+.. image:: https://img.shields.io/pypi/pyversions/swolfpy_processmodels.svg
+    :target: https://pypi.org/project/swolfpy_processmodels/
+    :alt: Supported Python Versions
+
+.. image:: https://img.shields.io/pypi/l/swolfpy_processmodels.svg
+    :target: https://pypi.org/project/swolfpy_processmodels/
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/swolfpy-processmodels.svg?label=Pypi%20downloads
+    :target: https://pypi.org/project/swolfpy-processmodels/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/format/swolfpy_processmodels.svg
+    :target: https://pypi.org/project/swolfpy_processmodels/
+    :alt: Format
+
+.. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
+        :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml/badge.svg?branch=master
+        :target: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml
+        :alt: Test
+
+.. image:: https://zenodo.org/badge/395802174.svg
+        :target: https://zenodo.org/badge/latestdoi/395802174
+        :alt: DOI
+
+.. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
+   :target: https://doi.org/10.1111/jiec.13236
+   :alt: JIE DOI
+
+
+* Free software: GNU GENERAL PUBLIC LICENSE V2
+* Website: https://swolfpy-project.github.io
+* Documentation: https://swolfpy.readthedocs.io.
+* Repository: https://github.com/SwolfPy-Project/swolfpy-processmodels
+
+
+Features
+--------
+* Life-cycle process models for solid waste management (SWM) processes.
+* Built-in Monte Carlo simulation
+
+.. list-table:: **Life-cycle process models**
+   :widths: auto
+   :header-rows: 1
+
+   * -
+     - Process model
+     - Description
+   * - 1
+     - Landfill (**LF**)
+     - Calculates emissions, material use, and energy use associated with construction, operations,
+       closure and post-closure activities, landfill gas and leachate management, and carbon storage.
+   * - 2
+     - Waste-to-Energy (**WTE**)
+     - Calculates emissions, mass flows, and resource use and recovery for the mass burn WTE process.
+   * - 3
+     - Gasification & Syngas Combustion (**GC**)
+     - Calculates emissions, mass flows, and resource use and recovery for the GC process (Produced syngas from
+       gasification is combusted to produce electricity by steam turbine).
+   * - 4
+     - Composting (**Comp**)
+     - Calculates emissions, mass flows, and resource use and recovery for aerobic composting process and final use of compost.
+   * - 5
+     - Home Composting (**HC**)
+     - Calculates emissions, mass flows, and resource use and recovery for home composting process and final use of compost.
+   * - 6
+     - Anaerobic Digestion (**AD**)
+     - Calculates emissions, mass flows, and resource use and recovery for anaerobic digestion process and final use of compost.
+   * - 7
+     - Single-Stream Material Recovery facility (**SS_MRF**)
+     - Calculates cost, emissions, and energy use associated with material recovery facilities.
+   * - 8
+     - Refuse-Derived Fuel (**RDF**)
+     - Calculates cost, emissions, and energy use associated with RDF production facilities.
+   * - 9
+     - Reprocessing (**Reproc**)
+     - Calculates emissions, mass flows, and resource use and recovery associated with recycling materials.
+   * - 10
+     - Transfer Station (**TS**)
+     - Calculates cost, emissions, and energy use associated with Transfer Stations.
+   * - 11
+     - Single Family Collection (**SF_Col**)
+     - Calculates cost, emissions, and fossil fuel use associated with MSW collection from single family sector.
+   * - 12
+     - Multi Family Collection (**MF_Col**)
+     - Calculates cost, emissions, and fossil fuel use associated with MSW collection from multi-family sector.
+   * - 13
+     - Commercial Collection (**COM_Col**)
+     - Calculates cost, emissions, and fossil fuel use associated with MSW collection from commercial sector.
+   * - 14
+     - Animal Feed (**AnF**)
+     - Calculates cost, emissions, and energy use associated with conversion of food waste to animal feed and final use of produced feed.
+
+.. Installation
+
+Installation
+------------
+1- Download and install miniconda from:  https://docs.conda.io/en/latest/miniconda.html
+
+2- Update conda in a terminal window or anaconda prompt::
+
+        conda update conda
+
+3- Create a new environment for swolfpy::
+
+        conda create --name swolfpy python=3.10
+
+4- Activate the environment::
+
+        conda activate swolfpy
+
+5- Install swolfpy_processmodels in the environment::
+
+        pip install swolfpy_processmodels
+
+6- Use in python (e.g., Landfill model)::
+
+        import swolfpy_processmodels as sppm
+        model = sppm.LF()
+        model.calc()
+        LCI_report = model.report()
+        LCI_report
+
+.. endInstallation
+
+=======
+History
+=======
+
+1.0.0 (2023-06-03)
+------------------
+
+* Upgrade to Python 3.10
+* Add PreCommit
+
+
+0.1.9 (2022-04-06)
+------------------
+
+* Add Multi-family and commercial Waste collection
+* Add Animal feed production
+* Refactor SF-collection model
+
+
+0.1.8 (2021-11-25)
+------------------
+
+* Update Landfill model.
+
+
+0.1.6 (2021-10-02)
+------------------
+
+* Add Home Composting (HC)
+* Add Gasification & Syngas combustion (GC)
+* Add Refuse-derived fuel (RDF)
+
+
+0.1.4 (2021-05-10)
+------------------
+
+* New Life-cycle model: TS
+* Add Cost calculations
+
+
+
+0.1.0 (2020-05-06)
+------------------
+
+* First release on PyPI. Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
```

### Comparing `swolfpy_processmodels-0.1.9/README.rst` & `swolfpy_processmodels-1.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ==============================================================
 Life-Cycle Process Models for SwolfPy (swolfpy_processmodels)
 ==============================================================
 
 .. image:: https://img.shields.io/pypi/v/swolfpy_processmodels.svg
         :target: https://pypi.python.org/pypi/swolfpy_processmodels
-        
+
 .. image:: https://img.shields.io/pypi/pyversions/swolfpy_processmodels.svg
     :target: https://pypi.org/project/swolfpy_processmodels/
     :alt: Supported Python Versions
 
 .. image:: https://img.shields.io/pypi/l/swolfpy_processmodels.svg
     :target: https://pypi.org/project/swolfpy_processmodels/
     :alt: License
@@ -51,28 +51,28 @@
 * Life-cycle process models for solid waste management (SWM) processes.
 * Built-in Monte Carlo simulation
 
 .. list-table:: **Life-cycle process models**
    :widths: auto
    :header-rows: 1
 
-   * - 
-     - Process model 
+   * -
+     - Process model
      - Description
    * - 1
      - Landfill (**LF**)
-     - Calculates emissions, material use, and energy use associated with construction, operations, 
+     - Calculates emissions, material use, and energy use associated with construction, operations,
        closure and post-closure activities, landfill gas and leachate management, and carbon storage.
    * - 2
      - Waste-to-Energy (**WTE**)
      - Calculates emissions, mass flows, and resource use and recovery for the mass burn WTE process.
    * - 3
      - Gasification & Syngas Combustion (**GC**)
      - Calculates emissions, mass flows, and resource use and recovery for the GC process (Produced syngas from
-       gasification is combusted to produce electricity by steam turbine). 
+       gasification is combusted to produce electricity by steam turbine).
    * - 4
      - Composting (**Comp**)
      - Calculates emissions, mass flows, and resource use and recovery for aerobic composting process and final use of compost.
    * - 5
      - Home Composting (**HC**)
      - Calculates emissions, mass flows, and resource use and recovery for home composting process and final use of compost.
    * - 6
@@ -82,55 +82,55 @@
      - Single-Stream Material Recovery facility (**SS_MRF**)
      - Calculates cost, emissions, and energy use associated with material recovery facilities.
    * - 8
      - Refuse-Derived Fuel (**RDF**)
      - Calculates cost, emissions, and energy use associated with RDF production facilities.
    * - 9
      - Reprocessing (**Reproc**)
-     - Calculates emissions, mass flows, and resource use and recovery associated with recycling materials.	 
+     - Calculates emissions, mass flows, and resource use and recovery associated with recycling materials.
    * - 10
      - Transfer Station (**TS**)
      - Calculates cost, emissions, and energy use associated with Transfer Stations.
    * - 11
      - Single Family Collection (**SF_Col**)
      - Calculates cost, emissions, and fossil fuel use associated with MSW collection from single family sector.
    * - 12
      - Multi Family Collection (**MF_Col**)
      - Calculates cost, emissions, and fossil fuel use associated with MSW collection from multi-family sector.
    * - 13
-     - Collection (**COM_Col**)
+     - Commercial Collection (**COM_Col**)
      - Calculates cost, emissions, and fossil fuel use associated with MSW collection from commercial sector.
    * - 14
      - Animal Feed (**AnF**)
      - Calculates cost, emissions, and energy use associated with conversion of food waste to animal feed and final use of produced feed.
-  
+
 .. Installation
 
 Installation
 ------------
 1- Download and install miniconda from:  https://docs.conda.io/en/latest/miniconda.html
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.7
+        conda create --name swolfpy python=3.10
 
 4- Activate the environment::
 
         conda activate swolfpy
 
 5- Install swolfpy_processmodels in the environment::
 
         pip install swolfpy_processmodels
 
 6- Use in python (e.g., Landfill model)::
 
-        import swolfpy_processmodels as sppm 
+        import swolfpy_processmodels as sppm
         model = sppm.LF()
         model.calc()
         LCI_report = model.report()
         LCI_report
 
 .. endInstallation
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/AD.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,412 +1,603 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Jul 17 16:35:15 2019
-
-@author: msardar2
-"""
-from .ProcessModel import ProcessModel
-from swolfpy_inputdata import AD_Input
-from .Common_subprocess import Flow, LCI
-from .Common_subprocess import compost_use
-from .AD_subprocess import screen, Post_screen, mix, curing
-from .AD_subprocess import add_water, Reactor, Dewater
 import numpy_financial as npf
 import plotly.graph_objects as go
 from plotly.offline import plot
+from swolfpy_inputdata import AD_Input
+
+from .AD_subprocess import Dewater, Post_screen, Reactor, add_water, curing, mix, screen
+from .Common_subprocess import LCI, Flow, compost_use
+from .ProcessModel import ProcessModel
 
 
 class AD(ProcessModel):
-    Process_Type = 'Treatment'
-    def __init__(self, process_name='AD', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Treatment"
+
+    def __init__(self, process_name="AD", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = AD_Input(input_data_path=input_data_path,
-                                  process_name=self.process_name,
-                                  CommonDataObjct=CommonDataObjct)
+        self.InputData = AD_Input(
+            input_data_path=input_data_path,
+            process_name=self.process_name,
+            CommonDataObjct=CommonDataObjct,
+        )
 
-        self.Assumed_Comp = self.InputData.process_data['Assumed_Comp']
+        self.Assumed_Comp = self.InputData.process_data["Assumed_Comp"]
 
         self.process_data = self.InputData.process_data
 
         self.flow_init = Flow(self.Material_Properties)
 
     def calc(self):
         self.LCI = LCI(index=self.Index, n_col=51)
 
         # Methane Yield (m3/dry Mg)
-        self.Material_Properties['Methane Yield'] = (
-            self.Material_Properties['Biogenic Carbon Content'].values / 100
-            * self.Material_Properties['Ultimate Biogenic C Converted to Biogas'].values / 100
-            * self.CommonData.STP['mole_to_L']['amount']
-            / self.CommonData.MW['C']['amount']
+        self.Material_Properties["Methane Yield"] = (
+            self.Material_Properties["Biogenic Carbon Content"].values
+            / 100
+            * self.Material_Properties["Ultimate Biogenic C Converted to Biogas"].values
+            / 100
+            * self.CommonData.STP["mole_to_L"]["amount"]
+            / self.CommonData.MW["C"]["amount"]
             * 0.5
-            * 1000)
+            * 1000
+        )
 
         ### Initial mass
         self.Input = Flow(self.Material_Properties)
         self.Input.init_flow(1000)
 
         ### Primary Pre_screen
-        self.S1_unders, self.S1_overs = screen(self.Input,
-                                               self.process_data['Pre Screen 1'].values / 100,
-                                               self.Material_Properties,
-                                               self.LCI,
-                                               self.flow_init)
+        self.S1_unders, self.S1_overs = screen(
+            self.Input,
+            self.process_data["Pre Screen 1"].values / 100,
+            self.flow_init,
+        )
 
         ### Secondary Pre_screen
-        self.S2_to_curing, self.S2_residuls = screen(self.S1_overs,
-                                                     self.process_data['Pre Screen 2'].values / 100,
-                                                     self.Material_Properties,
-                                                     self.LCI,
-                                                     self.flow_init)
+        self.S2_to_curing, self.S2_residuals = screen(
+            self.S1_overs,
+            self.process_data["Pre Screen 2"].values / 100,
+            self.flow_init,
+        )
 
-        self.LCI.add(name='Residual',
-             flow=self.S2_residuls.data['mass'].values / 1000)
+        self.LCI.add(name="Residual", flow=self.S2_residuals.data["mass"].values / 1000)
 
         # Dsl use for grinding
-        self.LCI.add(name=('Technosphere', 'Equipment_Diesel'),
-                     flow=(self.S2_to_curing.data['mass'].values / 1000
-                           * self.InputData.shredding['Mtgp']['amount']
-                           * self.InputData.shredding['Mtgf']['amount']))
+        self.LCI.add(
+            name=("Technosphere", "Equipment_Diesel"),
+            flow=(
+                self.S2_to_curing.data["mass"].values
+                / 1000
+                * self.InputData.shredding["Mtgp"]["amount"]
+                * self.InputData.shredding["Mtgf"]["amount"]
+            ),
+        )
 
         ### Adding Water
         """
         M: Moisture, S: solids, Liq: Added water, mc=moisture content
         mc = (Liq + M)/(S + M + Liq)
         mc*Liq = Liq + M - S*mc - mc*M
         Liq = (M - S*mc - mc*M)/(mc-1)
         S + M = mass ==> Liq = (M - mass*mc)/(mc-1)
         Liq = (mass*mc - M)/(1-mc)
         """
-        self.water_flow = ((self.S1_unders.data['mass'].values
-                            * self.InputData.Material_Properties['ad_mcReactor']['amount']
-                            - self.S1_unders.data['moist_cont'].values)
-                           / (1 - self.InputData.Material_Properties['ad_mcReactor']['amount']))
-
-        self.to_reactor = add_water(self.S1_unders,
-                                    self.water_flow,
-                                    self.Material_Properties,
-                                    self.process_data,
-                                    self.flow_init)
+        self.water_flow = (
+            self.S1_unders.data["mass"].values
+            * self.InputData.Material_Properties["ad_mcReactor"]["amount"]
+            - self.S1_unders.data["moist_cont"].values
+        ) / (1 - self.InputData.Material_Properties["ad_mcReactor"]["amount"])
+
+        self.to_reactor = add_water(
+            self.S1_unders,
+            self.water_flow,
+            self.Material_Properties,
+            self.process_data,
+            self.flow_init,
+        )
 
         ### Reactor
-        self.digestate = Reactor(self.to_reactor, self.CommonData, self.process_data, self.InputData, self.Material_Properties,
-                                 self.LCI, self.flow_init)
+        self.digestate = Reactor(
+            self.to_reactor,
+            self.CommonData,
+            self.process_data,
+            self.InputData,
+            self.Material_Properties,
+            self.LCI,
+            self.flow_init,
+        )
 
         ### Dewatering
-        self.Dig_to_Curing_1, self.liq_rem, self.liq_treatment_vol = Dewater(self.digestate, self.to_reactor, self.CommonData, self.process_data, self.InputData,
-                                                                             self.Material_Properties, self.water_flow, self.Assumed_Comp.values,
-                                                                             self.LCI, self.flow_init)
+        self.Dig_to_Curing_1, self.liq_rem, self.liq_treatment_vol = Dewater(
+            self.digestate,
+            self.to_reactor,
+            self.CommonData,
+            self.InputData,
+            self.Material_Properties,
+            self.Assumed_Comp.values,
+            self.LCI,
+            self.flow_init,
+        )
 
         ### Mix Dig_to_Curing_1 and S2_to_curing
-        self.Dig_to_Curing = mix(self.Dig_to_Curing_1, self.S2_to_curing, self.Material_Properties, self.flow_init)
+        self.Dig_to_Curing = mix(
+            self.Dig_to_Curing_1, self.S2_to_curing, self.Material_Properties, self.flow_init
+        )
 
         ### Curing
-        self.compost_to_ps, self.WC_SC = curing(self.Dig_to_Curing, self.to_reactor, self.CommonData, self.process_data,
-                                                  self.InputData, self.Assumed_Comp, self.Material_Properties, self.LCI,
-                                                  self.flow_init)
+        self.compost_to_ps, self.WC_SC = curing(
+            self.Dig_to_Curing,
+            self.to_reactor,
+            self.CommonData,
+            self.process_data,
+            self.InputData,
+            self.Assumed_Comp,
+            self.LCI,
+            self.flow_init,
+        )
 
         ### Post_screen
-        self.FinalCompost, self.Compost_WC, self.Screen_rejects = Post_screen(self.compost_to_ps, self.WC_SC, self.InputData, self.Assumed_Comp.values,
-                                                                self.Material_Properties, self.LCI, self.flow_init)
+        self.FinalCompost, self.Compost_WC, self.Screen_rejects = Post_screen(
+            self.compost_to_ps,
+            self.WC_SC,
+            self.InputData,
+            self.LCI,
+            self.flow_init,
+        )
 
         ### AD Diesel and electricity use (general)
-        self.LCI.add(name=('Technosphere', 'Equipment_Diesel'),
-                     flow=self.InputData.Fac_Energy['Dsl_facility']['amount'])
-        self.LCI.add(name=('Technosphere', 'Electricity_consumption'),
-                     flow=self.InputData.Fac_Energy['elec_facility']['amount'])
-        self.LCI.add(name=('Technosphere', 'Electricity_consumption'),
-                     flow=self.InputData.Fac_Energy['elec_preproc']['amount'])
+        self.LCI.add(
+            name=("Technosphere", "Equipment_Diesel"),
+            flow=self.InputData.Fac_Energy["Dsl_facility"]["amount"],
+        )
+        self.LCI.add(
+            name=("Technosphere", "Electricity_consumption"),
+            flow=self.InputData.Fac_Energy["elec_facility"]["amount"],
+        )
+        self.LCI.add(
+            name=("Technosphere", "Electricity_consumption"),
+            flow=self.InputData.Fac_Energy["elec_preproc"]["amount"],
+        )
 
         ### Compost use
-        compost_use(input_flow=self.FinalCompost,
-                    common_data=self.CommonData,
-                    process_data=self.process_data,
-                    material_properties=self.Material_Properties,
-                    input_data=self.InputData,
-                    lci=self.LCI)
+        compost_use(
+            input_flow=self.FinalCompost,
+            common_data=self.CommonData,
+            process_data=self.process_data,
+            material_properties=self.Material_Properties,
+            input_data=self.InputData,
+            lci=self.LCI,
+        )
 
         ### Transportation Compost
-        self.LCI.add(name=('Technosphere', 'Internal_Process_Transportation_Medium_Duty_Diesel_Truck'),
-                     flow=self.FinalCompost.data['mass'].values * self.InputData.Land_app['distLand']['amount'])
-        self.LCI.add(name=('Technosphere', 'Empty_Return_Medium_Duty_Diesel_Truck'),
-                     flow=self.FinalCompost.data['mass'].values / 1000 / self.InputData.Land_app['land_payload']['amount'] * self.InputData.Land_app['distLand']['amount'])
+        self.LCI.add(
+            name=("Technosphere", "Internal_Process_Transportation_Medium_Duty_Diesel_Truck"),
+            flow=self.FinalCompost.data["mass"].values
+            * self.InputData.Land_app["distLand"]["amount"],
+        )
+        self.LCI.add(
+            name=("Technosphere", "Empty_Return_Medium_Duty_Diesel_Truck"),
+            flow=self.FinalCompost.data["mass"].values
+            / 1000
+            / self.InputData.Land_app["land_payload"]["amount"]
+            * self.InputData.Land_app["distLand"]["amount"],
+        )
 
         ### Cost Calculation
-        capital_cost = -npf.pmt(rate=self.InputData.Economic_parameters['Inerest_rate']['amount'],
-                        nper=self.InputData.Economic_parameters['lifetime']['amount'],
-                        pv=self.InputData.Economic_parameters['Unit_capital_cost']['amount'])
-        self.LCI.add(name=('biosphere3','Capital_Cost'),
-                     flow=capital_cost)
-        self.LCI.add(name=('biosphere3','Operational_Cost'),
-                     flow=[self.InputData.Operational_Cost[y]['amount'] for y in self.Index])
+        capital_cost = -npf.pmt(
+            rate=self.InputData.Economic_parameters["Interest_rate"]["amount"],
+            nper=self.InputData.Economic_parameters["lifetime"]["amount"],
+            pv=self.InputData.Economic_parameters["Unit_capital_cost"]["amount"],
+        )
+        self.LCI.add(name=("biosphere3", "Capital_Cost"), flow=capital_cost)
+        self.LCI.add(
+            name=("biosphere3", "Operational_Cost"),
+            flow=[self.InputData.Operational_Cost[y]["amount"] for y in self.Index],
+        )
 
     def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
-        #self.create_uncertainty_from_inputs()
+        # self.create_uncertainty_from_inputs()
 
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
-        #self.uncertainty_input_next()
+        # self.uncertainty_input_next()
         self.calc()
-        return(input_list)
+        return input_list
 
     def report(self):
         report = {}
         report["process name"] = (self.process_name, self.Process_Type, self.__class__)
 
         self.lci_report = self.LCI.report()
 
         # Set the value zero if the flow is not in the LCI dataframe.
-        for i in [('Technosphere', 'Nitrogen_Fertilizer'),
-                  ('Technosphere', 'Phosphorous_Fertilizer'),
-                  ('Technosphere', 'Potassium_Fertilizer'),
-                  ('Technosphere', 'Peat'),
-                  ('Technosphere', 'compost_to_LF'),
-                  'Ammonium, ion (ground water)',
-                  'Ammonium, ion (surface water)',
-                  'Nitrate (ground water)',
-                  'Nitrate (surface water)',
-                  ('Technosphere', 'market_for_excavation_skid_steer_loader'),
-                  'Carbon dioxide, fossil',
-                  'Carbon dioxide, non-fossil']:
+        for i in [
+            ("Technosphere", "Nitrogen_Fertilizer"),
+            ("Technosphere", "Phosphorous_Fertilizer"),
+            ("Technosphere", "Potassium_Fertilizer"),
+            ("Technosphere", "Peat"),
+            ("Technosphere", "compost_to_LF"),
+            "Ammonium, ion (ground water)",
+            "Ammonium, ion (surface water)",
+            "Nitrate (ground water)",
+            "Nitrate (surface water)",
+            ("Technosphere", "market_for_excavation_skid_steer_loader"),
+            "Carbon dioxide, fossil",
+            "Carbon dioxide, non-fossil",
+        ]:
             if i not in self.lci_report.columns:
                 self.lci_report[i] = 0
 
-        net_elec = ((self.lci_report[('Technosphere', 'Electricity_production')].values
-                     - self.lci_report[('Technosphere', 'Electricity_consumption')].values)
-                    * self.Assumed_Comp.values).sum()
+        net_elec = (
+            (
+                self.lci_report[("Technosphere", "Electricity_production")].values
+                - self.lci_report[("Technosphere", "Electricity_consumption")].values
+            )
+            * self.Assumed_Comp.values
+        ).sum()
         if net_elec >= 0:
-            self.lci_report[('Technosphere', 'Electricity_production')] = (
-                self.lci_report[('Technosphere', 'Electricity_production')].values
-                - self.lci_report[('Technosphere', 'Electricity_consumption')].values)
-            self.lci_report[('Technosphere', 'Electricity_consumption')] = 0
+            self.lci_report[("Technosphere", "Electricity_production")] = (
+                self.lci_report[("Technosphere", "Electricity_production")].values
+                - self.lci_report[("Technosphere", "Electricity_consumption")].values
+            )
+            self.lci_report[("Technosphere", "Electricity_consumption")] = 0
         else:
-            self.lci_report[('Technosphere', 'Electricity_consumption')] = (
-                self.lci_report[('Technosphere', 'Electricity_consumption')].values
-                - self.lci_report[('Technosphere', 'Electricity_production')].values)
-            self.lci_report[('Technosphere', 'Electricity_production')] = 0
-
-        self.lci_report['report_Methane, non-fossil'] = (self.lci_report['Methane, non-fossil'].values
-                                                         + self.lci_report['Methane, non-fossil (unburned)'].values
-                                                         + self.lci_report['Fugitive (Leaked) Methane'].values)
-
-        self.lci_report['report_ CO2 non-fossil'] = (self.lci_report['CO2-biogenic emissions from digested liquids treatment'].values
-                                                     + self.lci_report['Carbon dioxide, non-fossil _ Curing'].values
-                                                     + self.lci_report['Carbon dioxide, non-fossil'].values
-                                                     + self.lci_report['Carbon dioxide, non-fossil (in biogas)'].values
-                                                     + self.lci_report['Carbon dioxide, non-fossil from comubstion'].values)
+            self.lci_report[("Technosphere", "Electricity_consumption")] = (
+                self.lci_report[("Technosphere", "Electricity_consumption")].values
+                - self.lci_report[("Technosphere", "Electricity_production")].values
+            )
+            self.lci_report[("Technosphere", "Electricity_production")] = 0
+
+        self.lci_report["report_Methane, non-fossil"] = (
+            self.lci_report["Methane, non-fossil"].values
+            + self.lci_report["Methane, non-fossil (unburned)"].values
+            + self.lci_report["Fugitive (Leaked) Methane"].values
+        )
+
+        self.lci_report["report_ CO2 non-fossil"] = (
+            self.lci_report["CO2-biogenic emissions from digested liquids treatment"].values
+            + self.lci_report["Carbon dioxide, non-fossil _ Curing"].values
+            + self.lci_report["Carbon dioxide, non-fossil"].values
+            + self.lci_report["Carbon dioxide, non-fossil (in biogas)"].values
+            + self.lci_report["Carbon dioxide, non-fossil from combustion"].values
+        )
 
         # NMVOC, non-methane volatile organic compounds, unspecified origin ('air',)
-        self.lci_report['report_ NMVOC'] = (self.lci_report['NMVOC, non-methane volatile organic compounds, unspecified origin'].values
-                                            + self.lci_report['NMVOCs'].values)
-
+        self.lci_report["report_ NMVOC"] = (
+            self.lci_report[
+                "NMVOC, non-methane volatile organic compounds, unspecified origin"
+            ].values
+            + self.lci_report["NMVOCs"].values
+        )
 
         self._bio_rename_dict = {
-            'Ammonia':('biosphere3', '87883a4e-1e3e-4c9d-90c0-f1bea36f8014'), # Ammonia ('air',)
-            'Direct Carbon Storage and Humus Formation':('biosphere3', 'e4e9febc-07c1-403d-8d3a-6707bb4d96e6'), # Carbon dioxide, from soil or biomass stock ('air',)
-            'report_ CO2 non-fossil':('biosphere3', 'eba59fd6-f37e-41dc-9ca3-c7ea22d602c7'), # Carbon dioxide, non-fossil ('air',)
-            'Carbon monoxide (CO)':('biosphere3', '2cb2333c-1599-46cf-8435-3dffce627524'), # Carbon monoxide, non-fossil ('air',)
-            'Carbon dioxide, fossil': ('biosphere3', '349b29d1-3e58-4c66-98b9-9d1a076efd2e'), # Carbon dioxide, fossil (air,)
-            'Dinitrogen monoxide':('biosphere3', '20185046-64bb-4c09-a8e7-e8a9e144ca98'), # Dinitrogen monoxide ('air',)
-            'report_Methane, non-fossil':('biosphere3', 'da1157e2-7593-4dfd-80dd-a3449b37a4d8') , # Methane, non-fossil ('air',)
-            'Nitrogen oxides (as NO2)':('biosphere3', 'c1b91234-6f24-417b-8309-46111d09c457'), # Nitrogen oxides ('air',)
-            'report_ NMVOC':('biosphere3', 'd3260d0e-8203-4cbb-a45a-6a13131a5108'), # NMVOC, non-methane volatile organic compounds, unspecified origin ('air',)
-            'PM2.5':('biosphere3', '21e46cb8-6233-4c99-bac3-c41d2ab99498'), # Particulates, < 2.5 um ('air',)
-            'Sulfur dioxide (SO2)':('biosphere3', 'fd7aa71c-508c-480d-81a6-8052aad92646'), # Sulfur dioxide ('air',)
-            'Arsenic':('biosphere3', '8c8ffaa5-84ed-4668-ba7d-80fd0f47013f'), # Arsenic, ion ('water', 'surface water')
-            'Barium':('biosphere3', '2c872773-0a29-4831-93b9-d49b116fa7d5'),  # Barium ('water', 'surface water')
-            'BOD':('biosphere3', '70d467b6-115e-43c5-add2-441de9411348'), # BOD5, Biological Oxygen Demand ('water', 'surface water')
-            'Cadmium':('biosphere3', 'af83b42f-a4e6-4457-be74-46a87798f82a'), # Cadmium, ion ('water', 'surface water')
-            'Chromium':('biosphere3', 'e34d3da4-a3d5-41be-84b5-458afe32c990'), # Chromium, ion ('water', 'surface water')
-            'COD':('biosphere3', 'fc0b5c85-3b49-42c2-a3fd-db7e57b696e3'), # COD, Chemical Oxygen Demand ('water', 'surface water')
-            'Copper':('biosphere3', '6d9550e2-e670-44c1-bad8-c0c4975ffca7'), # Copper, ion ('water', 'surface water')
-            'Iron':('biosphere3', '7c335b9c-a403-47a8-bb6d-2e7d3c3a230e'), # Iron, ion ('water', 'surface water')
-            'Lead':('biosphere3', 'b3ebdcc3-c588-4997-95d2-9785b26b34e1'), # Lead ('water', 'surface water')
-            'Mercury':('biosphere3', '66bfb434-78ab-4183-b1a7-7f87d08974fa'), # Mercury ('water', 'surface water')
-            'Total N':('biosphere3', 'ae70ca6c-807a-482b-9ddc-e449b4893fe3'), # Nitrogen ('water', 'surface water')
-            'Phosphate':('biosphere3', '1727b41d-377e-43cd-bc01-9eaba946eccb'),  # Phosphate ('water', 'surface water')
-            'Selenium':('biosphere3', '544dbea9-1d18-44ff-b92b-7866e3baa6dd'), # Selenium ('water', 'surface water')
-            'Silver':('biosphere3', 'af9793ba-25a1-4928-a14a-4bcf7d5bd3f7'),  # Silver, ion ('water', 'surface water')
-            'Total suspended solids':('biosphere3', '3844f446-ded5-4727-8421-17a00ef4eba7'), # Suspended solids, unspecified ('water', 'surface water')
-            'Zinc':('biosphere3', '541b633c-17a3-4047-bce6-0c0e4fdb7c10'), # Zinc, ion ('water', 'surface water')
-            'Nitrate (ground water)':('biosphere3', 'b9291c72-4b1d-4275-8068-4c707dc3ce33'), # Nitrate ('water', 'ground-')
-            'Nitrate (surface water)':('biosphere3', '7ce56135-2ca5-4fba-ad52-d62a34bfeb35'), # Nitrate ('water', 'surface water')
-            'Ammonium, ion (ground water)':('biosphere3', '736f52e8-9703-4076-8909-7ae80a7f8005'), #'Ammonium, ion' (kilogram, None, ('water', 'ground-'))
-            'Ammonium, ion (surface water)':('biosphere3', '13331e67-6006-48c4-bdb4-340c12010036') # 'Ammonium, ion' (kilogram, None, ('water', 'surface water'))
-            }
+            "Ammonia": ("biosphere3", "87883a4e-1e3e-4c9d-90c0-f1bea36f8014"),  # Ammonia ('air',)
+            "Direct Carbon Storage and Humus Formation": (
+                "biosphere3",
+                "e4e9febc-07c1-403d-8d3a-6707bb4d96e6",
+            ),  # Carbon dioxide, from soil or biomass stock ('air',)
+            "report_ CO2 non-fossil": (
+                "biosphere3",
+                "eba59fd6-f37e-41dc-9ca3-c7ea22d602c7",
+            ),  # Carbon dioxide, non-fossil ('air',)
+            "Carbon monoxide (CO)": (
+                "biosphere3",
+                "2cb2333c-1599-46cf-8435-3dffce627524",
+            ),  # Carbon monoxide, non-fossil ('air',)
+            "Carbon dioxide, fossil": (
+                "biosphere3",
+                "349b29d1-3e58-4c66-98b9-9d1a076efd2e",
+            ),  # Carbon dioxide, fossil (air,)
+            "Dinitrogen monoxide": (
+                "biosphere3",
+                "20185046-64bb-4c09-a8e7-e8a9e144ca98",
+            ),  # Dinitrogen monoxide ('air',)
+            "report_Methane, non-fossil": (
+                "biosphere3",
+                "da1157e2-7593-4dfd-80dd-a3449b37a4d8",
+            ),  # Methane, non-fossil ('air',)
+            "Nitrogen oxides (as NO2)": (
+                "biosphere3",
+                "c1b91234-6f24-417b-8309-46111d09c457",
+            ),  # Nitrogen oxides ('air',)
+            "report_ NMVOC": (
+                "biosphere3",
+                "d3260d0e-8203-4cbb-a45a-6a13131a5108",
+            ),  # NMVOC, non-methane volatile organic compounds, unspecified origin ('air',)
+            "PM2.5": (
+                "biosphere3",
+                "21e46cb8-6233-4c99-bac3-c41d2ab99498",
+            ),  # Particulates, < 2.5 um ('air',)
+            "Sulfur dioxide (SO2)": (
+                "biosphere3",
+                "fd7aa71c-508c-480d-81a6-8052aad92646",
+            ),  # Sulfur dioxide ('air',)
+            "Arsenic": (
+                "biosphere3",
+                "8c8ffaa5-84ed-4668-ba7d-80fd0f47013f",
+            ),  # Arsenic, ion ('water', 'surface water')
+            "Barium": (
+                "biosphere3",
+                "2c872773-0a29-4831-93b9-d49b116fa7d5",
+            ),  # Barium ('water', 'surface water')
+            "BOD": (
+                "biosphere3",
+                "70d467b6-115e-43c5-add2-441de9411348",
+            ),  # BOD5, Biological Oxygen Demand ('water', 'surface water')
+            "Cadmium": (
+                "biosphere3",
+                "af83b42f-a4e6-4457-be74-46a87798f82a",
+            ),  # Cadmium, ion ('water', 'surface water')
+            "Chromium": (
+                "biosphere3",
+                "e34d3da4-a3d5-41be-84b5-458afe32c990",
+            ),  # Chromium, ion ('water', 'surface water')
+            "COD": (
+                "biosphere3",
+                "fc0b5c85-3b49-42c2-a3fd-db7e57b696e3",
+            ),  # COD, Chemical Oxygen Demand ('water', 'surface water')
+            "Copper": (
+                "biosphere3",
+                "6d9550e2-e670-44c1-bad8-c0c4975ffca7",
+            ),  # Copper, ion ('water', 'surface water')
+            "Iron": (
+                "biosphere3",
+                "7c335b9c-a403-47a8-bb6d-2e7d3c3a230e",
+            ),  # Iron, ion ('water', 'surface water')
+            "Lead": (
+                "biosphere3",
+                "b3ebdcc3-c588-4997-95d2-9785b26b34e1",
+            ),  # Lead ('water', 'surface water')
+            "Mercury": (
+                "biosphere3",
+                "66bfb434-78ab-4183-b1a7-7f87d08974fa",
+            ),  # Mercury ('water', 'surface water')
+            "Total N": (
+                "biosphere3",
+                "ae70ca6c-807a-482b-9ddc-e449b4893fe3",
+            ),  # Nitrogen ('water', 'surface water')
+            "Phosphate": (
+                "biosphere3",
+                "1727b41d-377e-43cd-bc01-9eaba946eccb",
+            ),  # Phosphate ('water', 'surface water')
+            "Selenium": (
+                "biosphere3",
+                "544dbea9-1d18-44ff-b92b-7866e3baa6dd",
+            ),  # Selenium ('water', 'surface water')
+            "Silver": (
+                "biosphere3",
+                "af9793ba-25a1-4928-a14a-4bcf7d5bd3f7",
+            ),  # Silver, ion ('water', 'surface water')
+            "Total suspended solids": (
+                "biosphere3",
+                "3844f446-ded5-4727-8421-17a00ef4eba7",
+            ),  # Suspended solids, unspecified ('water', 'surface water')
+            "Zinc": (
+                "biosphere3",
+                "541b633c-17a3-4047-bce6-0c0e4fdb7c10",
+            ),  # Zinc, ion ('water', 'surface water')
+            "Nitrate (ground water)": (
+                "biosphere3",
+                "b9291c72-4b1d-4275-8068-4c707dc3ce33",
+            ),  # Nitrate ('water', 'ground-')
+            "Nitrate (surface water)": (
+                "biosphere3",
+                "7ce56135-2ca5-4fba-ad52-d62a34bfeb35",
+            ),  # Nitrate ('water', 'surface water')
+            "Ammonium, ion (ground water)": (
+                "biosphere3",
+                "736f52e8-9703-4076-8909-7ae80a7f8005",
+            ),  #'Ammonium, ion' (kilogram, None, ('water', 'ground-'))
+            "Ammonium, ion (surface water)": (
+                "biosphere3",
+                "13331e67-6006-48c4-bdb4-340c12010036",
+            ),  # 'Ammonium, ion' (kilogram, None, ('water', 'surface water'))
+        }
 
         tech_flows = [
-            ('Technosphere', 'Electricity_production'),
-            ('Technosphere', 'Electricity_consumption'),
-            ('Technosphere', 'Equipment_Diesel'),
-            ('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'),
-            ('Technosphere', 'Internal_Process_Transportation_Medium_Duty_Diesel_Truck'),
-            ('Technosphere', 'Empty_Return_Heavy_Duty_Diesel_Truck'),
-            ('Technosphere', 'Empty_Return_Medium_Duty_Diesel_Truck'),
-            ('Technosphere', 'Nitrogen_Fertilizer'),
-            ('Technosphere', 'Phosphorous_Fertilizer'),
-            ('Technosphere', 'Potassium_Fertilizer'),
-            ('Technosphere', 'Peat'),
-            ('Technosphere', 'compost_to_LF'),
-            ('Technosphere', 'market_for_excavation_skid_steer_loader')]
+            ("Technosphere", "Electricity_production"),
+            ("Technosphere", "Electricity_consumption"),
+            ("Technosphere", "Equipment_Diesel"),
+            ("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"),
+            ("Technosphere", "Internal_Process_Transportation_Medium_Duty_Diesel_Truck"),
+            ("Technosphere", "Empty_Return_Heavy_Duty_Diesel_Truck"),
+            ("Technosphere", "Empty_Return_Medium_Duty_Diesel_Truck"),
+            ("Technosphere", "Nitrogen_Fertilizer"),
+            ("Technosphere", "Phosphorous_Fertilizer"),
+            ("Technosphere", "Potassium_Fertilizer"),
+            ("Technosphere", "Peat"),
+            ("Technosphere", "compost_to_LF"),
+            ("Technosphere", "market_for_excavation_skid_steer_loader"),
+        ]
 
         report["Waste"] = {}
         for y in self.Index:
             report["Waste"][y] = {}
-            report["Waste"][y]['Other_Residual'] = self.lci_report['Residual'][y]
+            report["Waste"][y]["Other_Residual"] = self.lci_report["Residual"][y]
 
         report["Technosphere"] = self.lci_report[tech_flows].transpose().to_dict()
 
         self.lci_report = self.lci_report.rename(columns=self._bio_rename_dict)
-        report["Biosphere"] = self.lci_report[list(self._bio_rename_dict.values())
-                                              + [('biosphere3','Capital_Cost'),
-                                                 ('biosphere3','Operational_Cost')]].transpose().to_dict()
-        return(report)
+        report["Biosphere"] = (
+            self.lci_report[
+                list(self._bio_rename_dict.values())
+                + [("biosphere3", "Capital_Cost"), ("biosphere3", "Operational_Cost")]
+            ]
+            .transpose()
+            .to_dict()
+        )
+        return report
 
     def plot(self, composition, saveHTML=False):
         source = []
         target = []
         value = []
-        lable = ['Incoming Mass', 'Screen 1', 'Screen 2', 'Residuals', 'Add Water', 'Mixer', 'Reactor', 'Dewater',
-                 'Curing', 'Post Screen', 'Finished Compost', 'WWT', 'Makeup Water', 'Wood Chips']
-        lable_link = []
+        label = [
+            "Incoming Mass",
+            "Screen 1",
+            "Screen 2",
+            "Residuals",
+            "Add Water",
+            "Mixer",
+            "Reactor",
+            "Dewater",
+            "Curing",
+            "Post Screen",
+            "Finished Compost",
+            "WWT",
+            "Makeup Water",
+            "Wood Chips",
+        ]
+        label_link = []
         color_link = []
 
         # Link for colors: https://www.rapidtables.com/web/color/RGB_Color.html
 
         self.Input.update(composition)
-        source.append(lable.index('Incoming Mass'))
-        target.append(lable.index('Screen 1'))
+        source.append(label.index("Incoming Mass"))
+        target.append(label.index("Screen 1"))
         value.append(self.Input.flow)
-        lable_link.append('Input')
+        label_link.append("Input")
         self.S1_unders.update(composition)
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(128,128,0))) # Olive
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(128, 128, 0)))  # Olive
 
-        source.append(lable.index('Screen 1'))
-        target.append(lable.index('Add Water'))
+        source.append(label.index("Screen 1"))
+        target.append(label.index("Add Water"))
         value.append(self.S1_unders.flow)
-        lable_link.append('S1_unders')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(128,128,0))) # Olive
+        label_link.append("S1_unders")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(128, 128, 0)))  # Olive
 
         self.S1_overs.update(composition)
-        source.append(lable.index('Screen 1'))
-        target.append(lable.index('Screen 2'))
+        source.append(label.index("Screen 1"))
+        target.append(label.index("Screen 2"))
         value.append(self.S1_overs.flow)
-        lable_link.append('S1_overs')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(128,128,128))) # Gray
+        label_link.append("S1_overs")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(128, 128, 128)))  # Gray
 
-        self.S2_residuls.update(composition)
-        source.append(lable.index('Screen 2'))
-        target.append(lable.index('Residuals'))
-        value.append(self.S2_residuls.flow)
-        lable_link.append('S2_residuls')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(128,128,128))) # Gray
+        self.S2_residuals.update(composition)
+        source.append(label.index("Screen 2"))
+        target.append(label.index("Residuals"))
+        value.append(self.S2_residuals.flow)
+        label_link.append("S2_residuals")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(128, 128, 128)))  # Gray
 
         self.S2_to_curing.update(composition)
-        source.append(lable.index('Screen 2'))
-        target.append(lable.index('Mixer'))
+        source.append(label.index("Screen 2"))
+        target.append(label.index("Mixer"))
         value.append(self.S2_to_curing.flow)
-        lable_link.append('S2_to_curing')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*	(128,128,0))) # Olive
+        label_link.append("S2_to_curing")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(128, 128, 0)))  # Olive
 
         self.to_reactor.update(composition)
-        source.append(lable.index('Add Water'))
-        target.append(lable.index('Reactor'))
+        source.append(label.index("Add Water"))
+        target.append(label.index("Reactor"))
         value.append(self.to_reactor.flow)
-        lable_link.append('to_reactor')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(85,107,47))) # dark olive green
+        label_link.append("to_reactor")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(85, 107, 47)))  # dark olive green
 
         self.digestate.update(composition)
-        source.append(lable.index('Reactor'))
-        target.append(lable.index('Dewater'))
+        source.append(label.index("Reactor"))
+        target.append(label.index("Dewater"))
         value.append(self.digestate.flow)
-        lable_link.append('digestate')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(107,142,35))) # olive drab
+        label_link.append("digestate")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(107, 142, 35)))  # olive drab
 
         self.Dig_to_Curing_1.update(composition)
-        source.append(lable.index('Dewater'))
-        target.append(lable.index('Mixer'))
+        source.append(label.index("Dewater"))
+        target.append(label.index("Mixer"))
         value.append(self.Dig_to_Curing_1.flow)
-        lable_link.append('Dig_to_Curing_1')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(124,252,0))) # lawn green
-
+        label_link.append("Dig_to_Curing_1")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(124, 252, 0)))  # lawn green
 
-        source.append(lable.index('Dewater'))
-        target.append(lable.index('Add Water'))
-        rec_water = sum(self.liq_rem * composition) - sum(self.liq_treatment_vol * composition) * 1000
+        source.append(label.index("Dewater"))
+        target.append(label.index("Add Water"))
+        rec_water = (
+            sum(self.liq_rem * composition) - sum(self.liq_treatment_vol * composition) * 1000
+        )
         value.append(rec_water)
-        lable_link.append('liq_rem')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(0,0,128))) # navy
+        label_link.append("liq_rem")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(0, 0, 128)))  # navy
 
         self.Dig_to_Curing.update(composition)
-        source.append(lable.index('Mixer'))
-        target.append(lable.index('Curing'))
+        source.append(label.index("Mixer"))
+        target.append(label.index("Curing"))
         value.append(self.Dig_to_Curing.flow)
-        lable_link.append('Dig_to_Curing')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(60,179,113))) # medium sea green
+        label_link.append("Dig_to_Curing")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(60, 179, 113)))  # medium sea green
 
         self.compost_to_ps.update(composition)
-        source.append(lable.index('Curing'))
-        target.append(lable.index('Post Screen'))
+        source.append(label.index("Curing"))
+        target.append(label.index("Post Screen"))
         value.append(self.compost_to_ps.flow)
-        lable_link.append('compost_to_ps')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(0,100,0))) # dark green
+        label_link.append("compost_to_ps")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(0, 100, 0)))  # dark green
 
-        source.append(lable.index('Curing'))
-        target.append(lable.index('Post Screen'))
+        source.append(label.index("Curing"))
+        target.append(label.index("Post Screen"))
         value.append(sum(self.WC_SC * composition))
-        lable_link.append('WC_SC')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(160,82,45))) # sienna
+        label_link.append("WC_SC")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(160, 82, 45)))  # sienna
 
-        source.append(lable.index('Wood Chips'))
-        target.append(lable.index('Curing'))
+        source.append(label.index("Wood Chips"))
+        target.append(label.index("Curing"))
         value.append(sum(self.WC_SC * composition) - sum(self.Screen_rejects * composition))
-        lable_link.append('Wood Chips')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(160,82,45))) # sienna
+        label_link.append("Wood Chips")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(160, 82, 45)))  # sienna
 
-        source.append(lable.index('Post Screen'))
-        target.append(lable.index('Curing'))
+        source.append(label.index("Post Screen"))
+        target.append(label.index("Curing"))
         value.append(sum(self.Screen_rejects * composition))
-        lable_link.append('Screen_rejects')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(160,82,45))) # sienna
+        label_link.append("Screen_rejects")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(160, 82, 45)))  # sienna
 
         self.FinalCompost.update(composition)
-        source.append(lable.index('Post Screen'))
-        target.append(lable.index('Finished Compost'))
+        source.append(label.index("Post Screen"))
+        target.append(label.index("Finished Compost"))
         value.append(self.FinalCompost.flow)
-        lable_link.append('FinalCompost')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(0,128,0))) # green
+        label_link.append("FinalCompost")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(0, 128, 0)))  # green
 
-        source.append(lable.index('Makeup Water'))
-        target.append(lable.index('Add Water'))
+        source.append(label.index("Makeup Water"))
+        target.append(label.index("Add Water"))
         value.append(sum(self.water_flow * composition) - rec_water)
-        lable_link.append('Makeup_water')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(0,0,255))) # blue
+        label_link.append("Makeup_water")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(0, 0, 255)))  # blue
 
-        source.append(lable.index('Dewater'))
-        target.append(lable.index('WWT'))
-        value.append(sum(self.liq_treatment_vol * composition)*1000)
-        lable_link.append('liq_treatment_vol')
-        color_link.append('rgba({}, {}, {}, 0.8)'.format(*(0,0,139))) #dark blue
-
-        fig = go.Figure(data=[go.Sankey(orientation="h",
-                                        valueformat=".0f",
-                                        valuesuffix="kg",
-                                        node=dict(pad=20,
-                                                  thickness=20,
-                                                  line=dict(color="black", width = 0.5),
-                                                  label=lable),
-                                        link=dict(source=source,
-                                                  target=target,
-                                                  value=value,
-                                                  label=lable_link,
-                                                  color=color_link))])
-
-        fig.update_layout(title_text="Mass flow diagram for AD process",
-                          font_size=14,
-                          hoverlabel=dict(font_size=14))
+        source.append(label.index("Dewater"))
+        target.append(label.index("WWT"))
+        value.append(sum(self.liq_treatment_vol * composition) * 1000)
+        label_link.append("liq_treatment_vol")
+        color_link.append("rgba({}, {}, {}, 0.8)".format(*(0, 0, 139)))  # dark blue
+
+        fig = go.Figure(
+            data=[
+                go.Sankey(
+                    orientation="h",
+                    valueformat=".0f",
+                    valuesuffix="kg",
+                    node={
+                        "pad": 20,
+                        "thickness": 20,
+                        "line": {"color": "black", "width": 0.5},
+                        "label": label,
+                    },
+                    link={
+                        "source": source,
+                        "target": target,
+                        "value": value,
+                        "label": label_link,
+                        "color": color_link,
+                    },
+                )
+            ]
+        )
+
+        fig.update_layout(
+            title_text="Mass flow diagram for AD process",
+            font_size=14,
+            hoverlabel={"font_size": 14},
+        )
         if not saveHTML:
             fig.show()
         else:
-            plot(fig, 'plot.html', auto_open=True)
+            plot(fig, "plot.html", auto_open=True)
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/AD_subprocess.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/AD_subprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,537 +1,746 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Fri Nov 22 21:23:49 2019
+from copy import deepcopy
 
-@author: msardar2
-"""
 import numpy as np
-from copy import deepcopy
 
 
-### AD_Screan
-def screen(input_flow, sep_eff, Material_Properties, LCI, flow_init):
+### AD_Screen
+def screen(input_flow, sep_eff, flow_init):
     product = deepcopy(flow_init)
     residual = deepcopy(flow_init)
 
-    residual.data['mass'] = input_flow.data['mass'].values * sep_eff
-    residual.data['sol_cont'] = input_flow.data['sol_cont'].values * sep_eff
-    residual.data['moist_cont'] = input_flow.data['moist_cont'].values * sep_eff
-    residual.data['vs_cont'] = input_flow.data['vs_cont'].values * sep_eff
-    residual.data['ash_cont'] = input_flow.data['ash_cont'].values * sep_eff
-
-    product.data['mass'] = input_flow.data['mass'].values - residual.data['mass'].values
-    product.data['sol_cont'] = input_flow.data['sol_cont'].values - residual.data['sol_cont'].values
-    product.data['moist_cont'] = input_flow.data['moist_cont'].values - residual.data['moist_cont'].values
-    product.data['vs_cont'] = input_flow.data['vs_cont'].values - residual.data['vs_cont'].values
-    product.data['ash_cont'] = input_flow.data['ash_cont'].values - residual.data['ash_cont'].values
+    residual.data["mass"] = input_flow.data["mass"].values * sep_eff
+    residual.data["sol_cont"] = input_flow.data["sol_cont"].values * sep_eff
+    residual.data["moist_cont"] = input_flow.data["moist_cont"].values * sep_eff
+    residual.data["vs_cont"] = input_flow.data["vs_cont"].values * sep_eff
+    residual.data["ash_cont"] = input_flow.data["ash_cont"].values * sep_eff
+
+    product.data["mass"] = input_flow.data["mass"].values - residual.data["mass"].values
+    product.data["sol_cont"] = input_flow.data["sol_cont"].values - residual.data["sol_cont"].values
+    product.data["moist_cont"] = (
+        input_flow.data["moist_cont"].values - residual.data["moist_cont"].values
+    )
+    product.data["vs_cont"] = input_flow.data["vs_cont"].values - residual.data["vs_cont"].values
+    product.data["ash_cont"] = input_flow.data["ash_cont"].values - residual.data["ash_cont"].values
 
     return (product, residual)
 
 
 ### AD_Add Water
 def add_water(input_flow, water_flow, Material_Properties, process_data, flow_init):
     product = deepcopy(flow_init)
-    product.data['mass'] = input_flow.data['mass'].values + water_flow
-    product.data['sol_cont'] = input_flow.data['sol_cont'].values
-    product.data['moist_cont'] = input_flow.data['moist_cont'].values + water_flow
-    product.data['vs_cont'] = input_flow.data['vs_cont'].values
-    product.data['ash_cont'] = input_flow.data['ash_cont'].values
+    product.data["mass"] = input_flow.data["mass"].values + water_flow
+    product.data["sol_cont"] = input_flow.data["sol_cont"].values
+    product.data["moist_cont"] = input_flow.data["moist_cont"].values + water_flow
+    product.data["vs_cont"] = input_flow.data["vs_cont"].values
+    product.data["ash_cont"] = input_flow.data["ash_cont"].values
 
     # Nitrogen and carbon in the input stream
-    product.data['C_cont'] = (input_flow.data['sol_cont'].values
-                              * (Material_Properties['Biogenic Carbon Content'].values / 100)
-                              * process_data['Degrades'].values)
-
-    product.data['N_cont'] = (input_flow.data['sol_cont'].values
-                              * (Material_Properties['Nitrogen Content'].values / 100)
-                              * process_data['Degrades'].values)
-
-    product.data['P_cont'] = (input_flow.data['sol_cont'].values
-                              * (Material_Properties['Phosphorus Content'].values / 100)
-                              * process_data['Degrades'].values)
-
-    product.data['K_cont'] = (input_flow.data['sol_cont'].values
-                              * (Material_Properties['Potassium Content'].values / 100)
-                              * process_data['Degrades'].values)
+    product.data["C_cont"] = (
+        input_flow.data["sol_cont"].values
+        * (Material_Properties["Biogenic Carbon Content"].values / 100)
+        * process_data["Degrades"].values
+    )
+
+    product.data["N_cont"] = (
+        input_flow.data["sol_cont"].values
+        * (Material_Properties["Nitrogen Content"].values / 100)
+        * process_data["Degrades"].values
+    )
+
+    product.data["P_cont"] = (
+        input_flow.data["sol_cont"].values
+        * (Material_Properties["Phosphorus Content"].values / 100)
+        * process_data["Degrades"].values
+    )
+
+    product.data["K_cont"] = (
+        input_flow.data["sol_cont"].values
+        * (Material_Properties["Potassium Content"].values / 100)
+        * process_data["Degrades"].values
+    )
     return product
 
 
 ### AD Reactor
 def Reactor(input_flow, CommonData, process_data, input_data, Material_Properties, lci, flow_init):
     # Short names
     Engine_param = input_data.Engine_param
     Flare_param = input_data.Flare_param
     Biogas_gen = input_data.Biogas_gen
 
     # Methane production
-    CH4_prod_vol = (input_flow.data['sol_cont'].values / 1000
-                    * Material_Properties['Methane Yield'].values
-                    * process_data['L0 reached'].values / 100)
-
-    CH4_prod_mass_asC = (CH4_prod_vol
-                         * CommonData.STP['m3CH4_to_kg']['amount']
-                         * CommonData.MW['C']['amount'] / CommonData.MW['CH4']['amount'])
-
-    # Mehtane Balance
-    CH4_fugitiv_mass_asC = (CH4_prod_mass_asC
-                            * (1 - Biogas_gen['ad_collEff']['amount']))
-
-    CH4_Energy_rec_asC = (CH4_prod_mass_asC
-                          * Biogas_gen['ad_collEff']['amount']
-                          * (1 - Biogas_gen['ad_downTime']['amount']))
-
-    CH4_Flare_asC = (CH4_prod_mass_asC
-                     * Biogas_gen['ad_collEff']['amount']
-                     * Biogas_gen['ad_downTime']['amount'])
-
-    CH4_unburn_AsC = (CH4_Energy_rec_asC
-                      * (1 - Engine_param['CH4_destruction']['amount'])
-                      + CH4_Flare_asC
-                      * (1 - Flare_param['CH4_destruction']['amount']))
-
-    CO2_from_CH4Comb = (CH4_Energy_rec_asC
-                        * Engine_param['CH4_destruction']['amount']
-                        + CH4_Flare_asC
-                        * Flare_param['CH4_destruction']['amount'])
+    CH4_prod_vol = (
+        input_flow.data["sol_cont"].values
+        / 1000
+        * Material_Properties["Methane Yield"].values
+        * process_data["L0 reached"].values
+        / 100
+    )
+
+    CH4_prod_mass_asC = (
+        CH4_prod_vol
+        * CommonData.STP["m3CH4_to_kg"]["amount"]
+        * CommonData.MW["C"]["amount"]
+        / CommonData.MW["CH4"]["amount"]
+    )
+
+    # Methane Balance
+    CH4_fugitive_mass_asC = CH4_prod_mass_asC * (1 - Biogas_gen["ad_collEff"]["amount"])
+
+    CH4_Energy_rec_asC = (
+        CH4_prod_mass_asC
+        * Biogas_gen["ad_collEff"]["amount"]
+        * (1 - Biogas_gen["ad_downTime"]["amount"])
+    )
+
+    CH4_Flare_asC = (
+        CH4_prod_mass_asC * Biogas_gen["ad_collEff"]["amount"] * Biogas_gen["ad_downTime"]["amount"]
+    )
+
+    CH4_unburn_AsC = CH4_Energy_rec_asC * (
+        1 - Engine_param["CH4_destruction"]["amount"]
+    ) + CH4_Flare_asC * (1 - Flare_param["CH4_destruction"]["amount"])
+
+    CO2_from_CH4Comb = (
+        CH4_Energy_rec_asC * Engine_param["CH4_destruction"]["amount"]
+        + CH4_Flare_asC * Flare_param["CH4_destruction"]["amount"]
+    )
 
     # ENergy content
-    CH4_Energy_EngCont = (CH4_prod_vol * Biogas_gen['ad_collEff']['amount']
-                          * (1 - Biogas_gen['ad_downTime']['amount'])
-                          * Biogas_gen['ad_ch4EngCont']['amount'])
-
-    CH4_Flare_EngCont = (CH4_prod_vol * Biogas_gen['ad_collEff']['amount']
-                         * Biogas_gen['ad_downTime']['amount']
-                         * Biogas_gen['ad_ch4EngCont']['amount'])
+    CH4_Energy_EngCont = (
+        CH4_prod_vol
+        * Biogas_gen["ad_collEff"]["amount"]
+        * (1 - Biogas_gen["ad_downTime"]["amount"])
+        * Biogas_gen["ad_ch4EngCont"]["amount"]
+    )
+
+    CH4_Flare_EngCont = (
+        CH4_prod_vol
+        * Biogas_gen["ad_collEff"]["amount"]
+        * Biogas_gen["ad_downTime"]["amount"]
+        * Biogas_gen["ad_ch4EngCont"]["amount"]
+    )
 
     # Calculate emissions based on the energy content
-    CO_Comb = (CH4_Energy_EngCont * Engine_param['CO']['amount']
-               + CH4_Flare_EngCont * Flare_param['CO']['amount']) / 10**6
-
-    NOx_Comb = (CH4_Energy_EngCont * Engine_param['NO2']['amount']
-                + CH4_Flare_EngCont * Flare_param['NO2']['amount']) / 10**6
-
-    SO2_Comb = (CH4_Energy_EngCont * Engine_param['SO2']['amount']
-                + CH4_Flare_EngCont * Flare_param['SO2']['amount']) / 10**6
-
-    NMVOCs_Comb = (CH4_Energy_EngCont * Engine_param['NMVOC']['amount']
-                   + CH4_Flare_EngCont * Flare_param['NMVOC']['amount']) / 10**6
-
-    PM2_5_Comb = (CH4_Energy_EngCont * Engine_param['PM']['amount']
-                  + CH4_Flare_EngCont * Flare_param['PM']['amount']) / 10**6
-
-    lci.add(name='Fugitive (Leaked) Methane',
-            flow=(CH4_fugitiv_mass_asC
-                  * CommonData.MW['CH4']['amount'] / CommonData.MW['C']['amount']))
-
-    lci.add(name='Carbon dioxide, non-fossil from comubstion',
-            flow=(CO2_from_CH4Comb
-                  * CommonData.MW['CO2']['amount'] / CommonData.MW['C']['amount']))
-
-    lci.add(name='Methane, non-fossil (unburned)',
-            flow=(CH4_unburn_AsC
-                  * CommonData.MW['CH4']['amount'] / CommonData.MW['C']['amount']))
-
-    lci.add(name='Carbon monoxide (CO)', flow=CO_Comb)
-    lci.add(name='Nitrogen oxides (as NO2)', flow=NOx_Comb)
-    lci.add(name='Sulfur dioxide (SO2)', flow=SO2_Comb)
-    lci.add(name='NMVOCs', flow=NMVOCs_Comb)
-    lci.add(name='PM2.5', flow=PM2_5_Comb)
+    CO_Comb = (
+        CH4_Energy_EngCont * Engine_param["CO"]["amount"]
+        + CH4_Flare_EngCont * Flare_param["CO"]["amount"]
+    ) / 10**6
+
+    NOx_Comb = (
+        CH4_Energy_EngCont * Engine_param["NO2"]["amount"]
+        + CH4_Flare_EngCont * Flare_param["NO2"]["amount"]
+    ) / 10**6
+
+    SO2_Comb = (
+        CH4_Energy_EngCont * Engine_param["SO2"]["amount"]
+        + CH4_Flare_EngCont * Flare_param["SO2"]["amount"]
+    ) / 10**6
+
+    NMVOCs_Comb = (
+        CH4_Energy_EngCont * Engine_param["NMVOC"]["amount"]
+        + CH4_Flare_EngCont * Flare_param["NMVOC"]["amount"]
+    ) / 10**6
+
+    PM2_5_Comb = (
+        CH4_Energy_EngCont * Engine_param["PM"]["amount"]
+        + CH4_Flare_EngCont * Flare_param["PM"]["amount"]
+    ) / 10**6
+
+    lci.add(
+        name="Fugitive (Leaked) Methane",
+        flow=(
+            CH4_fugitive_mass_asC * CommonData.MW["CH4"]["amount"] / CommonData.MW["C"]["amount"]
+        ),
+    )
+
+    lci.add(
+        name="Carbon dioxide, non-fossil from combustion",
+        flow=(CO2_from_CH4Comb * CommonData.MW["CO2"]["amount"] / CommonData.MW["C"]["amount"]),
+    )
+
+    lci.add(
+        name="Methane, non-fossil (unburned)",
+        flow=(CH4_unburn_AsC * CommonData.MW["CH4"]["amount"] / CommonData.MW["C"]["amount"]),
+    )
+
+    lci.add(name="Carbon monoxide (CO)", flow=CO_Comb)
+    lci.add(name="Nitrogen oxides (as NO2)", flow=NOx_Comb)
+    lci.add(name="Sulfur dioxide (SO2)", flow=SO2_Comb)
+    lci.add(name="NMVOCs", flow=NMVOCs_Comb)
+    lci.add(name="PM2.5", flow=PM2_5_Comb)
 
     # Biogas production
-    BioGas_vol = CH4_prod_vol / Biogas_gen['ad_ch4stoich']['amount']
-    BioGas_mass = (CH4_prod_vol * CommonData.STP['m3CH4_to_kg']['amount']
-                   + (BioGas_vol - CH4_prod_vol) * CommonData.STP['m3CO2_to_kg']['amount'])
+    BioGas_vol = CH4_prod_vol / Biogas_gen["ad_ch4stoich"]["amount"]
+    BioGas_mass = (
+        CH4_prod_vol * CommonData.STP["m3CH4_to_kg"]["amount"]
+        + (BioGas_vol - CH4_prod_vol) * CommonData.STP["m3CO2_to_kg"]["amount"]
+    )
 
     # Electricity production
-    Elec_prod =  CH4_Energy_EngCont / Biogas_gen['ad_HeatRate']['amount']
-    lci.add(name=('Technosphere', 'Electricity_production'), flow=Elec_prod)
+    Elec_prod = CH4_Energy_EngCont / Biogas_gen["ad_HeatRate"]["amount"]
+    lci.add(name=("Technosphere", "Electricity_production"), flow=Elec_prod)
 
     # CO2 production
-    CO2_prod_mass_asC = ((BioGas_vol - CH4_prod_vol)
-                         * CommonData.STP['m3CO2_to_kg']['amount']
-                         * CommonData.MW['C']['amount'] / CommonData.MW['CO2']['amount'])
-
-    lci.add(name='Carbon dioxide, non-fossil (in biogas)',
-            flow=(CO2_prod_mass_asC
-                  * CommonData.MW['CO2']['amount'] / CommonData.MW['C']['amount']))
+    CO2_prod_mass_asC = (
+        (BioGas_vol - CH4_prod_vol)
+        * CommonData.STP["m3CO2_to_kg"]["amount"]
+        * CommonData.MW["C"]["amount"]
+        / CommonData.MW["CO2"]["amount"]
+    )
+
+    lci.add(
+        name="Carbon dioxide, non-fossil (in biogas)",
+        flow=(CO2_prod_mass_asC * CommonData.MW["CO2"]["amount"] / CommonData.MW["C"]["amount"]),
+    )
 
     # Water and Volatile solid in Biogas
-    BioGas_VS = BioGas_mass * Biogas_gen['perSolDec']['amount'] / 100
+    BioGas_VS = BioGas_mass * Biogas_gen["perSolDec"]["amount"] / 100
     BioGas_Water = BioGas_mass - BioGas_VS
 
     # Product
     product = deepcopy(flow_init)
-    product.data['vs_cont'] = (input_flow.data['vs_cont'].values
-                               - BioGas_VS)
+    product.data["vs_cont"] = input_flow.data["vs_cont"].values - BioGas_VS
 
-    product.data['ash_cont'] = input_flow.data['ash_cont'].values
+    product.data["ash_cont"] = input_flow.data["ash_cont"].values
 
-    product.data['sol_cont'] = (product.data['vs_cont'].values
-                                + product.data['ash_cont'])
+    product.data["sol_cont"] = product.data["vs_cont"].values + product.data["ash_cont"]
 
-    product.data['moist_cont'] = (input_flow.data['moist_cont'].values
-                                  - BioGas_Water)
+    product.data["moist_cont"] = input_flow.data["moist_cont"].values - BioGas_Water
 
-    product.data['mass'] = (product.data['moist_cont'].values
-                            + product.data['sol_cont'].values)
+    product.data["mass"] = product.data["moist_cont"].values + product.data["sol_cont"].values
 
-    product.data['C_cont'] = (input_flow.data['C_cont'].values
-                              - CO2_prod_mass_asC
-                              - CH4_prod_mass_asC)
+    product.data["C_cont"] = (
+        input_flow.data["C_cont"].values - CO2_prod_mass_asC - CH4_prod_mass_asC
+    )
 
-    product.data['N_cont'] = input_flow.data['N_cont'].values
-    product.data['P_cont'] = input_flow.data['P_cont'].values
-    product.data['K_cont'] = input_flow.data['K_cont'].values
+    product.data["N_cont"] = input_flow.data["N_cont"].values
+    product.data["P_cont"] = input_flow.data["P_cont"].values
+    product.data["K_cont"] = input_flow.data["K_cont"].values
 
     return product
 
 
 ### AD Dewater
-def Dewater(input_flow, input_to_reactor, CommonData, process_data, input_data, Material_Properties,
-            added_water, assumed_comp, lci, flow_init):
-    if input_data.AD_operation['isDw']['amount'] == 1:
+def Dewater(
+    input_flow,
+    input_to_reactor,
+    CommonData,
+    input_data,
+    Material_Properties,
+    assumed_comp,
+    lci,
+    flow_init,
+):
+    if input_data.AD_operation["isDw"]["amount"] == 1:
         # Calculating water removed
         """
         M: Moisture, S: solids, Liq: removed water, mc=moisture content
         mc = (M - Liq)/(S + M - Liq)
         -mc*Liq = M -Liq - S*mc - mc*M
         Liq = (M - S*mc - mc*M)/(1-mc)
         S + M = mass ==> Liq = (M - mass*mc)/(1-mc)
         """
-        liq_rem = ((input_flow.data['moist_cont'].values
-                    - input_flow.data['mass'].values
-                    * input_data.Dewater['ad_mcDigestate']['amount'])
-                   / (1 - input_data.Dewater['ad_mcDigestate']['amount']))
-
-        # Liquid to reatment, recirculate water
-        total_liq_to_treatment = (liq_rem
-                                  * (1 - input_data.AD_operation['recircMax']['amount']))
-
-        liq_treatment_vol = (total_liq_to_treatment / 1000
-                             / input_data.Dig_prop['digliqdens']['amount'])
+        liq_rem = (
+            input_flow.data["moist_cont"].values
+            - input_flow.data["mass"].values * input_data.Dewater["ad_mcDigestate"]["amount"]
+        ) / (1 - input_data.Dewater["ad_mcDigestate"]["amount"])
+
+        # Liquid to treatment, recirculate water
+        total_liq_to_treatment = liq_rem * (1 - input_data.AD_operation["recircMax"]["amount"])
+
+        liq_treatment_vol = (
+            total_liq_to_treatment / 1000 / input_data.Dig_prop["digliqdens"]["amount"]
+        )
         """
         Assumption: All the nutrients remains in the waste water flow to WWT.
         The assumed composition is used to calculate the fraction of incoming
         water that is removed.
         """
-        remv_to_incom = (sum(liq_rem * assumed_comp)
-                         / sum(input_flow.data['moist_cont'] * assumed_comp))
+        remv_to_incom = sum(liq_rem * assumed_comp) / sum(
+            input_flow.data["moist_cont"] * assumed_comp
+        )
 
         # Product
         product = deepcopy(flow_init)
-        product.data['vs_cont'] = input_flow.data['vs_cont'].values
-        product.data['ash_cont'] = input_flow.data['ash_cont'].values
-        product.data['sol_cont'] = input_flow.data['sol_cont'].values
-        product.data['moist_cont'] = input_flow.data['moist_cont'].values - liq_rem
-        product.data['mass'] = product.data['moist_cont'].values + product.data['sol_cont'].values
-        product.data['C_cont']= input_flow.data['C_cont'].values
-
-        product.data['N_cont'] = ((input_flow.data['N_cont'].values
-                                   * input_data.Dig_prop['perNSolid']['amount'] / 100)
-                                  + (input_flow.data['N_cont'].values
-                                     * (1 - input_data.Dig_prop['perNSolid']['amount'] / 100)
-                                     * (1 - remv_to_incom)))
-
-        product.data['P_cont'] = ((input_flow.data['P_cont'].values
-                                   * input_data.Dig_prop['perPSolid']['amount'] / 100)
-                                  + (input_flow.data['P_cont'].values
-                                     * (1 - input_data.Dig_prop['perPSolid']['amount'] / 100)
-                                     * (1 - remv_to_incom)))
-
-        product.data['K_cont'] = ((input_flow.data['K_cont'].values
-                                   * input_data.Dig_prop['perKSolid']['amount'] / 100)
-                                  + (input_flow.data['K_cont'].values
-                                     * (1 - input_data.Dig_prop['perKSolid']['amount'] / 100)
-                                     * (1 - remv_to_incom)))
+        product.data["vs_cont"] = input_flow.data["vs_cont"].values
+        product.data["ash_cont"] = input_flow.data["ash_cont"].values
+        product.data["sol_cont"] = input_flow.data["sol_cont"].values
+        product.data["moist_cont"] = input_flow.data["moist_cont"].values - liq_rem
+        product.data["mass"] = product.data["moist_cont"].values + product.data["sol_cont"].values
+        product.data["C_cont"] = input_flow.data["C_cont"].values
+
+        product.data["N_cont"] = (
+            input_flow.data["N_cont"].values * input_data.Dig_prop["perNSolid"]["amount"] / 100
+        ) + (
+            input_flow.data["N_cont"].values
+            * (1 - input_data.Dig_prop["perNSolid"]["amount"] / 100)
+            * (1 - remv_to_incom)
+        )
+
+        product.data["P_cont"] = (
+            input_flow.data["P_cont"].values * input_data.Dig_prop["perPSolid"]["amount"] / 100
+        ) + (
+            input_flow.data["P_cont"].values
+            * (1 - input_data.Dig_prop["perPSolid"]["amount"] / 100)
+            * (1 - remv_to_incom)
+        )
+
+        product.data["K_cont"] = (
+            input_flow.data["K_cont"].values * input_data.Dig_prop["perKSolid"]["amount"] / 100
+        ) + (
+            input_flow.data["K_cont"].values
+            * (1 - input_data.Dig_prop["perKSolid"]["amount"] / 100)
+            * (1 - remv_to_incom)
+        )
 
         # Resource use
-        Electricity = input_data.Dewater['elec_dw']['amount'] * input_flow.data['sol_cont'].values / 1000
-        lci.add(name=('Technosphere', 'Electricity_consumption'), flow=Electricity)
+        Electricity = (
+            input_data.Dewater["elec_dw"]["amount"] * input_flow.data["sol_cont"].values / 1000
+        )
+        lci.add(name=("Technosphere", "Electricity_consumption"), flow=Electricity)
 
         # POTW
-        solid_content = 1 - Material_Properties['Moisture Content'].values / 100
+        solid_content = 1 - Material_Properties["Moisture Content"].values / 100
         # Allocation factor
         """
         AF_total: total emission(Mg) * volume of waste water(m3)
         """
         AF_total = {}
-        AF_total['COD'] = sum(solid_content
-                              * Material_Properties['Biogenic Carbon Content'].values / 100
-                              * assumed_comp
-                              * liq_treatment_vol)
-
-        AF_total['BOD'] = sum(solid_content
-                              * Material_Properties['Methane Yield'].values
-                              * assumed_comp
-                              * liq_treatment_vol)
-
-        AF_total['TSS'] = sum(assumed_comp * liq_treatment_vol)
-
-        AF_total['Total_N'] = sum(input_to_reactor.data['N_cont'].values
-                                  * assumed_comp
-                                  * liq_treatment_vol)
-
-        AF_total['Phosphate'] = sum(input_to_reactor.data['P_cont'].values
-                                    * assumed_comp
-                                    * liq_treatment_vol)
-
-        for i in ['Iron', 'Copper', 'Cadmium', 'Arsenic', 'Mercury', 'Selenium',
-                  'Chromium', 'Lead', 'Zinc', 'Barium', 'Silver']:
-            AF_total[i] = sum(solid_content
-                              * Material_Properties[i].values / 100
-                              * assumed_comp
-                              * liq_treatment_vol)
+        AF_total["COD"] = sum(
+            solid_content
+            * Material_Properties["Biogenic Carbon Content"].values
+            / 100
+            * assumed_comp
+            * liq_treatment_vol
+        )
+
+        AF_total["BOD"] = sum(
+            solid_content
+            * Material_Properties["Methane Yield"].values
+            * assumed_comp
+            * liq_treatment_vol
+        )
+
+        AF_total["TSS"] = sum(assumed_comp * liq_treatment_vol)
+
+        AF_total["Total_N"] = sum(
+            input_to_reactor.data["N_cont"].values * assumed_comp * liq_treatment_vol
+        )
+
+        AF_total["Phosphate"] = sum(
+            input_to_reactor.data["P_cont"].values * assumed_comp * liq_treatment_vol
+        )
+
+        for i in [
+            "Iron",
+            "Copper",
+            "Cadmium",
+            "Arsenic",
+            "Mercury",
+            "Selenium",
+            "Chromium",
+            "Lead",
+            "Zinc",
+            "Barium",
+            "Silver",
+        ]:
+            AF_total[i] = sum(
+                solid_content
+                * Material_Properties[i].values
+                / 100
+                * assumed_comp
+                * liq_treatment_vol
+            )
 
         AF = {}
-        AF['COD'] = (solid_content
-                     * Material_Properties['Biogenic Carbon Content'].values / 100
-                     * liq_treatment_vol / AF_total['COD'])
-
-        AF['BOD'] = (solid_content
-                     * Material_Properties['Methane Yield'].values
-                     * liq_treatment_vol / AF_total['BOD'])
-
-        AF['TSS'] = liq_treatment_vol / AF_total['TSS']
-
-        AF['Total_N'] = (input_to_reactor.data['N_cont'].values
-                         * liq_treatment_vol / AF_total['Total_N'])
-
-        AF['Phosphate'] = (solid_content
-                           * Material_Properties['Phosphorus Content'].values / 100
-                           * liq_treatment_vol / AF_total['Phosphate'])
-
-        for i in ['Iron', 'Copper', 'Cadmium', 'Arsenic', 'Mercury', 'Selenium',
-                  'Chromium', 'Lead', 'Zinc', 'Barium', 'Silver']:
+        AF["COD"] = (
+            solid_content
+            * Material_Properties["Biogenic Carbon Content"].values
+            / 100
+            * liq_treatment_vol
+            / AF_total["COD"]
+        )
+
+        AF["BOD"] = (
+            solid_content
+            * Material_Properties["Methane Yield"].values
+            * liq_treatment_vol
+            / AF_total["BOD"]
+        )
+
+        AF["TSS"] = liq_treatment_vol / AF_total["TSS"]
+
+        AF["Total_N"] = (
+            input_to_reactor.data["N_cont"].values * liq_treatment_vol / AF_total["Total_N"]
+        )
+
+        AF["Phosphate"] = (
+            solid_content
+            * Material_Properties["Phosphorus Content"].values
+            / 100
+            * liq_treatment_vol
+            / AF_total["Phosphate"]
+        )
+
+        for i in [
+            "Iron",
+            "Copper",
+            "Cadmium",
+            "Arsenic",
+            "Mercury",
+            "Selenium",
+            "Chromium",
+            "Lead",
+            "Zinc",
+            "Barium",
+            "Silver",
+        ]:
             if AF_total[i] == 0:
-                AF[i]=0
+                AF[i] = 0
             else:
-                AF[i] = (solid_content
-                         * Material_Properties[i].values/100
-                         * liq_treatment_vol / AF_total[i])
+                AF[i] = (
+                    solid_content
+                    * Material_Properties[i].values
+                    / 100
+                    * liq_treatment_vol
+                    / AF_total[i]
+                )
 
         # Emission from POTW
-        Emission={}
+        Emission = {}
 
-        Emission['Total_N'] =  (input_to_reactor.data['N_cont'].values
-                                * (1 - input_data.Dig_prop['perNSolid']['amount'] / 100)
-                                * remv_to_incom
-                                * (1-CommonData.WWT['n_rem']['amount']/100))
-
-        Emission['Phosphate'] = (input_to_reactor.data['P_cont'].values
-                                 * (1 - input_data.Dig_prop['perPSolid']['amount'] / 100)
-                                 * remv_to_incom
-                                 *(94.97/30.97)
-                                 * (1 - CommonData.WWT['p_rem']['amount'] /100))
-
-        for i,j,k in [('COD','lchCODcont','cod_rem'),('BOD','lchBODcont','bod_rem'),('TSS','lchTSScont','tss_rem')\
-                      ,('Iron','conc_Fe','metals_rem'),('Copper','conc_Cu','metals_rem'),('Cadmium','conc_Cd','metals_rem')\
-                      ,('Arsenic','conc_As','metals_rem'),('Mercury','conc_Hg','metals_rem'),('Selenium','conc_Se','metals_rem')\
-                      ,('Chromium','conc_Cr','metals_rem'),('Lead','conc_Pb','metals_rem'),('Zinc','conc_Zn','metals_rem')\
-                      ,('Barium','conc_Ba','metals_rem'),('Silver','conc_Ag','metals_rem')]:
-            Emission[i] = (input_data.Digestate_treatment[j]['amount']
-                           * liq_treatment_vol
-                           * (1 - CommonData.WWT[k]['amount'] / 100)
-                           * AF[i])
-
-        for i,j in [('COD','COD'),('BOD','BOD'),('TSS','Total suspended solids')\
-                      ,('Iron','Iron'),('Copper','Copper'),('Cadmium','Cadmium')\
-                      ,('Arsenic','Arsenic'),('Mercury','Mercury'),('Phosphate','Phosphate'),('Selenium','Selenium')\
-                      ,('Chromium','Chromium'),('Lead','Lead'),('Zinc','Zinc')\
-                      ,('Barium','Barium'),('Silver','Silver'),('Total_N','Total N')]:
+        Emission["Total_N"] = (
+            input_to_reactor.data["N_cont"].values
+            * (1 - input_data.Dig_prop["perNSolid"]["amount"] / 100)
+            * remv_to_incom
+            * (1 - CommonData.WWT["n_rem"]["amount"] / 100)
+        )
+
+        Emission["Phosphate"] = (
+            input_to_reactor.data["P_cont"].values
+            * (1 - input_data.Dig_prop["perPSolid"]["amount"] / 100)
+            * remv_to_incom
+            * (94.97 / 30.97)
+            * (1 - CommonData.WWT["p_rem"]["amount"] / 100)
+        )
+
+        for i, j, k in [
+            ("COD", "lchCODcont", "cod_rem"),
+            ("BOD", "lchBODcont", "bod_rem"),
+            ("TSS", "lchTSScont", "tss_rem"),
+            ("Iron", "conc_Fe", "metals_rem"),
+            ("Copper", "conc_Cu", "metals_rem"),
+            ("Cadmium", "conc_Cd", "metals_rem"),
+            ("Arsenic", "conc_As", "metals_rem"),
+            ("Mercury", "conc_Hg", "metals_rem"),
+            ("Selenium", "conc_Se", "metals_rem"),
+            ("Chromium", "conc_Cr", "metals_rem"),
+            ("Lead", "conc_Pb", "metals_rem"),
+            ("Zinc", "conc_Zn", "metals_rem"),
+            ("Barium", "conc_Ba", "metals_rem"),
+            ("Silver", "conc_Ag", "metals_rem"),
+        ]:
+            Emission[i] = (
+                input_data.Digestate_treatment[j]["amount"]
+                * liq_treatment_vol
+                * (1 - CommonData.WWT[k]["amount"] / 100)
+                * AF[i]
+            )
+
+        for i, j in [
+            ("COD", "COD"),
+            ("BOD", "BOD"),
+            ("TSS", "Total suspended solids"),
+            ("Iron", "Iron"),
+            ("Copper", "Copper"),
+            ("Cadmium", "Cadmium"),
+            ("Arsenic", "Arsenic"),
+            ("Mercury", "Mercury"),
+            ("Phosphate", "Phosphate"),
+            ("Selenium", "Selenium"),
+            ("Chromium", "Chromium"),
+            ("Lead", "Lead"),
+            ("Zinc", "Zinc"),
+            ("Barium", "Barium"),
+            ("Silver", "Silver"),
+            ("Total_N", "Total N"),
+        ]:
             lci.add(name=j, flow=Emission[i])
 
-
-        BOD_removed = (input_data.Digestate_treatment['lchBODcont']['amount']
-                       * AF['BOD'] * liq_treatment_vol
-                       * CommonData.WWT['bod_rem']['amount'] / 100)
-
-        lci.add(name='CO2-biogenic emissions from digested liquids treatment',
-                flow=(BOD_removed
-                      * CommonData.Leachate_treat['co2bod']['amount']))
+        BOD_removed = (
+            input_data.Digestate_treatment["lchBODcont"]["amount"]
+            * AF["BOD"]
+            * liq_treatment_vol
+            * CommonData.WWT["bod_rem"]["amount"]
+            / 100
+        )
+
+        lci.add(
+            name="CO2-biogenic emissions from digested liquids treatment",
+            flow=(BOD_removed * CommonData.Leachate_treat["co2bod"]["amount"]),
+        )
 
         # Sludge to LF
-        sludge_prod = liq_treatment_vol * CommonData.Leachate_treat['sludgef']['amount'] # Unit kg
+        sludge_prod = liq_treatment_vol * CommonData.Leachate_treat["sludgef"]["amount"]  # Unit kg
 
-        # Resouce use
-        lci.add(name=('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'),
-                flow=(input_data.Digestate_treatment['ad_distPOTW']['amount']
-                      * liq_treatment_vol * 1000
-                      * input_data.Dig_prop['digliqdens']['amount']))
-
-        lci.add(name=('Technosphere', 'Empty_Return_Heavy_Duty_Diesel_Truck'),
-                flow=(liq_treatment_vol
-                      * input_data.Dig_prop['digliqdens']['amount']
-                      / input_data.Digestate_treatment['payload_POTW']['amount']
-                      * input_data.Digestate_treatment['ad_distPOTW']['amount']
-                      * input_data.Digestate_treatment['ad_erPOTW']['amount']))
-
-        lci.add(name=('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'),
-                flow=(input_data.Digestate_treatment['wwtp_lf_dist']['amount']
-                      * sludge_prod))
-
-        lci.add(name=('Technosphere', 'Empty_Return_Heavy_Duty_Diesel_Truck'),
-                flow=(input_data.Digestate_treatment['wwtp_lf_dist']['amount']
-                      * sludge_prod / 1000
-                      / input_data.Digestate_treatment['payload_LFPOTW']['amount']
-                      * input_data.Digestate_treatment['er_wwtpLF']['amount']))
-
-        lci.add(name=('Technosphere', 'Electricity_consumption'),
-                flow=(BOD_removed
-                      * CommonData.Leachate_treat['elecBOD']['amount']))
+        # Resource use
+        lci.add(
+            name=("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"),
+            flow=(
+                input_data.Digestate_treatment["ad_distPOTW"]["amount"]
+                * liq_treatment_vol
+                * 1000
+                * input_data.Dig_prop["digliqdens"]["amount"]
+            ),
+        )
+
+        lci.add(
+            name=("Technosphere", "Empty_Return_Heavy_Duty_Diesel_Truck"),
+            flow=(
+                liq_treatment_vol
+                * input_data.Dig_prop["digliqdens"]["amount"]
+                / input_data.Digestate_treatment["payload_POTW"]["amount"]
+                * input_data.Digestate_treatment["ad_distPOTW"]["amount"]
+                * input_data.Digestate_treatment["ad_erPOTW"]["amount"]
+            ),
+        )
+
+        lci.add(
+            name=("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"),
+            flow=(input_data.Digestate_treatment["wwtp_lf_dist"]["amount"] * sludge_prod),
+        )
+
+        lci.add(
+            name=("Technosphere", "Empty_Return_Heavy_Duty_Diesel_Truck"),
+            flow=(
+                input_data.Digestate_treatment["wwtp_lf_dist"]["amount"]
+                * sludge_prod
+                / 1000
+                / input_data.Digestate_treatment["payload_LFPOTW"]["amount"]
+                * input_data.Digestate_treatment["er_wwtpLF"]["amount"]
+            ),
+        )
+
+        lci.add(
+            name=("Technosphere", "Electricity_consumption"),
+            flow=(BOD_removed * CommonData.Leachate_treat["elecBOD"]["amount"]),
+        )
 
     else:
         product = deepcopy(input_flow)
         liq_rem = np.zeros_like(input_flow.data.index)
         liq_treatment_vol = np.zeros_like(input_flow.data.index)
         # add zero flows to LCI as placeholder
-        for i,j in [('COD' ,'COD'), ('BOD', 'BOD'), ('TSS', 'Total suspended solids'),
-                    ('Iron', 'Iron'), ('Copper', 'Copper'), ('Cadmium', 'Cadmium'),
-                    ('Arsenic', 'Arsenic'), ('Mercury', 'Mercury'), ('Phosphate', 'Phosphate'),
-                    ('Selenium', 'Selenium'), ('Chromium', 'Chromium'),
-                    ('Lead', 'Lead'), ('Zinc', 'Zinc'), ('Barium', 'Barium'),
-                    ('Silver', 'Silver'), ('Total_N', 'Total N')]:
+        for i, j in [
+            ("COD", "COD"),
+            ("BOD", "BOD"),
+            ("TSS", "Total suspended solids"),
+            ("Iron", "Iron"),
+            ("Copper", "Copper"),
+            ("Cadmium", "Cadmium"),
+            ("Arsenic", "Arsenic"),
+            ("Mercury", "Mercury"),
+            ("Phosphate", "Phosphate"),
+            ("Selenium", "Selenium"),
+            ("Chromium", "Chromium"),
+            ("Lead", "Lead"),
+            ("Zinc", "Zinc"),
+            ("Barium", "Barium"),
+            ("Silver", "Silver"),
+            ("Total_N", "Total N"),
+        ]:
             lci.add(name=j, flow=0)
-        lci.add(name='CO2-biogenic emissions from digested liquids treatment', flow=0)
-        lci.add(name=('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'),
-                flow=0)
-        lci.add(name=('Technosphere', 'Empty_Return_Heavy_Duty_Diesel_Truck'), flow=0)
-        lci.add(name=('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'), flow=0)
-        lci.add(name=('Technosphere', 'Electricity_consumption'), flow=0)
+        lci.add(name="CO2-biogenic emissions from digested liquids treatment", flow=0)
+        lci.add(
+            name=("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"), flow=0
+        )
+        lci.add(name=("Technosphere", "Empty_Return_Heavy_Duty_Diesel_Truck"), flow=0)
+        lci.add(
+            name=("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"), flow=0
+        )
+        lci.add(name=("Technosphere", "Electricity_consumption"), flow=0)
 
     return product, liq_rem, liq_treatment_vol
 
 
 ### AD_Mixing two flows
 def mix(input1, input2, Material_Properties, flow_init):
     product = deepcopy(flow_init)
-    product.data['mass'] = (input1.data['mass'].values
-                            + input2.data['mass'].values)
+    product.data["mass"] = input1.data["mass"].values + input2.data["mass"].values
 
-    product.data['sol_cont'] = (input1.data['sol_cont'].values
-                                + input2.data['sol_cont'].values)
+    product.data["sol_cont"] = input1.data["sol_cont"].values + input2.data["sol_cont"].values
 
-    product.data['moist_cont'] = (input1.data['moist_cont'].values
-                                  + input2.data['moist_cont'].values)
+    product.data["moist_cont"] = input1.data["moist_cont"].values + input2.data["moist_cont"].values
 
-    product.data['vs_cont'] = (input1.data['vs_cont'].values
-                               + input2.data['vs_cont'].values)
+    product.data["vs_cont"] = input1.data["vs_cont"].values + input2.data["vs_cont"].values
 
-    product.data['ash_cont'] = (input1.data['ash_cont'].values
-                                + input2.data['ash_cont'].values)
+    product.data["ash_cont"] = input1.data["ash_cont"].values + input2.data["ash_cont"].values
 
-    product.data['C_cont'] = (input1.data['C_cont'].values
-                              + input2.data['sol_cont'].values
-                              * Material_Properties['Biogenic Carbon Content'].values / 100)
+    product.data["C_cont"] = (
+        input1.data["C_cont"].values
+        + input2.data["sol_cont"].values
+        * Material_Properties["Biogenic Carbon Content"].values
+        / 100
+    )
 
-    product.data['N_cont'] = (input1.data['N_cont'].values
-                              + input2.data['sol_cont'].values
-                              * Material_Properties['Nitrogen Content'].values / 100)
+    product.data["N_cont"] = (
+        input1.data["N_cont"].values
+        + input2.data["sol_cont"].values * Material_Properties["Nitrogen Content"].values / 100
+    )
 
-    product.data['P_cont'] = (input1.data['P_cont'].values
-                              + input2.data['sol_cont'].values
-                              * Material_Properties['Phosphorus Content'].values / 100)
+    product.data["P_cont"] = (
+        input1.data["P_cont"].values
+        + input2.data["sol_cont"].values * Material_Properties["Phosphorus Content"].values / 100
+    )
 
-    product.data['K_cont'] = (input1.data['K_cont'].values
-                              + input2.data['sol_cont'].values
-                              * Material_Properties['Potassium Content'].values / 100)
+    product.data["K_cont"] = (
+        input1.data["K_cont"].values
+        + input2.data["sol_cont"].values * Material_Properties["Potassium Content"].values / 100
+    )
     return product
 
+
 ### AD Curing
-def curing(input_flow, input_to_reactor, CommonData, process_data, input_data, assumed_comp, Material_Properties, lci, flow_init):
-        if input_data.AD_operation['isCured']['amount'] == 1:
-            input_flow.update(assumed_comp)
-            # Calculate wood chips\screen rejects for moisture control
-            WC_SR = ((input_flow.data['moist_cont']
-                      - input_data.Dig_prop['mcInitComp']['amount']
-                      * input_flow.flow)
-                     / (input_data.Dig_prop['mcInitComp']['amount']
-                        - input_data.Material_Properties['wcMC']['amount']))
-
-            # Carbon balance
-            C_Remain = np.where(input_flow.data['C_cont'].values / input_to_reactor.data['C_cont'].apply(lambda x: 1 if x <= 0 else x ).values
-                                <= (1 - process_data['C_loss'].values / 100),
-                                input_flow.data['C_cont'].values,
-                                input_to_reactor.data['C_cont'].values * (1 - process_data['C_loss'].values / 100))
-            C_loss = input_flow.data['C_cont'].values - C_Remain
-
-            C_loss_as_CH4 = input_data.Curing_Bio['ad_pCasCH4']['amount'] * C_loss
-            C_loss_as_CO2 = C_loss - C_loss_as_CH4
-
-            lci.add(name='Methane, non-fossil',
-                    flow=C_loss_as_CH4 * CommonData.MW['CH4']['amount'] / CommonData.MW['C']['amount'])
-            lci.add(name='Carbon dioxide, non-fossil _ Curing',
-                    flow=C_loss_as_CO2 * CommonData.MW['CO2']['amount'] / CommonData.MW['C']['amount'])
-
-            # Nitrogen balance
-            N_loss = input_flow.data['N_cont'].values * process_data['N_loss'].values
-            N_loss_as_N2O = N_loss * input_data.Curing_Bio['ad_pNasN2O']['amount']
-            N_loss_as_NH3 = N_loss * input_data.Curing_Bio['ad_pNasNH3']['amount']
-
-            lci.add(name='Ammonia',
-                    flow=N_loss_as_NH3 * CommonData.MW['Ammonia']['amount'] / CommonData.MW['N']['amount'])
-            lci.add(name='Dinitrogen monoxide',
-                    flow=N_loss_as_N2O * CommonData.MW['Nitrous_Oxide']['amount'] / CommonData.MW['N']['amount'] / 2)
-
-            # VOC emission
-            VS_loss = input_data.Curing_Bio['VSlossPerCloss']['amount'] * C_loss / CommonData.MW['C']['amount']
-            VOC_emitted = VS_loss * process_data['VOC to VS_loss'].values / 1000000
-            lci.add(name='NMVOC, non-methane volatile organic compounds, unspecified origin',
-                    flow=VOC_emitted)
-
-            # Product
-            product = deepcopy(flow_init)
-            product.data['vs_cont'] = input_flow.data['vs_cont'].values - VS_loss
-            product.data['ash_cont'] = input_flow.data['ash_cont'].values
-            product.data['sol_cont'] = product.data['vs_cont'].values + product.data['ash_cont'].values
-
-            product.data['C_cont'] = input_flow.data['C_cont'].values - C_loss
-            product.data['N_cont'] = input_flow.data['N_cont'].values - N_loss
-            product.data['P_cont'] = input_flow.data['P_cont'].values
-            product.data['K_cont'] = input_flow.data['K_cont'].values
-
-            # Product
-            product.data['moist_cont'] = (product.data['sol_cont'].values
-                                          / (1 - input_data.Material_Properties['ad_mcFC']['amount'])
-                                          * input_data.Material_Properties['ad_mcFC']['amount'])
-
-            product.data['mass'] = product.data['moist_cont'].values + product.data['sol_cont'].values
-
-            # Resource use
-            loder_dsl = (input_flow.data['mass'].values / 1000
-                         * input_data.Loader['hpFEL']['amount']
-                         * input_data.Loader['mfFEL']['amount']
-                         * input_data.AD_operation['ophrsperday']['amount'])
-
-            WC_shred_dsl = (input_data.shredding['Mtgp']['amount']
-                            * input_data.shredding['Mtgf']['amount']
-                            * WC_SR / 1000)
-
-            Windrow_turner_dsl = ((WC_SR + input_flow.data['mass'].values) / 1000
-                                  * input_data.Windrow_turn['Tcur']['amount']
-                                  * input_data.Windrow_turn['Mwta']['amount']
-                                  * input_data.Windrow_turn['turnFreq']['amount']
-                                  * input_data.Windrow_turn['Mwfa']['amount'])
-
-            lci.add(name=('Technosphere', 'Equipment_Diesel'),
-                    flow=(loder_dsl
-                          + WC_shred_dsl
-                          + Windrow_turner_dsl))
+def curing(
+    input_flow,
+    input_to_reactor,
+    CommonData,
+    process_data,
+    input_data,
+    assumed_comp,
+    lci,
+    flow_init,
+):
+    if input_data.AD_operation["isCured"]["amount"] == 1:
+        input_flow.update(assumed_comp)
+        # Calculate wood chips\screen rejects for moisture control
+        WC_SR = (
+            input_flow.data["moist_cont"]
+            - input_data.Dig_prop["mcInitComp"]["amount"] * input_flow.flow
+        ) / (
+            input_data.Dig_prop["mcInitComp"]["amount"]
+            - input_data.Material_Properties["wcMC"]["amount"]
+        )
+
+        # Carbon balance
+        C_Remain = np.where(
+            input_flow.data["C_cont"].values
+            / input_to_reactor.data["C_cont"].apply(lambda x: 1 if x <= 0 else x).values
+            <= (1 - process_data["C_loss"].values / 100),
+            input_flow.data["C_cont"].values,
+            input_to_reactor.data["C_cont"].values * (1 - process_data["C_loss"].values / 100),
+        )
+        C_loss = input_flow.data["C_cont"].values - C_Remain
+
+        C_loss_as_CH4 = input_data.Curing_Bio["ad_pCasCH4"]["amount"] * C_loss
+        C_loss_as_CO2 = C_loss - C_loss_as_CH4
+
+        lci.add(
+            name="Methane, non-fossil",
+            flow=C_loss_as_CH4 * CommonData.MW["CH4"]["amount"] / CommonData.MW["C"]["amount"],
+        )
+        lci.add(
+            name="Carbon dioxide, non-fossil _ Curing",
+            flow=C_loss_as_CO2 * CommonData.MW["CO2"]["amount"] / CommonData.MW["C"]["amount"],
+        )
+
+        # Nitrogen balance
+        N_loss = input_flow.data["N_cont"].values * process_data["N_loss"].values
+        N_loss_as_N2O = N_loss * input_data.Curing_Bio["ad_pNasN2O"]["amount"]
+        N_loss_as_NH3 = N_loss * input_data.Curing_Bio["ad_pNasNH3"]["amount"]
+
+        lci.add(
+            name="Ammonia",
+            flow=N_loss_as_NH3 * CommonData.MW["Ammonia"]["amount"] / CommonData.MW["N"]["amount"],
+        )
+        lci.add(
+            name="Dinitrogen monoxide",
+            flow=N_loss_as_N2O
+            * CommonData.MW["Nitrous_Oxide"]["amount"]
+            / CommonData.MW["N"]["amount"]
+            / 2,
+        )
+
+        # VOC emission
+        VS_loss = (
+            input_data.Curing_Bio["VSlossPerCloss"]["amount"]
+            * C_loss
+            / CommonData.MW["C"]["amount"]
+        )
+        VOC_emitted = VS_loss * process_data["VOC to VS_loss"].values / 1000000
+        lci.add(
+            name="NMVOC, non-methane volatile organic compounds, unspecified origin",
+            flow=VOC_emitted,
+        )
+
+        # Product
+        product = deepcopy(flow_init)
+        product.data["vs_cont"] = input_flow.data["vs_cont"].values - VS_loss
+        product.data["ash_cont"] = input_flow.data["ash_cont"].values
+        product.data["sol_cont"] = product.data["vs_cont"].values + product.data["ash_cont"].values
+
+        product.data["C_cont"] = input_flow.data["C_cont"].values - C_loss
+        product.data["N_cont"] = input_flow.data["N_cont"].values - N_loss
+        product.data["P_cont"] = input_flow.data["P_cont"].values
+        product.data["K_cont"] = input_flow.data["K_cont"].values
+
+        # Product
+        product.data["moist_cont"] = (
+            product.data["sol_cont"].values
+            / (1 - input_data.Material_Properties["ad_mcFC"]["amount"])
+            * input_data.Material_Properties["ad_mcFC"]["amount"]
+        )
+
+        product.data["mass"] = product.data["moist_cont"].values + product.data["sol_cont"].values
+
+        # Resource use
+        loader_dsl = (
+            input_flow.data["mass"].values
+            / 1000
+            * input_data.Loader["hpFEL"]["amount"]
+            * input_data.Loader["mfFEL"]["amount"]
+            * input_data.AD_operation["ophrsperday"]["amount"]
+        )
+
+        WC_shred_dsl = (
+            input_data.shredding["Mtgp"]["amount"]
+            * input_data.shredding["Mtgf"]["amount"]
+            * WC_SR
+            / 1000
+        )
+
+        Windrow_turner_dsl = (
+            (WC_SR + input_flow.data["mass"].values)
+            / 1000
+            * input_data.Windrow_turn["Tcur"]["amount"]
+            * input_data.Windrow_turn["Mwta"]["amount"]
+            * input_data.Windrow_turn["turnFreq"]["amount"]
+            * input_data.Windrow_turn["Mwfa"]["amount"]
+        )
+
+        lci.add(
+            name=("Technosphere", "Equipment_Diesel"),
+            flow=(loader_dsl + WC_shred_dsl + Windrow_turner_dsl),
+        )
+
+    return product, WC_SR
 
-        return product, WC_SR
 
 ### AD Post_screen
-def Post_screen(input_flow, input_WC_SR, input_data, assumed_comp, Material_Properties, lci, flow_init):
+def Post_screen(input_flow, input_WC_SR, input_data, lci, flow_init):
     product = deepcopy(flow_init)
 
-    Screen_rejects = input_WC_SR * input_data.Post_Screen['ad_scrEff_WC']['amount']
+    Screen_rejects = input_WC_SR * input_data.Post_Screen["ad_scrEff_WC"]["amount"]
     Remain_WC = input_WC_SR - Screen_rejects
 
     # Product
     product = deepcopy(input_flow)
 
     # Resource use
-    Electricity = (input_data.Post_Screen['ad_engScreen']['amount']
-                   * (input_flow.data['mass'].values + input_WC_SR))
-    lci.add(name=('Technosphere', 'Electricity_consumption'),
-            flow=Electricity)
+    Electricity = input_data.Post_Screen["ad_engScreen"]["amount"] * (
+        input_flow.data["mass"].values + input_WC_SR
+    )
+    lci.add(name=("Technosphere", "Electricity_consumption"), flow=Electricity)
     return product, Remain_WC, Screen_rejects
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/AnF.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/AnF.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Jan  6 12:48:05 2022
+import numpy as np
+import numpy_financial as npf
+from swolfpy_inputdata import AnF_Input
 
-@author: msardar2
-"""
+from .Common_subprocess import LCI, Flow
+from .MRF_subprocess import (
+    Conveyor,
+    Dewater,
+    Drum_Feeder,
+    Dryer,
+    Electricity,
+    Pelletizer,
+    Shredder,
+    Sorting,
+    Sterilizer,
+)
 from .ProcessModel import ProcessModel
-from swolfpy_inputdata import AnF_Input
-from .Common_subprocess import Flow, LCI
-from .MRF_subprocess import Drum_Feeder, Sorting, Shredder, Sterilizer, Dewater, Dryer, Pelletizer
-from .MRF_subprocess import Conveyor, Electricity
-import numpy_financial as npf
-import numpy as np
 
 
 class AnF(ProcessModel):
-    Process_Type = 'Treatment'
-    def __init__(self, process_name='Animal Feed', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Treatment"
+
+    def __init__(self, process_name="Animal Feed", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = AnF_Input(input_data_path=input_data_path,
-                                  process_name=self.process_name,
-                                  CommonDataObjct=CommonDataObjct)
+        self.InputData = AnF_Input(
+            input_data_path=input_data_path,
+            process_name=self.process_name,
+            CommonDataObjct=CommonDataObjct,
+        )
 
-        self.Assumed_Comp = self.InputData.process_data['Assumed_Comp']
+        self.Assumed_Comp = self.InputData.process_data["Assumed_Comp"]
 
         self.process_data = self.InputData.process_data
 
         self.flow_init = Flow(self.Material_Properties)
 
     def calc(self):
         self.LCI = LCI(index=self.Index)
@@ -34,143 +42,152 @@
         # Initial mass at tipping floor
         self._Input = np.array(self.Assumed_Comp)
 
         # Drum Feeder
         self._DF_feed = Drum_Feeder(self._Input, self.InputData, self.LCI)
 
         # Disk Screen
-        self._DS_rmnd, self._DS_rmvd = Sorting(Input=self._DF_feed,
-                                               sep_eff=self.process_data['Disk Screen'].values/100,
-                                               InputData=self.InputData,
-                                               Eqpt_data=self.InputData.Eq_DS,
-                                               LCI=self.LCI)
+        self._DS_rmnd, self._DS_rmvd = Sorting(
+            Input=self._DF_feed,
+            sep_eff=self.process_data["Disk Screen"].values / 100,
+            InputData=self.InputData,
+            Eqpt_data=self.InputData.Eq_DS,
+            LCI=self.LCI,
+        )
 
         # Manual Sorting
-        self._MS_rmnd, self._MS_rmvd = Sorting(Input=self._DS_rmnd,
-                                               sep_eff=self.process_data['Manual Sort (Negative)'].values/100,
-                                               InputData=self.InputData,
-                                               Eqpt_data=self.InputData.Eq_Neg_Sort,
-                                               LCI=self.LCI)
+        self._MS_rmnd, self._MS_rmvd = Sorting(
+            Input=self._DS_rmnd,
+            sep_eff=self.process_data["Manual Sort (Negative)"].values / 100,
+            InputData=self.InputData,
+            Eqpt_data=self.InputData.Eq_Neg_Sort,
+            LCI=self.LCI,
+        )
 
-        self.LCI.add('Other_Residual', self._MS_rmvd + self._DS_rmvd)
+        self.LCI.add("Other_Residual", self._MS_rmvd + self._DS_rmvd)
 
         # Shredding/Grinding
-        self._Shred = Shredder(Input=self._MS_rmnd,
-                              InputData=self.InputData,
-                              LCI=self.LCI)
-
-        # Sterlizing
-        self._Sterilized = Sterilizer(Input=self._Shred,
-                                      InputData=self.InputData,
-                                      LCI=self.LCI)
+        self._Shred = Shredder(Input=self._MS_rmnd, InputData=self.InputData, LCI=self.LCI)
+
+        # Sterilizing
+        self._Sterilized = Sterilizer(Input=self._Shred, InputData=self.InputData, LCI=self.LCI)
 
         # Dewatering
         self._Dewatered, self._waste_water = Dewater(
             Input=self._Sterilized,
             InputData=self.InputData,
             MaterialProperties=self.Material_Properties,
-            LCI=self.LCI)
+            LCI=self.LCI,
+        )
 
-        if self.InputData.AnF_operation['isDried']['amount']:
+        if self.InputData.AnF_operation["isDried"]["amount"]:
             # Pelletizing
-            self._Pellet = Pelletizer(Input=self._Dewatered,
-                                  InputData=self.InputData,
-                                  LCI=self.LCI)
+            self._Pellet = Pelletizer(Input=self._Dewatered, InputData=self.InputData, LCI=self.LCI)
 
             # Drier
-            self._Dried = Dryer(Input=self._Pellet,
-                          InputData=self.InputData,
-                          LCI=self.LCI)
+            self._Dried = Dryer(Input=self._Pellet, InputData=self.InputData, LCI=self.LCI)
 
         # conveyor
         self._Mass_toConveyor = (
-            self._DS_rmnd
-            + self._MS_rmnd
-            + self._Shred
-            + self._Sterilized
-            + self._Dewatered)
-
-        if self.InputData.AnF_operation['isDried']['amount']:
-            self._Mass_toConveyor += (
-                self._Pellet
-                + self._Dried)
+            self._DS_rmnd + self._MS_rmnd + self._Shred + self._Sterilized + self._Dewatered
+        )
+
+        if self.InputData.AnF_operation["isDried"]["amount"]:
+            self._Mass_toConveyor += self._Pellet + self._Dried
         Conveyor(self._Mass_toConveyor, self.InputData, self.LCI)
 
         # Solid content of Feed
-        if self.InputData.AnF_operation['isDried']['amount']:
-            self._Feed_sol = (
-                self._Dried
-                * (1 - self.InputData.AnF_operation['Dried_moist']['amount']))
+        if self.InputData.AnF_operation["isDried"]["amount"]:
+            self._Feed_sol = self._Dried * (
+                1 - self.InputData.AnF_operation["Dried_moist"]["amount"]
+            )
         else:
-            self._Feed_sol = (
-                self._Dewatered
-                * (1 - self.InputData.AnF_operation['Dew_moist']['amount']))
+            self._Feed_sol = self._Dewatered * (
+                1 - self.InputData.AnF_operation["Dew_moist"]["amount"]
+            )
 
         # Calculating avoided feed production
 
-        # Mositure content of avoided maize grain is 14%
+        # Moisture content of avoided maize grain is 14%
         # Source: maize grain, feed production, RoW - Ecoinvent
-        self._avoid_feed = (self._Feed_sol / 0.86
-                            * self.InputData.AnF_operation['FeedSubFac']['amount'])
+        self._avoid_feed = (
+            self._Feed_sol / 0.86 * self.InputData.AnF_operation["FeedSubFac"]["amount"]
+        )
 
-        self.LCI.add(('Technosphere', 'Feed_Production'), -self._avoid_feed * 1000)  # Mg to kg
+        self.LCI.add(("Technosphere", "Feed_Production"), -self._avoid_feed * 1000)  # Mg to kg
 
         # Wastewater treatment
         total_BOD = (
             self._waste_water
             * 1000  # 1000L/Mg
-            * self.InputData.Wastewater['BOD_conc']['amount']
-            / 1000) # kg/1000gr
+            * self.InputData.Wastewater["BOD_conc"]["amount"]
+            / 1000
+        )  # kg/1000gr
 
-        BOD_removed = (
-            total_BOD
-            * self.CommonData.WWT['bod_rem']['amount'] / 100)
-
-        self._BOD_elec = (
-            BOD_removed
-            * self.InputData.Wastewater['BOD_elec']['amount'])
-
-        self._BOD_CO2 = (
-            BOD_removed
-            * self.InputData.Wastewater['BOD_CO2']['amount'])
+        BOD_removed = total_BOD * self.CommonData.WWT["bod_rem"]["amount"] / 100
 
-        self.LCI.add(('Technosphere', 'Electricity_consumption'), self._BOD_elec)
-        self.LCI.add('Bio-CO2 emissions from wastewater treatment', self._BOD_CO2)
+        self._BOD_elec = BOD_removed * self.InputData.Wastewater["BOD_elec"]["amount"]
+
+        self._BOD_CO2 = BOD_removed * self.InputData.Wastewater["BOD_CO2"]["amount"]
+
+        self.LCI.add(("Technosphere", "Electricity_consumption"), self._BOD_elec)
+        self.LCI.add("Bio-CO2 emissions from wastewater treatment", self._BOD_CO2)
 
         # General Electricity
         Electricity(self._Input, self.InputData, self.LCI)
 
         # Capital Cost
-        Land_req = self.InputData.Electricity['Area_rate']['amount'] * self.InputData.Constr_cost['Land_req_factor']['amount']
-        Land_cost = Land_req * self.InputData.Constr_cost['Land_rate']['amount'] / 4046.86  # 1acr = 4046.86 m2
-        Constr_cost =  Land_req * (self.InputData.Constr_cost['Paving_rate']['amount'] +
-                                   self.InputData.Constr_cost['Grading_rate']['amount']) / 10000  # 1ha = 10000m2
-        Constr_cost += (self.InputData.Electricity['Area_rate']['amount'] * self.InputData.Constr_cost['Constr_rate']['amount'] / 0.0929)  # 1ft2 = 0.0929 m2
-        Constr_cost *= (1 + self.InputData.Constr_cost['Eng_rate']['amount'])
-
-        Miscellaneous_Costs = (self.InputData.Constr_cost['Landscaping_rate']['amount'] / 10000 * Land_req) # 1 ha = 10000m2
+        Land_req = (
+            self.InputData.Electricity["Area_rate"]["amount"]
+            * self.InputData.Constr_cost["Land_req_factor"]["amount"]
+        )
+        Land_cost = (
+            Land_req * self.InputData.Constr_cost["Land_rate"]["amount"] / 4046.86
+        )  # 1acr = 4046.86 m2
+        Constr_cost = (
+            Land_req
+            * (
+                self.InputData.Constr_cost["Paving_rate"]["amount"]
+                + self.InputData.Constr_cost["Grading_rate"]["amount"]
+            )
+            / 10000
+        )  # 1ha = 10000m2
+        Constr_cost += (
+            self.InputData.Electricity["Area_rate"]["amount"]
+            * self.InputData.Constr_cost["Constr_rate"]["amount"]
+            / 0.0929
+        )  # 1ft2 = 0.0929 m2
+        Constr_cost *= 1 + self.InputData.Constr_cost["Eng_rate"]["amount"]
+
+        Miscellaneous_Costs = (
+            self.InputData.Constr_cost["Landscaping_rate"]["amount"] / 10000 * Land_req
+        )  # 1 ha = 10000m2
 
         # Assumes fenc along three sides of square
-        Miscellaneous_Costs += np.sqrt(Land_req * 156) * 3 * self.InputData.Constr_cost['Fencing_Rate']['amount'] / 156
+        Miscellaneous_Costs += (
+            np.sqrt(Land_req * 156) * 3 * self.InputData.Constr_cost["Fencing_Rate"]["amount"] / 156
+        )
 
         # Total capital cost
-        Unit_capital_cost = Land_cost + Constr_cost +  Miscellaneous_Costs  # $/tpd
-        Unit_capital_cost /= self.InputData.Labor['Day_year']['amount']  # $/t.yr
-        capital_cost = -npf.pmt(rate=self.InputData.Constr_cost['Inerest_rate']['amount'],
-                        nper=self.InputData.Constr_cost['lifetime']['amount'],
-                        pv=Unit_capital_cost)
-        self.LCI.add(('biosphere3', 'Capital_Cost'), capital_cost * self._Input)
+        Unit_capital_cost = Land_cost + Constr_cost + Miscellaneous_Costs  # $/tpd
+        Unit_capital_cost /= self.InputData.Labor["Day_year"]["amount"]  # $/t.yr
+        capital_cost = -npf.pmt(
+            rate=self.InputData.Constr_cost["Interest_rate"]["amount"],
+            nper=self.InputData.Constr_cost["lifetime"]["amount"],
+            pv=Unit_capital_cost,
+        )
+        self.LCI.add(("biosphere3", "Capital_Cost"), capital_cost * self._Input)
 
     def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
 
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
         self.calc()
-        return(input_list)
+        return input_list
 
     def report(self):
         report = {}
         report["process name"] = (self.process_name, self.Process_Type, self.__class__)
         report["Waste"] = {}
         report["Technosphere"] = {}
         report["Biosphere"] = {}
@@ -178,24 +195,41 @@
         for x in ["Waste", "Technosphere", "Biosphere"]:
             for y in self.Index:
                 report[x][y] = {}
 
         lci_report = self.LCI.report(input_mass=self._Input)
 
         for y in self.Index:
-            # Output Technospphere Database
-            report["Technosphere"][y][('Technosphere', 'Electricity_consumption')] = lci_report[('Technosphere', 'Electricity_consumption')][y]
-            report["Technosphere"][y][('Technosphere', 'Equipment_Diesel')] = lci_report[('Technosphere', 'Equipment_Diesel')][y]
-            report["Technosphere"][y][('Technosphere', 'Equipment_LPG')] = lci_report[('Technosphere', 'Equipment_LPG')][y]
-            report["Technosphere"][y][('Technosphere', 'Feed_Production')] = lci_report[('Technosphere', 'Feed_Production')][y]
+            # Output Technosphere Database
+            report["Technosphere"][y][("Technosphere", "Electricity_consumption")] = lci_report[
+                ("Technosphere", "Electricity_consumption")
+            ][y]
+            report["Technosphere"][y][("Technosphere", "Equipment_Diesel")] = lci_report[
+                ("Technosphere", "Equipment_Diesel")
+            ][y]
+            report["Technosphere"][y][("Technosphere", "Equipment_LPG")] = lci_report[
+                ("Technosphere", "Equipment_LPG")
+            ][y]
+            report["Technosphere"][y][("Technosphere", "Feed_Production")] = lci_report[
+                ("Technosphere", "Feed_Production")
+            ][y]
 
             # Cost
-            report["Biosphere"][y][('biosphere3','Operational_Cost')] = lci_report[('biosphere3','Operational_Cost')][y]
-            report["Biosphere"][y][('biosphere3', 'Capital_Cost')] = lci_report[('biosphere3', 'Capital_Cost')][y]
+            report["Biosphere"][y][("biosphere3", "Operational_Cost")] = lci_report[
+                ("biosphere3", "Operational_Cost")
+            ][y]
+            report["Biosphere"][y][("biosphere3", "Capital_Cost")] = lci_report[
+                ("biosphere3", "Capital_Cost")
+            ][y]
 
             # Emissions
-            report["Biosphere"][y][('biosphere3', 'eba59fd6-f37e-41dc-9ca3-c7ea22d602c7')] = (  # Carbon dioxide, non-fossil ('air',)
-                lci_report['Bio-CO2 emissions from wastewater treatment'][y])
+            report["Biosphere"][y][
+                ("biosphere3", "eba59fd6-f37e-41dc-9ca3-c7ea22d602c7")
+            ] = lci_report[  # Carbon dioxide, non-fossil ('air',)
+                "Bio-CO2 emissions from wastewater treatment"
+            ][
+                y
+            ]
 
             # Waste products
-            report["Waste"][y]['Other_Residual'] = lci_report['Other_Residual'][y]
-        return report
+            report["Waste"][y]["Other_Residual"] = lci_report["Other_Residual"][y]
+        return report
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/COM_Col.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/MF_Col.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,886 +1,1014 @@
 # -*- coding: utf-8 -*-
-"""
-@author: msardar2
-"""
+import warnings
+
+import numpy as np
+import numpy_financial as npf
 import pandas as pd
-from swolfpy_inputdata import COM_Col_Input
+from swolfpy_inputdata import MF_Col_Input
+
 from .ProcessModel import ProcessModel
-import numpy_financial as npf
-import numpy as np
-import warnings
 
 
-class COM_Col(ProcessModel):
-    Process_Type = 'Collection'
-    def __init__(self, process_name, Collection_scheme,
-                 Treatment_processes=None,
-                 Distance=None,
-                 CommonDataObjct=None,
-                 input_data_path=None):
+class MF_Col(ProcessModel):
+    Process_Type = "Collection"
+
+    def __init__(
+        self,
+        process_name,
+        Collection_scheme,
+        Treatment_processes=None,
+        Distance=None,
+        CommonDataObjct=None,
+        input_data_path=None,
+    ):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = COM_Col_Input(input_data_path,
-                                       process_name=self.process_name,
-                                       CommonDataObjct=CommonDataObjct)
+        self.InputData = MF_Col_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
         self.process_name = process_name
 
         if Treatment_processes is not None:
             self.Treat_proc = Treatment_processes
             if Distance:
                 self.Distance = Distance
             else:
-                raise Exception('User should define both Distance and Treatment_processes together!')
+                raise ValueError(
+                    "User should define both Distance and Treatment_processes together!"
+                )
         else:
             self.Treat_proc = False
 
         self.process_data = self.InputData.process_data
         self.col_schm = Collection_scheme
 
     @staticmethod
     def scheme():
         """
-        Retrun the dictionary for collection_scheme. all the
-        contributions are zero; user should define them according to his/her case.
+        Return the dictionary for collection_scheme.
+
+        all the contributions are zero; user should define them according to his/her case.
         """
-        SepOrg = ['N/A', 'SSYW', 'SSO', 'SSO_AnF']
-        SepRec = ['N/A', 'SSR', 'DSR', 'MSR', 'MSRDO']
+        SepOrg = ["N/A", "SSYW", "SSO"]
+        SepRec = ["N/A", "SSR", "DSR", "MSR", "MSRDO"]
         scheme = {}
         for i in SepOrg:
             for j in SepRec:
-                scheme[('RWC', i, j)] = 0
+                scheme[("RWC", i, j)] = 0
         for i in SepOrg:
-            scheme[('REC_WetRes', i, 'REC_WetRes')] = 0
+            scheme[("REC_WetRes", i, "REC_WetRes")] = 0
         for j in SepRec:
-            scheme[('ORG_DryRes', 'ORG_DryRes', j)] = 0
+            scheme[("ORG_DryRes", "ORG_DryRes", j)] = 0
         return scheme
 
     def _normalize_scheme(self, DropOff=True, warn=True):
         """
-        Used in optimization. Check that sum of the contributions is 1.
+        Used in optimization.
+
+        Check that sum of the contributions is 1.
         """
         if not DropOff:
             for k in self.col_schm:
-                if 'DO' in k:
+                if "DO" in k:
                     self.col_schm[k] = 0
 
-        contribution =  sum(self.col_schm.values())
+        contribution = sum(self.col_schm.values())
         if abs(contribution - 1) > 0.01:
             if warn:
-                warnings.warn('Error in collection scheme: Sum(Contribution) != 1')
+                warnings.warn("Error in collection scheme: Sum(Contribution) != 1")
             for k, v in self.col_schm.items():
                 self.col_schm[k] = v / contribution
 
     def calc_composition(self):
         # Creating the sel.col Data frame
-        col_data = np.zeros((12, 62), dtype=float)
+        col_data = np.zeros((11, 62), dtype=float)
         col_data[:] = np.nan
         col_columns = []
-        col_index = ['RWC', 'SSR', 'DSR', 'MSR',
-                     'SSYW', 'SSO', 'SSO_AnF', 'ORG', 'DryRes', 'REC',
-                     'WetRes', 'MSRDO']
+        col_index = [
+            "RWC",
+            "SSR",
+            "DSR",
+            "MSR",
+            "SSYW",
+            "SSO",
+            "ORG",
+            "DryRes",
+            "REC",
+            "WetRes",
+            "MSRDO",
+        ]
         col_i = 0
 
         for key, val in self.InputData.den_asmd.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('den_asmd')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("den_asmd")
         col_i += 1
 
         for key, val in self.InputData.HS.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('HS')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("HS")
         col_i += 1
 
         for key, val in self.InputData.Prtcp.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Prtcp')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Prtcp")
         col_i += 1
 
         for key, val in self.InputData.Fr.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Fr')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Fr")
         col_i += 1
 
         for key, val in self.InputData.TL.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('TL')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("TL")
         col_i += 1
 
         for key, val in self.InputData.S.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('S')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("S")
         col_i += 1
 
         for key, val in self.InputData.Nw.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Nw')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Nw")
         col_i += 1
 
         for key, val in self.InputData.Rb.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Rb')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Rb")
         col_i += 1
 
         for key, val in self.InputData.Col_Root.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.LCC.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.DropOff.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.Mpg.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.Speed.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
-        for key in ['CD', 'WV', 'WP', 'wt_lim', 'max_weight', 'F1_', 'F1_idle',
-                    'F2_', 'F2_idle', 'bw', 'bv', 'Lt', 'Ut', 'Vt', 'Fract_CNG',
-                    'grg_area', 'off_area', 'grg_enrg', 'off_enrg', 'Lb']:
-            col_data[:, col_i] = self.InputData.Col[key]['amount']
+        for key in [
+            "CD",
+            "WV",
+            "WP",
+            "wt_lim",
+            "max_weight",
+            "F1_",
+            "F1_idle",
+            "F2_",
+            "F2_idle",
+            "bw",
+            "bv",
+            "Lt",
+            "Ut",
+            "Vt",
+            "Fract_CNG",
+            "grg_area",
+            "off_area",
+            "grg_enrg",
+            "off_enrg",
+            "Lb",
+        ]:
+            col_data[:, col_i] = self.InputData.Col[key]["amount"]
             col_columns.append(key)
             col_i += 1
 
-        self.col = pd.DataFrame(data=col_data,
-                                columns=col_columns,
-                                index=['RWC', 'SSR', 'DSR', 'MSR',
-                                       'SSYW', 'SSO', 'SSO_AnF', 'ORG', 'DryRes', 'REC',
-                                        'WetRes', 'MSRDO'],
-                                dtype=float)
+        self.col = pd.DataFrame(
+            data=col_data,
+            columns=col_columns,
+            index=[
+                "RWC",
+                "SSR",
+                "DSR",
+                "MSR",
+                "SSYW",
+                "SSO",
+                "ORG",
+                "DryRes",
+                "REC",
+                "WetRes",
+                "MSRDO",
+            ],
+            dtype=float,
+        )
 
-        self.col['Fract_Dies'] = 1 - self.InputData.Col['Fract_CNG']['amount']
+        self.col["Fract_Dies"] = 1 - self.InputData.Col["Fract_CNG"]["amount"]
 
         self._col_schm = {
-            'RWC': {'Contribution': 0,
-                    'separate_col':{'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSO_AnF': 0}},
-            'ORG_DryRes': {'Contribution': 0,
-                           'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSO_AnF': 0}},
-            'REC_WetRes': {'Contribution': 0,
-                           'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSO_AnF': 0}}}
+            "RWC": {
+                "Contribution": 0,
+                "separate_col": {"SSR": 0, "DSR": 0, "MSR": 0, "MSRDO": 0, "SSYW": 0, "SSO": 0},
+            },
+            "ORG_DryRes": {
+                "Contribution": 0,
+                "separate_col": {"SSR": 0, "DSR": 0, "MSR": 0, "MSRDO": 0, "SSYW": 0, "SSO": 0},
+            },
+            "REC_WetRes": {
+                "Contribution": 0,
+                "separate_col": {"SSR": 0, "DSR": 0, "MSR": 0, "MSRDO": 0, "SSYW": 0, "SSO": 0},
+            },
+        }
 
         for k, v in self.col_schm.items():
-            if k[0] == 'RWC':
-                self._col_schm['RWC']['Contribution'] += v
-            elif k[0] == 'ORG_DryRes':
-                self._col_schm['ORG_DryRes']['Contribution'] += v
-            elif k[0] == 'REC_WetRes':
-                self._col_schm['REC_WetRes']['Contribution'] += v
+            if k[0] == "RWC":
+                self._col_schm["RWC"]["Contribution"] += v
+            elif k[0] == "ORG_DryRes":
+                self._col_schm["ORG_DryRes"]["Contribution"] += v
+            elif k[0] == "REC_WetRes":
+                self._col_schm["REC_WetRes"]["Contribution"] += v
             else:
-                raise Exception(f'Error in collection scheme keys: "{k[0]}" is not defined!')
+                raise ValueError(f'Error in collection scheme keys: "{k[0]}" is not defined!')
 
         for k, v in self.col_schm.items():
             if v > 0:
-                if k[1] not in ['N/A', 'ORG_DryRes', 'REC_WetRes']:
-                    self._col_schm[k[0]]['separate_col'][k[1]] += v / self._col_schm[k[0]]['Contribution']
-                if k[2] not in ['N/A', 'ORG_DryRes', 'REC_WetRes']:
-                    self._col_schm[k[0]]['separate_col'][k[2]] += v / self._col_schm[k[0]]['Contribution']
-
-        # Commercial Waste Generation Rate (kg/location-week)
-        g_res = self.InputData.Col['comm_gen']['amount']
-        gen_per_week = g_res * self.process_data['Comp']
+                if k[1] not in ["N/A", "ORG_DryRes", "REC_WetRes"]:
+                    self._col_schm[k[0]]["separate_col"][k[1]] += (
+                        v / self._col_schm[k[0]]["Contribution"]
+                    )
+                if k[2] not in ["N/A", "ORG_DryRes", "REC_WetRes"]:
+                    self._col_schm[k[0]]["separate_col"][k[2]] += (
+                        v / self._col_schm[k[0]]["Contribution"]
+                    )
+
+        # Single Family Residential Waste Generation Rate (kg/household-week)
+        g_res = (
+            7
+            * self.InputData.Col["res_per_dwel"]["amount"]
+            * self.InputData.Col["res_gen"]["amount"]
+        )
+        gen_per_week = g_res * self.process_data["Comp"]
         total_waste_gen = (
-            g_res
-            * self.InputData.Col['comm_loc']['amount']
-            * 365 / 7 / 1000)  # 52 weeks per year & 1000 kg = 1 Mg
+            g_res * self.InputData.Col["houses_res"]["amount"] * 365 / 7 / 1000
+        )  # 52 weeks per year & 1000 kg = 1 Mg
 
         # Total fraction where this service is offered
         self.col_proc = {
-            'RWC': self._col_schm['RWC']['Contribution'],
-            'ORG': self._col_schm['ORG_DryRes']['Contribution'],
-            'DryRes': self._col_schm['ORG_DryRes']['Contribution'],
-            'REC': self._col_schm['REC_WetRes']['Contribution'],
-            'WetRes': self._col_schm['REC_WetRes']['Contribution']}
+            "RWC": self._col_schm["RWC"]["Contribution"],
+            "ORG": self._col_schm["ORG_DryRes"]["Contribution"],
+            "DryRes": self._col_schm["ORG_DryRes"]["Contribution"],
+            "REC": self._col_schm["REC_WetRes"]["Contribution"],
+            "WetRes": self._col_schm["REC_WetRes"]["Contribution"],
+        }
 
-        for i in ['SSR', 'DSR', 'MSR', 'MSRDO', 'SSYW', 'SSO', 'SSO_AnF']:
+        for i in ["SSR", "DSR", "MSR", "MSRDO", "SSYW", "SSO"]:
             self.col_proc[i] = 0
-            for j in ['RWC', 'ORG_DryRes', 'REC_WetRes']:
+            for j in ["RWC", "ORG_DryRes", "REC_WetRes"]:
                 self.col_proc[i] += (
-                    self._col_schm[j]['Contribution']
-                    * self._col_schm[j]['separate_col'][i])
+                    self._col_schm[j]["Contribution"] * self._col_schm[j]["separate_col"][i]
+                )
 
         # Is this collection process offered? (1: in use, 0: not used)
         self.P_use = {}
         for j in self.col_proc.keys():
             self.P_use[j] = 1 if self.col_proc[j] > 0 else 0
 
         # Mass separated by collection process (kg/week.Household)
-        columns = ['RWC', 'SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'SSO_AnF',
-                   'ORG', 'DryRes', 'REC', 'WetRes',
-                   'MSRDO']
-        self.mass = pd.DataFrame(index=self.Index,
-                                 columns=columns,
-                                 data=0.0,
-                                 dtype=float)
-
-        for i in ['SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'SSO_AnF', 'ORG', 'REC', 'MSRDO']:
-            self.mass[i] = (
-                gen_per_week.values
-                * self.process_data[i].values
-                * self.P_use[i])
-
+        columns = [
+            "RWC",
+            "SSR",
+            "DSR",
+            "MSR",
+            "SSYW",
+            "SSO",
+            "ORG",
+            "DryRes",
+            "REC",
+            "WetRes",
+            "MSRDO",
+        ]
+        self.mass = pd.DataFrame(index=self.Index, columns=columns, data=0.0, dtype=float)
 
+        for i in ["SSR", "DSR", "MSR", "SSYW", "SSO", "ORG", "REC", "MSRDO"]:
+            self.mass[i] = gen_per_week.values * self.process_data[i].values * self.P_use[i]
 
         def separate_col_mass(j):
             mass = np.zeros(len(self.CommonData.Index))
-            for i in ['SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'SSO_AnF', 'MSRDO']:
-                mass += self.mass[i].values * self._col_schm[j]['separate_col'][i]
+            for i in ["SSR", "DSR", "MSR", "SSYW", "SSO", "MSRDO"]:
+                mass += self.mass[i].values * self._col_schm[j]["separate_col"][i]
             return mass
 
         # Calculating the residual waste after separate collection
-        self.mass['RWC']= (
-            gen_per_week.values
-            * self.process_data['RWC'].values
-            - separate_col_mass('RWC')) * self.P_use['RWC']
+        self.mass["RWC"] = (
+            gen_per_week.values * self.process_data["RWC"].values - separate_col_mass("RWC")
+        ) * self.P_use["RWC"]
 
         # ORG_DryRes
-        self.mass['DryRes']= (
-            (gen_per_week.values
-             * self.process_data['DryRes'].values
-             - separate_col_mass('ORG_DryRes')
-             - self.mass['ORG'].values) * self.P_use['DryRes'])
+        self.mass["DryRes"] = (
+            gen_per_week.values * self.process_data["DryRes"].values
+            - separate_col_mass("ORG_DryRes")
+            - self.mass["ORG"].values
+        ) * self.P_use["DryRes"]
 
         # REC_WetRes
-        self.mass['WetRes'] = (
-            gen_per_week.values
-            * self.process_data['WetRes'].values
-            - separate_col_mass('REC_WetRes')
-            - self.mass['REC'].values) * self.P_use['WetRes']
+        self.mass["WetRes"] = (
+            gen_per_week.values * self.process_data["WetRes"].values
+            - separate_col_mass("REC_WetRes")
+            - self.mass["REC"].values
+        ) * self.P_use["WetRes"]
 
         # Annual Mass Flows (Mg/yr)
         self.col_massflow = pd.DataFrame(index=self.Index)
         for i in columns:
-            self.col_massflow[i] = (self.mass[i]
-                                    * self.InputData.Col['comm_loc']['amount']
-                                    * 365 / 7 / 1000
-                                    * self.col_proc[i])
+            self.col_massflow[i] = (
+                self.mass[i]
+                * self.InputData.Col["houses_res"]["amount"]
+                * 365
+                / 7
+                / 1000
+                * self.col_proc[i]
+            )
 
         # Check for negative mass flows
         if (self.col_massflow.values < 0).any().any():
-            raise Exception(f'Negative mass flows in collection model [{self.process_name}]!')
-            # warnings.warn('Negative mass flows in collection model [{self.process_name}]!')
+            raise ValueError(f"Negative mass flows in collection model [{self.process_name}]!")
 
         # Check generated mass = Collected mass
         ratio = self.col_massflow.sum().sum() / total_waste_gen
         if ratio > 1.01 or ratio < 0.99:
-            raise Exception(f'Mass balance error in collection model [{self.process_name}]!')
-            # warnings.warn(f'Mass balance error in collection model [{self.process_name}]!')
+            raise ValueError(f"Mass balance error in collection model [{self.process_name}]!")
 
         # Volume Composition of each collection process for each sector
-        mass_to_cyd = (1 / (self.process_data['Bulk_Density'].values + 0.000001)
-                       * 1.30795)  # m3 --> Cubic yard
-        mass_to_cyd[self.process_data['Bulk_Density'].values <= 0] = 0.0
+        mass_to_cyd = (
+            1 / (self.process_data["Bulk_Density"].values + 0.000001) * 1.30795
+        )  # m3 --> Cubic yard
+        mass_to_cyd[self.process_data["Bulk_Density"].values <= 0] = 0.0
 
-        for i in ['RWC', 'SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'SSO_AnF', 'MSRDO']:
+        for i in ["RWC", "SSR", "DSR", "MSR", "SSYW", "SSO", "MSRDO"]:
             vol = (self.mass[i].values * mass_to_cyd).sum()  # Unit kg/cyd
             if vol > 0:
-                self.col.loc[i, 'den_c'] = (self.mass[i].values
-                                            * 2.205 / vol).sum()  # Unit lb/cyd
+                self.col.loc[i, "den_c"] = (self.mass[i].values * 2.205 / vol).sum()  # Unit lb/cyd
             else:
-                self.col.loc[i, 'den_c'] = 0
+                self.col.loc[i, "den_c"] = 0
 
-        for i, j in [('ORG', 'DryRes'), ('REC', 'WetRes')]:
+        for i, j in [("ORG", "DryRes"), ("REC", "WetRes")]:
             m = self.mass[i].values + self.mass[j].values
             vol = (m * mass_to_cyd).sum()  # Unit kg/cyd
             if vol > 0:
-                self.col.loc[i, 'den_c'] = (m * 2.205 / vol).sum()  # Unit lb/cyd
+                self.col.loc[i, "den_c"] = (m * 2.205 / vol).sum()  # Unit lb/cyd
             else:
-                self.col.loc[i, 'den_c'] = 0
+                self.col.loc[i, "den_c"] = 0
 
     def find_destination(self, product, Treatment_processes):
         destination = {}
         for P in Treatment_processes:
-            if product in Treatment_processes[P]['input_type']:
+            if product in Treatment_processes[P]["input_type"]:
                 destination[P] = (
-                    self.Distance.Distance[(self.process_name, P)]['Heavy Duty Truck']
-                    / 1.60934)  # Convert the distance from km to mile
+                    self.Distance.Distance[(self.process_name, P)]["Heavy Duty Truck"] / 1.60934
+                )  # Convert the distance from km to mile
         return destination
 
     # calculating LCI and cost for different locations
     def calc_destin(self):
         if self.Treat_proc:
             self.dest = {}
             self.result_destination = {}
 
-            Collection_Index = ['RWC', 'SSR', 'DSR', 'MSR', 'SSYW',
-                                'SSO', 'SSO_AnF', 'ORG', 'DryRes', 'REC', 'WetRes',
-                                'MSRDO']
+            Collection_Index = [
+                "RWC",
+                "SSR",
+                "DSR",
+                "MSR",
+                "SSYW",
+                "SSO",
+                "ORG",
+                "DryRes",
+                "REC",
+                "WetRes",
+                "MSRDO",
+            ]
             for i in Collection_Index:
                 self.dest[i] = self.find_destination(i, self.Treat_proc)
                 self.result_destination[i] = {}
 
             # Number of times we need to run the collection
             n_run = max([len(self.dest[i]) for i in self.dest.keys()])
 
             for i in range(n_run):
-                for j in ['RWC', 'SSR', 'DSR', 'MSR', 'MSRDO', 'SSYW',
-                          'SSO', 'SSO_AnF', 'MSRDO', 'ORG', 'REC']:
+                for j in [
+                    "RWC",
+                    "SSR",
+                    "DSR",
+                    "MSR",
+                    "MSRDO",
+                    "SSYW",
+                    "SSO",
+                    "MSRDO",
+                    "ORG",
+                    "REC",
+                ]:
                     if len(self.dest[j]) > i:
                         # Distance btwn collection route and destination
-                        self.col['Drf'][j] = self.dest[j][list(self.dest[j].keys())[i]]
+                        self.col["Drf"][j] = self.dest[j][list(self.dest[j].keys())[i]]
 
                         # Distance between destination and garage
-                        self.col['Dfg'][j] = (
-                            self.dest[j][list(self.dest[j].keys())[i]]
-                            + self.col['Dgr'][j])
+                        self.col["Dfg"][j] = (
+                            self.dest[j][list(self.dest[j].keys())[i]] + self.col["Dgr"][j]
+                        )
 
                 self.calc_lci()
                 for j in self.dest.keys():
                     if len(self.dest[j]) > i:
                         key = list(self.dest[j].keys())[i]
                         self.result_destination[j][key] = {}
 
-                        self.result_destination[j][key][('Technosphere', 'Equipment_Diesel')] = (
-                            self.output['FuelMg'][j]
-                            + self.output['FuelMg_dov'][j])
-
-                        self.result_destination[j][key][('Technosphere', 'Equipment_CNG')] = (
-                            self.output['FuelMg_CNG'][j])
-
-                        self.result_destination[j][key][('Technosphere', 'Electricity_consumption')] = (
-                            self.output['ElecMg'][j])
-
-                        self.result_destination[j][key][('biosphere3', 'Operational_Cost')] = (
-                            self.output['C_collection'][j])
+                        self.result_destination[j][key][("Technosphere", "Equipment_Diesel")] = (
+                            self.output["FuelMg"][j] + self.output["FuelMg_dov"][j]
+                        )
+
+                        self.result_destination[j][key][
+                            ("Technosphere", "Equipment_CNG")
+                        ] = self.output["FuelMg_CNG"][j]
+
+                        self.result_destination[j][key][
+                            ("Technosphere", "Electricity_consumption")
+                        ] = self.output["ElecMg"][j]
+
+                        self.result_destination[j][key][
+                            ("biosphere3", "Operational_Cost")
+                        ] = self.output["C_collection"][j]
         else:
             self.calc_lci()
             self.result_destination = {}
 
     def calc_lci(self):
         # Selected compartment compaction density  (lb/yd3)
         # Override calculated density den_c and use an average assumed in-truck density
-        d_msw = self.col['den_asmd'].values
-        d_msw[d_msw <= 0] = self.col['den_c'].values[d_msw <= 0]
-        self.col['d_msw'] = d_msw
+        d_msw = self.col["den_asmd"].values
+        d_msw[d_msw <= 0] = self.col["den_c"].values[d_msw <= 0]
+        self.col["d_msw"] = d_msw
 
         # Travel time between service stops, adjusted based on participation (min/stop)
-        self.col['Tbtw'] = self.col['Dbtw'].values / self.col['Vbet'].values * 60
+        self.col["Tbtw"] = self.col["Dbtw"].values / self.col["Vbet"].values * 60
 
         # Travel time btwn route and disposal fac. (min/trip)
-        self.col['Trf'] = self.col['Drf'].values / self.col['Vrf'].values * 60
+        self.col["Trf"] = self.col["Drf"].values / self.col["Vrf"].values * 60
 
         # Time from grg to 1st collection route (min/day-vehicle)
-        self.col['Tgr'] = self.col['Dgr'].values / self.col['Vgr'].values * 60
+        self.col["Tgr"] = self.col["Dgr"].values / self.col["Vgr"].values * 60
 
         # Time from disposal fac. to garage (min/day-vehicle)
-        self.col['Tfg'] = self.col['Dfg'].values / self.col['Vfg'].values * 60
+        self.col["Tfg"] = self.col["Dfg"].values / self.col["Vfg"].values * 60
 
-        for i in ['RWC', 'SSR', 'DSR', 'MSR',
-                  'SSYW', 'SSO', 'SSO_AnF', 'MSRDO']:
-            self.col.loc[i, 'mass'] = self.mass[i].values.sum()
+        for i in ["RWC", "SSR", "DSR", "MSR", "SSYW", "SSO", "MSRDO"]:
+            self.col.loc[i, "mass"] = self.mass[i].values.sum()
 
         # Mass of ORG_DryRes and REC_WetRec
-        for i, j in [('ORG', 'DryRes'), ('REC', 'WetRes')]:
-            self.col.loc[i, 'mass'] = (self.mass[i].values + self.mass[j].values).sum()
-
-
+        for i, j in [("ORG", "DryRes"), ("REC", "WetRes")]:
+            self.col.loc[i, "mass"] = (self.mass[i].values + self.mass[j].values).sum()
 
         # Calculations for collection vehicle activities
         # Houses per trip (Volume limited) and (mass limited)
         Ht_v = np.zeros(self.col.shape[0])
         Ht_m = np.zeros(self.col.shape[0])
 
-        fltr = self.col['mass'].values > 0
+        fltr = self.col["mass"].values > 0
         Ht_v[fltr] = (
-            self.col['Ut'].values[fltr]
-            * self.col['Vt'].values[fltr]
-            * self.col['d_msw'].values[fltr]
+            self.col["Ut"].values[fltr]
+            * self.col["Vt"].values[fltr]
+            * self.col["d_msw"].values[fltr]
             * 0.4536  # lb to kg
-            * self.col['Fr'].values[fltr]
-            / self.col['mass'].values[fltr])
+            * self.col["Fr"].values[fltr]
+            / self.col["mass"].values[fltr]
+        )
 
         Ht_m[fltr] = (
-            self.col['max_weight'].values[fltr]
-            * self.col['Fr'].values[fltr]
+            self.col["max_weight"].values[fltr]
+            * self.col["Fr"].values[fltr]
             * 1000
-            / self.col['mass'].values[fltr])
+            / self.col["mass"].values[fltr]
+        )
 
-        self.col['Ht_v'] = Ht_v
-        self.col['Ht_m'] = Ht_m
+        self.col["Ht_v"] = Ht_v
+        self.col["Ht_m"] = Ht_m
 
         # Households per trip (limited by mass or volume)
-        Ht = self.col['Ht_v'].values
-        fltr_2 = self.col['wt_lim'].values == 1
-        fltr_3 = Ht[fltr_2] > self.col['Ht_m'].values[fltr_2]
-        Ht[fltr_2][fltr_3] = self.col['Ht_m'].values[fltr_3]
-        self.col['Ht'] = Ht
+        Ht = self.col["Ht_v"].values
+        fltr_2 = self.col["wt_lim"].values == 1
+        fltr_3 = Ht[fltr_2] > self.col["Ht_m"].values[fltr_2]
+        Ht[fltr_2][fltr_3] = self.col["Ht_m"].values[fltr_3]
+        self.col["Ht"] = Ht
 
         # Time per trip (min/trip)
         # Collection
-        self.col['Tc'] = (
-            self.col['Tbtw'].values * (self.col['Ht'].values / self.col['HS'].values - 1)  # collection travel
-            + self.col['TL'].values * self.col['Ht'].values / self.col['HS'].values  # collection loading
-            + 2 * self.col['Trf'].values  # travel
-            + self.col['S'].values)  # unload time
+        self.col["Tc"] = (
+            self.col["Tbtw"].values
+            * (self.col["Ht"].values / self.col["HS"].values - 1)  # collection travel
+            + self.col["TL"].values
+            * self.col["Ht"].values
+            / self.col["HS"].values  # collection loading
+            + 2 * self.col["Trf"].values  # travel
+            + self.col["S"].values
+        )  # unload time
 
         # Trips per day per vehicle (trip/day-vehicle)
-        self.col['RD'] = (
-            self.col['WV'].values * 60
-            - (self.col['F1_'].values + self.col['F2_'].values + self.col['Tfg'].values)
-            - 0.5 * (self.col['Trf'].values + self.col['S'].values)) / self.col['Tc'].values
+        self.col["RD"] = (
+            self.col["WV"].values * 60
+            - (self.col["F1_"].values + self.col["F2_"].values + self.col["Tfg"].values)
+            - 0.5 * (self.col["Trf"].values + self.col["S"].values)
+        ) / self.col["Tc"].values
 
         # Check that the inputs are realistic
-        if any(self.col['RD'].values < 0):
-            raise Exception("Travelling time is too long that the truck cannot make a loop trip in one day!")
+        if any(self.col["RD"].values < 0):
+            raise ValueError(
+                "Traveling time is too long that the truck cannot make a loop trip in one day!"
+            )
 
         # Daily weight of refuse collected per vehicle (Mg/vehicle-day)
-        self.col['RefD'] = (
-            self.col['Ht'].values
-            * self.col['mass'].values / 1000
-            / self.col['Fr'].values
-            * self.col['RD'].values)
+        self.col["RefD"] = (
+            self.col["Ht"].values
+            * self.col["mass"].values
+            / 1000
+            / self.col["Fr"].values
+            * self.col["RD"].values
+        )
 
         # Number of collection stops per day (stops/vehicle-day)
-        self.col['SD'] = (
-            self.col['Ht'].values
-            * self.col['RD'].values
-            / self.col['HS'].values)
+        self.col["SD"] = self.col["Ht"].values * self.col["RD"].values / self.col["HS"].values
 
         # Calculations for collection vehicle activities (Drop off)
-        for i in ['MSRDO']:
+        for i in ["MSRDO"]:
             # volume of recyclables deposited at drop-off site per week (cy/week-house)
-            self.col.loc[i, 'Ht'] = (
+            self.col.loc[i, "Ht"] = (
                 self.mass[i].values.sum()
-                * self.InputData.Col['comm_loc']['amount']
+                * self.InputData.Col["houses_res"]["amount"]
                 * self.col_proc[i]
                 / 0.4536  # lb to kg
-                / self.col['d_msw'][i])
+                / self.col["d_msw"][i]
+            )
 
             # collection vehicle trips per week (trips/week)
-            self.col.loc[i, 'DO_trip_week'] = (
-                self.col['Ht'][i]
-                / (self.col['Vt'][i] * self.col['Ut'][i]))
+            self.col.loc[i, "DO_trip_week"] = self.col["Ht"][i] / (
+                self.col["Vt"][i] * self.col["Ut"][i]
+            )
 
             # time per trip (min/trip) -- load+travel+unload time
-            self.col.loc[i, 'Tc'] = (
-                self.col['TL'][i]
-                + 2 * self.col['Trf'][i]
-                + self.col['S'][i])
+            self.col.loc[i, "Tc"] = self.col["TL"][i] + 2 * self.col["Trf"][i] + self.col["S"][i]
 
             # trips per day per vehicle (trip/day-vehicle)
-            self.col.loc[i, 'RD'] = (
-                self.col['WV'][i] * 60
-                - (self.col['F1_'][i]
-                   + self.col['F2_'][i]
-                   + self.col['Tfg'][i]
-                   + self.col['Tgr'][i])
-                + self.col['Trf'][i]) / self.col['Tc'][i]
+            self.col.loc[i, "RD"] = (
+                self.col["WV"][i] * 60
+                - (
+                    self.col["F1_"][i]
+                    + self.col["F2_"][i]
+                    + self.col["Tfg"][i]
+                    + self.col["Tgr"][i]
+                )
+                + self.col["Trf"][i]
+            ) / self.col["Tc"][i]
 
             # daily weight of refuse collected per vehicle (tons/day-vehicle)
-            self.col.loc[i, 'RefD'] = (
-                self.col['Vt'][i]
-                * self.col['Ut'][i]
-                * self.col['d_msw'][i]
+            self.col.loc[i, "RefD"] = (
+                self.col["Vt"][i]
+                * self.col["Ut"][i]
+                * self.col["d_msw"][i]
                 * 0.4536  # lb to kg
                 / 1000  # kg to Mg
-                * self.col['RD'][i])
+                * self.col["RD"][i]
+            )
 
             # number of collection stops per day (stops/vehicle-day) (1 stop per trip)
-            self.col.loc[i, 'SD'] = self.col['RD'][i]
+            self.col.loc[i, "SD"] = self.col["RD"][i]
 
         # Daily collection vehicle activity times
         # loading time at collection stops (min/day-vehicle) & loading time at drop-off site (min/day-vehicle)
-        self.col['LD'] = self.col['SD'].values * self.col['TL'].values
+        self.col["LD"] = self.col["SD"].values * self.col["TL"].values
 
         # travel time between collection stops (min/day-vehicle)
-        fltr_3 = self.col['SD'].values - 1 >= 1
+        fltr_3 = self.col["SD"].values - 1 >= 1
         Tb = np.zeros(self.col.shape[0])
-        Tb[fltr_3] = (self.col['SD'].values[fltr_3] - 1) * self.col['Tbtw'].values[fltr_3]
-        self.col['Tb'] = Tb
+        Tb[fltr_3] = (self.col["SD"].values[fltr_3] - 1) * self.col["Tbtw"].values[fltr_3]
+        self.col["Tb"] = Tb
 
         # travel time between route and disposal facility (min/day-vehicle)
-        self.col['F_R'] = (2 * self.col['RD'].values + 0.5) * self.col['Trf'].values
+        self.col["F_R"] = (2 * self.col["RD"].values + 0.5) * self.col["Trf"].values
 
         # unloading time at disposal facility (min/day-vehicle)
-        self.col['UD'] = (self.col['RD'].values + 0.5) * self.col['S'].values
+        self.col["UD"] = (self.col["RD"].values + 0.5) * self.col["S"].values
 
-        for i in ['MSRDO']:
-            self.col.loc[i, 'Tb'] = 0
+        for i in ["MSRDO"]:
+            self.col.loc[i, "Tb"] = 0
 
             # travel time between disposal facility and drop-off site (min/day-vehicle)
-            self.col.loc[i, 'F_R'] = (2 * self.col['RD'][i] - 1) * self.col['Trf'][i]
+            self.col.loc[i, "F_R"] = (2 * self.col["RD"][i] - 1) * self.col["Trf"][i]
 
             # unloading time at disposal facility (min/day-vehicle)
-            self.col.loc[i, 'UD'] = self.col['RD'][i] * self.col['S'][i]
-
+            self.col.loc[i, "UD"] = self.col["RD"][i] * self.col["S"][i]
 
         # Daily fuel usage - Diesel
-        fltr_4 = self.col['MPG_all'].values != 0
+        fltr_4 = self.col["MPG_all"].values != 0
 
         # from garage to first collection route (gallons/day-vehicle)
         diesel_gr = (
-            self.col['Fract_Dies'].values
-            * self.col['Dgr'].values
-            *((1 - self.col['fDgr'].values)
-              / self.col['MPG_urban'].values
-              + self.col['fDgr'].values
-              /self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["Dgr"].values
+            * (
+                (1 - self.col["fDgr"].values) / self.col["MPG_urban"].values
+                + self.col["fDgr"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_gr[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dgr'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
-
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dgr"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         # break time, if spent idling
         diesel_idl = (
-            self.col['Fract_Dies'].values
-            * (self.col['F1_'].values
-               * self.col['F1_idle'].values
-               + self.col['F2_'].values
-               * self.col['F2_idle'].values)
+            self.col["Fract_Dies"].values
+            * (
+                self.col["F1_"].values * self.col["F1_idle"].values
+                + self.col["F2_"].values * self.col["F2_idle"].values
+            )
             / 60
-            * self.col['GPH_idle_cv'].values)
+            * self.col["GPH_idle_cv"].values
+        )
 
         diesel_idl[fltr_4] = 0
 
         # from first through last collection stop (gallons/day-vehicle)
         diesel_col = (
-            self.col['Fract_Dies'].values
-            * self.col['Dbtw'].values
-            * self.col['SD'].values
-            / self.col['MPG_collection'].values)
+            self.col["Fract_Dies"].values
+            * self.col["Dbtw"].values
+            * self.col["SD"].values
+            / self.col["MPG_collection"].values
+        )
 
         diesel_col[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dbtw'].values[fltr_4]
-            * self.col['SD'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dbtw"].values[fltr_4]
+            * self.col["SD"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
-
-        index_dict = dict(zip(self.col.index,
-                              np.arange(len(self.col.index))))
+        index_dict = dict(zip(self.col.index, np.arange(len(self.col.index))))
         fltr_DO = [False for i in self.col.index]
-        for i in ['MSRDO']:
+        for i in ["MSRDO"]:
             fltr_DO[index_dict[i]] = True
         diesel_col[fltr_DO] = 0
 
-       # between disposal facility and route (gallons/day-vehicle)
+        # between disposal facility and route (gallons/day-vehicle)
         diesel_rf = (
-            self.col['Fract_Dies'].values
-            * self.col['F_R'].values / 60
-            * self.col['Vrf'].values
-            * ((1 - self.col['fDrd'].values) / self.col['MPG_urban'].values
-               + self.col['fDrd'].values / self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["F_R"].values
+            / 60
+            * self.col["Vrf"].values
+            * (
+                (1 - self.col["fDrd"].values) / self.col["MPG_urban"].values
+                + self.col["fDrd"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_rf[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['F_R'].values[fltr_4] / 60
-            * self.col['Vrf'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["F_R"].values[fltr_4]
+            / 60
+            * self.col["Vrf"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         # unloading at disposal facility (gallons/day-vehicle)
         diesel_ud = (
-            self.col['Fract_Dies'].values
-            * self.col['UD'].values / 60
-            * self.col['GPH_idle_cv'].values)
+            self.col["Fract_Dies"].values
+            * self.col["UD"].values
+            / 60
+            * self.col["GPH_idle_cv"].values
+        )
 
         diesel_ud[fltr_4] = 0
 
-       # from disposal facility to garage (gallons/day-vehicle)
+        # from disposal facility to garage (gallons/day-vehicle)
         diesel_fg = (
-            self.col['Fract_Dies'].values
-            * self.col['Dfg'].values
-            * ((1 - self.col['fDfg'].values) / self.col['MPG_urban'].values
-               + self.col['fDfg'].values / self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["Dfg"].values
+            * (
+                (1 - self.col["fDfg"].values) / self.col["MPG_urban"].values
+                + self.col["fDfg"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_fg[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dfg'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dfg"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
         FuelD = pd.Series(
-            (diesel_gr + diesel_idl + diesel_col
-             + diesel_rf + diesel_ud + diesel_fg),
-             index=self.col.index)
+            (diesel_gr + diesel_idl + diesel_col + diesel_rf + diesel_ud + diesel_fg),
+            index=self.col.index,
+        )
+
         for key, val in self.col_proc.items():
             if val == 0:
                 FuelD[key] = 0
 
-        self.col['FuelD'] = FuelD
+        self.col["FuelD"] = FuelD
 
         # Daily fuel usage - CNG - diesel gal equivalent
-        fltr_6 = self.col['MPG_all_CNG'].values != 0
+        fltr_6 = self.col["MPG_all_CNG"].values != 0
 
         # from garage to first collection route ((diesel gal equivalent/day-vehicle)
         CNG_gr = (
-            self.col['Fract_CNG'].values
-            * self.col['Dgr'].values
-            *((1 - self.col['fDgr'].values)
-              / self.col['MPG_urban_CNG'].values
-              + self.col['fDgr'].values
-              /self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["Dgr"].values
+            * (
+                (1 - self.col["fDgr"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDgr"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_gr[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dgr'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
-
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dgr"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         # break time, if spent idling
         CNG_idl = (
-            self.col['Fract_CNG'].values
-            * (self.col['F1_'].values
-               * self.col['F1_idle'].values
-               + self.col['F2_'].values
-               * self.col['F2_idle'].values)
+            self.col["Fract_CNG"].values
+            * (
+                self.col["F1_"].values * self.col["F1_idle"].values
+                + self.col["F2_"].values * self.col["F2_idle"].values
+            )
             / 60
-            * self.col['GPH_idle_CNG'].values)
+            * self.col["GPH_idle_CNG"].values
+        )
 
         CNG_idl[fltr_6] = 0
 
         # from first through last collection stop (diesel gal equivalent/day-vehicle)
         CNG_col = (
-            self.col['Fract_CNG'].values
-            * self.col['Dbtw'].values
-            * self.col['SD'].values
-            / self.col['MPG_col_CNG'].values)
+            self.col["Fract_CNG"].values
+            * self.col["Dbtw"].values
+            * self.col["SD"].values
+            / self.col["MPG_col_CNG"].values
+        )
 
         CNG_col[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dbtw'].values[fltr_6]
-            * self.col['SD'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dbtw"].values[fltr_6]
+            * self.col["SD"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         CNG_col[fltr_DO] = 0
 
-       # between disposal facility and route (diesel gal equivalent/day-vehicle)
+        # between disposal facility and route (diesel gal equivalent/day-vehicle)
         CNG_rf = (
-            self.col['Fract_CNG'].values
-            * self.col['F_R'].values / 60
-            * self.col['Vrf'].values
-            * ((1 - self.col['fDrd'].values) / self.col['MPG_urban_CNG'].values
-               + self.col['fDrd'].values / self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["F_R"].values
+            / 60
+            * self.col["Vrf"].values
+            * (
+                (1 - self.col["fDrd"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDrd"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_rf[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['F_R'].values[fltr_6] / 60
-            * self.col['Vrf'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["F_R"].values[fltr_6]
+            / 60
+            * self.col["Vrf"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         # unloading at disposal facility (diesel gal equivalent/day-vehicle)
         CNG_ud = (
-            self.col['Fract_CNG'].values
-            * self.col['UD'].values / 60
-            * self.col['GPH_idle_CNG'].values)
+            self.col["Fract_CNG"].values
+            * self.col["UD"].values
+            / 60
+            * self.col["GPH_idle_CNG"].values
+        )
 
         CNG_ud[fltr_6] = 0
 
-       # from disposal facility to garage (diesel gal equivalent/day-vehicle)
+        # from disposal facility to garage (diesel gal equivalent/day-vehicle)
         CNG_fg = (
-            self.col['Fract_CNG'].values
-            * self.col['Dfg'].values
-            * ((1 - self.col['fDfg'].values) / self.col['MPG_urban_CNG'].values
-               + self.col['fDfg'].values / self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["Dfg"].values
+            * (
+                (1 - self.col["fDfg"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDfg"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_fg[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dfg'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dfg"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         FuelD_CNG = pd.Series(
-            (CNG_gr + CNG_idl + CNG_col
-             + CNG_rf + CNG_ud + CNG_fg),
-             index=self.col.index)
+            (CNG_gr + CNG_idl + CNG_col + CNG_rf + CNG_ud + CNG_fg), index=self.col.index
+        )
 
         for key, val in self.col_proc.items():
             if val == 0:
                 FuelD_CNG[key] = 0
 
-        self.col['FuelD_CNG'] = FuelD_CNG
+        self.col["FuelD_CNG"] = FuelD_CNG
 
         # ENERGY CONSUMPTION
         # Energy consumption by collection vehicles
         # total coll. vehicle fuel use per Mg of refuse (L/Mg)
         FuelMg = np.zeros(self.col.shape[0])
-        flter_7 = self.col['RefD'].values > 0
+        flter_7 = self.col["RefD"].values > 0
         FuelMg[flter_7] = (
-            self.col['FuelD'].values[flter_7]
+            self.col["FuelD"].values[flter_7]
             * 3.785  # gal to ltr
-            / self.col['RefD'].values[flter_7])
-        self.col['FuelMg'] = FuelMg
+            / self.col["RefD"].values[flter_7]
+        )
+        self.col["FuelMg"] = FuelMg
 
         # total coll. vehicle CNG fuel use per Mg of refuse (diesel L equivalent/Mg)
         FuelMg_CNG = np.zeros(self.col.shape[0])
         FuelMg_CNG[flter_7] = (
-            self.col['FuelD_CNG'].values[flter_7]
+            self.col["FuelD_CNG"].values[flter_7]
             * 3.785  # gal to ltr
-            / self.col['RefD'].values[flter_7])
-        self.col['FuelMg_CNG'] = FuelMg_CNG
+            / self.col["RefD"].values[flter_7]
+        )
+        self.col["FuelMg_CNG"] = FuelMg_CNG
 
         # Energy consumption by drop-off vehicles
         P_use_Seri = pd.Series(index=self.col.index)
         col_proc_Seri = pd.Series(index=self.col.index)
-        self.col_proc
+
         for key, val in index_dict.items():
             P_use_Seri[val] = self.P_use[key]
             col_proc_Seri[val] = self.col_proc[key]
 
         # fuel usage per trip to drop-off site (gallons/trip)
         FuelT = np.zeros(self.col.shape[0])
         FuelT[fltr_DO] = (
             P_use_Seri.values[fltr_DO]
-            * self.col['RTDdos'].values[fltr_DO]
-            * self.col['DED'].values[fltr_DO]
-            / self.col['dropoff_MPG'].values[fltr_DO] )
-        self.col['FuelT'] = FuelT
+            * self.col["RTDdos"].values[fltr_DO]
+            * self.col["DED"].values[fltr_DO]
+            / self.col["dropoff_MPG"].values[fltr_DO]
+        )
+        self.col["FuelT"] = FuelT
 
-        for i in ['MSRDO']:
+        for i in ["MSRDO"]:
             # weight of refuse delivered per trip (kg/trip)
-            self.col.loc[i, 'RefT'] = (
+            self.col.loc[i, "RefT"] = (
                 self.mass[i].values.sum()
-                * self.col['Prtcp'][i]
-                * 365 / 7
-                / (self.col['FREQdos'][i] * 12))
+                * self.col["Prtcp"][i]
+                * 365
+                / 7
+                / (self.col["FREQdos"][i] * 12)
+            )
 
         # total dropoff vehicle  fuel use per Mg of refuse (L/Mg)
         FuelMg_dov = np.zeros(self.col.shape[0])
-        flter_8 = self.col['RefT'].values > 0
+        flter_8 = self.col["RefT"].values > 0
         FuelMg_dov[flter_8] = (
-            self.col['FuelT'].values[flter_8]
+            self.col["FuelT"].values[flter_8]
             * 3.785  # gal to ltr
-            / (self.col['RefT'].values[flter_8] / 1000))
-        self.col['FuelMg_dov'] = FuelMg_dov
+            / (self.col["RefT"].values[flter_8] / 1000)
+        )
+        self.col["FuelMg_dov"] = FuelMg_dov
 
         # Energy consumption by garage
         # daily electricity usage per vehicle  (kWh/vehicle-day)
-        self.col['ElecD'] = (
-            P_use_Seri.values
-            * (self.col['grg_area'].values * self.col['grg_enrg'].values
-               + self.col['off_area'].values * self.col['off_enrg'].values))
+        self.col["ElecD"] = P_use_Seri.values * (
+            self.col["grg_area"].values * self.col["grg_enrg"].values
+            + self.col["off_area"].values * self.col["off_enrg"].values
+        )
 
         # electricity usage per Mg of refuse  (kWh/Mg)
         ElecMg = np.zeros(self.col.shape[0])
-        ElecMg[flter_7] = (
-            self.col['ElecD'].values[flter_7]
-            / self.col['RefD'].values[flter_7])
-        self.col['ElecMg'] =  ElecMg
+        ElecMg[flter_7] = self.col["ElecD"].values[flter_7] / self.col["RefD"].values[flter_7]
+        self.col["ElecMg"] = ElecMg
 
         # Mass
         # total mass of refuse collected per year (Mg)
-        self.col['TotalMass'] = self.col_massflow.sum()
+        self.col["TotalMass"] = self.col_massflow.sum()
 
         # COLLECTION COSTS
         # Breakdown of capital costs
 
         # annual capital cost per vehicle ($/vehicle-year)
-        self.col['C_cap_v'] = (
-            (1 + self.col['e'].values)
-            * npf.pmt(self.InputData.LCC['Discount_rate']['amount'],
-                      self.col['Lt'].values,
-                      -self.col['Pt'].values))
+        self.col["C_cap_v"] = (1 + self.col["e"].values) * npf.pmt(
+            self.InputData.LCC["Discount_rate"]["amount"],
+            self.col["Lt"].values,
+            -self.col["Pt"].values,
+        )
 
         # number of collection vehicles (vehicles)
-        self.col['Nt'] = (
-            self.InputData.Col['comm_loc']['amount']
+        self.col["Nt"] = (
+            self.InputData.Col["houses_res"]["amount"]
             * col_proc_Seri.values
-            * self.col['Fr'].values
-            / (self.col['Ht'].values
-               * self.col['RD'].values
-               * self.col['CD'].values))
+            * self.col["Fr"].values
+            / (self.col["Ht"].values * self.col["RD"].values * self.col["CD"].values)
+        )
 
         # annualized capital cost per bin ($/bin-year)
-        self.col['Cb'] = (
-            (1 + self.col['e'].values)
-            * npf.pmt(self.InputData.LCC['Discount_rate']['amount'],
-                      self.col['Lb'].values,
-                      -self.col['Pb'].values))
+        self.col["Cb"] = (1 + self.col["e"].values) * npf.pmt(
+            self.InputData.LCC["Discount_rate"]["amount"],
+            self.col["Lb"].values,
+            -self.col["Pb"].values,
+        )
 
         # no. of bins per vehicle (bins/vehicle)
-        self.col['Nb'] = (
-            self.col['Rb'].values
-            * (self.col['Ht'].values / self.col['Prtcp'].values)
-            * self.col['RD'].values
-            * self.col['CD'].values
-            / self.col['Fr'].values)
+        self.col["Nb"] = (
+            self.col["Rb"].values
+            * (self.col["Ht"].values / self.col["HS"].values)
+            * self.col["RD"].values
+            * self.col["CD"].values
+            / self.col["Fr"].values
+        )
 
         # bin annual cost per vehicle ($/vehicle-year)
-        self.col['C_cap_b'] = (
-            self.col['Cb'].values * self.col['Nb'].values)
+        self.col["C_cap_b"] = self.col["Cb"].values * self.col["Nb"].values
 
         # Breakdown of operating costs
         # labor cost per vehicle ($/vehicle-year)
-        self.col['Cw'] = (
-            (1 + self.col['a'].values)
-            * ((1 + self.col['bw'].values)
-               * (self.col['Wa'].values * self.col['Nw'].values
-                  + self.col['Wd'].values)
-               * self.col['WP'].values
-               * self.col['CD'].values
-               * 365 / 7))
+        self.col["Cw"] = (1 + self.col["a"].values) * (
+            (1 + self.col["bw"].values)
+            * (self.col["Wa"].values * self.col["Nw"].values + self.col["Wd"].values)
+            * self.col["WP"].values
+            * self.col["CD"].values
+            * 365
+            / 7
+        )
 
         # O&M cost per vehicle ($/vehicle-year)
-        self.col['Cvo'] = self.col['c'].values
+        self.col["Cvo"] = self.col["c"].values
 
         # other expenses per vehicle ($/vehicle-year)
-        self.col['Coe'] = self.col['d'].values * (self.col['Nw'].values + 1)
+        self.col["Coe"] = self.col["d"].values * (self.col["Nw"].values + 1)
 
         # Annual operating cost ($/vehicle-year)
-        self.col['C_op'] = (
-            (1 + self.col['e'].values)
-            * (self.col['Cw'].values
-               + self.col['Cvo'].values
-               + self.col['Coe'].values))
+        self.col["C_op"] = (1 + self.col["e"].values) * (
+            self.col["Cw"].values + self.col["Cvo"].values + self.col["Coe"].values
+        )
 
         # Total annual cost per vehicle -- cap + O&M ($/vehicle-year)
-        self.col['C_vehicle'] = (
-            (1 + self.col['bv'].values)
-            * self.col['C_cap_v'].values
-            + self.col['C_op'].values)
+        self.col["C_vehicle"] = (1 + self.col["bv"].values) * self.col["C_cap_v"].values + self.col[
+            "C_op"
+        ].values
 
         # Total annual cost per house, including bins ($/house-year)
         # Includes all houses provided service, even if not participating
-        hpdv = (self.col['Ht'].values
-                * self.col['RD'].values
-                * self.col['CD'].values
-                / self.col['Fr'].values)
+        hpdv = (
+            self.col["Ht"].values
+            * self.col["RD"].values
+            * self.col["CD"].values
+            / self.col["Fr"].values
+        )
 
         fltr_9 = hpdv > 0.0
 
         C_house = np.zeros(self.col.shape[0])
 
         C_house[fltr_9] = (
-            self.col['C_vehicle'].values[fltr_9]
-            / hpdv[fltr_9]
-            * self.col['Prtcp'].values[fltr_9])
+            self.col["C_vehicle"].values[fltr_9] / hpdv[fltr_9] * self.col["Prtcp"].values[fltr_9]
+        )
 
-        C_house += (self.col['Cb'].values * self.col['Rb'].values)
+        C_house += self.col["Cb"].values * self.col["Rb"].values
         C_house[np.isnan(C_house)] = 0.0
-        self.col['C_house'] = C_house
+        self.col["C_house"] = C_house
 
         # ☻ ton of refuse collected - Cap+OM+bins ($/Mg)
-        self.col['C_collection'] = (
-            (self.col['C_house'] * 7 / 365)
-            / (self.mass.sum() / 1000)).replace([np.inf, np.nan], 0)
+        self.col["C_collection"] = (
+            (self.col["C_house"] * 7 / 365) / (self.mass.sum() / 1000)
+        ).replace([np.inf, np.nan], 0)
 
         # OUTPUT
-        # Energy use is calculated for ORG and it is same with Dryres
-        self.col.loc['DryRes', 'FuelMg'] = self.col['FuelMg']['ORG']
-        self.col.loc['DryRes', 'FuelMg_CNG'] = self.col['FuelMg_CNG']['ORG']
-        self.col.loc['DryRes', 'ElecMg'] = self.col['ElecMg']['ORG']
+        # Energy use is calculated for ORG and it is same with Dryers
+        self.col.loc["DryRes", "FuelMg"] = self.col["FuelMg"]["ORG"]
+        self.col.loc["DryRes", "FuelMg_CNG"] = self.col["FuelMg_CNG"]["ORG"]
+        self.col.loc["DryRes", "ElecMg"] = self.col["ElecMg"]["ORG"]
 
         # Energy use is calculated for REC and it is same with WetRes
-        self.col.loc['WetRes', 'FuelMg'] = self.col['FuelMg']['REC']
-        self.col.loc['WetRes', 'FuelMg_CNG'] = self.col['FuelMg_CNG']['REC']
-        self.col.loc['WetRes', 'ElecMg'] = self.col['ElecMg']['REC']
-
-
-        self.output = self.col[['TotalMass', 'FuelMg', 'FuelMg_CNG',
-                                'ElecMg', 'FuelMg_dov', 'C_collection']]
+        self.col.loc["WetRes", "FuelMg"] = self.col["FuelMg"]["REC"]
+        self.col.loc["WetRes", "FuelMg_CNG"] = self.col["FuelMg_CNG"]["REC"]
+        self.col.loc["WetRes", "ElecMg"] = self.col["ElecMg"]["REC"]
+
+        self.output = self.col[
+            ["TotalMass", "FuelMg", "FuelMg_CNG", "ElecMg", "FuelMg_dov", "C_collection"]
+        ]
         self.output = self.output.fillna(0.0)
 
     def calc(self):
         self.calc_composition()
         self.calc_destin()
 
     # setup for Monte Carlo simulation
@@ -895,21 +1023,19 @@
 
     def report(self):
         # report
         self.collection = {}
         Waste = {}
         Technosphere = {}
         Biosphere = {}
-        self.collection["process name"] = (self.process_name,
-                                           self.Process_Type,
-                                           self.__class__)
+        self.collection["process name"] = (self.process_name, self.Process_Type, self.__class__)
         self.collection["Waste"] = Waste
         self.collection["Technosphere"] = Technosphere
         self.collection["Biosphere"] = Biosphere
-        self.collection['LCI'] = self.result_destination
+        self.collection["LCI"] = self.result_destination
 
         for x in [Waste, Technosphere, Biosphere]:
             for y in self.Index:
                 x[y] = {}
 
         for y in self.Index:
             for x in self.col_massflow.columns:
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/Common_subprocess.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Common_subprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,273 +1,371 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Jun 10 13:24:59 2021
+from copy import deepcopy
 
-@author: msardar
-"""
 import numpy as np
 import pandas as pd
-from copy import deepcopy
 
 
-class LCI():
+class LCI:
     """
-    This class store the LCI data in ``numpy.ndarray`` instead of ``pandas.DataFrame`` for speedup.
-    Column names (flows names) are stored in ``self.col_dict``.
+    This class store the LCI data in ``numpy.ndarray`` instead of ``pandas.DataFrame`` for
+    speedup. Column names (flows names) are stored in ``self.col_dict``.
 
     Parameters
     ----------
     index : list
         List of waste fractions that are used as row index.
     n_col : int, optional
         The number of columns in the LCI ``ndarray``. The default is 30.
-
     """
 
     def __init__(self, index, n_col=30):
         self.index = index
         self.lci = np.zeros((len(index), n_col))
-        self.col_dict={}
-        self.col_index=0
+        self.col_dict = {}
+        self.col_index = 0
 
     def add(self, name, flow):
         """
         Add new flow to the LCI.
 
         Parameters
         ----------
         name : str
             Name of the flow in the LCI.
         flow : ``numpy.array``.
-
         """
         if isinstance(flow, np.ndarray):
             if any(np.isnan(flow)):
-                raise ValueError(f'The Value for the {name} is nan!')
+                raise ValueError(f"The Value for the {name} is nan!")
         if name not in self.col_dict:
             self.col_dict[name] = self.col_index
             self.col_index += 1
         self.lci[:, self.col_dict[name]] += flow
 
     def report(self, input_mass=None, transpose=False):
         """
         Creates ``DataFrame`` from the LCI ``ndarray`` and return it.
 
         Parameters
         ----------
         input_mass : ``numpy.array``, optional
             Initial mass flows to calculate LCI accordingly. The default is None.
         transpose : boolean, optional
-
         """
         LCI = deepcopy(self.lci)
         if input_mass is not None:
             non_zero_fltr = input_mass > 0
             zero_fltr = input_mass == 0
             for j in range(self.col_index):
                 LCI[non_zero_fltr, j] /= input_mass[non_zero_fltr]
                 LCI[zero_fltr, j] = 0.0
         if transpose:
-            report = pd.DataFrame(LCI[:, :self.col_index].transpose(),
-                                  columns=self.index,
-                                  index=list(self.col_dict.keys()))
+            report = pd.DataFrame(
+                LCI[:, : self.col_index].transpose(),
+                columns=self.index,
+                index=list(self.col_dict.keys()),
+            )
         else:
-            report = pd.DataFrame(LCI[:, :self.col_index],
-                      columns=list(self.col_dict.keys()),
-                      index=self.index)
+            report = pd.DataFrame(
+                LCI[:, : self.col_index], columns=list(self.col_dict.keys()), index=self.index
+            )
         return report
 
 
-class Flow():
+class Flow:
     """
     Creates a ``pandas.DataFrame`` for the flow.
 
     Parameters
     ----------
     material_properties : ``pandas.DataFrame``
-        Materail properties of the waste fractions.
-
+        Material properties of the waste fractions.
     """
 
     def __init__(self, material_properties):
         self.prop = material_properties
-        self.data = pd.DataFrame(index=self.prop.index,
-                                 columns=['mass', 'sol_cont', 'moist_cont', 'vs_cont', 'ash_cont'])
+        self.data = pd.DataFrame(
+            index=self.prop.index, columns=["mass", "sol_cont", "moist_cont", "vs_cont", "ash_cont"]
+        )
 
     # Create new flow
     def init_flow(self, mass_flows):
         """
         Fill the flow ``DataFrame`` based on the mass_flows.
 
         Parameters
         ----------
         mass_flows : ``numpy.array`` or ``pandas.Series``.
-
         """
-        self.data['mass'] = mass_flows
-        self.data['sol_cont'] = self.data['mass'].values * (1 - self.prop['Moisture Content'].values / 100)
-        self.data['moist_cont'] = self.data['mass'].values * (self.prop['Moisture Content'].values / 100)
-        self.data['vs_cont'] = self.data['sol_cont'].values * self.prop['Volatile Solids'].values / 100
-        self.data['ash_cont'] = self.data['sol_cont'].values * self.prop['Ash Content'].values / 100
+        self.data["mass"] = mass_flows
+        self.data["sol_cont"] = self.data["mass"].values * (
+            1 - self.prop["Moisture Content"].values / 100
+        )
+        self.data["moist_cont"] = self.data["mass"].values * (
+            self.prop["Moisture Content"].values / 100
+        )
+        self.data["vs_cont"] = (
+            self.data["sol_cont"].values * self.prop["Volatile Solids"].values / 100
+        )
+        self.data["ash_cont"] = self.data["sol_cont"].values * self.prop["Ash Content"].values / 100
 
     # Update flow
     def update(self, assumed_comp):
         """
         Calculates the flows properties based on the assumed composition.
 
         Parameters
         ----------
         assumed_comp : ``pd.Series``
             Assumed waste composition for the flow.
-
         """
-        self.flow = sum(self.data['mass'].values * assumed_comp.values)
-        self.water = sum(self.data['moist_cont'].values * assumed_comp.values)
+        self.flow = sum(self.data["mass"].values * assumed_comp.values)
+        self.water = sum(self.data["moist_cont"].values * assumed_comp.values)
         self.moist_cont = self.water / self.flow
-        self.ash = sum(self.data['ash_cont'].values * assumed_comp.values)
-        self.solid = sum(self.data['sol_cont'].values * assumed_comp.values)
+        self.ash = sum(self.data["ash_cont"].values * assumed_comp.values)
+        self.solid = sum(self.data["sol_cont"].values * assumed_comp.values)
 
 
-def compost_use(input_flow, common_data, process_data, material_properties,
-                input_data, lci, include_diesel=True):
+def compost_use(
+    input_flow, common_data, process_data, material_properties, input_data, lci, include_diesel=True
+):
     """
-    Calculates the emissions and offsets from final compost use (i.e., land application, ADC)
-
+    Calculates the emissions and offsets from final compost use (i.e., land application,
+    ADC)
     """
     # Compost to land application
-    if input_data.Compost_use['choice_BU']['amount'] == 1:
+    if input_data.Compost_use["choice_BU"]["amount"] == 1:
         # Carbon in final compost
-        C_storage = input_flow.data['C_cont'].values * common_data.Land_app['perCStor']['amount'] / 100
-        C_released = input_flow.data['C_cont'].values - C_storage
-        C_storage_hummus_formation = input_flow.data['C_cont'].values * common_data.Land_app['humFormFac']['amount']
-
-        lci.add(name='Carbon dioxide, non-fossil',
-                flow=C_released * common_data.MW['CO2']['amount'] / common_data.MW['C']['amount'])
-        lci.add(name='Direct Carbon Storage and Humus Formation',
-                flow=-(C_storage + C_storage_hummus_formation) * common_data.MW['CO2']['amount'] / common_data.MW['C']['amount'])
-
-        #Nitrogen in final compost
-        input_flow.data['N_cont'] = input_flow.data['N_cont'].values
-        input_flow.data['P_cont'] = input_flow.data['P_cont'].values
-        input_flow.data['K_cont'] = input_flow.data['K_cont'].values
-
-        N2O = input_flow.data['N_cont'].values * common_data.Land_app['perN2Oevap']['amount'] / 100
-        NH3 = input_flow.data['N_cont'].values * common_data.Land_app['perNasNH3fc']['amount'] / 100 * common_data.Land_app['perNH3evap']['amount'] / 100
-        NO3_GW = input_flow.data['N_cont'].values * common_data.Land_app['NO3leach']['amount']
-        NO3_SW = input_flow.data['N_cont'].values * common_data.Land_app['NO3runoff']['amount']
-
-        lci.add(name='Dinitrogen monoxide',
-                flow=N2O * common_data.MW['Nitrous_Oxide']['amount'] / (common_data.MW['N']['amount'] * 2))
-        lci.add(name='Ammonia',
-                flow=NH3 * common_data.MW['Ammonia']['amount'] / common_data.MW['N']['amount'])
-        lci.add(name='Nitrate (ground water)',
-                flow=NO3_GW * common_data.MW['Nitrate']['amount'] / common_data.MW['N']['amount'])
-        lci.add(name='Nitrate (surface water)',
-                flow=NO3_SW * common_data.MW['Nitrate']['amount'] / common_data.MW['N']['amount'])
-
-        if input_data.Compost_use['fertOff']['amount'] == 1:
-            # Nutrients availble in the final compost
-            Navail = input_flow.data['N_cont'].values * common_data.Land_app['MFEN']['amount']
-            Pavail = input_flow.data['P_cont'].values * common_data.Land_app['MFEP']['amount']
-            Kavail = input_flow.data['K_cont'].values * common_data.Land_app['MFEK']['amount']
+        C_storage = (
+            input_flow.data["C_cont"].values * common_data.Land_app["perCStor"]["amount"] / 100
+        )
+        C_released = input_flow.data["C_cont"].values - C_storage
+        C_storage_hummus_formation = (
+            input_flow.data["C_cont"].values * common_data.Land_app["humFormFac"]["amount"]
+        )
+
+        lci.add(
+            name="Carbon dioxide, non-fossil",
+            flow=C_released * common_data.MW["CO2"]["amount"] / common_data.MW["C"]["amount"],
+        )
+        lci.add(
+            name="Direct Carbon Storage and Humus Formation",
+            flow=-(C_storage + C_storage_hummus_formation)
+            * common_data.MW["CO2"]["amount"]
+            / common_data.MW["C"]["amount"],
+        )
+
+        # Nitrogen in final compost
+        input_flow.data["N_cont"] = input_flow.data["N_cont"].values
+        input_flow.data["P_cont"] = input_flow.data["P_cont"].values
+        input_flow.data["K_cont"] = input_flow.data["K_cont"].values
+
+        N2O = input_flow.data["N_cont"].values * common_data.Land_app["perN2Oevap"]["amount"] / 100
+        NH3 = (
+            input_flow.data["N_cont"].values
+            * common_data.Land_app["perNasNH3fc"]["amount"]
+            / 100
+            * common_data.Land_app["perNH3evap"]["amount"]
+            / 100
+        )
+        NO3_GW = input_flow.data["N_cont"].values * common_data.Land_app["NO3leach"]["amount"]
+        NO3_SW = input_flow.data["N_cont"].values * common_data.Land_app["NO3runoff"]["amount"]
+
+        lci.add(
+            name="Dinitrogen monoxide",
+            flow=N2O
+            * common_data.MW["Nitrous_Oxide"]["amount"]
+            / (common_data.MW["N"]["amount"] * 2),
+        )
+        lci.add(
+            name="Ammonia",
+            flow=NH3 * common_data.MW["Ammonia"]["amount"] / common_data.MW["N"]["amount"],
+        )
+        lci.add(
+            name="Nitrate (ground water)",
+            flow=NO3_GW * common_data.MW["Nitrate"]["amount"] / common_data.MW["N"]["amount"],
+        )
+        lci.add(
+            name="Nitrate (surface water)",
+            flow=NO3_SW * common_data.MW["Nitrate"]["amount"] / common_data.MW["N"]["amount"],
+        )
+
+        if input_data.Compost_use["fertOff"]["amount"] == 1:
+            # Nutrients available in the final compost
+            Navail = input_flow.data["N_cont"].values * common_data.Land_app["MFEN"]["amount"]
+            Pavail = input_flow.data["P_cont"].values * common_data.Land_app["MFEP"]["amount"]
+            Kavail = input_flow.data["K_cont"].values * common_data.Land_app["MFEK"]["amount"]
 
             if include_diesel:
                 # Diesel use for applying the compost
-                Diesel_use = input_flow.data['mass'].values / 1000 * common_data.Land_app['cmpLandDies']['amount']
-                Diesel_offset = -(Navail * common_data.Land_app['DslAppN']['amount']
-                                  + Pavail * common_data.Land_app['DslAppP']['amount']
-                                  + Kavail * common_data.Land_app['DslAppK']['amount'])
+                Diesel_use = (
+                    input_flow.data["mass"].values
+                    / 1000
+                    * common_data.Land_app["cmpLandDies"]["amount"]
+                )
+                Diesel_offset = -(
+                    Navail * common_data.Land_app["DslAppN"]["amount"]
+                    + Pavail * common_data.Land_app["DslAppP"]["amount"]
+                    + Kavail * common_data.Land_app["DslAppK"]["amount"]
+                )
                 Net_diesel = Diesel_use + Diesel_offset
-                lci.add(name=('Technosphere', 'Equipment_Diesel'),
-                        flow=Net_diesel)
+                lci.add(name=("Technosphere", "Equipment_Diesel"), flow=Net_diesel)
 
             # Offset from fertilizer
-            lci.add(name=('Technosphere', 'Nitrogen_Fertilizer'),
-                    flow=-Navail)
-            lci.add(name=('Technosphere', 'Phosphorous_Fertilizer'),
-                    flow=-Pavail)
-            lci.add(name=('Technosphere', 'Potassium_Fertilizer'),
-                    flow=-Kavail)
+            lci.add(name=("Technosphere", "Nitrogen_Fertilizer"), flow=-Navail)
+            lci.add(name=("Technosphere", "Phosphorous_Fertilizer"), flow=-Pavail)
+            lci.add(name=("Technosphere", "Potassium_Fertilizer"), flow=-Kavail)
 
             # offset from applying fertilizer
-            Fert_N2O = -Navail * common_data.Land_app['fert_N2O']['amount'] / 100
-            Fert_NH3 = -Navail * common_data.Land_app['fert_NH3']['amount'] / 100 * common_data.Land_app['fert_NH3Evap']['amount'] / 100
-            Fert_NO3_GW = -Navail * common_data.Land_app['fert_NO3Leach']['amount'] /100
-            Fert_NO3_SW = -Navail * common_data.Land_app['fert_NO3Run']['amount'] / 100
-
-            lci.add(name='Dinitrogen monoxide',
-                    flow=Fert_N2O * common_data.MW['Nitrous_Oxide']['amount']/common_data.MW['N']['amount']/2)
-            lci.add(name='Ammonia',
-                    flow=Fert_NH3 * common_data.MW['Ammonia']['amount']/common_data.MW['N']['amount'])
-            lci.add(name='Nitrate (ground water)',
-                    flow=Fert_NO3_GW * common_data.MW['Nitrate']['amount']/common_data.MW['N']['amount'])
-            lci.add(name='Nitrate (surface water)',
-                    flow=Fert_NO3_SW * common_data.MW['Nitrate']['amount']/common_data.MW['N']['amount'])
+            Fert_N2O = -Navail * common_data.Land_app["fert_N2O"]["amount"] / 100
+            Fert_NH3 = (
+                -Navail
+                * common_data.Land_app["fert_NH3"]["amount"]
+                / 100
+                * common_data.Land_app["fert_NH3Evap"]["amount"]
+                / 100
+            )
+            Fert_NO3_GW = -Navail * common_data.Land_app["fert_NO3Leach"]["amount"] / 100
+            Fert_NO3_SW = -Navail * common_data.Land_app["fert_NO3Run"]["amount"] / 100
+
+            lci.add(
+                name="Dinitrogen monoxide",
+                flow=Fert_N2O
+                * common_data.MW["Nitrous_Oxide"]["amount"]
+                / common_data.MW["N"]["amount"]
+                / 2,
+            )
+            lci.add(
+                name="Ammonia",
+                flow=Fert_NH3 * common_data.MW["Ammonia"]["amount"] / common_data.MW["N"]["amount"],
+            )
+            lci.add(
+                name="Nitrate (ground water)",
+                flow=Fert_NO3_GW
+                * common_data.MW["Nitrate"]["amount"]
+                / common_data.MW["N"]["amount"],
+            )
+            lci.add(
+                name="Nitrate (surface water)",
+                flow=Fert_NO3_SW
+                * common_data.MW["Nitrate"]["amount"]
+                / common_data.MW["N"]["amount"],
+            )
 
         # Peat offsets
-        if input_data.Compost_use['peatOff']['amount'] == 1:
-            compost_vol = input_flow.data['mass'].values / input_data.Material_Properties['densFC']['amount']
-            peat_vol = compost_vol * common_data.Land_app['PeatSubFac']['amount']
-            peat_mass = peat_vol * common_data.Land_app['densPeat']['amount'] / 1000  # Mg
+        if input_data.Compost_use["peatOff"]["amount"] == 1:
+            compost_vol = (
+                input_flow.data["mass"].values / input_data.Material_Properties["densFC"]["amount"]
+            )
+            peat_vol = compost_vol * common_data.Land_app["PeatSubFac"]["amount"]
+            peat_mass = peat_vol * common_data.Land_app["densPeat"]["amount"] / 1000  # Mg
 
             # Avoided emissions from peat saving
-            peat_C = (peat_mass
-                      * (1 - common_data.Land_app['PeatMoist']['amount'])
-                      * common_data.Land_app['PeatC']['amount'])
-            peat_C_release = peat_C * (1 - common_data.Land_app['perCStorPeat']['amount'] / 100)
-
-            lci.add(name=('Technosphere', 'Peat'),
-                    flow=-peat_mass)
-            lci.add(name='Carbon dioxide, fossil',
-                    flow=-peat_C_release * common_data.MW['CO2']['amount'] / common_data.MW['C']['amount'])
+            peat_C = (
+                peat_mass
+                * (1 - common_data.Land_app["PeatMoist"]["amount"])
+                * common_data.Land_app["PeatC"]["amount"]
+            )
+            peat_C_release = peat_C * (1 - common_data.Land_app["perCStorPeat"]["amount"] / 100)
+
+            lci.add(name=("Technosphere", "Peat"), flow=-peat_mass)
+            lci.add(
+                name="Carbon dioxide, fossil",
+                flow=-peat_C_release
+                * common_data.MW["CO2"]["amount"]
+                / common_data.MW["C"]["amount"],
+            )
 
     # Compost as AD
-    if input_data.Compost_use['choice_BU']['amount'] == 0:
+    if input_data.Compost_use["choice_BU"]["amount"] == 0:
         # Carbon in final compost
-        Max_C_storage = (1 - material_properties['Moisture Content'].values / 100) * material_properties['Carbon Storage Factor'].values
-        C_storage = np.where(input_flow.data['C_cont'].values * (common_data.ADC['perCStor_LF']['amount'] / 100) <= Max_C_storage,
-                             input_flow.data['C_cont'].values * (common_data.ADC['perCStor_LF']['amount'] / 100),
-                             Max_C_storage)
-
-        C_released = (input_flow.data['C_cont'].values - C_storage) * (1 - common_data.ADC['frac_CH4']['amount'] / 100)
-        C_CH4 = (input_flow.data['C_cont'].values - C_storage) * (common_data.ADC['frac_CH4']['amount'] / 100)
-        C_CH4_Oxidized = C_CH4 * process_data['Methane Oxidized'].values / 100
-        C_CH4_Flared = C_CH4 * process_data['Methane Flared'].values / 100
-        C_CH4_Emitted = C_CH4 * process_data['Methane Emitted'].values / 100
-        C_CH4_EnergyRec = C_CH4 * process_data['Methane to Energy'].values / 100
-        C_CH4_EnergyRec_mass = C_CH4_EnergyRec * (common_data.MW['CH4']['amount'] / common_data.MW['C']['amount'])
-        CH4_LHV = common_data.LHV['CH4']['amount'] / common_data.STP['m3CH4_to_kg']['amount']  # MJ/kgCH4
-        C_CH4_Electricity = C_CH4_EnergyRec_mass * CH4_LHV * (common_data.ADC['Elec_eff']['amount'] / 100) / 3.6  #kWhElec
-
-        lci.add(name='Direct Carbon Storage and Humus Formation',
-                flow=-(C_storage * common_data.MW['CO2']['amount'] / common_data.MW['C']['amount']))
-        lci.add(name='Carbon dioxide, non-fossil',
-                flow=(C_released + C_CH4_EnergyRec + C_CH4_Flared + C_CH4_Oxidized) * common_data.MW['CO2']['amount'] / common_data.MW['C']['amount'])
-        lci.add(name='Methane, non-fossil',
-                flow=C_CH4_Emitted * common_data.MW['CH4']['amount'] / common_data.MW['C']['amount'])
-        lci.add(name=('Technosphere', 'Electricity_production'),
-                flow=C_CH4_Electricity)
-
-        #General emissions from LF
-        lci.add(name=('Technosphere', 'compost_to_LF'),
-                flow=(input_flow.data['mass'].values / 1000) * common_data.ADC['Aloc_ADC']['amount'])
-
-        #Amomonium emission from LF (Calculated base on the ammomium/N_cont ratio in LF)
-        NH4_LF = common_data.ADC['Frac_NH4']['amount'] * input_flow.data['N_cont']
-        NH4_GW=  NH4_LF * (1 - common_data.ADC['LCRS_eff']['amount'])
-        NH4_SW=  NH4_LF * common_data.ADC['LCRS_eff']['amount'] * (1 - common_data.ADC['NH4_rmv_eff']['amount'])
-        NO3_SW = NH4_LF * common_data.ADC['LCRS_eff']['amount'] * common_data.ADC['NH4_rmv_eff']['amount']
-
-        lci.add(name='Ammonium, ion (ground water)',
-                flow=NH4_GW * common_data.MW['Ammonium']['amount']/common_data.MW['N']['amount'])
-        lci.add(name='Ammonium, ion (surface water)',
-                flow=NH4_SW * common_data.MW['Ammonium']['amount']/common_data.MW['N']['amount'])
-        lci.add(name='Nitrate (surface water)',
-                flow=NO3_SW * common_data.MW['Nitrate']['amount']/common_data.MW['N']['amount'])
-
-        #Avoided excavation
-        compost_vol = input_flow.data['mass'].values / input_data.Material_Properties['densFC']['amount']
-        dc_soil_vol = compost_vol * (common_data.ADC['DC_thick']['amount'] / common_data.ADC['ADC_thick']['amount'])\
-            * common_data.ADC['DC_subs_fac']['amount']
+        Max_C_storage = (
+            1 - material_properties["Moisture Content"].values / 100
+        ) * material_properties["Carbon Storage Factor"].values
+        C_storage = np.where(
+            input_flow.data["C_cont"].values * (common_data.ADC["perCStor_LF"]["amount"] / 100)
+            <= Max_C_storage,
+            input_flow.data["C_cont"].values * (common_data.ADC["perCStor_LF"]["amount"] / 100),
+            Max_C_storage,
+        )
+
+        C_released = (input_flow.data["C_cont"].values - C_storage) * (
+            1 - common_data.ADC["frac_CH4"]["amount"] / 100
+        )
+        C_CH4 = (input_flow.data["C_cont"].values - C_storage) * (
+            common_data.ADC["frac_CH4"]["amount"] / 100
+        )
+        C_CH4_Oxidized = C_CH4 * process_data["Methane Oxidized"].values / 100
+        C_CH4_Flared = C_CH4 * process_data["Methane Flared"].values / 100
+        C_CH4_Emitted = C_CH4 * process_data["Methane Emitted"].values / 100
+        C_CH4_EnergyRec = C_CH4 * process_data["Methane to Energy"].values / 100
+        C_CH4_EnergyRec_mass = C_CH4_EnergyRec * (
+            common_data.MW["CH4"]["amount"] / common_data.MW["C"]["amount"]
+        )
+        CH4_LHV = (
+            common_data.LHV["CH4"]["amount"] / common_data.STP["m3CH4_to_kg"]["amount"]
+        )  # MJ/kgCH4
+        C_CH4_Electricity = (
+            C_CH4_EnergyRec_mass * CH4_LHV * (common_data.ADC["Elec_eff"]["amount"] / 100) / 3.6
+        )  # kWhElec
+
+        lci.add(
+            name="Direct Carbon Storage and Humus Formation",
+            flow=-(C_storage * common_data.MW["CO2"]["amount"] / common_data.MW["C"]["amount"]),
+        )
+        lci.add(
+            name="Carbon dioxide, non-fossil",
+            flow=(C_released + C_CH4_EnergyRec + C_CH4_Flared + C_CH4_Oxidized)
+            * common_data.MW["CO2"]["amount"]
+            / common_data.MW["C"]["amount"],
+        )
+        lci.add(
+            name="Methane, non-fossil",
+            flow=C_CH4_Emitted * common_data.MW["CH4"]["amount"] / common_data.MW["C"]["amount"],
+        )
+        lci.add(name=("Technosphere", "Electricity_production"), flow=C_CH4_Electricity)
+
+        # General emissions from LF
+        lci.add(
+            name=("Technosphere", "compost_to_LF"),
+            flow=(input_flow.data["mass"].values / 1000) * common_data.ADC["Aloc_ADC"]["amount"],
+        )
+
+        # Ammonium emission from LF (Calculated base on the ammonium/N_cont ratio in LF)
+        NH4_LF = common_data.ADC["Frac_NH4"]["amount"] * input_flow.data["N_cont"]
+        NH4_GW = NH4_LF * (1 - common_data.ADC["LCRS_eff"]["amount"])
+        NH4_SW = (
+            NH4_LF
+            * common_data.ADC["LCRS_eff"]["amount"]
+            * (1 - common_data.ADC["NH4_rmv_eff"]["amount"])
+        )
+        NO3_SW = (
+            NH4_LF
+            * common_data.ADC["LCRS_eff"]["amount"]
+            * common_data.ADC["NH4_rmv_eff"]["amount"]
+        )
+
+        lci.add(
+            name="Ammonium, ion (ground water)",
+            flow=NH4_GW * common_data.MW["Ammonium"]["amount"] / common_data.MW["N"]["amount"],
+        )
+        lci.add(
+            name="Ammonium, ion (surface water)",
+            flow=NH4_SW * common_data.MW["Ammonium"]["amount"] / common_data.MW["N"]["amount"],
+        )
+        lci.add(
+            name="Nitrate (surface water)",
+            flow=NO3_SW * common_data.MW["Nitrate"]["amount"] / common_data.MW["N"]["amount"],
+        )
+
+        # Avoided excavation
+        compost_vol = (
+            input_flow.data["mass"].values / input_data.Material_Properties["densFC"]["amount"]
+        )
+        dc_soil_vol = (
+            compost_vol
+            * (common_data.ADC["DC_thick"]["amount"] / common_data.ADC["ADC_thick"]["amount"])
+            * common_data.ADC["DC_subs_fac"]["amount"]
+        )
 
-        lci.add(name=('Technosphere', 'market_for_excavation_skid_steer_loader'),
-                flow=dc_soil_vol)
+        lci.add(name=("Technosphere", "market_for_excavation_skid_steer_loader"), flow=dc_soil_vol)
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/Distance.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Distance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Jan  6 14:50:00 2020
-
-@author: msardar2
-"""
-import pandas as pd
 import numpy as np
+import pandas as pd
 
 
-class Distance():
+class Distance:
     """
     Python class for importing the distances between the process models.
-    
+
     Transport modes include:
-    
+
     * Heavy Duty Truck
     * Medium Duty Truck
-    * Rail 
+    * Rail
     * Barge
     * Cargo Ship
-        
-    :param data: `Dictionary` that includes `Pandas DataFrame` for the distances between the process models as `value` and 
-        tranport modes as `key`. `DataFrame` should use the name of processes as both `column` and row `index`.
+
+    :param data: `Dictionary` that includes `Pandas DataFrame` for the distances between the process models as `value` and
+        transport modes as `key`. `DataFrame` should use the name of processes as both `column` and row `index`.
     :type Data: dict
 
     :Example:
 
     >>> from swolfpy_processmodels import Distance
     >>> data = Distance.create_distance_table(['LF','WTE','AD'], ['Heavy Duty Truck'], default_dist=20)
     >>> data
@@ -34,50 +29,53 @@
                          WTE NaN   NaN  20.0
                          AD  NaN   NaN   NaN}
     >>> distance = Distance(data)
     >>> distance.Distance[('LF','WTE')]
     {'Heavy Duty Truck': 20.0}
     >>> distance.Distance[('LF','WTE')]['Heavy Duty Truck']
     20.0
-
     """
+
     def __init__(self, data=None):
         """
-        Create Distance object.                    
+        Create Distance object.
         """
         self.data = data
         self.Distance = {}
         self.transport_modes = list(self.data.keys())
         for mode in self.transport_modes:
             for i in self.data[mode].columns:
                 for j in self.data[mode].index:
-                    if (i,j) not in self.Distance.keys():
-                        self.Distance[(i,j)] = {}
-                    if (j,i) not in self.Distance.keys():
-                        self.Distance[(j,i)] = {}
-                    if not pd.isna(self.data[mode][i][j]) and self.data[mode][i][j]!='':
-                        self.Distance[(i,j)][mode] = self.data[mode][i][j]
-                        self.Distance[(j,i)][mode] = self.data[mode][i][j]
-                        if not pd.isna(self.data[mode][j][i]) and self.data[mode][j][i]!='' and self.data[mode][j][i]!=self.data[mode][i][j]:
-                            raise Exception(f'Distance from {i} to {j} is not equal to distance from {j} to {i} in transport mode of {mode}')    
+                    if (i, j) not in self.Distance.keys():
+                        self.Distance[(i, j)] = {}
+                    if (j, i) not in self.Distance.keys():
+                        self.Distance[(j, i)] = {}
+                    if not pd.isna(self.data[mode][i][j]) and self.data[mode][i][j] != "":
+                        self.Distance[(i, j)][mode] = self.data[mode][i][j]
+                        self.Distance[(j, i)][mode] = self.data[mode][i][j]
+                        if (
+                            not pd.isna(self.data[mode][j][i])
+                            and self.data[mode][j][i] != ""
+                            and self.data[mode][j][i] != self.data[mode][i][j]
+                        ):
+                            raise ValueError(
+                                f"Distance from {i} to {j} is not equal to distance from {j} to {i} in transport mode of {mode}"
+                            )
 
     @staticmethod
     def create_distance_table(process_names, transport_modes, default_dist=np.nan):
         """
         Static method for creating the data structure for distances and transport modes.
 
         :param process_names: `List` of process names (e.g., ``['LF', 'WTE']``)
         :param transport_modes: `List` of transport modes (i.e., Heavy Duty Truck, Medium Duty Truck, Rail, Barge, Cargo Ship).
             Example: ``['Heavy Duty Truck', 'Medium Duty Truck']``
         :param default_dist: Default distance that is used to fill the `DataFrame`.
-        
         """
-        dist_dict = dict()
-        dist_array = np.full((len(process_names), len(process_names)),
-                     np.nan,
-                     dtype='float')
-        dist_array[np.triu_indices_from(dist_array, k=1)] = default_dist 
+        dist_dict = {}
+        dist_array = np.full((len(process_names), len(process_names)), np.nan, dtype="float")
+        dist_array[np.triu_indices_from(dist_array, k=1)] = default_dist
         for mode in transport_modes:
-            dist_dict[mode] = pd.DataFrame(data=dist_array,
-                                           columns=process_names,
-                                           index=process_names)
-        return(dist_dict)
+            dist_dict[mode] = pd.DataFrame(
+                data=dist_array, columns=process_names, index=process_names
+            )
+        return dist_dict
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/GC.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/GC.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,471 +1,585 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Sep  2 12:42:12 2021
-
-@author: msardar2
-"""
-import pandas as pd
 import numpy_financial as npf
+import pandas as pd
 from swolfpy_inputdata import GC_Input
+
 from .ProcessModel import ProcessModel
 
 
 class GC(ProcessModel):
-    """
-    """
-    Process_Type = 'RDF'
-    def __init__(self, process_name='Gasification Syngas Combustion',
-                 input_data_path=None, CommonDataObjct=None):
+    Process_Type = "RDF"
+
+    def __init__(
+        self,
+        process_name="Gasification Syngas Combustion",
+        input_data_path=None,
+        CommonDataObjct=None,
+    ):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = GC_Input(input_data_path, process_name=self.process_name,
-                                  CommonDataObjct=CommonDataObjct)
+        self.InputData = GC_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
         self.process_data = self.InputData.process_data
 
     def calc(self):
         self._input_rdf = pd.DataFrame(index=self.CommonData.Index)
-        self._input_rdf['mass'] = self.process_data['Assumed_Comp'].values
-        self._input_rdf['moist'] = (self._input_rdf['mass'].values
-                                    * self.Material_Properties['Moisture Content'].values / 100)
-        self._input_rdf['solid'] = self._input_rdf['mass'].values - self._input_rdf['moist'].values
-        self._input_rdf['solid_comp'] = self._input_rdf['solid'].values / sum(self._input_rdf['solid'].values)
-
+        self._input_rdf["mass"] = self.process_data["Assumed_Comp"].values
+        self._input_rdf["moist"] = (
+            self._input_rdf["mass"].values
+            * self.Material_Properties["Moisture Content"].values
+            / 100
+        )
+        self._input_rdf["solid"] = self._input_rdf["mass"].values - self._input_rdf["moist"].values
+        self._input_rdf["solid_comp"] = self._input_rdf["solid"].values / sum(
+            self._input_rdf["solid"].values
+        )
 
         # RDF drying: Energy use (heat & electricity)
-        moist_cont = self._input_rdf['moist'].sum() / self._input_rdf['mass'].sum()
-        if  moist_cont > self.InputData.Dryer['moist_cont']['amount']:
-            water_evap = (moist_cont - self._input_rdf['solid'].sum()
-                          / (1 - self.InputData.Dryer['moist_cont']['amount'])
-                          * self.InputData.Dryer['moist_cont']['amount'])
+        moist_cont = self._input_rdf["moist"].sum() / self._input_rdf["mass"].sum()
+        if moist_cont > self.InputData.Dryer["moist_cont"]["amount"]:
+            water_evap = (
+                moist_cont
+                - self._input_rdf["solid"].sum()
+                / (1 - self.InputData.Dryer["moist_cont"]["amount"])
+                * self.InputData.Dryer["moist_cont"]["amount"]
+            )
         else:
             water_evap = 0
 
         # Dried RDF: chemical/physical properties
-        self._dry_rdf = pd.DataFrame(columns=['value', 'unit'])
+        self._dry_rdf = pd.DataFrame(columns=["value", "unit"])
         if water_evap > 0:
-            self._dry_rdf.loc['moist', 'value'] = (self._input_rdf['moist'].sum()
-                                                   - water_evap)
-            self._dry_rdf.loc['moist_cont', 'value'] = self.InputData.Dryer['moist_cont']['amount']
+            self._dry_rdf.loc["moist", "value"] = self._input_rdf["moist"].sum() - water_evap
+            self._dry_rdf.loc["moist_cont", "value"] = self.InputData.Dryer["moist_cont"]["amount"]
         else:
-            self._dry_rdf.loc['moist', 'value'] = self._input_rdf['moist'].sum()
-            self._dry_rdf.loc['moist_cont', 'value'] = moist_cont
+            self._dry_rdf.loc["moist", "value"] = self._input_rdf["moist"].sum()
+            self._dry_rdf.loc["moist_cont", "value"] = moist_cont
 
-        self._dry_rdf.loc['solid', 'value'] = self._input_rdf['solid'].sum()
-        self._dry_rdf.loc['mass', 'value'] = (self._dry_rdf.loc['solid', 'value']
-                                              + self._dry_rdf.loc['moist', 'value'])
-        self._dry_rdf.loc['ash', 'value'] = sum(self._input_rdf['solid'].values
-                                                * self.Material_Properties['Ash Content']
-                                                / 100)
-        self._dry_rdf.loc[['moist', 'solid', 'mass', 'ash'], 'unit'] = 'Mg/Mg RDF'
-        self._dry_rdf.loc['moist_cont', 'unit'] = 'fraction'
-
-        agent_ratio, ratio, CH4 = self._feed_stock_spec(self._input_rdf['solid'],
-                                                        self._dry_rdf.loc['moist', 'value'],
-                                                        self._dry_rdf.loc['mass', 'value'])
+        self._dry_rdf.loc["solid", "value"] = self._input_rdf["solid"].sum()
+        self._dry_rdf.loc["mass", "value"] = (
+            self._dry_rdf.loc["solid", "value"] + self._dry_rdf.loc["moist", "value"]
+        )
+        self._dry_rdf.loc["ash", "value"] = sum(
+            self._input_rdf["solid"].values * self.Material_Properties["Ash Content"] / 100
+        )
+        self._dry_rdf.loc[["moist", "solid", "mass", "ash"], "unit"] = "Mg/Mg RDF"
+        self._dry_rdf.loc["moist_cont", "unit"] = "fraction"
+
+        agent_ratio, ratio, CH4 = self._feed_stock_spec(
+            self._input_rdf["solid"],
+            self._dry_rdf.loc["moist", "value"],
+            self._dry_rdf.loc["mass", "value"],
+        )
         # Calculation of C, H, N, O
-        self._dry_rdf.loc['C_mole', :] = (sum(self._input_rdf['solid']
-                                              * (self.Material_Properties['Biogenic Carbon Content']
-                                                 + self.Material_Properties['Fossil Carbon Content'])
-                                              / 100
-                                              / self.CommonData.MW['C']['amount']),
-                                          'Mg mole/Mg RDF')
-
-        self._dry_rdf.loc['frac_biogenic_C', :] = (
-            sum(self._input_rdf['solid'] * self.Material_Properties['Biogenic Carbon Content'])
-            / sum(self._input_rdf['solid']
-                  * (self.Material_Properties['Biogenic Carbon Content']
-                     + self.Material_Properties['Fossil Carbon Content']))), 'fraction'
+        self._dry_rdf.loc["C_mole", :] = (
+            sum(
+                self._input_rdf["solid"]
+                * (
+                    self.Material_Properties["Biogenic Carbon Content"]
+                    + self.Material_Properties["Fossil Carbon Content"]
+                )
+                / 100
+                / self.CommonData.MW["C"]["amount"]
+            ),
+            "Mg mole/Mg RDF",
+        )
+
+        self._dry_rdf.loc["frac_biogenic_C", :] = (
+            sum(self._input_rdf["solid"] * self.Material_Properties["Biogenic Carbon Content"])
+            / sum(
+                self._input_rdf["solid"]
+                * (
+                    self.Material_Properties["Biogenic Carbon Content"]
+                    + self.Material_Properties["Fossil Carbon Content"]
+                )
+            )
+        ), "fraction"
 
         def helper_sld_cont(cont, element):
-            sld_cont = sum(self._input_rdf['solid']
-                           * self.Material_Properties[cont]
-                           / 100
-                           / self.CommonData.MW[element]['amount'])
-            return sld_cont, 'Mg mole/Mg RDF'
-
-        self._dry_rdf.loc['H_mole', :] = helper_sld_cont('Hydrogen Content', 'H')
-        self._dry_rdf.loc['N_mole', :] = helper_sld_cont('Nitrogen Content', 'N')
-        self._dry_rdf.loc['O_mole', :] = helper_sld_cont('Oxygen Content', 'O')
-        self._dry_rdf.loc['S_mole', :] = helper_sld_cont('Sulphur', 'S')
-        self._dry_rdf.loc['Cl_mole', :] = helper_sld_cont('Chlorine', 'Cl')
+            sld_cont = sum(
+                self._input_rdf["solid"]
+                * self.Material_Properties[cont]
+                / 100
+                / self.CommonData.MW[element]["amount"]
+            )
+            return sld_cont, "Mg mole/Mg RDF"
+
+        self._dry_rdf.loc["H_mole", :] = helper_sld_cont("Hydrogen Content", "H")
+        self._dry_rdf.loc["N_mole", :] = helper_sld_cont("Nitrogen Content", "N")
+        self._dry_rdf.loc["O_mole", :] = helper_sld_cont("Oxygen Content", "O")
+        self._dry_rdf.loc["S_mole", :] = helper_sld_cont("Sulphur", "S")
+        self._dry_rdf.loc["Cl_mole", :] = helper_sld_cont("Chlorine", "Cl")
 
         def helper_react(element):
-            self._dry_rdf.loc[element + '_react', :] = (
-                self._dry_rdf.loc[element, 'value']
-                * self.InputData.Gasifier['frac_react']['amount'],
-                'Mg mole/Mg RDF')
+            self._dry_rdf.loc[element + "_react", :] = (
+                self._dry_rdf.loc[element, "value"]
+                * self.InputData.Gasifier["frac_react"]["amount"],
+                "Mg mole/Mg RDF",
+            )
 
         # Calculation of reated C, H, N, O
-        for element in ['C_mole', 'H_mole', 'N_mole', 'O_mole', 'S_mole', 'Cl_mole']:
+        for element in ["C_mole", "H_mole", "N_mole", "O_mole", "S_mole", "Cl_mole"]:
             helper_react(element)
 
         # Add the H and O of moisture
-        self._dry_rdf.loc['H_mole_react_tot', :] = (self._dry_rdf.loc['H_mole_react', 'value']
-                                                    + self._dry_rdf.loc['moist', 'value']
-                                                    / self.CommonData.MW['H2O']['amount']
-                                                    * 2,
-                                                    'Mg mole/Mg RDF')
-        self._dry_rdf.loc['O_mole_react_tot', :] = (self._dry_rdf.loc['O_mole_react', 'value']
-                                                    + self._dry_rdf.loc['moist', 'value']
-                                                    / self.CommonData.MW['H2O']['amount'],
-                                                    'Mg mole/Mg RDF')
-
-        self._dry_rdf.loc['C_cont', :] = (sum(self._input_rdf['solid']
-                                              * (self.Material_Properties['Biogenic Carbon Content']
-                                                 + self.Material_Properties['Fossil Carbon Content'])
-                                              / 100) / self._input_rdf['solid'].sum(),
-                                          'Mg mole/Mg RDF')
+        self._dry_rdf.loc["H_mole_react_tot", :] = (
+            self._dry_rdf.loc["H_mole_react", "value"]
+            + self._dry_rdf.loc["moist", "value"] / self.CommonData.MW["H2O"]["amount"] * 2,
+            "Mg mole/Mg RDF",
+        )
+        self._dry_rdf.loc["O_mole_react_tot", :] = (
+            self._dry_rdf.loc["O_mole_react", "value"]
+            + self._dry_rdf.loc["moist", "value"] / self.CommonData.MW["H2O"]["amount"],
+            "Mg mole/Mg RDF",
+        )
+
+        self._dry_rdf.loc["C_cont", :] = (
+            sum(
+                self._input_rdf["solid"]
+                * (
+                    self.Material_Properties["Biogenic Carbon Content"]
+                    + self.Material_Properties["Fossil Carbon Content"]
+                )
+                / 100
+            )
+            / self._input_rdf["solid"].sum(),
+            "Mg mole/Mg RDF",
+        )
 
         # Mass ratio of gasifier agent to RDF
-        self._dry_rdf.loc['agent_ratio', :] = (agent_ratio, 'Mg/Mg Dry RDF')
-        self._dry_rdf.loc['agent_mass', :] = (agent_ratio
-                                              * self._dry_rdf.loc['mass', 'value'],
-                                              'Mg/Mg RDF')
-
-
-        self._dry_rdf.loc['agent_O_mole', :] = (self._dry_rdf.loc['agent_mass', 'value']
-                                                / self.CommonData.Air['MW']['amount']
-                                                * self.CommonData.Air['O_cont']['amount'] * 2,
-                                                'Mg mole/Mg RDF')
-        self._dry_rdf.loc['agent_N_mole', :] = (self._dry_rdf.loc['agent_mass', 'value']
-                                                / self.CommonData.Air['MW']['amount']
-                                                * self.CommonData.Air['N_cont']['amount'] * 2,
-                                                'Mg mole/Mg RDF')
-
-        self._dry_rdf.loc['O_mole_final', :] = (self._dry_rdf.loc['O_mole_react_tot', 'value']
-                                                + self._dry_rdf.loc['agent_O_mole', 'value'],
-                                                'Mg mole/Mg RDF')
-
-        self._dry_rdf.loc['N_mole_final', :] = (self._dry_rdf.loc['N_mole_react', 'value']
-                                                + self._dry_rdf.loc['agent_N_mole', 'value'],
-                                                'Mg mole/Mg RDF')
+        self._dry_rdf.loc["agent_ratio", :] = (agent_ratio, "Mg/Mg Dry RDF")
+        self._dry_rdf.loc["agent_mass", :] = (
+            agent_ratio * self._dry_rdf.loc["mass", "value"],
+            "Mg/Mg RDF",
+        )
+
+        self._dry_rdf.loc["agent_O_mole", :] = (
+            self._dry_rdf.loc["agent_mass", "value"]
+            / self.CommonData.Air["MW"]["amount"]
+            * self.CommonData.Air["O_cont"]["amount"]
+            * 2,
+            "Mg mole/Mg RDF",
+        )
+        self._dry_rdf.loc["agent_N_mole", :] = (
+            self._dry_rdf.loc["agent_mass", "value"]
+            / self.CommonData.Air["MW"]["amount"]
+            * self.CommonData.Air["N_cont"]["amount"]
+            * 2,
+            "Mg mole/Mg RDF",
+        )
+
+        self._dry_rdf.loc["O_mole_final", :] = (
+            self._dry_rdf.loc["O_mole_react_tot", "value"]
+            + self._dry_rdf.loc["agent_O_mole", "value"],
+            "Mg mole/Mg RDF",
+        )
+
+        self._dry_rdf.loc["N_mole_final", :] = (
+            self._dry_rdf.loc["N_mole_react", "value"] + self._dry_rdf.loc["agent_N_mole", "value"],
+            "Mg mole/Mg RDF",
+        )
 
         # gasification products
-        self.gasifier_products = pd.DataFrame(columns=['value', 'unit'])
-        self.gasifier_products.loc['H2/CO', :] = (ratio, 'mole/mole')
-        CH4_mole = CH4 * self._dry_rdf.loc['mass', 'value']
-        self.gasifier_products.loc['CH4', :] = CH4_mole, 'Mg mole/Mg RDF'
+        self.gasifier_products = pd.DataFrame(columns=["value", "unit"])
+        self.gasifier_products.loc["H2/CO", :] = (ratio, "mole/mole")
+        CH4_mole = CH4 * self._dry_rdf.loc["mass", "value"]
+        self.gasifier_products.loc["CH4", :] = CH4_mole, "Mg mole/Mg RDF"
 
         CO_mole, CO2_mole, H2_mole, N2_mole, H2O_mole = GC._gasifier_products(
-            C_mole=self._dry_rdf.loc['C_mole_react', 'value'],
-            H_mole=self._dry_rdf.loc['H_mole_react_tot', 'value'],
-            O_mole=self._dry_rdf.loc['O_mole_final', 'value'],
-            N_mol=self._dry_rdf.loc['N_mole_final', 'value'],
+            C_mole=self._dry_rdf.loc["C_mole_react", "value"],
+            H_mole=self._dry_rdf.loc["H_mole_react_tot", "value"],
+            O_mole=self._dry_rdf.loc["O_mole_final", "value"],
+            N_mol=self._dry_rdf.loc["N_mole_final", "value"],
             CH4_mole=CH4_mole,
             ratio=ratio,
-            moist_mole=self._dry_rdf.loc['moist', 'value']/self.CommonData.MW['H2O']['amount'])
+            moist_mole=self._dry_rdf.loc["moist", "value"] / self.CommonData.MW["H2O"]["amount"],
+        )
 
-        self.gasifier_products.loc['CO', :] = CO_mole, 'Mg mole/Mg RDF'
-        self.gasifier_products.loc['CO2', :] = CO2_mole, 'Mg mole/Mg RDF'
-        self.gasifier_products.loc['H2', :] = H2_mole, 'Mg mole/Mg RDF'
-        self.gasifier_products.loc['N2', :] = N2_mole, 'Mg mole/Mg RDF'
-        self.gasifier_products.loc['H2O', :] = H2O_mole, 'Mg mole/Mg RDF'
-
-        self.gasifier_products.loc['Bottom Ash', :] = (
-            self._dry_rdf.loc['ash', 'value']
-            + self._dry_rdf.loc['solid', 'value']
-            * (1 - self.InputData.Gasifier['frac_react']['amount'])), 'Mg/Mg RDF'
+        self.gasifier_products.loc["CO", :] = CO_mole, "Mg mole/Mg RDF"
+        self.gasifier_products.loc["CO2", :] = CO2_mole, "Mg mole/Mg RDF"
+        self.gasifier_products.loc["H2", :] = H2_mole, "Mg mole/Mg RDF"
+        self.gasifier_products.loc["N2", :] = N2_mole, "Mg mole/Mg RDF"
+        self.gasifier_products.loc["H2O", :] = H2O_mole, "Mg mole/Mg RDF"
+
+        self.gasifier_products.loc["Bottom Ash", :] = (
+            self._dry_rdf.loc["ash", "value"]
+            + self._dry_rdf.loc["solid", "value"]
+            * (1 - self.InputData.Gasifier["frac_react"]["amount"])
+        ), "Mg/Mg RDF"
 
         # Energy calculations
-        self.energy = pd.DataFrame(columns=['value', 'unit'])
+        self.energy = pd.DataFrame(columns=["value", "unit"])
 
-        self.energy.loc['LHV_SYNGAS', :] = (
-            self.gasifier_products.loc['CO', 'value'] * self.CommonData.LHV['CO_mole']['amount']
-            + self.gasifier_products.loc['H2', 'value'] * self.CommonData.LHV['H2_mole']['amount']
-            + self.gasifier_products.loc['CH4', 'value'] * self.CommonData.LHV['CH4_mole']['amount']
-            ) * 1000, 'MJ/Mg RDF'
-
-        self.energy.loc['LHV_RDF', :] = (
-            sum(self._input_rdf['solid'] * self.CommonData.Material_Properties['Lower Heating Value'])
-            - sum(self._input_rdf['moist']) * self.CommonData.Evap_heat['water']['amount']) * 1000, 'MJ/Mg RDF'
+        self.energy.loc["LHV_SYNGAS", :] = (
+            self.gasifier_products.loc["CO", "value"] * self.CommonData.LHV["CO_mole"]["amount"]
+            + self.gasifier_products.loc["H2", "value"] * self.CommonData.LHV["H2_mole"]["amount"]
+            + self.gasifier_products.loc["CH4", "value"] * self.CommonData.LHV["CH4_mole"]["amount"]
+        ) * 1000, "MJ/Mg RDF"
+
+        self.energy.loc["LHV_RDF", :] = (
+            sum(
+                self._input_rdf["solid"]
+                * self.CommonData.Material_Properties["Lower Heating Value"]
+            )
+            - sum(self._input_rdf["moist"]) * self.CommonData.Evap_heat["water"]["amount"]
+        ) * 1000, "MJ/Mg RDF"
 
         # Cold Gas Efficiency
-        self.energy.loc['Cold Gas Eff', :] = (
-            self.energy.loc['LHV_SYNGAS', 'value']
-            / self.energy.loc['LHV_RDF', 'value'] * 100), '%'
+        self.energy.loc["Cold Gas Eff", :] = (
+            self.energy.loc["LHV_SYNGAS", "value"] / self.energy.loc["LHV_RDF", "value"] * 100
+        ), "%"
 
         total_moles = CO_mole + CO2_mole + H2_mole + N2_mole + H2O_mole + CH4_mole
-        self.syngas = pd.DataFrame(columns=['value', 'unit'])
-        self.syngas.loc['CO', :] = CO_mole / total_moles * 100, '%mole'
-        self.syngas.loc['CO2', :] = CO2_mole / total_moles* 100, '%mole'
-        self.syngas.loc['H2', :] = H2_mole / total_moles* 100, '%mole'
-        self.syngas.loc['N2', :] = N2_mole / total_moles* 100, '%mole'
-        self.syngas.loc['H2O', :] = H2O_mole / total_moles* 100, '%mole'
-        self.syngas.loc['CH4', :] = CH4_mole / total_moles* 100, '%mole'
-        self.syngas.loc['LHV', :] = (
-            self.energy.loc['LHV_SYNGAS', 'value']
-            / (total_moles
-               * self.CommonData.STP['mole_to_L']['amount'] * 1000)
-            ), 'MJ/NM3'
+        self.syngas = pd.DataFrame(columns=["value", "unit"])
+        self.syngas.loc["CO", :] = CO_mole / total_moles * 100, "%mole"
+        self.syngas.loc["CO2", :] = CO2_mole / total_moles * 100, "%mole"
+        self.syngas.loc["H2", :] = H2_mole / total_moles * 100, "%mole"
+        self.syngas.loc["N2", :] = N2_mole / total_moles * 100, "%mole"
+        self.syngas.loc["H2O", :] = H2O_mole / total_moles * 100, "%mole"
+        self.syngas.loc["CH4", :] = CH4_mole / total_moles * 100, "%mole"
+        self.syngas.loc["LHV", :] = (
+            self.energy.loc["LHV_SYNGAS", "value"]
+            / (total_moles * self.CommonData.STP["mole_to_L"]["amount"] * 1000)
+        ), "MJ/NM3"
 
         # Sensible heat of syngas: Gasifier temp at 900 C
         # Syngas is cooled to 150 C
-        self.energy.loc['Sensible_Heat_SYNGAS', :] = (
-            CO_mole * self.CommonData.Heat_cap['CO']['amount']
-            + CO2_mole * self.CommonData.Heat_cap['CO2']['amount']
-            + H2_mole * self.CommonData.Heat_cap['H2']['amount']
-            + N2_mole * self.CommonData.Heat_cap['N2']['amount']
-            + H2O_mole * self.CommonData.Heat_cap['H2O']['amount']
-            + CH4_mole * self.CommonData.Heat_cap['CH4']['amount']
-            ) * (900 - 150), 'MJ/Mg RDF'
+        self.energy.loc["Sensible_Heat_SYNGAS", :] = (
+            CO_mole * self.CommonData.Heat_cap["CO"]["amount"]
+            + CO2_mole * self.CommonData.Heat_cap["CO2"]["amount"]
+            + H2_mole * self.CommonData.Heat_cap["H2"]["amount"]
+            + N2_mole * self.CommonData.Heat_cap["N2"]["amount"]
+            + H2O_mole * self.CommonData.Heat_cap["H2O"]["amount"]
+            + CH4_mole * self.CommonData.Heat_cap["CH4"]["amount"]
+        ) * (900 - 150), "MJ/Mg RDF"
 
         # Hot gas eff
-        self.energy.loc['Hot Gas Eff', :] = (
-            (self.energy.loc['LHV_SYNGAS', 'value']
-             + self.energy.loc['Sensible_Heat_SYNGAS', 'value'])
-            / self.energy.loc['LHV_RDF', 'value'] * 100), '%'
+        self.energy.loc["Hot Gas Eff", :] = (
+            (
+                self.energy.loc["LHV_SYNGAS", "value"]
+                + self.energy.loc["Sensible_Heat_SYNGAS", "value"]
+            )
+            / self.energy.loc["LHV_RDF", "value"]
+            * 100
+        ), "%"
 
         # Dryer
         if water_evap > 0:
-            self.energy.loc['Elec Dryer', :] = (
-                water_evap * 1000
-                * self.InputData.Dryer['elec_use']['amount']
-                / 3.6), 'kWh/Mg RDF'
-            self.energy.loc['Heat Dryer', :] = (
-                water_evap * 1000
-                * self.InputData.Dryer['heat_use']['amount']
-                ), 'MJ/Mg RDF'
+            self.energy.loc["Elec Dryer", :] = (
+                water_evap * 1000 * self.InputData.Dryer["elec_use"]["amount"] / 3.6
+            ), "kWh/Mg RDF"
+            self.energy.loc["Heat Dryer", :] = (
+                water_evap * 1000 * self.InputData.Dryer["heat_use"]["amount"]
+            ), "MJ/Mg RDF"
         else:
-            self.energy.loc['Elec Dryer', :] = 0.0, 'kWh/Mg RDF'
-            self.energy.loc['Heat Dryer', :] = 0.0, 'MJ/Mg RDF'
+            self.energy.loc["Elec Dryer", :] = 0.0, "kWh/Mg RDF"
+            self.energy.loc["Heat Dryer", :] = 0.0, "MJ/Mg RDF"
 
         # Steam turbine for electricity production
-        self.energy.loc['Elec Steam_Turbin HP', :] = (
-            self.energy.loc['LHV_SYNGAS', 'value']
-            * self.InputData.Energy['elec_gen_eff_HP']['amount']
-            / 3.6), 'kWh/Mg RDF'
+        self.energy.loc["Elec Steam_Turbine HP", :] = (
+            self.energy.loc["LHV_SYNGAS", "value"]
+            * self.InputData.Energy["elec_gen_eff_HP"]["amount"]
+            / 3.6
+        ), "kWh/Mg RDF"
 
         # Elec produced from MP steam recovered from excess heat
-        self.energy.loc['Elec Steam_Turbin MP', :] = (
-            (self.energy.loc['Sensible_Heat_SYNGAS', 'value']
-             * self.InputData.Energy['heat_rec_eff']['amount']
-             - self.energy.loc['Heat Dryer', 'value'])
-            * self.InputData.Energy['elec_gen_eff_MP']['amount']
-            / 3.6), 'kWh/Mg RDF'
+        self.energy.loc["Elec Steam_Turbine MP", :] = (
+            (
+                self.energy.loc["Sensible_Heat_SYNGAS", "value"]
+                * self.InputData.Energy["heat_rec_eff"]["amount"]
+                - self.energy.loc["Heat Dryer", "value"]
+            )
+            * self.InputData.Energy["elec_gen_eff_MP"]["amount"]
+            / 3.6
+        ), "kWh/Mg RDF"
 
         # Internal electricity use for syngas cleaning and ...
-        self.energy.loc['Elec Internal_use', :] = (
-            self.energy.loc['LHV_RDF', 'value']
-            * self.InputData.Energy['frac_lhv_internal_elec']['amount']
-            / 3.6), 'kWh/Mg RDF'
+        self.energy.loc["Elec Internal_use", :] = (
+            self.energy.loc["LHV_RDF", "value"]
+            * self.InputData.Energy["frac_lhv_internal_elec"]["amount"]
+            / 3.6
+        ), "kWh/Mg RDF"
 
         # Net electricity production
-        self.energy.loc['Net Elec prod', :] = (
-            self.energy.loc['Elec Steam_Turbin HP', 'value']
-            + self.energy.loc['Elec Steam_Turbin MP', 'value']
-            - self.energy.loc['Elec Internal_use', 'value']
-            - self.energy.loc['Elec Dryer', 'value']), 'kWh/Mg RDF'
+        self.energy.loc["Net Elec prod", :] = (
+            self.energy.loc["Elec Steam_Turbine HP", "value"]
+            + self.energy.loc["Elec Steam_Turbine MP", "value"]
+            - self.energy.loc["Elec Internal_use", "value"]
+            - self.energy.loc["Elec Dryer", "value"]
+        ), "kWh/Mg RDF"
 
         # Emissions
         self.bio_flows = self._biosphere_flows()
 
         # Add cost
         self._calc_cost()
 
     def _feed_stock_spec(self, solids, moist, mass):
         """
-        Calculates agent_ratio, ratio, CH4
+        Calculates agent_ratio, ratio, CH4.
         """
         # Calculate O, H, N, and C content (Mg Mole / Mg)
-        C_cont = sum(solids
-                     * (self.Material_Properties['Biogenic Carbon Content']
-                        + self.Material_Properties['Fossil Carbon Content'])
-                     / 100
-                     * self.InputData.Gasifier['frac_react']['amount']
-                     / self.CommonData.MW['C']['amount']) / mass
-
-        N_cont = sum(solids
-                     * self.Material_Properties['Nitrogen Content']
-                     / 100
-                     * self.InputData.Gasifier['frac_react']['amount']
-                     / self.CommonData.MW['N']['amount']) / mass
-
-        H_cont = sum(solids
-                     * self.Material_Properties['Hydrogen Content']
-                     / 100
-                     * self.InputData.Gasifier['frac_react']['amount']
-                     / self.CommonData.MW['H']['amount']) / mass
-
-        O_cont = sum(solids
-                     * self.Material_Properties['Oxygen Content']
-                     / 100
-                     * self.InputData.Gasifier['frac_react']['amount']
-                     / self.CommonData.MW['O']['amount']) / mass
+        C_cont = (
+            sum(
+                solids
+                * (
+                    self.Material_Properties["Biogenic Carbon Content"]
+                    + self.Material_Properties["Fossil Carbon Content"]
+                )
+                / 100
+                * self.InputData.Gasifier["frac_react"]["amount"]
+                / self.CommonData.MW["C"]["amount"]
+            )
+            / mass
+        )
+
+        N_cont = (
+            sum(
+                solids
+                * self.Material_Properties["Nitrogen Content"]
+                / 100
+                * self.InputData.Gasifier["frac_react"]["amount"]
+                / self.CommonData.MW["N"]["amount"]
+            )
+            / mass
+        )
+
+        H_cont = (
+            sum(
+                solids
+                * self.Material_Properties["Hydrogen Content"]
+                / 100
+                * self.InputData.Gasifier["frac_react"]["amount"]
+                / self.CommonData.MW["H"]["amount"]
+            )
+            / mass
+        )
+
+        O_cont = (
+            sum(
+                solids
+                * self.Material_Properties["Oxygen Content"]
+                / 100
+                * self.InputData.Gasifier["frac_react"]["amount"]
+                / self.CommonData.MW["O"]["amount"]
+            )
+            / mass
+        )
 
         # Add O and H content of moisture
-        H_cont += (moist / self.CommonData.MW['H2O']['amount'] * 2) / mass
-        O_cont += (moist / self.CommonData.MW['H2O']['amount']) / mass
+        H_cont += (moist / self.CommonData.MW["H2O"]["amount"] * 2) / mass
+        O_cont += (moist / self.CommonData.MW["H2O"]["amount"]) / mass
 
         # Calculate moist content (Mg moist/Mg)
         moist_cont = moist / mass
 
         agent_ratio = GC._agent_ratio(C_cont, H_cont, O_cont, moist_cont)
 
         # Add O and N content of agent
-        O_cont += agent_ratio / self.CommonData.Air['MW']['amount'] * self.CommonData.Air['O_cont']['amount'] * 2
-        N_cont += agent_ratio / self.CommonData.Air['MW']['amount'] * self.CommonData.Air['N_cont']['amount'] * 2
+        O_cont += (
+            agent_ratio
+            / self.CommonData.Air["MW"]["amount"]
+            * self.CommonData.Air["O_cont"]["amount"]
+            * 2
+        )
+        N_cont += (
+            agent_ratio
+            / self.CommonData.Air["MW"]["amount"]
+            * self.CommonData.Air["N_cont"]["amount"]
+            * 2
+        )
 
-        ash = sum(solids
-                  * self.Material_Properties['Ash Content']
-                  / 100) / mass
+        ash = sum(solids * self.Material_Properties["Ash Content"] / 100) / mass
 
         ratio, CH4 = GC._gasifier_prod_spec(C_cont, H_cont, O_cont, N_cont, moist_cont, ash)
 
         return agent_ratio, ratio, CH4
 
     @staticmethod
     def _agent_ratio(C_mole, H_mole, O_mole, moist):
         """
-        Calculates the mass ratio of gasifying agent to feedstock
+        Calculates the mass ratio of gasifying agent to feedstock.
         """
-        ratio = (47.056 * C_mole
-                 + 14.687 * H_mole
-                 - 21.327 * O_mole
-                 + 0.957 * moist)
+        ratio = 47.056 * C_mole + 14.687 * H_mole - 21.327 * O_mole + 0.957 * moist
         return ratio
 
     @staticmethod
     def _gasifier_prod_spec(C_mole, H_mole, O_mole, N_mole, moist, ash):
         """
-        Calculates the H2/CO and CH4 in the gasifier products
+        Calculates the H2/CO and CH4 in the gasifier products.
         """
-        ratio = (2.038698561 * ash
-                 - 157.4311171 * C_mole
-                 - 41.41348052 * H_mole
-                 + 33.9749132 * N_mole
-                 + 106.660806 * O_mole
-                 + 0.940837584 * (O_mole / C_mole)
-                 + 0.862032712 * (O_mole / H_mole)
-                 - 2.578002065 * (O_mole / (C_mole + H_mole / 4))
-                 - 0.568261819 * (C_mole / H_mole)
-                 - 3.2554175 * moist)
+        ratio = (
+            2.038698561 * ash
+            - 157.4311171 * C_mole
+            - 41.41348052 * H_mole
+            + 33.9749132 * N_mole
+            + 106.660806 * O_mole
+            + 0.940837584 * (O_mole / C_mole)
+            + 0.862032712 * (O_mole / H_mole)
+            - 2.578002065 * (O_mole / (C_mole + H_mole / 4))
+            - 0.568261819 * (C_mole / H_mole)
+            - 3.2554175 * moist
+        )
 
         if ratio <= 0:
-            raise ValueError('Ratio of H2/CO cannot be negative! Check _gasifier_prod_spec method')
+            raise ValueError("Ratio of H2/CO cannot be negative! Check _gasifier_prod_spec method")
 
-        CH4 = (- 0.00001681 * ash
-               + 0.001043993 * C_mole
-               + 0.000369682 * H_mole
-               - 0.000209205 * N_mole
-               - 0.000907571 * O_mole
-               + 7.58E-06 * (C_mole / O_mole)
-               - 7.95E-06 * (O_mole / H_mole)
-               + 1.31E-05 * (O_mole / (C_mole + H_mole / 4))
-               + 7.46E-06 * (C_mole / H_mole)
-               + 2.11E-05 * moist)
+        CH4 = (
+            -0.00001681 * ash
+            + 0.001043993 * C_mole
+            + 0.000369682 * H_mole
+            - 0.000209205 * N_mole
+            - 0.000907571 * O_mole
+            + 7.58e-06 * (C_mole / O_mole)
+            - 7.95e-06 * (O_mole / H_mole)
+            + 1.31e-05 * (O_mole / (C_mole + H_mole / 4))
+            + 7.46e-06 * (C_mole / H_mole)
+            + 2.11e-05 * moist
+        )
 
         CH4 = 0 if CH4 <= 0 else CH4
         return ratio, CH4
 
+    @staticmethod
     def _gasifier_products(C_mole, H_mole, O_mole, N_mol, CH4_mole, ratio, moist_mole):
         """
-        Calculates the syngas
+        Calculates the syngas.
         """
         CO_mole = (4 * C_mole - 8 * CH4_mole - 2 * O_mole + H_mole) / (2 + 2 * ratio)
         if CO_mole > C_mole:
-            raise Exception("More CO is produced than the incoming C!")
+            raise ValueError("More CO is produced than the incoming C!")
 
         CO2_mole = C_mole - CO_mole - CH4_mole
         if CO2_mole < 0:
-            raise Exception("Error in C balance: The CO and CH4 are more than incoming C!")
+            raise ValueError("Error in C balance: The CO and CH4 are more than incoming C!")
 
         H2_mole = CO_mole * ratio
         if H2_mole * 2 + CH4_mole * 4 > H_mole:
-            raise Exception("Error in H balance")
+            raise ValueError("Error in H balance")
 
         N2_mole = N_mol / 2
 
         H2O_mole = (H_mole - 4 * CH4_mole - 2 * H2_mole + 2 * moist_mole) / 2
         if H2O_mole < 0:
-            raise Exception("Error in water balance or H balance!")
+            raise ValueError("Error in water balance or H balance!")
         return CO_mole, CO2_mole, H2_mole, N2_mole, H2O_mole
 
     def _stack_vol_flow(self):
         """
         Calculate the exhaust flow @ 7% oxygen
         """
-        alpha = (0.535 * self.gasifier_products.loc['CO', 'value']
-                 + 0.07 * self.gasifier_products.loc['CO2', 'value']
-                 + 0.465 * self.gasifier_products.loc['H2', 'value']
-                 - 0.1625 * self._dry_rdf.loc['Cl_mole_react', 'value']
-                 + 0.035 * self._dry_rdf.loc['N_mole_react', 'value']
-                 + 0.07 * self.gasifier_products.loc['N2', 'value']
-                 + self._dry_rdf.loc['S_mole_react', 'value']) / 0.6654
-
-        O2_exhaust = (-self.gasifier_products.loc['CO', 'value'] / 2
-                      + alpha
-                      + self._dry_rdf.loc['Cl_mole_react', 'value'] / 4
-                      - self.gasifier_products.loc['H2', 'value'] / 2
-                      - self._dry_rdf.loc['S_mole_react', 'value'])
-        HCl_exhaust = self._dry_rdf.loc['Cl_mole_react', 'value']
-        N2_exhaust = (self._dry_rdf.loc['N_mole_react', 'value'] / 2
-                      + self.gasifier_products.loc['N2', 'value']
-                      + 3.78 * alpha)
-        SO2_exhaust = self._dry_rdf.loc['S_mole_react', 'value']
-        CO2_exhaust = (self.gasifier_products.loc['CO', 'value']
-                       + self.gasifier_products.loc['CO2', 'value'])
-        vol_flow = ((O2_exhaust + HCl_exhaust
-                     + N2_exhaust + SO2_exhaust
-                     + CO2_exhaust)
-                    * self.CommonData.STP['mole_to_L']['amount']
-                    / 1000 * 10**6)
+        alpha = (
+            0.535 * self.gasifier_products.loc["CO", "value"]
+            + 0.07 * self.gasifier_products.loc["CO2", "value"]
+            + 0.465 * self.gasifier_products.loc["H2", "value"]
+            - 0.1625 * self._dry_rdf.loc["Cl_mole_react", "value"]
+            + 0.035 * self._dry_rdf.loc["N_mole_react", "value"]
+            + 0.07 * self.gasifier_products.loc["N2", "value"]
+            + self._dry_rdf.loc["S_mole_react", "value"]
+        ) / 0.6654
+
+        O2_exhaust = (
+            -self.gasifier_products.loc["CO", "value"] / 2
+            + alpha
+            + self._dry_rdf.loc["Cl_mole_react", "value"] / 4
+            - self.gasifier_products.loc["H2", "value"] / 2
+            - self._dry_rdf.loc["S_mole_react", "value"]
+        )
+        HCl_exhaust = self._dry_rdf.loc["Cl_mole_react", "value"]
+        N2_exhaust = (
+            self._dry_rdf.loc["N_mole_react", "value"] / 2
+            + self.gasifier_products.loc["N2", "value"]
+            + 3.78 * alpha
+        )
+        SO2_exhaust = self._dry_rdf.loc["S_mole_react", "value"]
+        CO2_exhaust = (
+            self.gasifier_products.loc["CO", "value"] + self.gasifier_products.loc["CO2", "value"]
+        )
+        vol_flow = (
+            (O2_exhaust + HCl_exhaust + N2_exhaust + SO2_exhaust + CO2_exhaust)
+            * self.CommonData.STP["mole_to_L"]["amount"]
+            / 1000
+            * 10**6
+        )
         return vol_flow
 
     def _biosphere_flows(self):
         """
         Calculate the flows to environment (emissions)
         """
-        bio_flows = dict()
+        bio_flows = {}
 
         # CO2 emissions from combustion and gasification
-        bio_flows['CO2'] = (
-            (self.gasifier_products.loc['CO2', 'value']
-             + self.gasifier_products.loc['CO', 'value']
-             + self.gasifier_products.loc['CH4', 'value'])
-            * self.CommonData.MW['CO2']['amount'] * 1000)
-        bio_flows['CO2_fossil'] = bio_flows['CO2'] * (1 - self._dry_rdf.loc['frac_biogenic_C', 'value'])
-        bio_flows['CO2_biogenic'] = bio_flows['CO2'] * self._dry_rdf.loc['frac_biogenic_C', 'value']
+        bio_flows["CO2"] = (
+            (
+                self.gasifier_products.loc["CO2", "value"]
+                + self.gasifier_products.loc["CO", "value"]
+                + self.gasifier_products.loc["CH4", "value"]
+            )
+            * self.CommonData.MW["CO2"]["amount"]
+            * 1000
+        )
+        bio_flows["CO2_fossil"] = bio_flows["CO2"] * (
+            1 - self._dry_rdf.loc["frac_biogenic_C", "value"]
+        )
+        bio_flows["CO2_biogenic"] = bio_flows["CO2"] * self._dry_rdf.loc["frac_biogenic_C", "value"]
 
         # Carbon storage: unreacted carbon
-        bio_flows['CO2_storage_biogenic'] = (
-            (self._dry_rdf.loc['C_mole', 'value']
-             - self._dry_rdf.loc['C_mole_react', 'value'])
-            * self.CommonData.MW['CO2']['amount'] * 1000
+        bio_flows["CO2_storage_biogenic"] = (
+            (self._dry_rdf.loc["C_mole", "value"] - self._dry_rdf.loc["C_mole_react", "value"])
+            * self.CommonData.MW["CO2"]["amount"]
+            * 1000
             * (-1)
-            * self._dry_rdf.loc['frac_biogenic_C', 'value'])
+            * self._dry_rdf.loc["frac_biogenic_C", "value"]
+        )
 
         # Stack emissions based on average concentration
         vol_flow = self._stack_vol_flow()
-        for i in ['PM', 'HCl', 'NOx', 'SOx']:
-            bio_flows[i] = (vol_flow
-                            * self.InputData.Stack[i]['amount']
-                            / 10**6)
-
-        bio_flows['Dioxins_Furans'] = (
-            vol_flow
-            * self.InputData.Stack['Dioxins_Furans']['amount']
-            / 10**12)
+        for i in ["PM", "HCl", "NOx", "SOx"]:
+            bio_flows[i] = vol_flow * self.InputData.Stack[i]["amount"] / 10**6
+
+        bio_flows["Dioxins_Furans"] = (
+            vol_flow * self.InputData.Stack["Dioxins_Furans"]["amount"] / 10**12
+        )
 
         # Metal emissions from stack based on fraction incoming metals
-        for element in ['Arsenic', 'Barium', 'Cadmium', 'Chromium', 'Copper',
-                        'Mercury', 'Nickel', 'Lead', 'Antimony', 'Selenium',
-                        'Zinc', 'Silver']:
-            bio_flows[element] = sum(self._input_rdf['solid']
-                                     * self.Material_Properties[element]
-                                     / 100) * 1000 * self.InputData.Stack[element]['amount']
+        for element in [
+            "Arsenic",
+            "Barium",
+            "Cadmium",
+            "Chromium",
+            "Copper",
+            "Mercury",
+            "Nickel",
+            "Lead",
+            "Antimony",
+            "Selenium",
+            "Zinc",
+            "Silver",
+        ]:
+            bio_flows[element] = (
+                sum(self._input_rdf["solid"] * self.Material_Properties[element] / 100)
+                * 1000
+                * self.InputData.Stack[element]["amount"]
+            )
         return bio_flows
 
     def _calc_cost(self):
         self.cost = {}
-        self.cost[('biosphere3', 'Capital_Cost')] = -npf.pmt(rate=self.InputData.Economic_params[' Interest_rate']['amount'],
-                                                             nper=self.InputData.Economic_params['lifetime']['amount'],
-                                                             pv=self.InputData.Economic_params['capital_cost']['amount'])
-        self.cost[('biosphere3', 'Operational_Cost')] = self.InputData.Economic_params['O&M_cost']['amount']
+        self.cost[("biosphere3", "Capital_Cost")] = -npf.pmt(
+            rate=self.InputData.Economic_params[" Interest_rate"]["amount"],
+            nper=self.InputData.Economic_params["lifetime"]["amount"],
+            pv=self.InputData.Economic_params["capital_cost"]["amount"],
+        )
+        self.cost[("biosphere3", "Operational_Cost")] = self.InputData.Economic_params["O&M_cost"][
+            "amount"
+        ]
 
     def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
 
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
         self.calc()
@@ -479,44 +593,78 @@
         Biosphere = {}
         self.GC["process name"] = (self.process_name, self.Process_Type, self.__class__)
         self.GC["Waste"] = Waste
         self.GC["Technosphere"] = Technosphere
         self.GC["Biosphere"] = Biosphere
 
         bio_dict = {
-            'CO2_fossil': ('biosphere3', '349b29d1-3e58-4c66-98b9-9d1a076efd2e'),  # 'Carbon dioxide, fossil' ('air')
-            'CO2_biogenic': ('biosphere3', 'eba59fd6-f37e-41dc-9ca3-c7ea22d602c7'),  #  'Carbon dioxide, non-fossil' ('air')
-            'CO2_storage_biogenic': ('biosphere3', 'e4e9febc-07c1-403d-8d3a-6707bb4d96e6'),  # 'Carbon dioxide, from soil or biomass stock' ('air')
-            'PM': ('biosphere3', '21e46cb8-6233-4c99-bac3-c41d2ab99498'),  # 'Particulates, < 2.5 um' ('air')
-            'HCl': ('biosphere3', 'c941d6d0-a56c-4e6c-95de-ac685635218d'),  # 'Hydrogen chloride' ('air')
-            'NOx': ('biosphere3', 'c1b91234-6f24-417b-8309-46111d09c457'),  # 'Nitrogen oxides' ('air')
-            'SOx': ('biosphere3', 'ba5fc0b6-770b-4da1-9b3f-e3b5087f07cd'),  # 'Sulfur oxides' ('air')
-            'Dioxins_Furans': ('biosphere3', '082903e4-45d8-4078-94cb-736b15279277'),  # 'Dioxins, measured as 2,3,7,8-tetrachlorodibenzo-p-dioxin' ('air')
-            'Arsenic': ('biosphere3', 'dc6dbdaa-9f13-43a8-8af5-6603688c6ad0'),  # 'Arsenic' ('air')
-            'Barium': ('biosphere3', '7e246e3a-5cff-43fc-a8e6-02d191424559'),  # 'Barium' ('air')
-            'Cadmium': ('biosphere3', '1c5a7322-9261-4d59-a692-adde6c12de92'),  # 'Cadmium' ('air')
-            'Chromium': ('biosphere3', 'e142b577-e934-4085-9a07-3983d4d92afb'),  # 'Chromium' ('air')
-            'Copper': ('biosphere3', 'ec8144d6-d123-43b1-9c17-a295422a0498'),  # 'Copper' ('air')
-            'Mercury': ('biosphere3', '71234253-b3a7-4dfe-b166-a484ad15bee7'),  # 'Mercury' ('air')
-            'Nickel': ('biosphere3', 'a5506f4b-113f-4713-95c3-c819dde6e48b'),  # 'Nickel' ('air')
-            'Lead': ('biosphere3', '8e123669-94d3-41d8-9480-a79211fe7c43'),  # 'Lead' ('air')
-            'Antimony': ('biosphere3', '77927dac-dea3-429d-a434-d5a71d92c4f7'),  # 'Antimony' ('air')
-            'Selenium': ('biosphere3', '454c61fd-c52b-4a04-9731-f141bb7b5264'),  # 'Selenium' ('air')
-            'Zinc': ('biosphere3', '5ce378a0-b48d-471c-977d-79681521efde'),  # 'Zinc' ('air')
-            'Silver': ('biosphere3', '7da45a0b-0dcf-413c-8de0-44d8ebca9e6e'),  # 'Silver' ('soil')
+            "CO2_fossil": (
+                "biosphere3",
+                "349b29d1-3e58-4c66-98b9-9d1a076efd2e",
+            ),  # 'Carbon dioxide, fossil' ('air')
+            "CO2_biogenic": (
+                "biosphere3",
+                "eba59fd6-f37e-41dc-9ca3-c7ea22d602c7",
+            ),  #  'Carbon dioxide, non-fossil' ('air')
+            "CO2_storage_biogenic": (
+                "biosphere3",
+                "e4e9febc-07c1-403d-8d3a-6707bb4d96e6",
+            ),  # 'Carbon dioxide, from soil or biomass stock' ('air')
+            "PM": (
+                "biosphere3",
+                "21e46cb8-6233-4c99-bac3-c41d2ab99498",
+            ),  # 'Particulates, < 2.5 um' ('air')
+            "HCl": (
+                "biosphere3",
+                "c941d6d0-a56c-4e6c-95de-ac685635218d",
+            ),  # 'Hydrogen chloride' ('air')
+            "NOx": (
+                "biosphere3",
+                "c1b91234-6f24-417b-8309-46111d09c457",
+            ),  # 'Nitrogen oxides' ('air')
+            "SOx": (
+                "biosphere3",
+                "ba5fc0b6-770b-4da1-9b3f-e3b5087f07cd",
+            ),  # 'Sulfur oxides' ('air')
+            "Dioxins_Furans": (
+                "biosphere3",
+                "082903e4-45d8-4078-94cb-736b15279277",
+            ),  # 'Dioxins, measured as 2,3,7,8-tetrachlorodibenzo-p-dioxin' ('air')
+            "Arsenic": ("biosphere3", "dc6dbdaa-9f13-43a8-8af5-6603688c6ad0"),  # 'Arsenic' ('air')
+            "Barium": ("biosphere3", "7e246e3a-5cff-43fc-a8e6-02d191424559"),  # 'Barium' ('air')
+            "Cadmium": ("biosphere3", "1c5a7322-9261-4d59-a692-adde6c12de92"),  # 'Cadmium' ('air')
+            "Chromium": (
+                "biosphere3",
+                "e142b577-e934-4085-9a07-3983d4d92afb",
+            ),  # 'Chromium' ('air')
+            "Copper": ("biosphere3", "ec8144d6-d123-43b1-9c17-a295422a0498"),  # 'Copper' ('air')
+            "Mercury": ("biosphere3", "71234253-b3a7-4dfe-b166-a484ad15bee7"),  # 'Mercury' ('air')
+            "Nickel": ("biosphere3", "a5506f4b-113f-4713-95c3-c819dde6e48b"),  # 'Nickel' ('air')
+            "Lead": ("biosphere3", "8e123669-94d3-41d8-9480-a79211fe7c43"),  # 'Lead' ('air')
+            "Antimony": (
+                "biosphere3",
+                "77927dac-dea3-429d-a434-d5a71d92c4f7",
+            ),  # 'Antimony' ('air')
+            "Selenium": (
+                "biosphere3",
+                "454c61fd-c52b-4a04-9731-f141bb7b5264",
+            ),  # 'Selenium' ('air')
+            "Zinc": ("biosphere3", "5ce378a0-b48d-471c-977d-79681521efde"),  # 'Zinc' ('air')
+            "Silver": ("biosphere3", "7da45a0b-0dcf-413c-8de0-44d8ebca9e6e"),  # 'Silver' ('soil')
         }
-        Biosphere['RDF'] = {}
+        Biosphere["RDF"] = {}
         for k, v in self.bio_flows.items():
             if k in bio_dict:
-                Biosphere['RDF'][bio_dict[k]] = v
+                Biosphere["RDF"][bio_dict[k]] = v
 
         for k, v in self.cost.items():
-            Biosphere['RDF'][k] = v
-
-        Technosphere['RDF'] = {}
-        Technosphere['RDF'][('Technosphere', 'Electricity_production')] = self.energy.loc['Net Elec prod', 'value']
+            Biosphere["RDF"][k] = v
 
+        Technosphere["RDF"] = {}
+        Technosphere["RDF"][("Technosphere", "Electricity_production")] = self.energy.loc[
+            "Net Elec prod", "value"
+        ]
 
-        Waste['RDF'] = {}
-        Waste['RDF']['Bottom_Ash'] = self.gasifier_products.loc['Bottom Ash', 'value']
+        Waste["RDF"] = {}
+        Waste["RDF"]["Bottom_Ash"] = self.gasifier_products.loc["Bottom Ash", "value"]
 
         return self.GC
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/HC_subprocess.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/HC_subprocess.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,94 +1,118 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Jun 14 15:07:13 2021
-
-@author: m.sardar
-"""
 from .Common_subprocess import Flow
 
 
 ### Active Composting
-def active_comp(input_flow, common_data, input_data ,process_data, material_properties, lci):
+def active_comp(input_flow, common_data, input_data, process_data, material_properties, lci):
     # Calculate organic C and N content
-    input_flow.data['C_cont'] = (input_flow.data['sol_cont'].values
-                                  * material_properties['Biogenic Carbon Content'].values / 100
-                                  * process_data['Degrades'].values)
-
-    input_flow.data['N_cont'] = (input_flow.data['sol_cont'].values
-                                  * material_properties['Nitrogen Content'].values / 100
-                                  * process_data['Degrades'].values)
-
-    input_flow.data['P_cont'] = (input_flow.data['sol_cont'].values
-                                  * material_properties['Phosphorus Content'].values / 100
-                                  * process_data['Degrades'].values)
-
-    input_flow.data['K_cont'] = (input_flow.data['sol_cont'].values
-                                  * material_properties['Potassium Content'].values / 100
-                                  * process_data['Degrades'].values)
+    input_flow.data["C_cont"] = (
+        input_flow.data["sol_cont"].values
+        * material_properties["Biogenic Carbon Content"].values
+        / 100
+        * process_data["Degrades"].values
+    )
+
+    input_flow.data["N_cont"] = (
+        input_flow.data["sol_cont"].values
+        * material_properties["Nitrogen Content"].values
+        / 100
+        * process_data["Degrades"].values
+    )
+
+    input_flow.data["P_cont"] = (
+        input_flow.data["sol_cont"].values
+        * material_properties["Phosphorus Content"].values
+        / 100
+        * process_data["Degrades"].values
+    )
+
+    input_flow.data["K_cont"] = (
+        input_flow.data["sol_cont"].values
+        * material_properties["Potassium Content"].values
+        / 100
+        * process_data["Degrades"].values
+    )
 
     # Degradation
-    C_loss = (input_flow.data['C_cont'].values
-              * process_data['C_loss'].values / 100
-              * input_data.Degradation_param['acDegProp']['amount'] / 100)
-
-    N_loss = (input_flow.data['N_cont'].values
-              * process_data['N_loss'].values / 100
-              * input_data.Degradation_param['acDegProp']['amount'] / 100)
+    C_loss = (
+        input_flow.data["C_cont"].values
+        * process_data["C_loss"].values
+        / 100
+        * input_data.Degradation_param["acDegProp"]["amount"]
+        / 100
+    )
+
+    N_loss = (
+        input_flow.data["N_cont"].values
+        * process_data["N_loss"].values
+        / 100
+        * input_data.Degradation_param["acDegProp"]["amount"]
+        / 100
+    )
 
-    VS_loss = C_loss * process_data['VS_loss to C_loss'].values
+    VS_loss = C_loss * process_data["VS_loss to C_loss"].values
 
-    VOCs_loss = VS_loss * process_data['VOC to VS_loss'].values / 10**6
+    VOCs_loss = VS_loss * process_data["VOC to VS_loss"].values / 10**6
 
     # Product: Final compost
     product = Flow(material_properties)
-    product.data['vs_cont'] = input_flow.data['vs_cont'].values - VS_loss
-    product.data['ash_cont'] = input_flow.data['ash_cont'].values
-    product.data['sol_cont'] = product.data['vs_cont'].values + product.data['ash_cont'].values
+    product.data["vs_cont"] = input_flow.data["vs_cont"].values - VS_loss
+    product.data["ash_cont"] = input_flow.data["ash_cont"].values
+    product.data["sol_cont"] = product.data["vs_cont"].values + product.data["ash_cont"].values
     # L = S / (1-Mc) * Mc
-    product.data['moist_cont'] = (product.data['sol_cont'].values
-                                  / (1 - input_data.Degradation_param['MCac']['amount'])
-                                  * input_data.Degradation_param['MCac']['amount'])
-    product.data['mass'] = product.data['sol_cont'].values + product.data['moist_cont'].values
-    product.data['C_cont']= input_flow.data['C_cont'].values - C_loss
-    product.data['N_cont']= input_flow.data['N_cont'].values - N_loss
-    product.data['P_cont']= input_flow.data['P_cont'].values
-    product.data['K_cont']= input_flow.data['K_cont'].values
+    product.data["moist_cont"] = (
+        product.data["sol_cont"].values
+        / (1 - input_data.Degradation_param["MCac"]["amount"])
+        * input_data.Degradation_param["MCac"]["amount"]
+    )
+    product.data["mass"] = product.data["sol_cont"].values + product.data["moist_cont"].values
+    product.data["C_cont"] = input_flow.data["C_cont"].values - C_loss
+    product.data["N_cont"] = input_flow.data["N_cont"].values - N_loss
+    product.data["P_cont"] = input_flow.data["P_cont"].values
+    product.data["K_cont"] = input_flow.data["K_cont"].values
 
     # C losses fate
-    C_loss_as_CH4 = C_loss * input_data.Degradation_param['pCasCH4']['amount']
-    C_loss_as_CO = C_loss * input_data.Degradation_param['pCasCO']['amount']
+    C_loss_as_CH4 = C_loss * input_data.Degradation_param["pCasCH4"]["amount"]
+    C_loss_as_CO = C_loss * input_data.Degradation_param["pCasCO"]["amount"]
     C_loss_as_CO2 = C_loss - C_loss_as_CH4 - C_loss_as_CO
 
-    lci.add(name='Carbon dioxide, non-fossil',
-            flow=(C_loss_as_CO2
-                  * common_data.MW['CO2']['amount'] / common_data.MW['C']['amount']))
-
-    lci.add(name='Methane, non-fossil',
-            flow=(C_loss_as_CH4
-                  * common_data.MW['CH4']['amount'] / common_data.MW['C']['amount']))
-
-    lci.add(name='Carbon monoxide, non-fossil',
-            flow=(C_loss_as_CO
-                  * common_data.MW['CO']['amount'] / common_data.MW['C']['amount']))
+    lci.add(
+        name="Carbon dioxide, non-fossil",
+        flow=(C_loss_as_CO2 * common_data.MW["CO2"]["amount"] / common_data.MW["C"]["amount"]),
+    )
+
+    lci.add(
+        name="Methane, non-fossil",
+        flow=(C_loss_as_CH4 * common_data.MW["CH4"]["amount"] / common_data.MW["C"]["amount"]),
+    )
+
+    lci.add(
+        name="Carbon monoxide, non-fossil",
+        flow=(C_loss_as_CO * common_data.MW["CO"]["amount"] / common_data.MW["C"]["amount"]),
+    )
 
     # N losses fate
-    N_loss_as_NH3 = N_loss * input_data.Degradation_param['pNasNH3']['amount']
-    N_loss_as_N2O = N_loss * input_data.Degradation_param['pNasN2O']['amount']
+    N_loss_as_NH3 = N_loss * input_data.Degradation_param["pNasNH3"]["amount"]
+    N_loss_as_N2O = N_loss * input_data.Degradation_param["pNasN2O"]["amount"]
     N_loss_as_N2 = N_loss - N_loss_as_NH3 - N_loss_as_N2O
 
-    lci.add(name='Ammonia',
-            flow=(N_loss_as_NH3
-                  * common_data.MW['Ammonia']['amount'] / common_data.MW['N']['amount']))
-
-    lci.add(name='Dinitrogen monoxide',
-            flow=(N_loss_as_N2O
-                  * common_data.MW['Nitrous_Oxide']['amount']
-                  / (common_data.MW['N']['amount'] * 2)))
+    lci.add(
+        name="Ammonia",
+        flow=(N_loss_as_NH3 * common_data.MW["Ammonia"]["amount"] / common_data.MW["N"]["amount"]),
+    )
+
+    lci.add(
+        name="Dinitrogen monoxide",
+        flow=(
+            N_loss_as_N2O
+            * common_data.MW["Nitrous_Oxide"]["amount"]
+            / (common_data.MW["N"]["amount"] * 2)
+        ),
+    )
 
-    lci.add(name='Nitrogen',
-            flow=N_loss_as_N2)
+    lci.add(name="Nitrogen", flow=N_loss_as_N2)
 
     # VOCs
-    lci.add(name='VOCs emitted', flow=VOCs_loss)
+    lci.add(name="VOCs emitted", flow=VOCs_loss)
 
-    return(product)
+    return product
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/LF.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/LF.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,774 +1,995 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Tue Aug 13 11:07:56 2019
+from copy import deepcopy
 
-@author: msardar2
-"""
 import numpy as np
 import pandas as pd
-from .ProcessModel import ProcessModel
 from swolfpy_inputdata import LF_Input
-from copy import deepcopy
+
+from .ProcessModel import ProcessModel
 
 
 class LF(ProcessModel):
-    Process_Type = 'Treatment'
-    def __init__(self, process_name='LF', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Treatment"
+
+    def __init__(self, process_name="LF", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = LF_Input(input_data_path,
-                                 process_name=self.process_name,
-                                 CommonDataObjct=CommonDataObjct)
+        self.InputData = LF_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
         self.process_data = self.InputData.process_data
 
         self.gas_emission_factor = self.InputData.gas_emission_factor
 
         self.lcht_Qlty = self.InputData.lcht_Qlty
 
         self.GasColPlan = self.InputData.GasColPlan
 
         self.timescale = 301
 
     # Landfill Gas Collection Efficiency
     def _Cal_LFG_Col_Ox(self):
-        self._n = int(self.InputData.LF_Op['optime']['amount'])
+        self._n = int(self.InputData.LF_Op["optime"]["amount"])
 
-        self._plan = {0: 'Typical',
-                      1: 'Best Case',
-                      2: 'Worst Case',
-                      3: 'California'}[self.InputData.LFG_param['LFG_col_plan']['amount']]
+        self._plan = {0: "Typical", 1: "Best Case", 2: "Worst Case", 3: "California"}[
+            self.InputData.LFG_param["LFG_col_plan"]["amount"]
+        ]
 
         # Parameters for LF operation (timing for LFG collection)
         index_n = np.arange(self._n)
         index_t = np.arange(self.timescale)
         self._param1 = pd.DataFrame(index=index_n)
 
         # Parameters for LF operation (timing for LFG collection)
-        t = (self.GasColPlan.loc['initColTime', self._plan]
-             - np.mod(index_n, self.GasColPlan.loc['cellFillTime', self._plan]))
+        t = self.GasColPlan.loc["initColTime", self._plan] - np.mod(
+            index_n, self.GasColPlan.loc["cellFillTime", self._plan]
+        )
         t[t < 0] = 0
-        self._param1['Time to initial collection'] = t
+        self._param1["Time to initial collection"] = t
 
-        self._param1['Time to interim cover'] = (
-            self.GasColPlan.loc['cellFillTime', self._plan]
-            - np.mod(index_n, self.GasColPlan.loc['cellFillTime', self._plan]))
-
-        self._param1['Time to long term cover'] = (
-            self.GasColPlan.loc['incColTime', self._plan]
-            - np.mod(index_n, self.GasColPlan.loc['cellFillTime', self._plan]))
+        self._param1["Time to interim cover"] = self.GasColPlan.loc[
+            "cellFillTime", self._plan
+        ] - np.mod(index_n, self.GasColPlan.loc["cellFillTime", self._plan])
+
+        self._param1["Time to long term cover"] = self.GasColPlan.loc[
+            "incColTime", self._plan
+        ] - np.mod(index_n, self.GasColPlan.loc["cellFillTime", self._plan])
 
         self.LFG_Coll_Eff = np.zeros((self.timescale, self._n))
 
-        xx, yy = np.mgrid[0:self.timescale, 0:self._n]
-        filter_FCover = xx + yy >= self.GasColPlan.loc['timeToFinCover', self._plan] + self.InputData.LF_Op['optime']['amount']
-        filter_IncCover = xx >= self._param1['Time to long term cover'].values
-        filter_IntCover = xx >= self._param1['Time to interim cover'].values
-        filter_InitCover = xx >= self._param1['Time to initial collection'].values
-
-        self.LFG_Coll_Eff[filter_InitCover] = self.InputData.LFG_param['initColEff']['amount']
-        self.LFG_Coll_Eff[filter_IntCover] = self.InputData.LFG_param['intColEff']['amount']
-        self.LFG_Coll_Eff[filter_IncCover] = self.InputData.LFG_param['incColEff']['amount']
-        self.LFG_Coll_Eff[filter_FCover] = self.InputData.LFG_param['finColEff']['amount']
+        xx, yy = np.mgrid[0 : self.timescale, 0 : self._n]
+        filter_FCover = (
+            xx + yy
+            >= self.GasColPlan.loc["timeToFinCover", self._plan]
+            + self.InputData.LF_Op["optime"]["amount"]
+        )
+        filter_IncCover = xx >= self._param1["Time to long term cover"].values
+        filter_IntCover = xx >= self._param1["Time to interim cover"].values
+        filter_InitCover = xx >= self._param1["Time to initial collection"].values
+
+        self.LFG_Coll_Eff[filter_InitCover] = self.InputData.LFG_param["initColEff"]["amount"]
+        self.LFG_Coll_Eff[filter_IntCover] = self.InputData.LFG_param["intColEff"]["amount"]
+        self.LFG_Coll_Eff[filter_IncCover] = self.InputData.LFG_param["incColEff"]["amount"]
+        self.LFG_Coll_Eff[filter_FCover] = self.InputData.LFG_param["finColEff"]["amount"]
 
         self._potential_LFG = pd.DataFrame(index=index_t)
-        self._potential_LFG['Average Collection Eff'] = self.LFG_Coll_Eff.mean(axis=1)
-
-        k = self.InputData.LFG_param['actk']['amount']
+        self._potential_LFG["Average Collection Eff"] = self.LFG_Coll_Eff.mean(axis=1)
 
-        decay_rate = (self.InputData.LFG_param['base_L0']['amount']
-            * (np.e**(-k * index_t)
-               - np.e**(-k * np.arange(1, self.timescale + 1))))
+        k = self.InputData.LFG_param["actk"]["amount"]
 
-        dumped_waste = np.concatenate((np.full(self._n - 1, self.InputData.LF_Op['annWaste']['amount']),
-                                       np.full(self.timescale - self._n + 1, 0)))
+        decay_rate = self.InputData.LFG_param["base_L0"]["amount"] * (
+            np.e ** (-k * index_t) - np.e ** (-k * np.arange(1, self.timescale + 1))
+        )
+
+        dumped_waste = np.concatenate(
+            (
+                np.full(self._n - 1, self.InputData.LF_Op["annWaste"]["amount"]),
+                np.full(self.timescale - self._n + 1, 0),
+            )
+        )
 
         methane_gen = []
         methane_col = []
 
         for i in index_t:
-            methane_gen.append(sum(dumped_waste[i::-1] * decay_rate[0:i+1]))
+            methane_gen.append(sum(dumped_waste[i::-1] * decay_rate[0 : i + 1]))
             methane_col.append(
-                sum(dumped_waste[i::-1]
-                * decay_rate[0:i+1]
-                * self._potential_LFG['Average Collection Eff'].values[0:i+1] / 100))
-
-        lfg_cfm = (methane_col
-                   / self.InputData.LFG_param['ch4prop']['amount']
-                   / 365 / 24 / 60  # yr to min
-                   * 35.3147)  # m3 to ft3
-
-        NMOC_CutOn = (methane_gen
-                      / self.InputData.LFG_param['ch4prop']['amount']
-                      * 10**3  # m3 --> L
-                      * self.InputData.Flare['NMOC_Conc']['amount'] / 10**6  # ppmv
-                      / 0.08206  # L.atm --> K.mol
-                      / (273.15 + self.InputData.Flare['Temp']['amount'])
-                      * self.InputData.Flare['NMOC_MW']['amount']
-                      / 10**6)  # g --> Mg
-
-        NMOC_CutOff = (methane_col
-                      / self.InputData.LFG_param['ch4prop']['amount']
-                      * 10**3  # m3 --> L
-                      * self.InputData.Flare['NMOC_Conc_actual']['amount'] / 10**6  # ppmv
-                      / 0.08206  # L.atm --> K.mol
-                      / (273.15 + self.InputData.Flare['Temp']['amount'])
-                      * self.InputData.Flare['NMOC_MW']['amount']
-                      / 10**6)  # g --> Mg
-
-        self.GasColPlan.loc['enrgOn', self._plan] = 10000
-        self.GasColPlan.loc['enrgOff', self._plan] = 0
-        if self.InputData.Energy_Rec['enrgRecovered']['amount'] == 1:
-            lfg_ok = np.where(lfg_cfm >= self.InputData.Energy_Rec['MinFowRec']['amount'])[0]
+                sum(
+                    dumped_waste[i::-1]
+                    * decay_rate[0 : i + 1]
+                    * self._potential_LFG["Average Collection Eff"].values[0 : i + 1]
+                    / 100
+                )
+            )
+
+        lfg_cfm = (
+            methane_col
+            / self.InputData.LFG_param["ch4prop"]["amount"]
+            / 365
+            / 24
+            / 60  # yr to min
+            * 35.3147
+        )  # m3 to ft3
+
+        NMOC_CutOn = (
+            methane_gen
+            / self.InputData.LFG_param["ch4prop"]["amount"]
+            * 10**3  # m3 --> L
+            * self.InputData.Flare["NMOC_Conc"]["amount"]
+            / 10**6  # ppmv
+            / 0.08206  # L.atm --> K.mol
+            / (273.15 + self.InputData.Flare["Temp"]["amount"])
+            * self.InputData.Flare["NMOC_MW"]["amount"]
+            / 10**6
+        )  # g --> Mg
+
+        NMOC_CutOff = (
+            methane_col
+            / self.InputData.LFG_param["ch4prop"]["amount"]
+            * 10**3  # m3 --> L
+            * self.InputData.Flare["NMOC_Conc_actual"]["amount"]
+            / 10**6  # ppmv
+            / 0.08206  # L.atm --> K.mol
+            / (273.15 + self.InputData.Flare["Temp"]["amount"])
+            * self.InputData.Flare["NMOC_MW"]["amount"]
+            / 10**6
+        )  # g --> Mg
+
+        self.GasColPlan.loc["enrgOn", self._plan] = 10000
+        self.GasColPlan.loc["enrgOff", self._plan] = 0
+        if self.InputData.Energy_Rec["enrgRecovered"]["amount"] == 1:
+            lfg_ok = np.where(lfg_cfm >= self.InputData.Energy_Rec["MinFowRec"]["amount"])[0]
             if len(lfg_ok):
-                self.GasColPlan.loc['enrgOn', self._plan] = (
-                        lfg_ok[0] + self.InputData.Energy_Rec['RecInstallTime']['amount'])
-                lfg_low = np.where(lfg_cfm[lfg_ok[0]:] <= self.InputData.Energy_Rec['MinFowRec']['amount'])[0]
+                self.GasColPlan.loc["enrgOn", self._plan] = (
+                    lfg_ok[0] + self.InputData.Energy_Rec["RecInstallTime"]["amount"]
+                )
+                lfg_low = np.where(
+                    lfg_cfm[lfg_ok[0] :] <= self.InputData.Energy_Rec["MinFowRec"]["amount"]
+                )[0]
                 if len(lfg_low):
-                    if lfg_ok[0] + lfg_low[0] > (self.GasColPlan.loc['enrgOn', self._plan]
-                                                 + self.InputData.Energy_Rec['MinYrRec']['amount']):
-                        self.GasColPlan.loc['enrgOff', self._plan] = lfg_ok[0] + lfg_low[0]
+                    if lfg_ok[0] + lfg_low[0] > (
+                        self.GasColPlan.loc["enrgOn", self._plan]
+                        + self.InputData.Energy_Rec["MinYrRec"]["amount"]
+                    ):
+                        self.GasColPlan.loc["enrgOff", self._plan] = lfg_ok[0] + lfg_low[0]
                     else:
-                        self.GasColPlan.loc['enrgOff', self._plan] = (
-                            self.GasColPlan.loc['enrgOn', self._plan]
-                            + self.InputData.Energy_Rec['MinYrRec']['amount']
-                            + 1)
+                        self.GasColPlan.loc["enrgOff", self._plan] = (
+                            self.GasColPlan.loc["enrgOn", self._plan]
+                            + self.InputData.Energy_Rec["MinYrRec"]["amount"]
+                            + 1
+                        )
                 else:
-                   self.GasColPlan.loc['enrgOff', self._plan] = self.timescale
+                    self.GasColPlan.loc["enrgOff", self._plan] = self.timescale
 
-        self.GasColPlan.loc['flareOn', self._plan] = 10000
-        self.GasColPlan.loc['flareOff', self._plan] = (self.InputData.LF_Op['optime']['amount']
-                                                       + self.InputData.Flare['TimeReq']['amount'])
+        self.GasColPlan.loc["flareOn", self._plan] = 10000
+        self.GasColPlan.loc["flareOff", self._plan] = (
+            self.InputData.LF_Op["optime"]["amount"] + self.InputData.Flare["TimeReq"]["amount"]
+        )
 
-        NMOC_high = np.where(NMOC_CutOn >= self.InputData.Flare['NMOC_Cufoff']['amount'])[0]
+        NMOC_high = np.where(NMOC_CutOn >= self.InputData.Flare["NMOC_Cutoff"]["amount"])[0]
         if len(NMOC_high):
-            self.GasColPlan.loc['flareOn', self._plan] = NMOC_high[0]
-            self.GasColPlan.loc['flareOff', self._plan] = NMOC_high[0] + self.InputData.Flare['MinYr']['amount']
-            if self.GasColPlan.loc['flareOff', self._plan] < (self.InputData.LF_Op['optime']['amount']
-                                                              + self.InputData.Flare['TimeReq']['amount']):
-                self.GasColPlan.loc['flareOff', self._plan] = (
-                    self.InputData.LF_Op['optime']['amount']
-                    + self.InputData.Flare['TimeReq']['amount'])
-
-
-        if NMOC_CutOff[int(self.GasColPlan.loc['flareOff', self._plan])] > self.InputData.Flare['NMOC_Cufoff']['amount']:
-            NMOC_low = np.where(NMOC_CutOff[int(self.GasColPlan.loc['flareOff', self._plan] + 1):] <= self.InputData.Flare['NMOC_Cufoff']['amount'])[0]
+            self.GasColPlan.loc["flareOn", self._plan] = NMOC_high[0]
+            self.GasColPlan.loc["flareOff", self._plan] = (
+                NMOC_high[0] + self.InputData.Flare["MinYr"]["amount"]
+            )
+            if self.GasColPlan.loc["flareOff", self._plan] < (
+                self.InputData.LF_Op["optime"]["amount"] + self.InputData.Flare["TimeReq"]["amount"]
+            ):
+                self.GasColPlan.loc["flareOff", self._plan] = (
+                    self.InputData.LF_Op["optime"]["amount"]
+                    + self.InputData.Flare["TimeReq"]["amount"]
+                )
+
+        if (
+            NMOC_CutOff[int(self.GasColPlan.loc["flareOff", self._plan])]
+            > self.InputData.Flare["NMOC_Cutoff"]["amount"]
+        ):
+            NMOC_low = np.where(
+                NMOC_CutOff[int(self.GasColPlan.loc["flareOff", self._plan] + 1) :]
+                <= self.InputData.Flare["NMOC_Cutoff"]["amount"]
+            )[0]
             if len(NMOC_low):
-                self.GasColPlan.loc['flareOff', self._plan] +=  1 + NMOC_low[0]
+                self.GasColPlan.loc["flareOff", self._plan] += 1 + NMOC_low[0]
             else:
-                self.GasColPlan.loc['flareOff', self._plan] = self.timescale
+                self.GasColPlan.loc["flareOff", self._plan] = self.timescale
 
-        if self.InputData.Flare['Flow_cutoff']['amount']:
-            if lfg_cfm[int(self.GasColPlan.loc['flareOff', self._plan])] > self.InputData.Flare['Flow_req']['amount']:
-                NMOC_flow_low = np.where(lfg_cfm[int(self.GasColPlan.loc['flareOff', self._plan] + 1):] < self.InputData.Flare['Flow_req']['amount'])[0]
+        if self.InputData.Flare["Flow_cutoff"]["amount"]:
+            if (
+                lfg_cfm[int(self.GasColPlan.loc["flareOff", self._plan])]
+                > self.InputData.Flare["Flow_req"]["amount"]
+            ):
+                NMOC_flow_low = np.where(
+                    lfg_cfm[int(self.GasColPlan.loc["flareOff", self._plan] + 1) :]
+                    < self.InputData.Flare["Flow_req"]["amount"]
+                )[0]
                 if len(NMOC_flow_low):
-                    self.GasColPlan.loc['flareOff', self._plan] += 1 + NMOC_flow_low[0]
+                    self.GasColPlan.loc["flareOff", self._plan] += 1 + NMOC_flow_low[0]
                 else:
-                    self.GasColPlan.loc['flareOff', self._plan] = self.timescale
+                    self.GasColPlan.loc["flareOff", self._plan] = self.timescale
 
         # Report in DF
-        self._potential_LFG['waste Mg/year'] = dumped_waste
-        self._potential_LFG['Methane Generated m3/year'] = methane_gen
-        self._potential_LFG['Methane Collected m3/year'] = methane_col
-        self._potential_LFG['LFG Collected cfm'] = lfg_cfm
-        self._potential_LFG['NMOC CutOn Mg/yr'] = NMOC_CutOn
-        self._potential_LFG['NMOC CutOff Mg/yr'] = NMOC_CutOff
+        self._potential_LFG["waste Mg/year"] = dumped_waste
+        self._potential_LFG["Methane Generated m3/year"] = methane_gen
+        self._potential_LFG["Methane Collected m3/year"] = methane_col
+        self._potential_LFG["LFG Collected cfm"] = lfg_cfm
+        self._potential_LFG["NMOC CutOn Mg/yr"] = NMOC_CutOn
+        self._potential_LFG["NMOC CutOff Mg/yr"] = NMOC_CutOff
 
         # Collection efficiency
-        filter_Off = xx + yy >= max(self.GasColPlan.loc['enrgOff', self._plan], self.GasColPlan.loc['flareOff', self._plan])
+        filter_Off = xx + yy >= max(
+            self.GasColPlan.loc["enrgOff", self._plan], self.GasColPlan.loc["flareOff", self._plan]
+        )
         self.LFG_Coll_Eff[filter_Off] = 0
 
         # Oxidation
-        self._LFG_Ox_Eff = np.full((int(self.timescale), int(self._n)), self.InputData.Ox['ox_nocol']['amount'])
+        self._LFG_Ox_Eff = np.full(
+            (int(self.timescale), int(self._n)), self.InputData.Ox["ox_nocol"]["amount"]
+        )
+
+        self.filter_ox_1 = xx + yy >= max(
+            self.GasColPlan.loc["enrgOff", self._plan], self.GasColPlan.loc["flareOff", self._plan]
+        )
+        self.filter_ox_2 = self.LFG_Coll_Eff >= self.InputData.LFG_param["incColEff"]["amount"]
 
-        self.filter_ox_1 = xx + yy >= max(self.GasColPlan.loc['enrgOff', self._plan], self.GasColPlan.loc['flareOff', self._plan])
-        self.filter_ox_2 = self.LFG_Coll_Eff >= self.InputData.LFG_param['incColEff']['amount']
+        self._LFG_Ox_Eff[self.filter_ox_2] = self.InputData.Ox["ox_col"]["amount"]
+        self._LFG_Ox_Eff[self.filter_ox_1] = self.InputData.Ox["ox_fincov"]["amount"]
 
-        self._LFG_Ox_Eff[self.filter_ox_2] = self.InputData.Ox['ox_col']['amount']
-        self._LFG_Ox_Eff[self.filter_ox_1] = self.InputData.Ox['ox_fincov']['amount']
-
-        # calculating average collection and oxdiation
+        # calculating average collection and oxidation
         self.Average_Collection = pd.Series(self.LFG_Coll_Eff.mean(axis=1), index=index_t)
         self.Average_Oxidation = pd.Series(self._LFG_Ox_Eff.mean(axis=1), index=index_t)
 
     # Landfill Gas
     def _Cal_LFG(self):
         self.LCI = LCI(self.Index)
-        self._param2 = pd.DataFrame(index=self.Index) # LFG generation parameter
+        self._param2 = pd.DataFrame(index=self.Index)  # LFG generation parameter
         self.LFG = pd.DataFrame(index=self.Index)
         n_waste_fracs = len(self.Index)
 
         # LFG generation parameter
-        self._param2['k'] = (self.Material_Properties['Lab Decay Rate'].values / 156
-                             * self.InputData.LFG_param['actk']['amount'] / 0.04)
+        self._param2["k"] = (
+            self.Material_Properties["Lab Decay Rate"].values
+            / 156
+            * self.InputData.LFG_param["actk"]["amount"]
+            / 0.04
+        )
 
         # Methane Yield (m3/dry Mg)
-        self.Material_Properties['Methane Yield'] = (
-            self.Material_Properties['Biogenic Carbon Content'].values / 100
-            * self.Material_Properties['Ultimate Biogenic C Converted to Biogas'].values / 100
-            * self.CommonData.STP['mole_to_L']['amount']
-            / self.CommonData.MW['C']['amount']
-            * self.InputData.LFG_param['ch4prop']['amount']
-            * 1000)
+        self.Material_Properties["Methane Yield"] = (
+            self.Material_Properties["Biogenic Carbon Content"].values
+            / 100
+            * self.Material_Properties["Ultimate Biogenic C Converted to Biogas"].values
+            / 100
+            * self.CommonData.STP["mole_to_L"]["amount"]
+            / self.CommonData.MW["C"]["amount"]
+            * self.InputData.LFG_param["ch4prop"]["amount"]
+            * 1000
+        )
 
-        self._param2['L0'] = self.Material_Properties['Methane Yield'].values
+        self._param2["L0"] = self.Material_Properties["Methane Yield"].values
 
-        self._param2['solid Content'] = 1 - self.Material_Properties['Moisture Content'].values / 100
+        self._param2["solid Content"] = (
+            1 - self.Material_Properties["Moisture Content"].values / 100
+        )
 
         # Methane generation
-        self._Methan_gen_by_year = (
-            self._param2['L0'].values.reshape(n_waste_fracs, 1)
-            * self._param2['solid Content'].values.reshape(n_waste_fracs, 1)
-            * (np.e**(-self._param2['k'].values.reshape(n_waste_fracs, 1) * np.arange(self.timescale))
-               - np.e**(-self._param2['k'].values.reshape(n_waste_fracs, 1) * np.arange(1, self.timescale + 1))))
-
-        self.LFG['Total generated Methane'] = self._Methan_gen_by_year.sum(axis=1)
-
-        self.LFG['Fraction of L0 Generated'] = np.divide(
-            self.LFG['Total generated Methane'].values,
-            self._param2['L0'].values * self._param2['solid Content'].values,
+        self._Methane_gen_by_year = (
+            self._param2["L0"].values.reshape(n_waste_fracs, 1)
+            * self._param2["solid Content"].values.reshape(n_waste_fracs, 1)
+            * (
+                np.e
+                ** (-self._param2["k"].values.reshape(n_waste_fracs, 1) * np.arange(self.timescale))
+                - np.e
+                ** (
+                    -self._param2["k"].values.reshape(n_waste_fracs, 1)
+                    * np.arange(1, self.timescale + 1)
+                )
+            )
+        )
+
+        self.LFG["Total generated Methane"] = self._Methane_gen_by_year.sum(axis=1)
+
+        self.LFG["Fraction of L0 Generated"] = np.divide(
+            self.LFG["Total generated Methane"].values,
+            self._param2["L0"].values * self._param2["solid Content"].values,
             out=np.zeros(n_waste_fracs),
-            where=self._param2['L0'].values>0.0)
+            where=self._param2["L0"].values > 0.0,
+        )
 
         # Methane collected
-        self.LFG['Total Methane collected'] = np.multiply(self._Methan_gen_by_year,
-                                                          self.Average_Collection.values / 100).sum(axis=1)
-
-        self.LFG['Collection Eff'] = np.divide(
-            self.LFG['Total Methane collected'].values,
-            self.LFG['Total generated Methane'].values,
+        self.LFG["Total Methane collected"] = np.multiply(
+            self._Methane_gen_by_year, self.Average_Collection.values / 100
+        ).sum(axis=1)
+
+        self.LFG["Collection Eff"] = np.divide(
+            self.LFG["Total Methane collected"].values,
+            self.LFG["Total generated Methane"].values,
             out=np.zeros(n_waste_fracs),
-            where=self.LFG['Total generated Methane'].values>0.0)
+            where=self.LFG["Total generated Methane"].values > 0.0,
+        )
 
         # Blower electricity use
-        self.LFG['Blower electricity use'] = (
-            (self.LFG['Total Methane collected'].values / self.InputData.LF_gas['blwrPRRm3']['amount'])
-            * (self.InputData.LF_gas['blwrPerLoad']['amount'] / 100)
-            * (100 / self.InputData.LF_gas['blwrEff']['amount'])
-            * 24 * 356.25)
+        self.LFG["Blower electricity use"] = (
+            (
+                self.LFG["Total Methane collected"].values
+                / self.InputData.LF_gas["blwrPRRm3"]["amount"]
+            )
+            * (self.InputData.LF_gas["blwrPerLoad"]["amount"] / 100)
+            * (100 / self.InputData.LF_gas["blwrEff"]["amount"])
+            * 24
+            * 356.25
+        )
 
         # Adding Blower electricity use to LCI
-        self.LCI.add('Electricity_consumption', self.LFG['Blower electricity use'].values)
+        self.LCI.add("Electricity_consumption", self.LFG["Blower electricity use"].values)
 
         # Methane combustion for Energy
         frac_cob = np.zeros(self.timescale)
-        ii = np.mgrid[:self.timescale]
-        if self.InputData.Energy_Rec['enrgRecovered']['amount'] == 1:
+        ii = np.mgrid[: self.timescale]
+        if self.InputData.Energy_Rec["enrgRecovered"]["amount"] == 1:
             fltr = np.logical_and(
-                ii <= self.GasColPlan.loc['enrgOff', self._plan],
-                ii > self.GasColPlan.loc['enrgOn', self._plan])
-            frac_cob[fltr] = 1 - self.InputData.Energy_Rec['EnrgRecDownTime']['amount'] / 100
+                ii <= self.GasColPlan.loc["enrgOff", self._plan],
+                ii > self.GasColPlan.loc["enrgOn", self._plan],
+            )
+            frac_cob[fltr] = 1 - self.InputData.Energy_Rec["EnrgRecDownTime"]["amount"] / 100
 
         # Percent of generation that combusted
         comb_col = np.multiply(frac_cob, self.Average_Collection.values / 100)
-        self.LFG['Total Methane combusted'] = np.multiply(self._Methan_gen_by_year, comb_col).sum(axis=1)
-
-        self.LFG['Percent of Generated used for Energy'] = np.divide(
-            self.LFG['Total Methane combusted'].values,
-            self.LFG['Total generated Methane'].values,
-            out=np.zeros(n_waste_fracs),
-            where=self.LFG['Total generated Methane'].values>0.0) * 100
-
-        self.LFG['Percent of Collected used for Energy'] = np.divide(
-            self.LFG['Total Methane combusted'].values,
-            self.LFG['Total Methane collected'].values,
-            out=np.zeros(n_waste_fracs),
-            where=self.LFG['Total Methane collected'].values>0.0) * 100
+        self.LFG["Total Methane combusted"] = np.multiply(self._Methane_gen_by_year, comb_col).sum(
+            axis=1
+        )
+
+        self.LFG["Percent of Generated used for Energy"] = (
+            np.divide(
+                self.LFG["Total Methane combusted"].values,
+                self.LFG["Total generated Methane"].values,
+                out=np.zeros(n_waste_fracs),
+                where=self.LFG["Total generated Methane"].values > 0.0,
+            )
+            * 100
+        )
+
+        self.LFG["Percent of Collected used for Energy"] = (
+            np.divide(
+                self.LFG["Total Methane combusted"].values,
+                self.LFG["Total Methane collected"].values,
+                out=np.zeros(n_waste_fracs),
+                where=self.LFG["Total Methane collected"].values > 0.0,
+            )
+            * 100
+        )
 
         # Electricity generated
-        self.LFG['Electricity generated'] = (
-            self.LFG['Total Methane combusted'].values
-            * self.InputData.Energy_Rec['convEff']['amount']
-            * self.CommonData.LHV['CH4']['amount']
-            / 3.6)
+        self.LFG["Electricity generated"] = (
+            self.LFG["Total Methane combusted"].values
+            * self.InputData.Energy_Rec["convEff"]["amount"]
+            * self.CommonData.LHV["CH4"]["amount"]
+            / 3.6
+        )
 
         # Adding the generated electricity to LCI
-        self.LCI.add('Electricity_production', self.LFG['Electricity generated'].values)
+        self.LCI.add("Electricity_production", self.LFG["Electricity generated"].values)
 
         # Methane Sent to Flare  (Includes downtime but not methane destruction efficiency)
-        self.LFG['Total Methane flared'] = (
-            self.LFG['Total Methane collected'].values
-            - self.LFG['Total Methane combusted'].values)
+        self.LFG["Total Methane flared"] = (
+            self.LFG["Total Methane collected"].values - self.LFG["Total Methane combusted"].values
+        )
 
         # Methane Oxidized
         # Percent of generated that oxidized
-        oxd_colec = np.multiply(1 - self.Average_Collection.values / 100,
-                                self.Average_Oxidation.values / 100)
-
-        self.LFG['Total Methane oxidized'] = np.multiply(self._Methan_gen_by_year, oxd_colec).sum(axis=1)
+        oxd_colec = np.multiply(
+            1 - self.Average_Collection.values / 100, self.Average_Oxidation.values / 100
+        )
+
+        self.LFG["Total Methane oxidized"] = np.multiply(self._Methane_gen_by_year, oxd_colec).sum(
+            axis=1
+        )
 
         # Methane Emitted
-        self.LFG['Total Methane Emitted'] = (
-            self.LFG['Total generated Methane'].values
-            - self.LFG['Total Methane combusted'].values
-            * self.InputData.Energy_Rec['EngineCombEff']['amount'] / 100
-            - self.LFG['Total Methane flared'].values
-            * self.InputData.Flare['FlareCombEff']['amount'] / 100
-            - self.LFG['Total Methane oxidized'].values)
-
-        self.LFG['Percent of Generated Methane Emitted'] = np.divide(
-            self.LFG['Total Methane Emitted'].values,
-            self.LFG['Total generated Methane'].values,
-            out=np.zeros(n_waste_fracs),
-            where=self.LFG['Total generated Methane'].values>0.0) * 100
+        self.LFG["Total Methane Emitted"] = (
+            self.LFG["Total generated Methane"].values
+            - self.LFG["Total Methane combusted"].values
+            * self.InputData.Energy_Rec["EngineCombEff"]["amount"]
+            / 100
+            - self.LFG["Total Methane flared"].values
+            * self.InputData.Flare["FlareCombEff"]["amount"]
+            / 100
+            - self.LFG["Total Methane oxidized"].values
+        )
+
+        self.LFG["Percent of Generated Methane Emitted"] = (
+            np.divide(
+                self.LFG["Total Methane Emitted"].values,
+                self.LFG["Total generated Methane"].values,
+                out=np.zeros(n_waste_fracs),
+                where=self.LFG["Total generated Methane"].values > 0.0,
+            )
+            * 100
+        )
 
         # Mass of methane in uncollected biogas used to calculated the emissions
-        self.LFG['Total methane in uncollected biogas'] = (
-            self.LFG['Total generated Methane'].values
-            - self.LFG['Total Methane collected'].values)
+        self.LFG["Total methane in uncollected biogas"] = (
+            self.LFG["Total generated Methane"].values - self.LFG["Total Methane collected"].values
+        )
 
         # Emission factor: Emission to the air from venting, flaring and combustion of biogas
-        Biogas_factor = (self.gas_emission_factor['Concentration_ppmv'].values
-                         / (self.InputData.LFG_param['ch4prop']['amount'] * 10**6))
+        Biogas_factor = self.gas_emission_factor["Concentration_ppmv"].values / (
+            self.InputData.LFG_param["ch4prop"]["amount"] * 10**6
+        )
+
+        Vent_factor = (
+            Biogas_factor
+            * (1 - self.gas_emission_factor["Destruction_Eff_Vent"].values / 100)
+            * (1 / self.CommonData.STP["mole_to_L"]["amount"])
+            * self.gas_emission_factor["MW"].values
+        )
+
+        Flare_factor = (
+            Biogas_factor
+            * (1 - self.gas_emission_factor["Destruction_Eff_Flare"].values / 100)
+            * (1 / self.CommonData.STP["mole_to_L"]["amount"])
+            * self.gas_emission_factor["MW"].values
+        )
+
+        Comb_factor = (
+            Biogas_factor
+            * (1 - self.gas_emission_factor["Destruction_Eff_User_Defined"].values / 100)
+            * (1 / self.CommonData.STP["mole_to_L"]["amount"])
+            * self.gas_emission_factor["MW"].values
+        )
+
+        self.emission_to_air = (
+            self.LFG["Total methane in uncollected biogas"].apply(lambda x: x * Vent_factor).values
+            + self.LFG["Total Methane flared"].apply(lambda x: x * Flare_factor).values
+            + self.LFG["Total Methane combusted"].apply(lambda x: x * Comb_factor).values
+        )
+
+        self.emission_to_air = np.array(
+            [list(self.emission_to_air[i]) for i in range(len(self.emission_to_air))]
+        )
 
-        Vent_factor = (Biogas_factor
-                       * (1 - self.gas_emission_factor['Destruction_Eff_Vent'].values / 100)
-                       * (1 / self.CommonData.STP['mole_to_L']['amount'])
-                       * self.gas_emission_factor['MW'].values)
-
-        Flare_factor = (Biogas_factor
-                        * (1 - self.gas_emission_factor['Destruction_Eff_Flare'].values / 100)
-                        * (1 / self.CommonData.STP['mole_to_L']['amount'])
-                        * self.gas_emission_factor['MW'].values)
-
-        Comb_factor = (Biogas_factor
-                       * (1 - self.gas_emission_factor['Destruction_Eff_User_Defined'].values / 100)
-                       * (1 / self.CommonData.STP['mole_to_L']['amount'])
-                       * self.gas_emission_factor['MW'].values)
-
-        self.emission_to_air = (self.LFG['Total methane in uncollected biogas'].apply(lambda x: x * Vent_factor).values
-                                + self.LFG['Total Methane flared'].apply(lambda x: x * Flare_factor).values
-                                + self.LFG['Total Methane combusted'].apply(lambda x: x * Comb_factor).values)
-
-        self.emission_to_air = np.array([list(self.emission_to_air[i]) for i in range(len(self.emission_to_air))])
-
-        self.emission_to_air = pd.DataFrame(self.emission_to_air,
-                                            index=self.Index,
-                                            columns=(self.gas_emission_factor['Exchange'].values
-                                                     + ' to '
-                                                     + self.gas_emission_factor['Subcompartment'].values))
+        self.emission_to_air = pd.DataFrame(
+            self.emission_to_air,
+            index=self.Index,
+            columns=(
+                self.gas_emission_factor["Exchange"].values
+                + " to "
+                + self.gas_emission_factor["Subcompartment"].values
+            ),
+        )
 
-        key1 = zip(self.emission_to_air.columns, self.gas_emission_factor['Biosphere_key'].values)
+        key1 = zip(self.emission_to_air.columns, self.gas_emission_factor["Biosphere_key"].values)
         self._key1 = dict(key1)
 
         # Direct CO2 and Methane emissions, Calculated in the model
-        self.LFG['Mass of emitted methane'] = (
-            self.LFG['Total Methane Emitted'].values
-            * self.CommonData.STP['m3CH4_to_kg']['amount'])
-
-        self.LFG['Mass of CO2 generated with methane'] = (
-            self.LFG['Total generated Methane'].values
-            * (1 / self.InputData.LFG_param['ch4prop']['amount'])
-            * (1 - self.InputData.LFG_param['ch4prop']['amount'])
-            * self.CommonData.STP['m3CO2_to_kg']['amount'])
-
-        self.LFG['Mass of CO2 generated with methane combustion'] = (
-            (self.LFG['Total Methane combusted'].values
-             * self.InputData.Energy_Rec['EngineCombEff']['amount'] / 100
-             + self.LFG['Total Methane flared'].values
-             * self.InputData.Flare['FlareCombEff']['amount'] / 100)
+        self.LFG["Mass of emitted methane"] = (
+            self.LFG["Total Methane Emitted"].values * self.CommonData.STP["m3CH4_to_kg"]["amount"]
+        )
+
+        self.LFG["Mass of CO2 generated with methane"] = (
+            self.LFG["Total generated Methane"].values
+            * (1 / self.InputData.LFG_param["ch4prop"]["amount"])
+            * (1 - self.InputData.LFG_param["ch4prop"]["amount"])
+            * self.CommonData.STP["m3CO2_to_kg"]["amount"]
+        )
+
+        self.LFG["Mass of CO2 generated with methane combustion"] = (
+            (
+                self.LFG["Total Methane combusted"].values
+                * self.InputData.Energy_Rec["EngineCombEff"]["amount"]
+                / 100
+                + self.LFG["Total Methane flared"].values
+                * self.InputData.Flare["FlareCombEff"]["amount"]
+                / 100
+            )
             * 1000
-            * (1 / self.CommonData.STP['mole_to_L']['amount'])
-            * self.CommonData.MW['CO2']['amount'] / 1000)
+            * (1 / self.CommonData.STP["mole_to_L"]["amount"])
+            * self.CommonData.MW["CO2"]["amount"]
+            / 1000
+        )
 
-        self.LFG['Mass of CO2 generated with methane oxidation'] = (
-            self.LFG['Total Methane oxidized'].values * 1000
-            * (1 / self.CommonData.STP['mole_to_L']['amount'])
-            * self.CommonData.MW['CO2']['amount'] / 1000)
-
-        self.LFG['Mass of CO2 storage'] = (
-            - (1 - self.Material_Properties['Moisture Content'].values / 100)
-            * self.Material_Properties['Carbon Storage Factor'].values
-            * self.CommonData.MW['CO2']['amount']
-            / self.CommonData.MW['C']['amount'])
+        self.LFG["Mass of CO2 generated with methane oxidation"] = (
+            self.LFG["Total Methane oxidized"].values
+            * 1000
+            * (1 / self.CommonData.STP["mole_to_L"]["amount"])
+            * self.CommonData.MW["CO2"]["amount"]
+            / 1000
+        )
+
+        self.LFG["Mass of CO2 storage"] = (
+            -(1 - self.Material_Properties["Moisture Content"].values / 100)
+            * self.Material_Properties["Carbon Storage Factor"].values
+            * self.CommonData.MW["CO2"]["amount"]
+            / self.CommonData.MW["C"]["amount"]
+        )
 
         # Adding the CO2 emissions to 'emission_to_air' dict
-        if 'Carbon dioxide, non-fossil to unspecified' in self.emission_to_air.columns:
-            self.emission_to_air['Carbon dioxide, non-fossil to unspecified'] += (
-                self.LFG['Mass of CO2 generated with methane'].values
-                + self.LFG['Mass of CO2 generated with methane combustion'].values
-                + self.LFG['Mass of CO2 generated with methane oxidation'].values)
+        if "Carbon dioxide, non-fossil to unspecified" in self.emission_to_air.columns:
+            self.emission_to_air["Carbon dioxide, non-fossil to unspecified"] += (
+                self.LFG["Mass of CO2 generated with methane"].values
+                + self.LFG["Mass of CO2 generated with methane combustion"].values
+                + self.LFG["Mass of CO2 generated with methane oxidation"].values
+            )
         else:
-            self.emission_to_air['Carbon dioxide, non-fossil to unspecified'] = (
-                self.LFG['Mass of CO2 generated with methane'].values
-                + self.LFG['Mass of CO2 generated with methane combustion'].values
-                + self.LFG['Mass of CO2 generated with methane oxidation'].values)
-
-            self._key1['Carbon dioxide, non-fossil to unspecified'] = ('biosphere3', 'eba59fd6-f37e-41dc-9ca3-c7ea22d602c7')
+            self.emission_to_air["Carbon dioxide, non-fossil to unspecified"] = (
+                self.LFG["Mass of CO2 generated with methane"].values
+                + self.LFG["Mass of CO2 generated with methane combustion"].values
+                + self.LFG["Mass of CO2 generated with methane oxidation"].values
+            )
+
+            self._key1["Carbon dioxide, non-fossil to unspecified"] = (
+                "biosphere3",
+                "eba59fd6-f37e-41dc-9ca3-c7ea22d602c7",
+            )
 
         # Adding the CO2 storage to 'emission_to_air' dict
-        if 'Carbon dioxide, from soil or biomass stock to unspecified' in self.emission_to_air.columns:
-            self.emission_to_air['Carbon dioxide, from soil or biomass stock to unspecified'] += self.LFG['Mass of CO2 storage'].values
+        if (
+            "Carbon dioxide, from soil or biomass stock to unspecified"
+            in self.emission_to_air.columns
+        ):
+            self.emission_to_air[
+                "Carbon dioxide, from soil or biomass stock to unspecified"
+            ] += self.LFG["Mass of CO2 storage"].values
         else:
-            self.emission_to_air['Carbon dioxide, from soil or biomass stock to unspecified'] = self.LFG['Mass of CO2 storage'].values
-            self._key1['Carbon dioxide, from soil or biomass stock to unspecified'] = ('biosphere3', 'e4e9febc-07c1-403d-8d3a-6707bb4d96e6')
+            self.emission_to_air[
+                "Carbon dioxide, from soil or biomass stock to unspecified"
+            ] = self.LFG["Mass of CO2 storage"].values
+            self._key1["Carbon dioxide, from soil or biomass stock to unspecified"] = (
+                "biosphere3",
+                "e4e9febc-07c1-403d-8d3a-6707bb4d96e6",
+            )
 
         # Adding the Methane emissions to 'emission_to_air' dict
-        if 'Methane, non-fossil to unspecified' in self.emission_to_air.columns:
-            self.emission_to_air['Methane, non-fossil to unspecified'] += self.LFG['Mass of emitted methane'].values
+        if "Methane, non-fossil to unspecified" in self.emission_to_air.columns:
+            self.emission_to_air["Methane, non-fossil to unspecified"] += self.LFG[
+                "Mass of emitted methane"
+            ].values
         else:
-            self.emission_to_air['Methane, non-fossil to unspecified'] = self.LFG['Mass of emitted methane'].values
-            self._key1['Methane, non-fossil to unspecified'] = ('biosphere3', 'da1157e2-7593-4dfd-80dd-a3449b37a4d8')
-
+            self.emission_to_air["Methane, non-fossil to unspecified"] = self.LFG[
+                "Mass of emitted methane"
+            ].values
+            self._key1["Methane, non-fossil to unspecified"] = (
+                "biosphere3",
+                "da1157e2-7593-4dfd-80dd-a3449b37a4d8",
+            )
 
     def _Leachate(self):
         """
-        Calculates the leachate flow and concentraions
+        Calculates the leachate flow and concentrations.
         """
         self._n_lcht = 100
         # LEACHATE GENERATION, QUANTITY AND CONSTITUENTS
         self._param3 = pd.DataFrame(index=np.arange(self._n_lcht), dtype=float)
-        self._param3['year'] = np.arange(1, 101)
+        self._param3["year"] = np.arange(1, 101)
 
-        self._param3['Time to initial cover placement'] = (
-            self.GasColPlan.loc['cellFillTime', self._plan]
-            - np.mod(np.arange(self._n_lcht), self.GasColPlan.loc['cellFillTime', self._plan]))
+        self._param3["Time to initial cover placement"] = self.GasColPlan.loc[
+            "cellFillTime", self._plan
+        ] - np.mod(np.arange(self._n_lcht), self.GasColPlan.loc["cellFillTime", self._plan])
 
-        k = self.InputData.LFG_param['actk']['amount']
+        k = self.InputData.LFG_param["actk"]["amount"]
         if k <= 0.03:
-            self._param3['Annual Precipitation (mm)'] = self.InputData.Leachate['precip_arid']['amount']
+            self._param3["Annual Precipitation (mm)"] = self.InputData.Leachate["precip_arid"][
+                "amount"
+            ]
         elif k <= 0.6:
-            self._param3['Annual Precipitation (mm)'] = self.InputData.Leachate['precip_mod']['amount']
+            self._param3["Annual Precipitation (mm)"] = self.InputData.Leachate["precip_mod"][
+                "amount"
+            ]
         elif k > 0.06:
-            self._param3['Annual Precipitation (mm)'] = self.InputData.Leachate['precip_wet']['amount']
-
-        if self.InputData.Leachate['is_bioreactor']['amount']:
-            self._param3['Annual Precipitation (mm)'] = self.InputData.Leachate['precip_bio']['amount']
+            self._param3["Annual Precipitation (mm)"] = self.InputData.Leachate["precip_wet"][
+                "amount"
+            ]
+
+        if self.InputData.Leachate["is_bioreactor"]["amount"]:
+            self._param3["Annual Precipitation (mm)"] = self.InputData.Leachate["precip_bio"][
+                "amount"
+            ]
+
+        self.LeachColEff = np.full(
+            (self._n_lcht, self._n), self.InputData.Leachate["prep_leach_init"]["amount"]
+        )
+        xx, yy = np.mgrid[0 : self._n_lcht, 0 : self._n]
+        filter_FCover = (
+            xx + yy
+            >= self.GasColPlan.loc["timeToFinCover", self._plan]
+            + self.InputData.LF_Op["optime"]["amount"]
+        )
+        filter_IntCover = (
+            xx.reshape(self._n, self._n_lcht)
+            >= self._param3["Time to initial cover placement"].values
+        ).reshape(self._n_lcht, self._n)
+        self.LeachColEff[filter_IntCover] = self.InputData.Leachate["prep_leach_red"]["amount"]
+        self.LeachColEff[filter_FCover] = self.InputData.Leachate["prep_leach_f"]["amount"]
 
-        self.LeachColEff = np.full((self._n_lcht, self._n), self.InputData.Leachate['prep_leach_init']['amount'])
-        xx, yy = np.mgrid[0:self._n_lcht, 0:self._n]
-        filter_FCover = xx + yy >= self.GasColPlan.loc['timeToFinCover', self._plan] + self.InputData.LF_Op['optime']['amount']
-        filter_IntCover = (xx.reshape(self._n, self._n_lcht) >= self._param3['Time to initial cover placement'].values).reshape(self._n_lcht, self._n)
-        self.LeachColEff[filter_IntCover] = self.InputData.Leachate['prep_leach_red']['amount']
-        self.LeachColEff[filter_FCover] = self.InputData.Leachate['prep_leach_f']['amount']
+        self._param3["Frac Precip to Leachate"] = self.LeachColEff.mean(axis=1)
 
-        self._param3['Frac Precip to Leachate'] = self.LeachColEff.mean(axis=1)
-
-        if self.InputData.Leachate['is_bioreactor']['amount']:
+        if self.InputData.Leachate["is_bioreactor"]["amount"]:
             Circulate = np.zeros(self._n_lcht)
-            fltr_cir = self._param3['year'].values < self.InputData.Leachate['LF_time2']['amount']
-            fltr_cir_off = self._param3['year'].values < self.InputData.Leachate['LF_time1']['amount']
-            Circulate[fltr_cir] = self.InputData.Leachate['frac_recirc']['amount']
+            fltr_cir = self._param3["year"].values < self.InputData.Leachate["LF_time2"]["amount"]
+            fltr_cir_off = (
+                self._param3["year"].values < self.InputData.Leachate["LF_time1"]["amount"]
+            )
+            Circulate[fltr_cir] = self.InputData.Leachate["frac_recirc"]["amount"]
             Circulate[fltr_cir_off] = 0.0
-            self._param3['frac Col Leach Recirculated'] = Circulate
+            self._param3["frac Col Leach Recirculated"] = Circulate
         else:
-            self._param3['frac Col Leach Recirculated'] =  0.0
+            self._param3["frac Col Leach Recirculated"] = 0.0
 
-        self._param3['frac Col Leach to WWTP'] = 1.0 - self._param3['frac Col Leach Recirculated'].values
+        self._param3["frac Col Leach to WWTP"] = (
+            1.0 - self._param3["frac Col Leach Recirculated"].values
+        )
 
         leach_col_eff = np.zeros(self._n_lcht)
-        fltr_1 = self._param3['year'].values < self.InputData.Leachate['LF_time3']['amount']
-        fltr_2 = self._param3['year'].values < self.InputData.Leachate['LF_time1']['amount']
-        leach_col_eff[fltr_1] = self.InputData.Leachate['Lcht_Col_Ef']['amount']
+        fltr_1 = self._param3["year"].values < self.InputData.Leachate["LF_time3"]["amount"]
+        fltr_2 = self._param3["year"].values < self.InputData.Leachate["LF_time1"]["amount"]
+        leach_col_eff[fltr_1] = self.InputData.Leachate["Lcht_Col_Ef"]["amount"]
         leach_col_eff[fltr_2] = 0.0
-        self._param3['Leach Col Eff'] = leach_col_eff
+        self._param3["Leach Col Eff"] = leach_col_eff
 
         """
         Annual Waste to landfill:
             <200000 Mg/y small landfill: 1500 lb/yd3 (890 kg/m3);
             >=200000 Mg/yr large landfill: 1800 lb/yds (1068 kg/m3)
         Equation are from regression in the landfill paper (Wang et. al. 2021)
         """
-        if self.InputData.LF_Op['annWaste']['amount'] < 200000:
+        if self.InputData.LF_Op["annWaste"]["amount"] < 200000:
             self._LF_msw_ha = (
                 29806
-                * np.log(self.InputData.LF_Op['annWaste']['amount']
-                         * self.InputData.LF_Op['optime']['amount'])
-                - 263324)
+                * np.log(
+                    self.InputData.LF_Op["annWaste"]["amount"]
+                    * self.InputData.LF_Op["optime"]["amount"]
+                )
+                - 263324
+            )
         else:
             self._LF_msw_ha = (
                 73172
-                * np.log(self.InputData.LF_Op['annWaste']['amount']
-                         * self.InputData.LF_Op['optime']['amount'])
-                - 837452)
+                * np.log(
+                    self.InputData.LF_Op["annWaste"]["amount"]
+                    * self.InputData.LF_Op["optime"]["amount"]
+                )
+                - 837452
+            )
 
         # Mass balance of Leachate
-        self._param3['Generated Leachate (m3/Mg MSW)'] = (
-            (self._param3['Annual Precipitation (mm)'].values / 1000)  # mm to m
-            * (self._param3['Frac Precip to Leachate'].values)
-            * (10000 / self._LF_msw_ha))  # Ha to m2
-
-        self._param3['Collected Leachate (m3/Mg MSW)'] = (
-            self._param3['Generated Leachate (m3/Mg MSW)'].values
-            * self._param3['Leach Col Eff'].values)
-
-        self._param3['Recirculated Leachate (m3/Mg MSW)'] = (
-            self._param3['Generated Leachate (m3/Mg MSW)'].values
-            * self._param3['frac Col Leach Recirculated'].values)
-        self._param3['Treated Leachate (m3/Mg MSW)'] = (
-            self._param3['Collected Leachate (m3/Mg MSW)'].values
-            * self._param3['frac Col Leach to WWTP'].values)
-        self._param3['Fugitive Leachate  (m3/Mg MSW)'] = (
-            self._param3['Generated Leachate (m3/Mg MSW)'].values
-            - self._param3['Treated Leachate (m3/Mg MSW)'].values
-            - self._param3['Recirculated Leachate (m3/Mg MSW)'].values)
+        self._param3["Generated Leachate (m3/Mg MSW)"] = (
+            (self._param3["Annual Precipitation (mm)"].values / 1000)  # mm to m
+            * (self._param3["Frac Precip to Leachate"].values)
+            * (10000 / self._LF_msw_ha)
+        )  # Ha to m2
+
+        self._param3["Collected Leachate (m3/Mg MSW)"] = (
+            self._param3["Generated Leachate (m3/Mg MSW)"].values
+            * self._param3["Leach Col Eff"].values
+        )
+
+        self._param3["Recirculated Leachate (m3/Mg MSW)"] = (
+            self._param3["Generated Leachate (m3/Mg MSW)"].values
+            * self._param3["frac Col Leach Recirculated"].values
+        )
+        self._param3["Treated Leachate (m3/Mg MSW)"] = (
+            self._param3["Collected Leachate (m3/Mg MSW)"].values
+            * self._param3["frac Col Leach to WWTP"].values
+        )
+        self._param3["Fugitive Leachate  (m3/Mg MSW)"] = (
+            self._param3["Generated Leachate (m3/Mg MSW)"].values
+            - self._param3["Treated Leachate (m3/Mg MSW)"].values
+            - self._param3["Recirculated Leachate (m3/Mg MSW)"].values
+        )
 
         # Concentration of other effluents in leachate  (kg/L)
         self.lcht_conc = np.zeros((self._n_lcht, self.lcht_Qlty.shape[0]))
-        self.lcht_conc[:2, :] = self.lcht_Qlty['Stage 1 (0-2 years, mg/L)'].values
-        self.lcht_conc[2:10, :] = self.lcht_Qlty['Stage 2 (3-10 years, mg/L)'].values
-        self.lcht_conc[10:40, :] = self.lcht_Qlty['Stage 3 (11-40 years, mg/L)'].values
-        self.lcht_conc[40:100, :] = self.lcht_Qlty['Stage 4 (41-100 years, mg/L)'].values
+        self.lcht_conc[:2, :] = self.lcht_Qlty["Stage 1 (0-2 years, mg/L)"].values
+        self.lcht_conc[2:10, :] = self.lcht_Qlty["Stage 2 (3-10 years, mg/L)"].values
+        self.lcht_conc[10:40, :] = self.lcht_Qlty["Stage 3 (11-40 years, mg/L)"].values
+        self.lcht_conc[40:100, :] = self.lcht_Qlty["Stage 4 (41-100 years, mg/L)"].values
         self.lcht_conc /= 10**6  # mg/L -> kg/L
 
-        self.lcht_conc = pd.DataFrame(
-            self.lcht_conc,
-            columns=self.lcht_Qlty['Emission'].values)
+        self.lcht_conc = pd.DataFrame(self.lcht_conc, columns=self.lcht_Qlty["Emission"].values)
 
         # Fugitive Leachate Emissions (leaks through liner) (kg/Mg MSW)
         self._Fugitive_Leachate = pd.Series(
-            (self.lcht_conc.values.T
-             * self._param3['Fugitive Leachate  (m3/Mg MSW)'].values).sum(axis=1)
+            (self.lcht_conc.values.T * self._param3["Fugitive Leachate  (m3/Mg MSW)"].values).sum(
+                axis=1
+            )
             * 1000,  # m3 -> L
-            index=self.lcht_Qlty['Emission'].values)
+            index=self.lcht_Qlty["Emission"].values,
+        )
 
         # Post-treatment effluent emissions (kg/Mg MSW)
         self._Effluent = pd.Series(
             np.multiply(
                 np.multiply(
-                    self.lcht_conc.values.T,
-                    self._param3['Treated Leachate (m3/Mg MSW)'].values).sum(axis=1),
-                1 - self.lcht_Qlty['Removal Efficiency (%)'].values / 100) * 1000,
-            index=self.lcht_Qlty['Emission'].values)
-
-
+                    self.lcht_conc.values.T, self._param3["Treated Leachate (m3/Mg MSW)"].values
+                ).sum(axis=1),
+                1 - self.lcht_Qlty["Removal Efficiency (%)"].values / 100,
+            )
+            * 1000,
+            index=self.lcht_Qlty["Emission"].values,
+        )
 
         self.lcht_Alloc = np.zeros((len(self.Index), self.lcht_Qlty.shape[0]))
-        comp = self.process_data['Assumed_Comp'].values
-        sld_cont = (1 - self.Material_Properties['Moisture Content'] / 100)
+        comp = self.process_data["Assumed_Comp"].values
+        sld_cont = 1 - self.Material_Properties["Moisture Content"] / 100
         sld_msw = (comp * sld_cont).sum()
         sld_alloc = sld_cont / sld_msw
-        for i, j in enumerate(self.lcht_Qlty['Allocation_base'].values):
-            if j == 'Solid Content':
+        for i, j in enumerate(self.lcht_Qlty["Allocation_base"].values):
+            if j == "Solid Content":
                 self.lcht_Alloc[:, i] = sld_alloc
-            elif j == 'Nitrogen Content' or j == 'Phosphorus Content':
-                m = self.Material_Properties[j].values * sld_cont * self.process_data['Degrades'].values
+            elif j in ["Nitrogen Content", "Phosphorus Content"]:
+                m = (
+                    self.Material_Properties[j].values
+                    * sld_cont
+                    * self.process_data["Degrades"].values
+                )
                 self.lcht_Alloc[:, i] = m / (m * comp).sum()
             else:
                 m = self.Material_Properties[j].values * sld_cont
                 self.lcht_Alloc[:, i] = m / (m * comp).sum()
 
-        self.lcht_Alloc = pd.DataFrame(self.lcht_Alloc,
-                                       columns=self.lcht_Qlty['Emission'].values,
-                                       index=self.Index)
+        self.lcht_Alloc = pd.DataFrame(
+            self.lcht_Alloc, columns=self.lcht_Qlty["Emission"].values, index=self.Index
+        )
 
         self.Surface_water_emission = pd.DataFrame(
             self.lcht_Alloc.values * self._Effluent.values,
             index=self.Index,
-            columns=self.lcht_Qlty['Emission'].values + "_ to SW")
+            columns=self.lcht_Qlty["Emission"].values + "_ to SW",
+        )
 
-        self._key2 = dict(zip(self.Surface_water_emission.columns, self.lcht_Qlty['Surface_water'].values))
+        self._key2 = dict(
+            zip(self.Surface_water_emission.columns, self.lcht_Qlty["Surface_water"].values)
+        )
 
         self.Ground_water_emission = pd.DataFrame(
             self.lcht_Alloc.values * self._Fugitive_Leachate.values,
             index=self.Index,
-            columns=self.lcht_Qlty['Emission'].values + "_ to GW")
+            columns=self.lcht_Qlty["Emission"].values + "_ to GW",
+        )
 
-        self._key3 = dict(zip(self.Ground_water_emission.columns, self.lcht_Qlty['Ground_water'].values))
+        self._key3 = dict(
+            zip(self.Ground_water_emission.columns, self.lcht_Qlty["Ground_water"].values)
+        )
 
         # Electricity Consumption for Leachate Treatment
-        BOD_removed = (sum(self.lcht_conc['BOD5, Biological Oxygen Demand'].values
-                           * self._param3['Treated Leachate (m3/Mg MSW)'].values)
-                       * 1000
-                       - self._Effluent['BOD5, Biological Oxygen Demand'])
+        BOD_removed = (
+            sum(
+                self.lcht_conc["BOD5, Biological Oxygen Demand"].values
+                * self._param3["Treated Leachate (m3/Mg MSW)"].values
+            )
+            * 1000
+            - self._Effluent["BOD5, Biological Oxygen Demand"]
+        )
 
-        BOD_elec = BOD_removed * self.InputData.BOD['LF_lcht_ec']['amount']
+        BOD_elec = BOD_removed * self.InputData.BOD["LF_lcht_ec"]["amount"]
 
         Pump_elec_per_litr = (
-            self.InputData.lcht_pump['leachAirPerLeach']['amount']
-            * (1 / self.InputData.lcht_pump['leachCompPowReq']['amount'])
+            self.InputData.lcht_pump["leachAirPerLeach"]["amount"]
+            * (1 / self.InputData.lcht_pump["leachCompPowReq"]["amount"])
             * (1 / 28.32)
             * (1 / (60 * 24 * 365.25))
-            * (self.InputData.lcht_pump['leachCompLoad']['amount'] / 100)
-            * (100 / self.InputData.lcht_pump['leachEff']['amount'])
-            * 8766 / 1.341)
-
-        Pump_elec = sum(self._param3['Collected Leachate (m3/Mg MSW)'].values
-                        * 1000 * Pump_elec_per_litr)
-
-        Leachate_elec = (self.lcht_Alloc['BOD5, Biological Oxygen Demand']
-                         * BOD_elec
-                         + Pump_elec)
+            * (self.InputData.lcht_pump["leachCompLoad"]["amount"] / 100)
+            * (100 / self.InputData.lcht_pump["leachEff"]["amount"])
+            * 8766
+            / 1.341
+        )
+
+        Pump_elec = sum(
+            self._param3["Collected Leachate (m3/Mg MSW)"].values * 1000 * Pump_elec_per_litr
+        )
+
+        Leachate_elec = self.lcht_Alloc["BOD5, Biological Oxygen Demand"] * BOD_elec + Pump_elec
 
         # Adding leachate collection electricity use to LCI
-        self.LCI.add('Electricity_consumption', Leachate_elec.values)
+        self.LCI.add("Electricity_consumption", Leachate_elec.values)
 
         # List of metals in Leachate
-        metals = ['Arsenic, ion', 'Barium', 'Cadmium, ion', 'Chromium, ion',
-                  'Lead','Mercury', 'Selenium', 'Silver, ion']
+        metals = [
+            "Arsenic, ion",
+            "Barium",
+            "Cadmium, ion",
+            "Chromium, ion",
+            "Lead",
+            "Mercury",
+            "Selenium",
+            "Silver, ion",
+        ]
 
-        # Calculating Slude generation and transport
-        LF_sldg_BOD = self.InputData.BOD['LF_sldg_per_BOD']['amount'] * BOD_removed
+        # Calculating Sludge generation and transport
+        LF_sldg_BOD = self.InputData.BOD["LF_sldg_per_BOD"]["amount"] * BOD_removed
 
         LF_sldg_PO4 = (
-            self._Effluent['Phosphate']
-            * (self.InputData.Leachate['LF_eff_PO4']['amount'] / 100)
-            / (1 - self.InputData.Leachate['LF_eff_PO4']['amount'] / 100))
-
-        LF_sldg_mtls = (self._Effluent[metals].sum()
-                        * (self.InputData.Leachate['LF_eff_mtls']['amount'] / 100)
-                        / (1 - self.InputData.Leachate['LF_eff_mtls']['amount'] / 100))
-
-        LF_sldg_tss = (self._Effluent['TSS']
-                       * (self.InputData.Leachate['LF_eff_TSS']['amount'] / 100)
-                       / (1 - self.InputData.Leachate['LF_eff_TSS']['amount'] / 100))
+            self._Effluent["Phosphate"]
+            * (self.InputData.Leachate["LF_eff_PO4"]["amount"] / 100)
+            / (1 - self.InputData.Leachate["LF_eff_PO4"]["amount"] / 100)
+        )
+
+        LF_sldg_mtls = (
+            self._Effluent[metals].sum()
+            * (self.InputData.Leachate["LF_eff_mtls"]["amount"] / 100)
+            / (1 - self.InputData.Leachate["LF_eff_mtls"]["amount"] / 100)
+        )
+
+        LF_sldg_tss = (
+            self._Effluent["TSS"]
+            * (self.InputData.Leachate["LF_eff_TSS"]["amount"] / 100)
+            / (1 - self.InputData.Leachate["LF_eff_TSS"]["amount"] / 100)
+        )
 
         # Generated sludge from Leachate treatment
         self.sludge = pd.DataFrame(index=self.Index)
-        self.sludge['sludge generated from BOD removal'] = (
-            self.lcht_Alloc['BOD5, Biological Oxygen Demand'].values
-            * LF_sldg_BOD)
-
-        self.sludge['sludge generated from phosphate removal'] = (
-            self.lcht_Alloc['Phosphate'].values
-            * LF_sldg_PO4)
-
-        self.sludge['sludge generated from metals removal'] = (
-            self.lcht_Alloc[metals].values
-            * LF_sldg_mtls).sum(axis=1)
-
-        self.sludge['sludge generated from suspended solids removal'] = (
-            self.lcht_Alloc['TSS'].values
-            * LF_sldg_tss)
-
-        self.sludge['total sludge generated'] = (
-            self.sludge['sludge generated from BOD removal'].values
-            + self.sludge['sludge generated from phosphate removal'].values
-            + self.sludge['sludge generated from metals removal'].values
-            + self.sludge['sludge generated from suspended solids removal'].values)
-
-        self.sludge['Medium-Heavy Duty Transportation'] = (
-            self.sludge['total sludge generated'].values / 1000
-            * self.InputData.Leachate['dis_POTW']['amount'])
-
-        self.LCI.add('Internal_Process_Transportation_Medium_Duty_Diesel_Truck',
-                     self.sludge['Medium-Heavy Duty Transportation'].values * 1000)
+        self.sludge["sludge generated from BOD removal"] = (
+            self.lcht_Alloc["BOD5, Biological Oxygen Demand"].values * LF_sldg_BOD
+        )
+
+        self.sludge["sludge generated from phosphate removal"] = (
+            self.lcht_Alloc["Phosphate"].values * LF_sldg_PO4
+        )
+
+        self.sludge["sludge generated from metals removal"] = (
+            self.lcht_Alloc[metals].values * LF_sldg_mtls
+        ).sum(axis=1)
+
+        self.sludge["sludge generated from suspended solids removal"] = (
+            self.lcht_Alloc["TSS"].values * LF_sldg_tss
+        )
+
+        self.sludge["total sludge generated"] = (
+            self.sludge["sludge generated from BOD removal"].values
+            + self.sludge["sludge generated from phosphate removal"].values
+            + self.sludge["sludge generated from metals removal"].values
+            + self.sludge["sludge generated from suspended solids removal"].values
+        )
+
+        self.sludge["Medium-Heavy Duty Transportation"] = (
+            self.sludge["total sludge generated"].values
+            / 1000
+            * self.InputData.Leachate["dis_POTW"]["amount"]
+        )
+
+        self.LCI.add(
+            "Internal_Process_Transportation_Medium_Duty_Diesel_Truck",
+            self.sludge["Medium-Heavy Duty Transportation"].values * 1000,
+        )
 
     # Life-Cycle Costs
     def _Add_cost(self):
         self.cost_DF = pd.DataFrame(index=self.Index)
-        self.cost_DF[('biosphere3', 'Operational_Cost')] = [
-            self.InputData.Operational_Cost[y]['amount'] for y in self.Index]
+        self.cost_DF[("biosphere3", "Operational_Cost")] = [
+            self.InputData.Operational_Cost[y]["amount"] for y in self.Index
+        ]
 
     # Life-Cycle Inventory
     def _Material_energy_use(self):
-        # Electricity used for office and maitenance buildings
+        # Electricity used for office and maintenance buildings
         bld_elec = 0.081  # kWh/Mg
-        self.LCI.add('Electricity_consumption', bld_elec)
+        self.LCI.add("Electricity_consumption", bld_elec)
 
         """
         Diesel use include:
         1. Fuel used for heavy equipment during construction
         2. Fuel used for heavy equipment during closure
         3. Fuel used for heavy equipment during operation
         4. Fuel used for heavy equipment during closure
         """
         diesel = 1.628  # L/Mg
-        self.LCI.add('Equipment_Diesel', diesel)
+        self.LCI.add("Equipment_Diesel", diesel)
 
         # Material Use
         """
         HDPE include:
         1. Mass of HDPE liner for construction
         2. Mass of HDPE Final Cover & Closure System
         3. Mass of HDPE replaced on a yearly basis for Post-Closure Care
         """
         HDPE_Liner = 0.074  # kg/Mg
-        self.LCI.add('HDPE_Liner', HDPE_Liner)
+        self.LCI.add("HDPE_Liner", HDPE_Liner)
 
         """
         HDPE Pipe include:
         1. HDPE pipe for construction
         2. HDPE pipe for final cover& Closure system
         """
         HDPE_Pipe = 0.0022  # m/Mg
-        self.LCI.add('HDPE_Pipe', HDPE_Pipe)
+        self.LCI.add("HDPE_Pipe", HDPE_Pipe)
 
         """
         PVC pipe for final cover and closure system
         """
         PVC_Pipe = 0.0011  # m/Mg
-        self.LCI.add('PVC_Pipe', PVC_Pipe)
+        self.LCI.add("PVC_Pipe", PVC_Pipe)
 
         """
         Steal
         """
         Steel = 0.2382  # kg/Mg
-        self.LCI.add('Steel', Steel)
+        self.LCI.add("Steel", Steel)
 
         """
         Concrete
         """
         Concrete = 0.0071  # kg/Mg
-        self.LCI.add('Concrete', Concrete)
+        self.LCI.add("Concrete", Concrete)
 
         """
         Asphalt
         """
         Asphalt = 0.0850  # kg/Mg
-        self.LCI.add('Asphalt', Asphalt)
-
+        self.LCI.add("Asphalt", Asphalt)
 
         """
         Sand
         """
         Sand = 33.751  # kg/Mg
-        self.LCI.add('Sand', Sand)
+        self.LCI.add("Sand", Sand)
 
         """
         Gravel
         """
         Gravel = 2.320  # kg/Mg
-        self.LCI.add('Gravel', Gravel)
+        self.LCI.add("Gravel", Gravel)
 
         """
         Clay
         """
         Clay = 57.115  # kg/Mg
-        self.LCI.add('Clay', Clay)
+        self.LCI.add("Clay", Clay)
 
         """
         Building
         """
-        Building = 2.29E-05  # m2/Mg
-        self.LCI.add('Building', Building)
+        Building = 2.29e-05  # m2/Mg
+        self.LCI.add("Building", Building)
 
         # Transportation
         # Heavy duty truck transportation required
-        HD_trans = 542.98    # kgkm/Mg
-        self.LCI.add('Internal_Process_Transportation_Heavy_Duty_Diesel_Truck', HD_trans)
+        HD_trans = 542.98  # kgkm/Mg
+        self.LCI.add("Internal_Process_Transportation_Heavy_Duty_Diesel_Truck", HD_trans)
         # Medium duty transportation required
         MD_trans = 1611.18  # kgkm/Mg
-        self.LCI.add('Internal_Process_Transportation_Medium_Duty_Diesel_Truck', MD_trans)
+        self.LCI.add("Internal_Process_Transportation_Medium_Duty_Diesel_Truck", MD_trans)
         # Heavy duty truck transportation required
-        HD_trans_empty  = 0.018  # vkm/Mg
-        self.LCI.add('Empty_Return_Heavy_Duty_Diesel_Truck', HD_trans_empty)
+        HD_trans_empty = 0.018  # vkm/Mg
+        self.LCI.add("Empty_Return_Heavy_Duty_Diesel_Truck", HD_trans_empty)
         # Medium duty transportation required
         MD_trans_empty = 0.067  # vkm/Mg
-        self.LCI.add('Empty_Return_Medium_Duty_Diesel_Truck', MD_trans_empty)
+        self.LCI.add("Empty_Return_Medium_Duty_Diesel_Truck", MD_trans_empty)
 
         self._key4 = {
-            'Electricity_production': ('Technosphere', 'Electricity_production'),
-            'Electricity_consumption': ('Technosphere', 'Electricity_consumption'),
-            'Equipment_Diesel': ('Technosphere', 'Equipment_Diesel'),
-            'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck': ('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'),
-            'Internal_Process_Transportation_Medium_Duty_Diesel_Truck': ('Technosphere', 'Internal_Process_Transportation_Medium_Duty_Diesel_Truck'),
-            'Empty_Return_Heavy_Duty_Diesel_Truck': ('Technosphere', 'Empty_Return_Heavy_Duty_Diesel_Truck'),
-            'Empty_Return_Medium_Duty_Diesel_Truck': ('Technosphere', 'Empty_Return_Medium_Duty_Diesel_Truck'),
-            'HDPE_Liner': ('Technosphere', 'HDPE_Liner'),
-            'HDPE_Pipe': ('Technosphere', 'HDPE_Pipe'),
-            'PVC_Pipe': ('Technosphere', 'PVC_Pipe'),
-            'Steel': ('Technosphere', 'Steel'),
-            'Concrete': ('Technosphere', 'Concrete'),
-            'Asphalt': ('Technosphere', 'Asphalt'),
-            'Sand': ('Technosphere', 'Sand'),
-            'Gravel': ('Technosphere', 'Gravel'),
-            'Clay': ('Technosphere', 'Clay'),
-            'Building': ('Technosphere', 'Building'),}
+            "Electricity_production": ("Technosphere", "Electricity_production"),
+            "Electricity_consumption": ("Technosphere", "Electricity_consumption"),
+            "Equipment_Diesel": ("Technosphere", "Equipment_Diesel"),
+            "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck": (
+                "Technosphere",
+                "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck",
+            ),
+            "Internal_Process_Transportation_Medium_Duty_Diesel_Truck": (
+                "Technosphere",
+                "Internal_Process_Transportation_Medium_Duty_Diesel_Truck",
+            ),
+            "Empty_Return_Heavy_Duty_Diesel_Truck": (
+                "Technosphere",
+                "Empty_Return_Heavy_Duty_Diesel_Truck",
+            ),
+            "Empty_Return_Medium_Duty_Diesel_Truck": (
+                "Technosphere",
+                "Empty_Return_Medium_Duty_Diesel_Truck",
+            ),
+            "HDPE_Liner": ("Technosphere", "HDPE_Liner"),
+            "HDPE_Pipe": ("Technosphere", "HDPE_Pipe"),
+            "PVC_Pipe": ("Technosphere", "PVC_Pipe"),
+            "Steel": ("Technosphere", "Steel"),
+            "Concrete": ("Technosphere", "Concrete"),
+            "Asphalt": ("Technosphere", "Asphalt"),
+            "Sand": ("Technosphere", "Sand"),
+            "Gravel": ("Technosphere", "Gravel"),
+            "Clay": ("Technosphere", "Clay"),
+            "Building": ("Technosphere", "Building"),
+        }
 
     # Calc function _ Do all the calculations
     def calc(self):
         self._Cal_LFG_Col_Ox()
         self._Cal_LFG()
         self._Leachate()
         self._Material_energy_use()
@@ -798,73 +1019,82 @@
             for y in self.Index:
                 x[y] = {}
 
         ### Output Biosphere Database
         LCI_DF = self.LCI.report()
 
         # Check the electricity production
-        if LCI_DF['Electricity_production'].values.sum() > 0:
-            LCI_DF['Electricity_production'] = (
-                LCI_DF['Electricity_production'].values
-                - LCI_DF['Electricity_consumption'].values)
-            LCI_DF['Electricity_consumption'] = 0
+        if LCI_DF["Electricity_production"].values.sum() > 0:
+            LCI_DF["Electricity_production"] = (
+                LCI_DF["Electricity_production"].values - LCI_DF["Electricity_consumption"].values
+            )
+            LCI_DF["Electricity_consumption"] = 0
         else:
-            LCI_DF['Electricity_consumption'] = (
-                LCI_DF['Electricity_consumption'].values
-                - LCI_DF['Electricity_production'].values)
-            LCI_DF['Electricity_production'] = 0
+            LCI_DF["Electricity_consumption"] = (
+                LCI_DF["Electricity_consumption"].values - LCI_DF["Electricity_production"].values
+            )
+            LCI_DF["Electricity_production"] = 0
 
         for y in self.Index:
             # Technosphere
             for x in self._key4:
                 Technosphere[y][self._key4[x]] = LCI_DF[x][y]
 
         self.bio_rename_dict = dict(self._key1, **self._key2)
         self.bio_rename_dict = dict(self.bio_rename_dict, **self._key3)
-        self.bio_rename_dict[('biosphere3', 'Operational_Cost')] = ('biosphere3', 'Operational_Cost')
-
-        self.LCI_bio = pd.concat([self.emission_to_air,
-                                  self.Surface_water_emission,
-                                  self.Ground_water_emission], axis=1)
+        self.bio_rename_dict[("biosphere3", "Operational_Cost")] = (
+            "biosphere3",
+            "Operational_Cost",
+        )
+
+        self.LCI_bio = pd.concat(
+            [self.emission_to_air, self.Surface_water_emission, self.Ground_water_emission], axis=1
+        )
 
         self.LCI_bio = self.LCI_bio.rename(columns=self.bio_rename_dict)
         self.LCI_bio_index = True
         keys = list(self.bio_rename_dict.keys())
         for x in keys:
             if "biosphere3" not in str(self.bio_rename_dict[x]):
                 self.bio_rename_dict.pop(x)
-        self.LCI_bio[('biosphere3','Operational_Cost')] = self.cost_DF[('biosphere3','Operational_Cost')].values
+        self.LCI_bio[("biosphere3", "Operational_Cost")] = self.cost_DF[
+            ("biosphere3", "Operational_Cost")
+        ].values
         self.Biosphere = self.LCI_bio[self.bio_rename_dict.values()].transpose().to_dict()
         self.LF["Biosphere"] = self.Biosphere
         return self.LF
 
 
 # LCI class
-class LCI():
+class LCI:
     """
     This class store the LCI data in numpy.ndarray instead of pandas for speedup.
-    Report function create pandas DataFrame and return it
-    Column names are stored in self.ColDict
+
+    Report function create pandas DataFrame and return it Column names are stored in
+    self.ColDict
     """
+
     def __init__(self, Index):
         self.Index = Index
         self.LCI = np.zeros((len(Index), 20))
         self.ColDict = {}
         self.ColNumber = 0
 
     def add(self, name, flow):
         if name not in self.ColDict:
             self.ColDict[name] = self.ColNumber
             self.ColNumber += 1
         self.LCI[:, self.ColDict[name]] += flow
 
     def report(self):
         LCI = deepcopy(self.LCI)
-        return pd.DataFrame(LCI[:, :len(self.ColDict)],
-                            columns=list(self.ColDict.keys()),
-                            index=self.Index)
+        return pd.DataFrame(
+            LCI[:, : len(self.ColDict)], columns=list(self.ColDict.keys()), index=self.Index
+        )
 
     def report_T(self):
         LCI = deepcopy(self.LCI)
-        return pd.DataFrame(LCI[:, :len(self.ColDict)].transpose(),
-                            index=list(self.ColDict.keys()),
-                            columns=self.Index)
+        return pd.DataFrame(
+            LCI[:, : len(self.ColDict)].transpose(),
+            index=list(self.ColDict.keys()),
+            columns=self.Index,
+        )
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/MF_Col.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/COM_Col.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,884 +1,1038 @@
 # -*- coding: utf-8 -*-
-"""
-@author: msardar2
-"""
+import warnings
+
+import numpy as np
+import numpy_financial as npf
 import pandas as pd
-from swolfpy_inputdata import MF_Col_Input
+from swolfpy_inputdata import COM_Col_Input
+
 from .ProcessModel import ProcessModel
-import numpy_financial as npf
-import numpy as np
-import warnings
 
 
-class MF_Col(ProcessModel):
-    Process_Type = 'Collection'
-    def __init__(self, process_name, Collection_scheme,
-                 Treatment_processes=None,
-                 Distance=None,
-                 CommonDataObjct=None,
-                 input_data_path=None):
+class COM_Col(ProcessModel):
+    Process_Type = "Collection"
+
+    def __init__(
+        self,
+        process_name,
+        Collection_scheme,
+        Treatment_processes=None,
+        Distance=None,
+        CommonDataObjct=None,
+        input_data_path=None,
+    ):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = MF_Col_Input(input_data_path,
-                                      process_name=self.process_name,
-                                      CommonDataObjct=CommonDataObjct)
+        self.InputData = COM_Col_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
         self.process_name = process_name
 
         if Treatment_processes is not None:
             self.Treat_proc = Treatment_processes
             if Distance:
                 self.Distance = Distance
             else:
-                raise Exception('User should define both Distance and Treatment_processes together!')
+                raise ValueError(
+                    "User should define both Distance and Treatment_processes together!"
+                )
         else:
             self.Treat_proc = False
 
         self.process_data = self.InputData.process_data
         self.col_schm = Collection_scheme
 
     @staticmethod
     def scheme():
         """
-        Retrun the dictionary for collection_scheme. all the
-        contributions are zero; user should define them according to his/her case.
+        Return the dictionary for collection_scheme.
+
+        all the contributions are zero; user should define them according to his/her case.
         """
-        SepOrg = ['N/A', 'SSYW', 'SSO']
-        SepRec = ['N/A', 'SSR', 'DSR', 'MSR', 'MSRDO']
+        SepOrg = ["N/A", "SSYW", "SSO", "SSO_AnF"]
+        SepRec = ["N/A", "SSR", "DSR", "MSR", "MSRDO"]
         scheme = {}
         for i in SepOrg:
             for j in SepRec:
-                scheme[('RWC', i, j)] = 0
+                scheme[("RWC", i, j)] = 0
         for i in SepOrg:
-            scheme[('REC_WetRes', i, 'REC_WetRes')] = 0
+            scheme[("REC_WetRes", i, "REC_WetRes")] = 0
         for j in SepRec:
-            scheme[('ORG_DryRes', 'ORG_DryRes', j)] = 0
+            scheme[("ORG_DryRes", "ORG_DryRes", j)] = 0
         return scheme
 
     def _normalize_scheme(self, DropOff=True, warn=True):
         """
-        Used in optimization. Check that sum of the contributions is 1.
+        Used in optimization.
+
+        Check that sum of the contributions is 1.
         """
         if not DropOff:
             for k in self.col_schm:
-                if 'DO' in k:
+                if "DO" in k:
                     self.col_schm[k] = 0
 
-        contribution =  sum(self.col_schm.values())
+        contribution = sum(self.col_schm.values())
         if abs(contribution - 1) > 0.01:
             if warn:
-                warnings.warn('Error in collection scheme: Sum(Contribution) != 1')
+                warnings.warn("Error in collection scheme: Sum(Contribution) != 1")
             for k, v in self.col_schm.items():
                 self.col_schm[k] = v / contribution
 
     def calc_composition(self):
         # Creating the sel.col Data frame
-        col_data = np.zeros((11, 62), dtype=float)
+        col_data = np.zeros((12, 62), dtype=float)
         col_data[:] = np.nan
         col_columns = []
-        col_index = ['RWC', 'SSR', 'DSR', 'MSR',
-                     'SSYW', 'SSO', 'ORG', 'DryRes', 'REC',
-                     'WetRes', 'MSRDO']
+        col_index = [
+            "RWC",
+            "SSR",
+            "DSR",
+            "MSR",
+            "SSYW",
+            "SSO",
+            "SSO_AnF",
+            "ORG",
+            "DryRes",
+            "REC",
+            "WetRes",
+            "MSRDO",
+        ]
         col_i = 0
 
         for key, val in self.InputData.den_asmd.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('den_asmd')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("den_asmd")
         col_i += 1
 
         for key, val in self.InputData.HS.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('HS')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("HS")
         col_i += 1
 
         for key, val in self.InputData.Prtcp.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Prtcp')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Prtcp")
         col_i += 1
 
         for key, val in self.InputData.Fr.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Fr')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Fr")
         col_i += 1
 
         for key, val in self.InputData.TL.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('TL')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("TL")
         col_i += 1
 
         for key, val in self.InputData.S.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('S')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("S")
         col_i += 1
 
         for key, val in self.InputData.Nw.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Nw')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Nw")
         col_i += 1
 
         for key, val in self.InputData.Rb.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Rb')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Rb")
         col_i += 1
 
         for key, val in self.InputData.Col_Root.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.LCC.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.DropOff.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.Mpg.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.Speed.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
-        for key in ['CD', 'WV', 'WP', 'wt_lim', 'max_weight', 'F1_', 'F1_idle',
-                    'F2_', 'F2_idle', 'bw', 'bv', 'Lt', 'Ut', 'Vt', 'Fract_CNG',
-                    'grg_area', 'off_area', 'grg_enrg', 'off_enrg', 'Lb']:
-            col_data[:, col_i] = self.InputData.Col[key]['amount']
+        for key in [
+            "CD",
+            "WV",
+            "WP",
+            "wt_lim",
+            "max_weight",
+            "F1_",
+            "F1_idle",
+            "F2_",
+            "F2_idle",
+            "bw",
+            "bv",
+            "Lt",
+            "Ut",
+            "Vt",
+            "Fract_CNG",
+            "grg_area",
+            "off_area",
+            "grg_enrg",
+            "off_enrg",
+            "Lb",
+        ]:
+            col_data[:, col_i] = self.InputData.Col[key]["amount"]
             col_columns.append(key)
             col_i += 1
 
-        self.col = pd.DataFrame(data=col_data,
-                                columns=col_columns,
-                                index=['RWC', 'SSR', 'DSR', 'MSR',
-                                       'SSYW', 'SSO', 'ORG', 'DryRes', 'REC',
-                                        'WetRes', 'MSRDO'],
-                                dtype=float)
+        self.col = pd.DataFrame(
+            data=col_data,
+            columns=col_columns,
+            index=[
+                "RWC",
+                "SSR",
+                "DSR",
+                "MSR",
+                "SSYW",
+                "SSO",
+                "SSO_AnF",
+                "ORG",
+                "DryRes",
+                "REC",
+                "WetRes",
+                "MSRDO",
+            ],
+            dtype=float,
+        )
 
-        self.col['Fract_Dies'] = 1 - self.InputData.Col['Fract_CNG']['amount']
+        self.col["Fract_Dies"] = 1 - self.InputData.Col["Fract_CNG"]["amount"]
 
         self._col_schm = {
-            'RWC': {'Contribution': 0,
-                    'separate_col':{'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0}},
-            'ORG_DryRes': {'Contribution': 0,
-                           'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0}},
-            'REC_WetRes': {'Contribution': 0,
-                           'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0}}}
+            "RWC": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSO_AnF": 0,
+                },
+            },
+            "ORG_DryRes": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSO_AnF": 0,
+                },
+            },
+            "REC_WetRes": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSO_AnF": 0,
+                },
+            },
+        }
 
         for k, v in self.col_schm.items():
-            if k[0] == 'RWC':
-                self._col_schm['RWC']['Contribution'] += v
-            elif k[0] == 'ORG_DryRes':
-                self._col_schm['ORG_DryRes']['Contribution'] += v
-            elif k[0] == 'REC_WetRes':
-                self._col_schm['REC_WetRes']['Contribution'] += v
+            if k[0] == "RWC":
+                self._col_schm["RWC"]["Contribution"] += v
+            elif k[0] == "ORG_DryRes":
+                self._col_schm["ORG_DryRes"]["Contribution"] += v
+            elif k[0] == "REC_WetRes":
+                self._col_schm["REC_WetRes"]["Contribution"] += v
             else:
-                raise Exception(f'Error in collection scheme keys: "{k[0]}" is not defined!')
+                raise ValueError(f'Error in collection scheme keys: "{k[0]}" is not defined!')
 
         for k, v in self.col_schm.items():
             if v > 0:
-                if k[1] not in ['N/A', 'ORG_DryRes', 'REC_WetRes']:
-                    self._col_schm[k[0]]['separate_col'][k[1]] += v / self._col_schm[k[0]]['Contribution']
-                if k[2] not in ['N/A', 'ORG_DryRes', 'REC_WetRes']:
-                    self._col_schm[k[0]]['separate_col'][k[2]] += v / self._col_schm[k[0]]['Contribution']
-
-        # Single Family Residential Waste Generation Rate (kg/household-week)
-        g_res = 7 * self.InputData.Col['res_per_dwel']['amount'] * self.InputData.Col['res_gen']['amount']
-        gen_per_week = g_res * self.process_data['Comp']
+                if k[1] not in ["N/A", "ORG_DryRes", "REC_WetRes"]:
+                    self._col_schm[k[0]]["separate_col"][k[1]] += (
+                        v / self._col_schm[k[0]]["Contribution"]
+                    )
+                if k[2] not in ["N/A", "ORG_DryRes", "REC_WetRes"]:
+                    self._col_schm[k[0]]["separate_col"][k[2]] += (
+                        v / self._col_schm[k[0]]["Contribution"]
+                    )
+
+        # Commercial Waste Generation Rate (kg/location-week)
+        g_res = self.InputData.Col["comm_gen"]["amount"]
+        gen_per_week = g_res * self.process_data["Comp"]
         total_waste_gen = (
-            g_res
-            * self.InputData.Col['houses_res']['amount']
-            * 365 / 7 / 1000)  # 52 weeks per year & 1000 kg = 1 Mg
+            g_res * self.InputData.Col["comm_loc"]["amount"] * 365 / 7 / 1000
+        )  # 52 weeks per year & 1000 kg = 1 Mg
 
         # Total fraction where this service is offered
         self.col_proc = {
-            'RWC': self._col_schm['RWC']['Contribution'],
-            'ORG': self._col_schm['ORG_DryRes']['Contribution'],
-            'DryRes': self._col_schm['ORG_DryRes']['Contribution'],
-            'REC': self._col_schm['REC_WetRes']['Contribution'],
-            'WetRes': self._col_schm['REC_WetRes']['Contribution']}
+            "RWC": self._col_schm["RWC"]["Contribution"],
+            "ORG": self._col_schm["ORG_DryRes"]["Contribution"],
+            "DryRes": self._col_schm["ORG_DryRes"]["Contribution"],
+            "REC": self._col_schm["REC_WetRes"]["Contribution"],
+            "WetRes": self._col_schm["REC_WetRes"]["Contribution"],
+        }
 
-        for i in ['SSR', 'DSR', 'MSR', 'MSRDO', 'SSYW', 'SSO']:
+        for i in ["SSR", "DSR", "MSR", "MSRDO", "SSYW", "SSO", "SSO_AnF"]:
             self.col_proc[i] = 0
-            for j in ['RWC', 'ORG_DryRes', 'REC_WetRes']:
+            for j in ["RWC", "ORG_DryRes", "REC_WetRes"]:
                 self.col_proc[i] += (
-                    self._col_schm[j]['Contribution']
-                    * self._col_schm[j]['separate_col'][i])
+                    self._col_schm[j]["Contribution"] * self._col_schm[j]["separate_col"][i]
+                )
 
         # Is this collection process offered? (1: in use, 0: not used)
         self.P_use = {}
         for j in self.col_proc.keys():
             self.P_use[j] = 1 if self.col_proc[j] > 0 else 0
 
         # Mass separated by collection process (kg/week.Household)
-        columns = ['RWC', 'SSR', 'DSR', 'MSR', 'SSYW', 'SSO',
-                   'ORG', 'DryRes', 'REC', 'WetRes',
-                   'MSRDO']
-        self.mass = pd.DataFrame(index=self.Index,
-                                 columns=columns,
-                                 data=0.0,
-                                 dtype=float)
-
-        for i in ['SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'ORG', 'REC', 'MSRDO']:
-            self.mass[i] = (
-                gen_per_week.values
-                * self.process_data[i].values
-                * self.P_use[i])
+        columns = [
+            "RWC",
+            "SSR",
+            "DSR",
+            "MSR",
+            "SSYW",
+            "SSO",
+            "SSO_AnF",
+            "ORG",
+            "DryRes",
+            "REC",
+            "WetRes",
+            "MSRDO",
+        ]
+        self.mass = pd.DataFrame(index=self.Index, columns=columns, data=0.0, dtype=float)
 
+        for i in ["SSR", "DSR", "MSR", "SSYW", "SSO", "SSO_AnF", "ORG", "REC", "MSRDO"]:
+            self.mass[i] = gen_per_week.values * self.process_data[i].values * self.P_use[i]
 
         def separate_col_mass(j):
             mass = np.zeros(len(self.CommonData.Index))
-            for i in ['SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'MSRDO']:
-                mass += self.mass[i].values * self._col_schm[j]['separate_col'][i]
+            for i in ["SSR", "DSR", "MSR", "SSYW", "SSO", "SSO_AnF", "MSRDO"]:
+                mass += self.mass[i].values * self._col_schm[j]["separate_col"][i]
             return mass
 
         # Calculating the residual waste after separate collection
-        self.mass['RWC']= (
-            gen_per_week.values
-            * self.process_data['RWC'].values
-            - separate_col_mass('RWC')) * self.P_use['RWC']
+        self.mass["RWC"] = (
+            gen_per_week.values * self.process_data["RWC"].values - separate_col_mass("RWC")
+        ) * self.P_use["RWC"]
 
         # ORG_DryRes
-        self.mass['DryRes']= (
-            (gen_per_week.values
-             * self.process_data['DryRes'].values
-             - separate_col_mass('ORG_DryRes')
-             - self.mass['ORG'].values) * self.P_use['DryRes'])
+        self.mass["DryRes"] = (
+            gen_per_week.values * self.process_data["DryRes"].values
+            - separate_col_mass("ORG_DryRes")
+            - self.mass["ORG"].values
+        ) * self.P_use["DryRes"]
 
         # REC_WetRes
-        self.mass['WetRes'] = (
-            gen_per_week.values
-            * self.process_data['WetRes'].values
-            - separate_col_mass('REC_WetRes')
-            - self.mass['REC'].values) * self.P_use['WetRes']
+        self.mass["WetRes"] = (
+            gen_per_week.values * self.process_data["WetRes"].values
+            - separate_col_mass("REC_WetRes")
+            - self.mass["REC"].values
+        ) * self.P_use["WetRes"]
 
         # Annual Mass Flows (Mg/yr)
         self.col_massflow = pd.DataFrame(index=self.Index)
         for i in columns:
-            self.col_massflow[i] = (self.mass[i]
-                                    * self.InputData.Col['houses_res']['amount']
-                                    * 365 / 7 / 1000
-                                    * self.col_proc[i])
+            self.col_massflow[i] = (
+                self.mass[i]
+                * self.InputData.Col["comm_loc"]["amount"]
+                * 365
+                / 7
+                / 1000
+                * self.col_proc[i]
+            )
 
         # Check for negative mass flows
         if (self.col_massflow.values < 0).any().any():
-            raise Exception(f'Negative mass flows in collection model [{self.process_name}]!')
-            # warnings.warn('Negative mass flows in collection model [{self.process_name}]!')
+            raise ValueError(f"Negative mass flows in collection model [{self.process_name}]!")
 
         # Check generated mass = Collected mass
         ratio = self.col_massflow.sum().sum() / total_waste_gen
         if ratio > 1.01 or ratio < 0.99:
-            raise Exception(f'Mass balance error in collection model [{self.process_name}]!')
-            # warnings.warn(f'Mass balance error in collection model [{self.process_name}]!')
+            raise ValueError(f"Mass balance error in collection model [{self.process_name}]!")
 
         # Volume Composition of each collection process for each sector
-        mass_to_cyd = (1 / (self.process_data['Bulk_Density'].values + 0.000001)
-                       * 1.30795)  # m3 --> Cubic yard
-        mass_to_cyd[self.process_data['Bulk_Density'].values <= 0] = 0.0
+        mass_to_cyd = (
+            1 / (self.process_data["Bulk_Density"].values + 0.000001) * 1.30795
+        )  # m3 --> Cubic yard
+        mass_to_cyd[self.process_data["Bulk_Density"].values <= 0] = 0.0
 
-        for i in ['RWC', 'SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'MSRDO']:
+        for i in ["RWC", "SSR", "DSR", "MSR", "SSYW", "SSO", "SSO_AnF", "MSRDO"]:
             vol = (self.mass[i].values * mass_to_cyd).sum()  # Unit kg/cyd
             if vol > 0:
-                self.col.loc[i, 'den_c'] = (self.mass[i].values
-                                            * 2.205 / vol).sum()  # Unit lb/cyd
+                self.col.loc[i, "den_c"] = (self.mass[i].values * 2.205 / vol).sum()  # Unit lb/cyd
             else:
-                self.col.loc[i, 'den_c'] = 0
+                self.col.loc[i, "den_c"] = 0
 
-        for i, j in [('ORG', 'DryRes'), ('REC', 'WetRes')]:
+        for i, j in [("ORG", "DryRes"), ("REC", "WetRes")]:
             m = self.mass[i].values + self.mass[j].values
             vol = (m * mass_to_cyd).sum()  # Unit kg/cyd
             if vol > 0:
-                self.col.loc[i, 'den_c'] = (m * 2.205 / vol).sum()  # Unit lb/cyd
+                self.col.loc[i, "den_c"] = (m * 2.205 / vol).sum()  # Unit lb/cyd
             else:
-                self.col.loc[i, 'den_c'] = 0
+                self.col.loc[i, "den_c"] = 0
 
     def find_destination(self, product, Treatment_processes):
         destination = {}
         for P in Treatment_processes:
-            if product in Treatment_processes[P]['input_type']:
+            if product in Treatment_processes[P]["input_type"]:
                 destination[P] = (
-                    self.Distance.Distance[(self.process_name, P)]['Heavy Duty Truck']
-                    / 1.60934)  # Convert the distance from km to mile
+                    self.Distance.Distance[(self.process_name, P)]["Heavy Duty Truck"] / 1.60934
+                )  # Convert the distance from km to mile
         return destination
 
     # calculating LCI and cost for different locations
     def calc_destin(self):
         if self.Treat_proc:
             self.dest = {}
             self.result_destination = {}
 
-            Collection_Index = ['RWC', 'SSR', 'DSR', 'MSR', 'SSYW',
-                                'SSO', 'ORG', 'DryRes', 'REC', 'WetRes',
-                                'MSRDO']
+            Collection_Index = [
+                "RWC",
+                "SSR",
+                "DSR",
+                "MSR",
+                "SSYW",
+                "SSO",
+                "SSO_AnF",
+                "ORG",
+                "DryRes",
+                "REC",
+                "WetRes",
+                "MSRDO",
+            ]
             for i in Collection_Index:
                 self.dest[i] = self.find_destination(i, self.Treat_proc)
                 self.result_destination[i] = {}
 
             # Number of times we need to run the collection
             n_run = max([len(self.dest[i]) for i in self.dest.keys()])
 
             for i in range(n_run):
-                for j in ['RWC', 'SSR', 'DSR', 'MSR', 'MSRDO', 'SSYW',
-                          'SSO', 'MSRDO', 'ORG', 'REC']:
+                for j in [
+                    "RWC",
+                    "SSR",
+                    "DSR",
+                    "MSR",
+                    "MSRDO",
+                    "SSYW",
+                    "SSO",
+                    "SSO_AnF",
+                    "MSRDO",
+                    "ORG",
+                    "REC",
+                ]:
                     if len(self.dest[j]) > i:
                         # Distance btwn collection route and destination
-                        self.col['Drf'][j] = self.dest[j][list(self.dest[j].keys())[i]]
+                        self.col["Drf"][j] = self.dest[j][list(self.dest[j].keys())[i]]
 
                         # Distance between destination and garage
-                        self.col['Dfg'][j] = (
-                            self.dest[j][list(self.dest[j].keys())[i]]
-                            + self.col['Dgr'][j])
+                        self.col["Dfg"][j] = (
+                            self.dest[j][list(self.dest[j].keys())[i]] + self.col["Dgr"][j]
+                        )
 
                 self.calc_lci()
                 for j in self.dest.keys():
                     if len(self.dest[j]) > i:
                         key = list(self.dest[j].keys())[i]
                         self.result_destination[j][key] = {}
 
-                        self.result_destination[j][key][('Technosphere', 'Equipment_Diesel')] = (
-                            self.output['FuelMg'][j]
-                            + self.output['FuelMg_dov'][j])
-
-                        self.result_destination[j][key][('Technosphere', 'Equipment_CNG')] = (
-                            self.output['FuelMg_CNG'][j])
-
-                        self.result_destination[j][key][('Technosphere', 'Electricity_consumption')] = (
-                            self.output['ElecMg'][j])
-
-                        self.result_destination[j][key][('biosphere3', 'Operational_Cost')] = (
-                            self.output['C_collection'][j])
+                        self.result_destination[j][key][("Technosphere", "Equipment_Diesel")] = (
+                            self.output["FuelMg"][j] + self.output["FuelMg_dov"][j]
+                        )
+
+                        self.result_destination[j][key][
+                            ("Technosphere", "Equipment_CNG")
+                        ] = self.output["FuelMg_CNG"][j]
+
+                        self.result_destination[j][key][
+                            ("Technosphere", "Electricity_consumption")
+                        ] = self.output["ElecMg"][j]
+
+                        self.result_destination[j][key][
+                            ("biosphere3", "Operational_Cost")
+                        ] = self.output["C_collection"][j]
         else:
             self.calc_lci()
             self.result_destination = {}
 
     def calc_lci(self):
         # Selected compartment compaction density  (lb/yd3)
         # Override calculated density den_c and use an average assumed in-truck density
-        d_msw = self.col['den_asmd'].values
-        d_msw[d_msw <= 0] = self.col['den_c'].values[d_msw <= 0]
-        self.col['d_msw'] = d_msw
+        d_msw = self.col["den_asmd"].values
+        d_msw[d_msw <= 0] = self.col["den_c"].values[d_msw <= 0]
+        self.col["d_msw"] = d_msw
 
         # Travel time between service stops, adjusted based on participation (min/stop)
-        self.col['Tbtw'] = self.col['Dbtw'].values / self.col['Vbet'].values * 60
+        self.col["Tbtw"] = self.col["Dbtw"].values / self.col["Vbet"].values * 60
 
         # Travel time btwn route and disposal fac. (min/trip)
-        self.col['Trf'] = self.col['Drf'].values / self.col['Vrf'].values * 60
+        self.col["Trf"] = self.col["Drf"].values / self.col["Vrf"].values * 60
 
         # Time from grg to 1st collection route (min/day-vehicle)
-        self.col['Tgr'] = self.col['Dgr'].values / self.col['Vgr'].values * 60
+        self.col["Tgr"] = self.col["Dgr"].values / self.col["Vgr"].values * 60
 
         # Time from disposal fac. to garage (min/day-vehicle)
-        self.col['Tfg'] = self.col['Dfg'].values / self.col['Vfg'].values * 60
+        self.col["Tfg"] = self.col["Dfg"].values / self.col["Vfg"].values * 60
 
-        for i in ['RWC', 'SSR', 'DSR', 'MSR',
-                  'SSYW', 'SSO', 'MSRDO']:
-            self.col.loc[i, 'mass'] = self.mass[i].values.sum()
+        for i in ["RWC", "SSR", "DSR", "MSR", "SSYW", "SSO", "SSO_AnF", "MSRDO"]:
+            self.col.loc[i, "mass"] = self.mass[i].values.sum()
 
         # Mass of ORG_DryRes and REC_WetRec
-        for i, j in [('ORG', 'DryRes'), ('REC', 'WetRes')]:
-            self.col.loc[i, 'mass'] = (self.mass[i].values + self.mass[j].values).sum()
+        for i, j in [("ORG", "DryRes"), ("REC", "WetRes")]:
+            self.col.loc[i, "mass"] = (self.mass[i].values + self.mass[j].values).sum()
 
         # Calculations for collection vehicle activities
         # Houses per trip (Volume limited) and (mass limited)
         Ht_v = np.zeros(self.col.shape[0])
         Ht_m = np.zeros(self.col.shape[0])
 
-        fltr = self.col['mass'].values > 0
+        fltr = self.col["mass"].values > 0
         Ht_v[fltr] = (
-            self.col['Ut'].values[fltr]
-            * self.col['Vt'].values[fltr]
-            * self.col['d_msw'].values[fltr]
+            self.col["Ut"].values[fltr]
+            * self.col["Vt"].values[fltr]
+            * self.col["d_msw"].values[fltr]
             * 0.4536  # lb to kg
-            * self.col['Fr'].values[fltr]
-            / self.col['mass'].values[fltr])
+            * self.col["Fr"].values[fltr]
+            / self.col["mass"].values[fltr]
+        )
 
         Ht_m[fltr] = (
-            self.col['max_weight'].values[fltr]
-            * self.col['Fr'].values[fltr]
+            self.col["max_weight"].values[fltr]
+            * self.col["Fr"].values[fltr]
             * 1000
-            / self.col['mass'].values[fltr])
+            / self.col["mass"].values[fltr]
+        )
 
-        self.col['Ht_v'] = Ht_v
-        self.col['Ht_m'] = Ht_m
+        self.col["Ht_v"] = Ht_v
+        self.col["Ht_m"] = Ht_m
 
         # Households per trip (limited by mass or volume)
-        Ht = self.col['Ht_v'].values
-        fltr_2 = self.col['wt_lim'].values == 1
-        fltr_3 = Ht[fltr_2] > self.col['Ht_m'].values[fltr_2]
-        Ht[fltr_2][fltr_3] = self.col['Ht_m'].values[fltr_3]
-        self.col['Ht'] = Ht
+        Ht = self.col["Ht_v"].values
+        fltr_2 = self.col["wt_lim"].values == 1
+        fltr_3 = Ht[fltr_2] > self.col["Ht_m"].values[fltr_2]
+        Ht[fltr_2][fltr_3] = self.col["Ht_m"].values[fltr_3]
+        self.col["Ht"] = Ht
 
         # Time per trip (min/trip)
         # Collection
-        self.col['Tc'] = (
-            self.col['Tbtw'].values * (self.col['Ht'].values / self.col['HS'].values - 1)  # collection travel
-            + self.col['TL'].values * self.col['Ht'].values / self.col['HS'].values  # collection loading
-            + 2 * self.col['Trf'].values  # travel
-            + self.col['S'].values)  # unload time
+        self.col["Tc"] = (
+            self.col["Tbtw"].values
+            * (self.col["Ht"].values / self.col["HS"].values - 1)  # collection travel
+            + self.col["TL"].values
+            * self.col["Ht"].values
+            / self.col["HS"].values  # collection loading
+            + 2 * self.col["Trf"].values  # travel
+            + self.col["S"].values
+        )  # unload time
 
         # Trips per day per vehicle (trip/day-vehicle)
-        self.col['RD'] = (
-            self.col['WV'].values * 60
-            - (self.col['F1_'].values + self.col['F2_'].values + self.col['Tfg'].values)
-            - 0.5 * (self.col['Trf'].values + self.col['S'].values)) / self.col['Tc'].values
+        self.col["RD"] = (
+            self.col["WV"].values * 60
+            - (self.col["F1_"].values + self.col["F2_"].values + self.col["Tfg"].values)
+            - 0.5 * (self.col["Trf"].values + self.col["S"].values)
+        ) / self.col["Tc"].values
 
         # Check that the inputs are realistic
-        if any(self.col['RD'].values < 0):
-            raise Exception("Travelling time is too long that the truck cannot make a loop trip in one day!")
+        if any(self.col["RD"].values < 0):
+            raise ValueError(
+                "Traveling time is too long that the truck cannot make a loop trip in one day!"
+            )
 
         # Daily weight of refuse collected per vehicle (Mg/vehicle-day)
-        self.col['RefD'] = (
-            self.col['Ht'].values
-            * self.col['mass'].values / 1000
-            / self.col['Fr'].values
-            * self.col['RD'].values)
+        self.col["RefD"] = (
+            self.col["Ht"].values
+            * self.col["mass"].values
+            / 1000
+            / self.col["Fr"].values
+            * self.col["RD"].values
+        )
 
         # Number of collection stops per day (stops/vehicle-day)
-        self.col['SD'] = (
-            self.col['Ht'].values
-            * self.col['RD'].values
-            / self.col['HS'].values)
+        self.col["SD"] = self.col["Ht"].values * self.col["RD"].values / self.col["HS"].values
 
         # Calculations for collection vehicle activities (Drop off)
-        for i in ['MSRDO']:
+        for i in ["MSRDO"]:
             # volume of recyclables deposited at drop-off site per week (cy/week-house)
-            self.col.loc[i, 'Ht'] = (
+            self.col.loc[i, "Ht"] = (
                 self.mass[i].values.sum()
-                * self.InputData.Col['houses_res']['amount']
+                * self.InputData.Col["comm_loc"]["amount"]
                 * self.col_proc[i]
                 / 0.4536  # lb to kg
-                / self.col['d_msw'][i])
+                / self.col["d_msw"][i]
+            )
 
             # collection vehicle trips per week (trips/week)
-            self.col.loc[i, 'DO_trip_week'] = (
-                self.col['Ht'][i]
-                / (self.col['Vt'][i] * self.col['Ut'][i]))
+            self.col.loc[i, "DO_trip_week"] = self.col["Ht"][i] / (
+                self.col["Vt"][i] * self.col["Ut"][i]
+            )
 
             # time per trip (min/trip) -- load+travel+unload time
-            self.col.loc[i, 'Tc'] = (
-                self.col['TL'][i]
-                + 2 * self.col['Trf'][i]
-                + self.col['S'][i])
+            self.col.loc[i, "Tc"] = self.col["TL"][i] + 2 * self.col["Trf"][i] + self.col["S"][i]
 
             # trips per day per vehicle (trip/day-vehicle)
-            self.col.loc[i, 'RD'] = (
-                self.col['WV'][i] * 60
-                - (self.col['F1_'][i]
-                   + self.col['F2_'][i]
-                   + self.col['Tfg'][i]
-                   + self.col['Tgr'][i])
-                + self.col['Trf'][i]) / self.col['Tc'][i]
+            self.col.loc[i, "RD"] = (
+                self.col["WV"][i] * 60
+                - (
+                    self.col["F1_"][i]
+                    + self.col["F2_"][i]
+                    + self.col["Tfg"][i]
+                    + self.col["Tgr"][i]
+                )
+                + self.col["Trf"][i]
+            ) / self.col["Tc"][i]
 
             # daily weight of refuse collected per vehicle (tons/day-vehicle)
-            self.col.loc[i, 'RefD'] = (
-                self.col['Vt'][i]
-                * self.col['Ut'][i]
-                * self.col['d_msw'][i]
+            self.col.loc[i, "RefD"] = (
+                self.col["Vt"][i]
+                * self.col["Ut"][i]
+                * self.col["d_msw"][i]
                 * 0.4536  # lb to kg
                 / 1000  # kg to Mg
-                * self.col['RD'][i])
+                * self.col["RD"][i]
+            )
 
             # number of collection stops per day (stops/vehicle-day) (1 stop per trip)
-            self.col.loc[i, 'SD'] = self.col['RD'][i]
+            self.col.loc[i, "SD"] = self.col["RD"][i]
 
         # Daily collection vehicle activity times
         # loading time at collection stops (min/day-vehicle) & loading time at drop-off site (min/day-vehicle)
-        self.col['LD'] = self.col['SD'].values * self.col['TL'].values
+        self.col["LD"] = self.col["SD"].values * self.col["TL"].values
 
         # travel time between collection stops (min/day-vehicle)
-        fltr_3 = self.col['SD'].values - 1 >= 1
+        fltr_3 = self.col["SD"].values - 1 >= 1
         Tb = np.zeros(self.col.shape[0])
-        Tb[fltr_3] = (self.col['SD'].values[fltr_3] - 1) * self.col['Tbtw'].values[fltr_3]
-        self.col['Tb'] = Tb
+        Tb[fltr_3] = (self.col["SD"].values[fltr_3] - 1) * self.col["Tbtw"].values[fltr_3]
+        self.col["Tb"] = Tb
 
         # travel time between route and disposal facility (min/day-vehicle)
-        self.col['F_R'] = (2 * self.col['RD'].values + 0.5) * self.col['Trf'].values
+        self.col["F_R"] = (2 * self.col["RD"].values + 0.5) * self.col["Trf"].values
 
         # unloading time at disposal facility (min/day-vehicle)
-        self.col['UD'] = (self.col['RD'].values + 0.5) * self.col['S'].values
+        self.col["UD"] = (self.col["RD"].values + 0.5) * self.col["S"].values
 
-        for i in ['MSRDO']:
-            self.col.loc[i, 'Tb'] = 0
+        for i in ["MSRDO"]:
+            self.col.loc[i, "Tb"] = 0
 
             # travel time between disposal facility and drop-off site (min/day-vehicle)
-            self.col.loc[i, 'F_R'] = (2 * self.col['RD'][i] - 1) * self.col['Trf'][i]
+            self.col.loc[i, "F_R"] = (2 * self.col["RD"][i] - 1) * self.col["Trf"][i]
 
             # unloading time at disposal facility (min/day-vehicle)
-            self.col.loc[i, 'UD'] = self.col['RD'][i] * self.col['S'][i]
-
+            self.col.loc[i, "UD"] = self.col["RD"][i] * self.col["S"][i]
 
         # Daily fuel usage - Diesel
-        fltr_4 = self.col['MPG_all'].values != 0
+        fltr_4 = self.col["MPG_all"].values != 0
 
         # from garage to first collection route (gallons/day-vehicle)
         diesel_gr = (
-            self.col['Fract_Dies'].values
-            * self.col['Dgr'].values
-            *((1 - self.col['fDgr'].values)
-              / self.col['MPG_urban'].values
-              + self.col['fDgr'].values
-              /self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["Dgr"].values
+            * (
+                (1 - self.col["fDgr"].values) / self.col["MPG_urban"].values
+                + self.col["fDgr"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_gr[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dgr'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
-
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dgr"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         # break time, if spent idling
         diesel_idl = (
-            self.col['Fract_Dies'].values
-            * (self.col['F1_'].values
-               * self.col['F1_idle'].values
-               + self.col['F2_'].values
-               * self.col['F2_idle'].values)
+            self.col["Fract_Dies"].values
+            * (
+                self.col["F1_"].values * self.col["F1_idle"].values
+                + self.col["F2_"].values * self.col["F2_idle"].values
+            )
             / 60
-            * self.col['GPH_idle_cv'].values)
+            * self.col["GPH_idle_cv"].values
+        )
 
         diesel_idl[fltr_4] = 0
 
         # from first through last collection stop (gallons/day-vehicle)
         diesel_col = (
-            self.col['Fract_Dies'].values
-            * self.col['Dbtw'].values
-            * self.col['SD'].values
-            / self.col['MPG_collection'].values)
+            self.col["Fract_Dies"].values
+            * self.col["Dbtw"].values
+            * self.col["SD"].values
+            / self.col["MPG_collection"].values
+        )
 
         diesel_col[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dbtw'].values[fltr_4]
-            * self.col['SD'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dbtw"].values[fltr_4]
+            * self.col["SD"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
-
-        index_dict = dict(zip(self.col.index,
-                              np.arange(len(self.col.index))))
+        index_dict = dict(zip(self.col.index, np.arange(len(self.col.index))))
         fltr_DO = [False for i in self.col.index]
-        for i in ['MSRDO']:
+        for i in ["MSRDO"]:
             fltr_DO[index_dict[i]] = True
         diesel_col[fltr_DO] = 0
 
-       # between disposal facility and route (gallons/day-vehicle)
+        # between disposal facility and route (gallons/day-vehicle)
         diesel_rf = (
-            self.col['Fract_Dies'].values
-            * self.col['F_R'].values / 60
-            * self.col['Vrf'].values
-            * ((1 - self.col['fDrd'].values) / self.col['MPG_urban'].values
-               + self.col['fDrd'].values / self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["F_R"].values
+            / 60
+            * self.col["Vrf"].values
+            * (
+                (1 - self.col["fDrd"].values) / self.col["MPG_urban"].values
+                + self.col["fDrd"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_rf[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['F_R'].values[fltr_4] / 60
-            * self.col['Vrf'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["F_R"].values[fltr_4]
+            / 60
+            * self.col["Vrf"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         # unloading at disposal facility (gallons/day-vehicle)
         diesel_ud = (
-            self.col['Fract_Dies'].values
-            * self.col['UD'].values / 60
-            * self.col['GPH_idle_cv'].values)
+            self.col["Fract_Dies"].values
+            * self.col["UD"].values
+            / 60
+            * self.col["GPH_idle_cv"].values
+        )
 
         diesel_ud[fltr_4] = 0
 
-       # from disposal facility to garage (gallons/day-vehicle)
+        # from disposal facility to garage (gallons/day-vehicle)
         diesel_fg = (
-            self.col['Fract_Dies'].values
-            * self.col['Dfg'].values
-            * ((1 - self.col['fDfg'].values) / self.col['MPG_urban'].values
-               + self.col['fDfg'].values / self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["Dfg"].values
+            * (
+                (1 - self.col["fDfg"].values) / self.col["MPG_urban"].values
+                + self.col["fDfg"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_fg[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dfg'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dfg"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
         FuelD = pd.Series(
-            (diesel_gr + diesel_idl + diesel_col
-             + diesel_rf + diesel_ud + diesel_fg),
-             index=self.col.index)
-
+            (diesel_gr + diesel_idl + diesel_col + diesel_rf + diesel_ud + diesel_fg),
+            index=self.col.index,
+        )
         for key, val in self.col_proc.items():
             if val == 0:
                 FuelD[key] = 0
 
-        self.col['FuelD'] = FuelD
+        self.col["FuelD"] = FuelD
 
         # Daily fuel usage - CNG - diesel gal equivalent
-        fltr_6 = self.col['MPG_all_CNG'].values != 0
+        fltr_6 = self.col["MPG_all_CNG"].values != 0
 
         # from garage to first collection route ((diesel gal equivalent/day-vehicle)
         CNG_gr = (
-            self.col['Fract_CNG'].values
-            * self.col['Dgr'].values
-            *((1 - self.col['fDgr'].values)
-              / self.col['MPG_urban_CNG'].values
-              + self.col['fDgr'].values
-              /self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["Dgr"].values
+            * (
+                (1 - self.col["fDgr"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDgr"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_gr[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dgr'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
-
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dgr"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         # break time, if spent idling
         CNG_idl = (
-            self.col['Fract_CNG'].values
-            * (self.col['F1_'].values
-               * self.col['F1_idle'].values
-               + self.col['F2_'].values
-               * self.col['F2_idle'].values)
+            self.col["Fract_CNG"].values
+            * (
+                self.col["F1_"].values * self.col["F1_idle"].values
+                + self.col["F2_"].values * self.col["F2_idle"].values
+            )
             / 60
-            * self.col['GPH_idle_CNG'].values)
+            * self.col["GPH_idle_CNG"].values
+        )
 
         CNG_idl[fltr_6] = 0
 
         # from first through last collection stop (diesel gal equivalent/day-vehicle)
         CNG_col = (
-            self.col['Fract_CNG'].values
-            * self.col['Dbtw'].values
-            * self.col['SD'].values
-            / self.col['MPG_col_CNG'].values)
+            self.col["Fract_CNG"].values
+            * self.col["Dbtw"].values
+            * self.col["SD"].values
+            / self.col["MPG_col_CNG"].values
+        )
 
         CNG_col[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dbtw'].values[fltr_6]
-            * self.col['SD'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dbtw"].values[fltr_6]
+            * self.col["SD"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         CNG_col[fltr_DO] = 0
 
-       # between disposal facility and route (diesel gal equivalent/day-vehicle)
+        # between disposal facility and route (diesel gal equivalent/day-vehicle)
         CNG_rf = (
-            self.col['Fract_CNG'].values
-            * self.col['F_R'].values / 60
-            * self.col['Vrf'].values
-            * ((1 - self.col['fDrd'].values) / self.col['MPG_urban_CNG'].values
-               + self.col['fDrd'].values / self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["F_R"].values
+            / 60
+            * self.col["Vrf"].values
+            * (
+                (1 - self.col["fDrd"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDrd"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_rf[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['F_R'].values[fltr_6] / 60
-            * self.col['Vrf'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["F_R"].values[fltr_6]
+            / 60
+            * self.col["Vrf"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         # unloading at disposal facility (diesel gal equivalent/day-vehicle)
         CNG_ud = (
-            self.col['Fract_CNG'].values
-            * self.col['UD'].values / 60
-            * self.col['GPH_idle_CNG'].values)
+            self.col["Fract_CNG"].values
+            * self.col["UD"].values
+            / 60
+            * self.col["GPH_idle_CNG"].values
+        )
 
         CNG_ud[fltr_6] = 0
 
-       # from disposal facility to garage (diesel gal equivalent/day-vehicle)
+        # from disposal facility to garage (diesel gal equivalent/day-vehicle)
         CNG_fg = (
-            self.col['Fract_CNG'].values
-            * self.col['Dfg'].values
-            * ((1 - self.col['fDfg'].values) / self.col['MPG_urban_CNG'].values
-               + self.col['fDfg'].values / self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["Dfg"].values
+            * (
+                (1 - self.col["fDfg"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDfg"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_fg[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dfg'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dfg"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         FuelD_CNG = pd.Series(
-            (CNG_gr + CNG_idl + CNG_col
-             + CNG_rf + CNG_ud + CNG_fg),
-             index=self.col.index)
+            (CNG_gr + CNG_idl + CNG_col + CNG_rf + CNG_ud + CNG_fg), index=self.col.index
+        )
 
         for key, val in self.col_proc.items():
             if val == 0:
                 FuelD_CNG[key] = 0
 
-        self.col['FuelD_CNG'] = FuelD_CNG
+        self.col["FuelD_CNG"] = FuelD_CNG
 
         # ENERGY CONSUMPTION
         # Energy consumption by collection vehicles
         # total coll. vehicle fuel use per Mg of refuse (L/Mg)
         FuelMg = np.zeros(self.col.shape[0])
-        flter_7 = self.col['RefD'].values > 0
+        flter_7 = self.col["RefD"].values > 0
         FuelMg[flter_7] = (
-            self.col['FuelD'].values[flter_7]
+            self.col["FuelD"].values[flter_7]
             * 3.785  # gal to ltr
-            / self.col['RefD'].values[flter_7])
-        self.col['FuelMg'] = FuelMg
+            / self.col["RefD"].values[flter_7]
+        )
+        self.col["FuelMg"] = FuelMg
 
         # total coll. vehicle CNG fuel use per Mg of refuse (diesel L equivalent/Mg)
         FuelMg_CNG = np.zeros(self.col.shape[0])
         FuelMg_CNG[flter_7] = (
-            self.col['FuelD_CNG'].values[flter_7]
+            self.col["FuelD_CNG"].values[flter_7]
             * 3.785  # gal to ltr
-            / self.col['RefD'].values[flter_7])
-        self.col['FuelMg_CNG'] = FuelMg_CNG
+            / self.col["RefD"].values[flter_7]
+        )
+        self.col["FuelMg_CNG"] = FuelMg_CNG
 
         # Energy consumption by drop-off vehicles
         P_use_Seri = pd.Series(index=self.col.index)
         col_proc_Seri = pd.Series(index=self.col.index)
-        self.col_proc
+
         for key, val in index_dict.items():
             P_use_Seri[val] = self.P_use[key]
             col_proc_Seri[val] = self.col_proc[key]
 
         # fuel usage per trip to drop-off site (gallons/trip)
         FuelT = np.zeros(self.col.shape[0])
         FuelT[fltr_DO] = (
             P_use_Seri.values[fltr_DO]
-            * self.col['RTDdos'].values[fltr_DO]
-            * self.col['DED'].values[fltr_DO]
-            / self.col['dropoff_MPG'].values[fltr_DO] )
-        self.col['FuelT'] = FuelT
+            * self.col["RTDdos"].values[fltr_DO]
+            * self.col["DED"].values[fltr_DO]
+            / self.col["dropoff_MPG"].values[fltr_DO]
+        )
+        self.col["FuelT"] = FuelT
 
-        for i in ['MSRDO']:
+        for i in ["MSRDO"]:
             # weight of refuse delivered per trip (kg/trip)
-            self.col.loc[i, 'RefT'] = (
+            self.col.loc[i, "RefT"] = (
                 self.mass[i].values.sum()
-                * self.col['Prtcp'][i]
-                * 365 / 7
-                / (self.col['FREQdos'][i] * 12))
+                * self.col["Prtcp"][i]
+                * 365
+                / 7
+                / (self.col["FREQdos"][i] * 12)
+            )
 
         # total dropoff vehicle  fuel use per Mg of refuse (L/Mg)
         FuelMg_dov = np.zeros(self.col.shape[0])
-        flter_8 = self.col['RefT'].values > 0
+        flter_8 = self.col["RefT"].values > 0
         FuelMg_dov[flter_8] = (
-            self.col['FuelT'].values[flter_8]
+            self.col["FuelT"].values[flter_8]
             * 3.785  # gal to ltr
-            / (self.col['RefT'].values[flter_8] / 1000))
-        self.col['FuelMg_dov'] = FuelMg_dov
+            / (self.col["RefT"].values[flter_8] / 1000)
+        )
+        self.col["FuelMg_dov"] = FuelMg_dov
 
         # Energy consumption by garage
         # daily electricity usage per vehicle  (kWh/vehicle-day)
-        self.col['ElecD'] = (
-            P_use_Seri.values
-            * (self.col['grg_area'].values * self.col['grg_enrg'].values
-               + self.col['off_area'].values * self.col['off_enrg'].values))
+        self.col["ElecD"] = P_use_Seri.values * (
+            self.col["grg_area"].values * self.col["grg_enrg"].values
+            + self.col["off_area"].values * self.col["off_enrg"].values
+        )
 
         # electricity usage per Mg of refuse  (kWh/Mg)
         ElecMg = np.zeros(self.col.shape[0])
-        ElecMg[flter_7] = (
-            self.col['ElecD'].values[flter_7]
-            / self.col['RefD'].values[flter_7])
-        self.col['ElecMg'] =  ElecMg
+        ElecMg[flter_7] = self.col["ElecD"].values[flter_7] / self.col["RefD"].values[flter_7]
+        self.col["ElecMg"] = ElecMg
 
         # Mass
         # total mass of refuse collected per year (Mg)
-        self.col['TotalMass'] = self.col_massflow.sum()
+        self.col["TotalMass"] = self.col_massflow.sum()
 
         # COLLECTION COSTS
         # Breakdown of capital costs
 
         # annual capital cost per vehicle ($/vehicle-year)
-        self.col['C_cap_v'] = (
-            (1 + self.col['e'].values)
-            * npf.pmt(self.InputData.LCC['Discount_rate']['amount'],
-                      self.col['Lt'].values,
-                      -self.col['Pt'].values))
+        self.col["C_cap_v"] = (1 + self.col["e"].values) * npf.pmt(
+            self.InputData.LCC["Discount_rate"]["amount"],
+            self.col["Lt"].values,
+            -self.col["Pt"].values,
+        )
 
         # number of collection vehicles (vehicles)
-        self.col['Nt'] = (
-            self.InputData.Col['houses_res']['amount']
+        self.col["Nt"] = (
+            self.InputData.Col["comm_loc"]["amount"]
             * col_proc_Seri.values
-            * self.col['Fr'].values
-            / (self.col['Ht'].values
-               * self.col['RD'].values
-               * self.col['CD'].values))
+            * self.col["Fr"].values
+            / (self.col["Ht"].values * self.col["RD"].values * self.col["CD"].values)
+        )
 
         # annualized capital cost per bin ($/bin-year)
-        self.col['Cb'] = (
-            (1 + self.col['e'].values)
-            * npf.pmt(self.InputData.LCC['Discount_rate']['amount'],
-                      self.col['Lb'].values,
-                      -self.col['Pb'].values))
+        self.col["Cb"] = (1 + self.col["e"].values) * npf.pmt(
+            self.InputData.LCC["Discount_rate"]["amount"],
+            self.col["Lb"].values,
+            -self.col["Pb"].values,
+        )
 
         # no. of bins per vehicle (bins/vehicle)
-        self.col['Nb'] = (
-            self.col['Rb'].values
-            * (self.col['Ht'].values / self.col['HS'].values)
-            * self.col['RD'].values
-            * self.col['CD'].values
-            / self.col['Fr'].values)
+        self.col["Nb"] = (
+            self.col["Rb"].values
+            * (self.col["Ht"].values / self.col["Prtcp"].values)
+            * self.col["RD"].values
+            * self.col["CD"].values
+            / self.col["Fr"].values
+        )
 
         # bin annual cost per vehicle ($/vehicle-year)
-        self.col['C_cap_b'] = (
-            self.col['Cb'].values * self.col['Nb'].values)
+        self.col["C_cap_b"] = self.col["Cb"].values * self.col["Nb"].values
 
         # Breakdown of operating costs
         # labor cost per vehicle ($/vehicle-year)
-        self.col['Cw'] = (
-            (1 + self.col['a'].values)
-            * ((1 + self.col['bw'].values)
-               * (self.col['Wa'].values * self.col['Nw'].values
-                  + self.col['Wd'].values)
-               * self.col['WP'].values
-               * self.col['CD'].values
-               * 365 / 7))
+        self.col["Cw"] = (1 + self.col["a"].values) * (
+            (1 + self.col["bw"].values)
+            * (self.col["Wa"].values * self.col["Nw"].values + self.col["Wd"].values)
+            * self.col["WP"].values
+            * self.col["CD"].values
+            * 365
+            / 7
+        )
 
         # O&M cost per vehicle ($/vehicle-year)
-        self.col['Cvo'] = self.col['c'].values
+        self.col["Cvo"] = self.col["c"].values
 
         # other expenses per vehicle ($/vehicle-year)
-        self.col['Coe'] = self.col['d'].values * (self.col['Nw'].values + 1)
+        self.col["Coe"] = self.col["d"].values * (self.col["Nw"].values + 1)
 
         # Annual operating cost ($/vehicle-year)
-        self.col['C_op'] = (
-            (1 + self.col['e'].values)
-            * (self.col['Cw'].values
-               + self.col['Cvo'].values
-               + self.col['Coe'].values))
+        self.col["C_op"] = (1 + self.col["e"].values) * (
+            self.col["Cw"].values + self.col["Cvo"].values + self.col["Coe"].values
+        )
 
         # Total annual cost per vehicle -- cap + O&M ($/vehicle-year)
-        self.col['C_vehicle'] = (
-            (1 + self.col['bv'].values)
-            * self.col['C_cap_v'].values
-            + self.col['C_op'].values)
+        self.col["C_vehicle"] = (1 + self.col["bv"].values) * self.col["C_cap_v"].values + self.col[
+            "C_op"
+        ].values
 
         # Total annual cost per house, including bins ($/house-year)
         # Includes all houses provided service, even if not participating
-        hpdv = (self.col['Ht'].values
-                * self.col['RD'].values
-                * self.col['CD'].values
-                / self.col['Fr'].values)
+        hpdv = (
+            self.col["Ht"].values
+            * self.col["RD"].values
+            * self.col["CD"].values
+            / self.col["Fr"].values
+        )
 
         fltr_9 = hpdv > 0.0
 
         C_house = np.zeros(self.col.shape[0])
 
         C_house[fltr_9] = (
-            self.col['C_vehicle'].values[fltr_9]
-            / hpdv[fltr_9]
-            * self.col['Prtcp'].values[fltr_9])
+            self.col["C_vehicle"].values[fltr_9] / hpdv[fltr_9] * self.col["Prtcp"].values[fltr_9]
+        )
 
-        C_house += (self.col['Cb'].values * self.col['Rb'].values)
+        C_house += self.col["Cb"].values * self.col["Rb"].values
         C_house[np.isnan(C_house)] = 0.0
-        self.col['C_house'] = C_house
+        self.col["C_house"] = C_house
 
         # ☻ ton of refuse collected - Cap+OM+bins ($/Mg)
-        self.col['C_collection'] = (
-            (self.col['C_house'] * 7 / 365)
-            / (self.mass.sum() / 1000)).replace([np.inf, np.nan], 0)
+        self.col["C_collection"] = (
+            (self.col["C_house"] * 7 / 365) / (self.mass.sum() / 1000)
+        ).replace([np.inf, np.nan], 0)
 
         # OUTPUT
-        # Energy use is calculated for ORG and it is same with Dryres
-        self.col.loc['DryRes', 'FuelMg'] = self.col['FuelMg']['ORG']
-        self.col.loc['DryRes', 'FuelMg_CNG'] = self.col['FuelMg_CNG']['ORG']
-        self.col.loc['DryRes', 'ElecMg'] = self.col['ElecMg']['ORG']
+        # Energy use is calculated for ORG and it is same with Dryers
+        self.col.loc["DryRes", "FuelMg"] = self.col["FuelMg"]["ORG"]
+        self.col.loc["DryRes", "FuelMg_CNG"] = self.col["FuelMg_CNG"]["ORG"]
+        self.col.loc["DryRes", "ElecMg"] = self.col["ElecMg"]["ORG"]
 
         # Energy use is calculated for REC and it is same with WetRes
-        self.col.loc['WetRes', 'FuelMg'] = self.col['FuelMg']['REC']
-        self.col.loc['WetRes', 'FuelMg_CNG'] = self.col['FuelMg_CNG']['REC']
-        self.col.loc['WetRes', 'ElecMg'] = self.col['ElecMg']['REC']
-
-
-        self.output = self.col[['TotalMass', 'FuelMg', 'FuelMg_CNG',
-                                'ElecMg', 'FuelMg_dov', 'C_collection']]
+        self.col.loc["WetRes", "FuelMg"] = self.col["FuelMg"]["REC"]
+        self.col.loc["WetRes", "FuelMg_CNG"] = self.col["FuelMg_CNG"]["REC"]
+        self.col.loc["WetRes", "ElecMg"] = self.col["ElecMg"]["REC"]
+
+        self.output = self.col[
+            ["TotalMass", "FuelMg", "FuelMg_CNG", "ElecMg", "FuelMg_dov", "C_collection"]
+        ]
         self.output = self.output.fillna(0.0)
 
     def calc(self):
         self.calc_composition()
         self.calc_destin()
 
     # setup for Monte Carlo simulation
@@ -893,21 +1047,19 @@
 
     def report(self):
         # report
         self.collection = {}
         Waste = {}
         Technosphere = {}
         Biosphere = {}
-        self.collection["process name"] = (self.process_name,
-                                           self.Process_Type,
-                                           self.__class__)
+        self.collection["process name"] = (self.process_name, self.Process_Type, self.__class__)
         self.collection["Waste"] = Waste
         self.collection["Technosphere"] = Technosphere
         self.collection["Biosphere"] = Biosphere
-        self.collection['LCI'] = self.result_destination
+        self.collection["LCI"] = self.result_destination
 
         for x in [Waste, Technosphere, Biosphere]:
             for y in self.Index:
                 x[y] = {}
 
         for y in self.Index:
             for x in self.col_massflow.columns:
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/MRF_subprocess.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/MRF_subprocess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,134 +1,153 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Tue Jan  7 11:12:21 2020
-
-@author: msardar2
-"""
 import numpy as np
 import numpy_financial as npf
 
 
 ### Resource use calculation for equipments
 def calc_resource(total_throughput, remaining, removed, Eqpt, InputData, LCI):
-    #Calculating resource use
-    #Elec use = (motor_size*Frac_motor)/(max_input*frac_input)  --> unit: kW/Mg
-    elec = Eqpt['motor']['amount'] * Eqpt['frac_motor']['amount'] / \
-                (Eqpt['Max_input']['amount'] * Eqpt['frac_MaxInput']['amount'])
-
-    if Eqpt['Calc_base']['amount'] == 0: # 0: calculation based on the removed mass
-        Aloc = (removed / sum(removed) if sum(removed) > 0 else 0)
-    elif Eqpt['Calc_base']['amount'] == 1: # 1: calculation based on the remaining mass
-        Aloc = (remaining / sum(remaining) if sum(remaining) > 0 else 0)
-    elif Eqpt['Calc_base']['amount'] == 2:  # 2: calculation based on the total throughput mass
-        Aloc = (total_throughput / sum(total_throughput) if sum(total_throughput) > 0 else 0)
-    else:
-        raise ValueError('Input parameter [Calc_base] is not valid')
-
-    elec_use =  sum(total_throughput) * elec *  Aloc
-    dsl_use = sum(total_throughput) * Eqpt['diesel_use']['amount'] * Aloc
-    LPG_use = sum(total_throughput) * Eqpt['LPG_use']['amount'] * Aloc
-
-    Cap = Eqpt['Investment_cost']['amount'] + Eqpt['Installation_cost']['amount']
-    Rate = InputData.Constr_cost['Inerest_rate']['amount']
-    Lftime = Eqpt['LifeTime']['amount']
+    # Calculating resource use
+    # Elec use = (motor_size*Frac_motor)/(max_input*frac_input)  --> unit: kW/Mg
+    elec = (
+        Eqpt["motor"]["amount"]
+        * Eqpt["frac_motor"]["amount"]
+        / (Eqpt["Max_input"]["amount"] * Eqpt["frac_MaxInput"]["amount"])
+    )
+
+    if Eqpt["Calc_base"]["amount"] == 0:  # 0: calculation based on the removed mass
+        Aloc = removed / sum(removed) if sum(removed) > 0 else 0
+    elif Eqpt["Calc_base"]["amount"] == 1:  # 1: calculation based on the remaining mass
+        Aloc = remaining / sum(remaining) if sum(remaining) > 0 else 0
+    elif Eqpt["Calc_base"]["amount"] == 2:  # 2: calculation based on the total throughput mass
+        Aloc = total_throughput / sum(total_throughput) if sum(total_throughput) > 0 else 0
+    else:
+        raise ValueError("Input parameter [Calc_base] is not valid")
+
+    elec_use = sum(total_throughput) * elec * Aloc
+    dsl_use = sum(total_throughput) * Eqpt["diesel_use"]["amount"] * Aloc
+    LPG_use = sum(total_throughput) * Eqpt["LPG_use"]["amount"] * Aloc
+
+    Cap = Eqpt["Investment_cost"]["amount"] + Eqpt["Installation_cost"]["amount"]
+    Rate = InputData.Constr_cost["Interest_rate"]["amount"]
+    Lifetime = Eqpt["LifeTime"]["amount"]
     TotalHour = (
-        InputData.Labor['Hr_shift']['amount']
-        * InputData.Labor['Shift_day']['amount']
-        * InputData.Labor['Day_year']['amount'])
+        InputData.Labor["Hr_shift"]["amount"]
+        * InputData.Labor["Shift_day"]["amount"]
+        * InputData.Labor["Day_year"]["amount"]
+    )
 
     # Average Cost of Ownership ($/Mg)
-    AveCostOwner = (
-        (npf.pmt(Rate, Lftime, -Cap) + Eqpt['O&M']['amount'])
-        / (TotalHour * Eqpt['Max_input']['amount'] * Eqpt['frac_MaxInput']['amount']))
+    AveCostOwner = (npf.pmt(Rate, Lifetime, -Cap) + Eqpt["O&M"]["amount"]) / (
+        TotalHour * Eqpt["Max_input"]["amount"] * Eqpt["frac_MaxInput"]["amount"]
+    )
 
     # Laborers Required (Sorter*hours/Mg)
-    LaborReq = Eqpt['N_Labor']['amount'] / (Eqpt['Max_input']['amount'] * Eqpt['frac_MaxInput']['amount'])
+    LaborReq = Eqpt["N_Labor"]["amount"] / (
+        Eqpt["Max_input"]["amount"] * Eqpt["frac_MaxInput"]["amount"]
+    )
     # Drivers Required (Driver*hours/Mg)
-    DriverReq = Eqpt['N_Driver']['amount'] / (Eqpt['Max_input']['amount'] * Eqpt['frac_MaxInput']['amount'])
+    DriverReq = Eqpt["N_Driver"]["amount"] / (
+        Eqpt["Max_input"]["amount"] * Eqpt["frac_MaxInput"]["amount"]
+    )
     # Labor (sorter+Driver) Cost ($/Mg input)
-    LaborCost = (LaborReq * InputData.Labor['Labor_rate']['amount'] + DriverReq * InputData.Labor['Driver_rate']['amount']) *\
-                (1 + InputData.Labor['Fringe_rate']['amount']) * (1 + InputData.Labor['Management_rate']['amount'])
+    LaborCost = (
+        (
+            LaborReq * InputData.Labor["Labor_rate"]["amount"]
+            + DriverReq * InputData.Labor["Driver_rate"]["amount"]
+        )
+        * (1 + InputData.Labor["Fringe_rate"]["amount"])
+        * (1 + InputData.Labor["Management_rate"]["amount"])
+    )
 
     TotalOMcost = sum(total_throughput) * Aloc * (AveCostOwner + LaborCost)
 
     # adding the resource use
-    LCI.add(('Technosphere', 'Electricity_consumption'), elec_use)
-    LCI.add(('Technosphere', 'Equipment_Diesel'), dsl_use)
-    LCI.add(('Technosphere', 'Equipment_LPG'), LPG_use)
-    LCI.add(('biosphere3', 'Operational_Cost'), TotalOMcost)
+    LCI.add(("Technosphere", "Electricity_consumption"), elec_use)
+    LCI.add(("Technosphere", "Equipment_Diesel"), dsl_use)
+    LCI.add(("Technosphere", "Equipment_LPG"), LPG_use)
+    LCI.add(("biosphere3", "Operational_Cost"), TotalOMcost)
+
 
 ### Drum Feeder
 def Drum_Feeder(Input, InputData, LCI):
-    #Mass Calculation
+    # Mass Calculation
     feed = Input
 
-    #Equipment input
+    # Equipment input
     Eqpt = InputData.Eq_DFeeder
 
-    #Resource use calculation
-    calc_resource(Input, Input, Input, Eqpt, InputData, LCI) # For Drum Feeder removed, remaining and throughput are same.
+    # Resource use calculation
+    calc_resource(
+        Input, Input, Input, Eqpt, InputData, LCI
+    )  # For Drum Feeder removed, remaining and throughput are same.
 
     return feed
 
+
 ### Flail Mill
 def Flail_Mill(Input, InputData, LCI):
     # Mass Calculation
     feed = Input
 
     # Equipment input
     Eqpt = InputData.Eq_FMill
 
     # Resource use calculation
-    calc_resource(Input, Input, Input, Eqpt, InputData, LCI) # For Drum Feeder removed, remaining and throughput are same.
+    calc_resource(
+        Input, Input, Input, Eqpt, InputData, LCI
+    )  # For Drum Feeder removed, remaining and throughput are same.
 
     return feed
 
+
 ### Trommel for separating <2"
 def Trommel(Input, sep_eff, InputData, LCI):
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
     Eqpt = InputData.Eq_Trommel
 
     # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Negative sort
 def Neg_Sort(Input, sep_eff, InputData, LCI):
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
     Eqpt = InputData.Eq_Neg_Sort
 
     # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Negative/positive sort
 def Sorting(Input, sep_eff, InputData, Eqpt_data, LCI):
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
     Eqpt = Eqpt_data
 
-    #Resource use calculation
+    # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Air Separator
 def Air_Sep(Input, sep_eff, InputData, LCI):
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
@@ -150,509 +169,567 @@
     Eqpt = InputData.Eq_Opt_Sort
 
     # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Shredder
 def Shredder(Input, InputData, LCI):
     # Mass Calculation
     feed = Input
 
     # Equipment input
     Eqpt = InputData.Eq_Shred
 
     # Resource use calculation
     # For Shredders removed, remaining and throughput are same.
     calc_resource(Input, Input, Input, Eqpt, InputData, LCI)
 
     return feed
 
+
 ### Pelletizer
 def Pelletizer(Input, InputData, LCI):
     # Mass Calculation
     feed = Input
 
     # Equipment input
     Eqpt = InputData.Eq_Pellet
 
     # Resource use calculation
     # For Shredders removed, remaining and throughput are same.
     calc_resource(Input, Input, Input, Eqpt, InputData, LCI)
 
     return feed
 
+
 ### Manual Sort 1 (Negative) for separating the plastic film
 def Man_Sort1(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
+    # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
-    #Equipment input
+    # Equipment input
     Eqpt = InputData.Eq_MS1
 
-    #Resource use calculation
+    # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Vacuum
 def Vacuum(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['Film']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["Film"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_Vac
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['Film']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["Film"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_Vac_Manual
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['Film']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Film"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Resource use calculation
-    if InputData.Rec_material['Film']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["Film"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
 
 ### Disc Screen 1: OCC separation
 def DS1(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['OCC']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["OCC"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_DS1
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['OCC']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["OCC"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_DS1_Manual
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['OCC']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["OCC"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Resource use calculation
-    if InputData.Rec_material['OCC']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["OCC"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### ### Disc Screen 2: Newspaper separation
 def DS2(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_DS2
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['Non_OCC_Fiber']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["Non_OCC_Fiber"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_DS2_Manual
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Resource use calculation
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
 
 ### Disc Screen 3: Fiber separation
 def DS3(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_DS3
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['Non_OCC_Fiber']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["Non_OCC_Fiber"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_DS3_Manual
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Resource use calculation
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
 
 ###  ### Manual Sort 2-DS2 (Negative)
 def MS2_DS2(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS2_DS2
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
 
-
 ###  ### Manual Sort 2-DS3 (Negative)
 def MS2_DS3(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['Non_OCC_Fiber']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["Non_OCC_Fiber"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS2_DS3
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
     return remained, removed
 
+
 ### ### Baler_1Way: product is baled OCC and mixed fiber
 def Baler_1Way(OCC, Non_OCC_Fiber, InputData, LCI):
     # Mass Calculation
     baled = OCC + Non_OCC_Fiber
 
     # Equipment input
     Eqpt = InputData.Eq_Baler_1Way
     # Resource use calculation
     calc_resource(baled, baled, baled, Eqpt, InputData, LCI)
 
     # Wire use calculation
     # Bale volume
-    Volumne = Eqpt['Bale_Width']['amount'] * Eqpt['Bale_Length']['amount'] * Eqpt['Bale_Height']['amount']
-    #Bale Wire Length
-    Wire_len = Eqpt['Straps_Per_Bale']['amount'] * 2 * (Eqpt['Bale_Height']['amount'] + Eqpt['Bale_Width']['amount'])
+    Volume = (
+        Eqpt["Bale_Width"]["amount"] * Eqpt["Bale_Length"]["amount"] * Eqpt["Bale_Height"]["amount"]
+    )
+    # Bale Wire Length
+    Wire_len = (
+        Eqpt["Straps_Per_Bale"]["amount"]
+        * 2
+        * (Eqpt["Bale_Height"]["amount"] + Eqpt["Bale_Width"]["amount"])
+    )
     # Wire use
-    Wire_use = (OCC / InputData.Rec_BaleDens['OCC']['amount'] +
-                Non_OCC_Fiber / InputData.Rec_BaleDens['Non_OCC_Fiber']['amount'])\
-               / Volumne*Wire_len / InputData.Baler_Wire['Len_to_Mass']['amount']
-
-    #Wire Transportation
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'), Wire_use*InputData.Baler_Wire['Trans_HDDT']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Medium_Duty_Diesel_Truck'), Wire_use*InputData.Baler_Wire['Trans_MDDT']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Barge'), Wire_use*InputData.Baler_Wire['Trans_Barge']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Cargo_Ship'), Wire_use*InputData.Baler_Wire['Trans_CargoShip']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Rail'), Wire_use*InputData.Baler_Wire['Trans_Rail']['amount'])
+    Wire_use = (
+        (
+            OCC / InputData.Rec_BaleDens["OCC"]["amount"]
+            + Non_OCC_Fiber / InputData.Rec_BaleDens["Non_OCC_Fiber"]["amount"]
+        )
+        / Volume
+        * Wire_len
+        / InputData.Baler_Wire["Len_to_Mass"]["amount"]
+    )
+
+    # Wire Transportation
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"),
+        Wire_use * InputData.Baler_Wire["Trans_HDDT"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Medium_Duty_Diesel_Truck"),
+        Wire_use * InputData.Baler_Wire["Trans_MDDT"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Barge"),
+        Wire_use * InputData.Baler_Wire["Trans_Barge"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Cargo_Ship"),
+        Wire_use * InputData.Baler_Wire["Trans_CargoShip"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Rail"),
+        Wire_use * InputData.Baler_Wire["Trans_Rail"]["amount"],
+    )
 
-    #Add Wire use to LCI
-    LCI.add(('Technosphere', 'Wire'), Wire_use)
+    # Add Wire use to LCI
+    LCI.add(("Technosphere", "Wire"), Wire_use)
     return baled
 
+
 ### Baler
 def Baler(Input, InputData, LCI):
     # Mass Calculation
     baled = Input
 
     # Equipment input
     Eqpt = InputData.Eq_Baler
 
     # Resource use calculation
     calc_resource(baled, baled, baled, Eqpt, InputData, LCI)
 
     # Wire use calculation
     # Bale volume
-    Volumne = Eqpt['Bale_Width']['amount'] * Eqpt['Bale_Length']['amount'] * Eqpt['Bale_Height']['amount']
-    #Bale Wire Length
-    Wire_len = Eqpt['Straps_Per_Bale']['amount'] * 2 * (Eqpt['Bale_Height']['amount'] + Eqpt['Bale_Width']['amount'])
+    Volume = (
+        Eqpt["Bale_Width"]["amount"] * Eqpt["Bale_Length"]["amount"] * Eqpt["Bale_Height"]["amount"]
+    )
+    # Bale Wire Length
+    Wire_len = (
+        Eqpt["Straps_Per_Bale"]["amount"]
+        * 2
+        * (Eqpt["Bale_Height"]["amount"] + Eqpt["Bale_Width"]["amount"])
+    )
     # Wire use
-    Wire_use = (baled
-                / Eqpt['Bale_Density']['amount']
-                / Volumne
-                * Wire_len
-                / InputData.Baler_Wire['Len_to_Mass']['amount'])
-
-    #Wire Transportation
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'), Wire_use*InputData.Baler_Wire['Trans_HDDT']['amount'])
+    Wire_use = (
+        baled
+        / Eqpt["Bale_Density"]["amount"]
+        / Volume
+        * Wire_len
+        / InputData.Baler_Wire["Len_to_Mass"]["amount"]
+    )
+
+    # Wire Transportation
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"),
+        Wire_use * InputData.Baler_Wire["Trans_HDDT"]["amount"],
+    )
 
     # Add Wire use to LCI
-    LCI.add(('Technosphere', 'Wire'), Wire_use)
+    LCI.add(("Technosphere", "Wire"), Wire_use)
 
     return baled
 
+
 ### Glass Breaker Screen
 def GBS(Input, sep_eff, InputData, LCI):  # GBS is always in system and working
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
     Eqpt = InputData.Eq_GBS
     # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Air Knife
 def AK(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['Glass']['amount'] == 1:
+    # Mass Calculation
+    if InputData.Rec_material["Glass"]["amount"] == 1:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['Glass']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["Glass"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_AK
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Optical Glass
 def OG(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['Glass']['amount'] == 1:
+    # Mass Calculation
+    if InputData.Rec_material["Glass"]["amount"] == 1:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['Glass']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["Glass"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_OG
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Manual Sort 3-G (Negative)
 def MS3_G(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['Glass']['amount'] == 1:
+    # Mass Calculation
+    if InputData.Rec_material["Glass"]["amount"] == 1:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['Glass']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["Glass"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS3_G
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Secondary sort glass
 def Glass_type(Input, InputData):
-    #Mass Calculation
+    # Mass Calculation
     Res_Glass = np.zeros(Input.shape[0])
     Brown_glass = np.zeros(Input.shape[0])
     Clear_glass = np.zeros(Input.shape[0])
     Green_glass = np.zeros(Input.shape[0])
     Mixed_Glass = np.zeros(Input.shape[0])
 
-    if InputData.Rec_material['Glass']['amount'] == 0:
+    if InputData.Rec_material["Glass"]["amount"] == 0:
         Res_Glass = Input
     else:
-        if InputData.Rec_Sorted_material['Glass_Brown']['amount'] == 1:    # Brown_glass index = 33
+        if InputData.Rec_Sorted_material["Glass_Brown"]["amount"] == 1:  # Brown_glass index = 33
             Brown_glass[33] = Input[33]
 
-        if InputData.Rec_Sorted_material['Glass_Green']['amount'] == 1:    # Green_glass index = 34
+        if InputData.Rec_Sorted_material["Glass_Green"]["amount"] == 1:  # Green_glass index = 34
             Green_glass[34] = Input[34]
 
-        if InputData.Rec_Sorted_material['Glass_Clear']['amount'] == 1:    # Clear_glass index = 35
+        if InputData.Rec_Sorted_material["Glass_Clear"]["amount"] == 1:  # Clear_glass index = 35
             Clear_glass[35] = Input[35]
 
         Mixed_Glass = Input - (Brown_glass + Green_glass + Clear_glass)
 
     return Res_Glass, Brown_glass, Clear_glass, Green_glass, Mixed_Glass
 
+
 ### Optical PET
 def OPET(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['PET']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["PET"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_OPET
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['PET']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["PET"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_OSPET
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['PET']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["PET"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-
-    #Resource use calculation
-    if InputData.Rec_material['PET']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["PET"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Manual Sort 4-PET (Negative)
 def MS4_PET(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['PET']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["PET"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['PET']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["PET"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS4_PET
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Optical HDPE
 def OHDPE(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['HDPE']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["HDPE"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_OHDPE
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['HDPE']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["HDPE"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_OSHDPE
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['HDPE']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["HDPE"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Resource use calculation
-    if InputData.Rec_material['HDPE']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["HDPE"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Manual Sort 4-HDPE (Negative)
 def MS4_HDPE(Input, sep_eff, InputData, LCI):
     # Mass Calculation
-    if InputData.Rec_material['HDPE']['amount'] > 0:
+    if InputData.Rec_material["HDPE"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
     # Equipment input
-    if InputData.Rec_material['HDPE']['amount'] > 0: # Manual recovery
+    if InputData.Rec_material["HDPE"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS4_HDPE
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### HDPE sold by type?
-def HDPE_type(Input, InputData):
+def HDPE_type(Input):
     # Mass Calculation
     HDPE_P = np.zeros(Input.shape[0])
     HDPE_T = np.zeros(Input.shape[0])
 
     # HDPE - Pigmented Containers index 19
     HDPE_P[19] = Input[19]
 
-    #HDPE - Translucent Containers index 18
+    # HDPE - Translucent Containers index 18
     HDPE_T[18] = Input[18]
 
     return HDPE_P, HDPE_T
 
+
 ### Magnet
 def Magnet_RDF(Input, sep_eff, InputData, LCI):
     # Equipment input
     Eqpt = InputData.Eq_Magnet
 
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Magnet
 def Magnet(Input, sep_eff, InputData, LCI):
     # Equipment input
-    if InputData.Rec_material['Ferrous']['amount'] == 1: # Automatic recovery
+    if InputData.Rec_material["Ferrous"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_Magnet
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['Ferrous']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["Ferrous"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_Magnet_Manual
         sep_eff = sep_eff[:, 1]
 
     # Mass Calculation
-    if InputData.Rec_material['Ferrous']['amount'] > 0:
+    if InputData.Rec_material["Ferrous"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
     # Resource use calculation
-    if InputData.Rec_material['Ferrous']['amount'] > 0:
+    if InputData.Rec_material["Ferrous"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Manual Sort 4-Fe (Negative)
 def MS4_Fe(Input, sep_eff, InputData, LCI):
     # Mass Calculation
-    if InputData.Rec_material['Ferrous']['amount'] > 0:
+    if InputData.Rec_material["Ferrous"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
     # Equipment input
-    if InputData.Rec_material['Ferrous']['amount'] > 0: # Manual recovery
+    if InputData.Rec_material["Ferrous"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS4_Fe
         # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Eddy Current Separator
 def ECS(Input, sep_eff, InputData, LCI):
-    #Equipment input
-    if InputData.Rec_material['Aluminous']['amount'] == 1: # Automatic recovery
+    # Equipment input
+    if InputData.Rec_material["Aluminous"]["amount"] == 1:  # Automatic recovery
         Eqpt = InputData.Eq_ECS
         sep_eff = sep_eff[:, 0]
-    elif InputData.Rec_material['Aluminous']['amount'] == 2: # Manual recovery
+    elif InputData.Rec_material["Aluminous"]["amount"] == 2:  # Manual recovery
         Eqpt = InputData.Eq_ECS_Manual
         sep_eff = sep_eff[:, 1]
 
-    #Mass Calculation
-    if InputData.Rec_material['Aluminous']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Aluminous"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Resource use calculation
-    if InputData.Rec_material['Aluminous']['amount'] > 0:
+    # Resource use calculation
+    if InputData.Rec_material["Aluminous"]["amount"] > 0:
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Eddy Current Separator (ECS)
 def ECS_RDF(Input, sep_eff, InputData, Eqpt_data, LCI):
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
@@ -662,153 +739,194 @@
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
 
 ### Manual Sort 4-Al (Negative)
 def MS4_Al(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
-    if InputData.Rec_material['Aluminous']['amount'] > 0:
+    # Mass Calculation
+    if InputData.Rec_material["Aluminous"]["amount"] > 0:
         removed = Input * sep_eff
     else:
         removed = np.zeros(len(LCI.Index))
     remained = Input - removed
 
-    #Equipment input
-    if InputData.Rec_material['Aluminous']['amount'] > 0: # Manual recovery
+    # Equipment input
+    if InputData.Rec_material["Aluminous"]["amount"] > 0:  # Manual recovery
         Eqpt = InputData.Eq_MS4_Al
-        #Resource use calculation
+        # Resource use calculation
         calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Manual Sort 5 (Positive)
 def MS5(Input, sep_eff, InputData, LCI):
-    #Mass Calculation
+    # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
-    #Equipment input
+    # Equipment input
     Eqpt = InputData.Eq_MS5
-    #Resource use calculation
+    # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### 2-Way Baler: product is baled plastics and metals (container)
 def Baler_2Way(Input, InputData, LCI):
-    #Mass Calculation
+    # Mass Calculation
     baled = Input
 
-    #Equipment input
+    # Equipment input
     Eqpt = InputData.Eq_Baler_2Way
-    #Resource use calculation
+    # Resource use calculation
     calc_resource(baled, baled, baled, Eqpt, InputData, LCI)
 
-    #Density
-    Density = np.ones(len(LCI.index)) * 10**12 #using big density for non-recycab
-    Density[[28, 29, 30, 32]] = InputData.Rec_BaleDens['Aluminous']['amount']
-    Density[[26, 27, 31]] = InputData.Rec_BaleDens['Ferrous']['amount']
-    Density[[18, 19]] = InputData.Rec_BaleDens['HDPE']['amount']
-    Density[20] = InputData.Rec_BaleDens['PET']['amount']
-    Density[24] = InputData.Rec_BaleDens['Film']['amount']
-
-    #Wire use calculation
-    #Bale volume
-    Volumne = Eqpt['Bale_Width']['amount'] * Eqpt['Bale_Length']['amount'] * Eqpt['Bale_Height']['amount']
-    #Bale Wire Length
-    Wire_len = Eqpt['Straps_Per_Bale']['amount'] * 2 * (Eqpt['Bale_Height']['amount']+Eqpt['Bale_Width']['amount'])
-    #Wire use
-    Wire_use = (Input / Density) / Volumne * Wire_len / InputData.Baler_Wire['Len_to_Mass']['amount']
-
-    #Add Wire use to LCI
-    LCI.add(('Technosphere', 'Wire'), Wire_use)
-
-    #Wire Transportation
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'), Wire_use * InputData.Baler_Wire['Trans_HDDT']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Medium_Duty_Diesel_Truck'), Wire_use * InputData.Baler_Wire['Trans_MDDT']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Barge'), Wire_use * InputData.Baler_Wire['Trans_Barge']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Cargo_Ship'), Wire_use * InputData.Baler_Wire['Trans_CargoShip']['amount'])
-    LCI.add(('Technosphere', 'Internal_Process_Transportation_Rail'), Wire_use * InputData.Baler_Wire['Trans_Rail']['amount'])
+    # Density
+    Density = np.ones(len(LCI.index)) * 10**12  # using big density for non-recyclables
+    Density[[28, 29, 30, 32]] = InputData.Rec_BaleDens["Aluminous"]["amount"]
+    Density[[26, 27, 31]] = InputData.Rec_BaleDens["Ferrous"]["amount"]
+    Density[[18, 19]] = InputData.Rec_BaleDens["HDPE"]["amount"]
+    Density[20] = InputData.Rec_BaleDens["PET"]["amount"]
+    Density[24] = InputData.Rec_BaleDens["Film"]["amount"]
+
+    # Wire use calculation
+    # Bale volume
+    Volume = (
+        Eqpt["Bale_Width"]["amount"] * Eqpt["Bale_Length"]["amount"] * Eqpt["Bale_Height"]["amount"]
+    )
+    # Bale Wire Length
+    Wire_len = (
+        Eqpt["Straps_Per_Bale"]["amount"]
+        * 2
+        * (Eqpt["Bale_Height"]["amount"] + Eqpt["Bale_Width"]["amount"])
+    )
+    # Wire use
+    Wire_use = (Input / Density) / Volume * Wire_len / InputData.Baler_Wire["Len_to_Mass"]["amount"]
+
+    # Add Wire use to LCI
+    LCI.add(("Technosphere", "Wire"), Wire_use)
+
+    # Wire Transportation
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck"),
+        Wire_use * InputData.Baler_Wire["Trans_HDDT"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Medium_Duty_Diesel_Truck"),
+        Wire_use * InputData.Baler_Wire["Trans_MDDT"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Barge"),
+        Wire_use * InputData.Baler_Wire["Trans_Barge"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Cargo_Ship"),
+        Wire_use * InputData.Baler_Wire["Trans_CargoShip"]["amount"],
+    )
+    LCI.add(
+        ("Technosphere", "Internal_Process_Transportation_Rail"),
+        Wire_use * InputData.Baler_Wire["Trans_Rail"]["amount"],
+    )
 
     return baled
 
+
 ### Densimetric table
 def Densimetric_Table(Input, sep_eff, InputData, LCI):
     # Mass Calculation
     removed = Input * sep_eff
     remained = Input - removed
 
     # Equipment input
     Eqpt = InputData.Eq_DMT
     # Resource use calculation
     calc_resource(Input, remained, removed, Eqpt, InputData, LCI)
 
     return remained, removed
 
+
 ### Rolling_Stock
 def Rolling_Stock(Input, InputData, LCI):
-    #Equipment input
+    # Equipment input
     Eqpt = InputData.Eq_Rolling_Stock
-    #Resource use calculation
+    # Resource use calculation
     calc_resource(Input, Input, Input, Eqpt, InputData, LCI)
 
+
 ### Conveyor
 def Conveyor(Input, InputData, LCI):
-    #Equipment input
+    # Equipment input
     Eqpt = InputData.Eq_Conveyor
-    #Resource use calculation
+    # Resource use calculation
     calc_resource(Input, Input, Input, Eqpt, InputData, LCI)
 
+
 ### Secondary sort for mixed paper
 def Mixed_paper_separation(Input, InputData):
-    #Mass Calculation
+    # Mass Calculation
     ONP = np.zeros(Input.shape[0])
     OFF = np.zeros(Input.shape[0])
     Fiber_Other = np.zeros(Input.shape[0])
 
     # Separate Newsprint index is 9
-    if InputData.Rec_Sorted_material['Newsprint']['amount'] == 1:
-        ONP[9] = Input[9] * InputData.Rec_Sep_eff['Newsprint']['amount']
+    if InputData.Rec_Sorted_material["Newsprint"]["amount"] == 1:
+        ONP[9] = Input[9] * InputData.Rec_Sep_eff["Newsprint"]["amount"]
 
     # Separate Office Paper index is 11
-    if InputData.Rec_Sorted_material['Office_Paper']['amount'] == 1:
-        OFF[11] = Input[11] * InputData.Rec_Sep_eff['Office_Paper']['amount']
+    if InputData.Rec_Sorted_material["Office_Paper"]["amount"] == 1:
+        OFF[11] = Input[11] * InputData.Rec_Sep_eff["Office_Paper"]["amount"]
 
     # Separate Magazines index is 12
-    if InputData.Rec_Sorted_material['Magazines']['amount'] == 1:
-        Fiber_Other[12] = Input[12] * InputData.Rec_Sep_eff['Magazines']['amount']
+    if InputData.Rec_Sorted_material["Magazines"]["amount"] == 1:
+        Fiber_Other[12] = Input[12] * InputData.Rec_Sep_eff["Magazines"]["amount"]
 
     # Separate Third_Class_Mail index is 13
-    if InputData.Rec_Sorted_material['Third_Class_Mail']['amount'] == 1:
-        Fiber_Other[13] = Input[13] * InputData.Rec_Sep_eff['Third_Class_Mail']['amount']
+    if InputData.Rec_Sorted_material["Third_Class_Mail"]["amount"] == 1:
+        Fiber_Other[13] = Input[13] * InputData.Rec_Sep_eff["Third_Class_Mail"]["amount"]
 
     # Separate Folding_Containers index is 14
-    if InputData.Rec_Sorted_material['Folding_Containers']['amount'] == 1:
-        Fiber_Other[14] = Input[14] * InputData.Rec_Sep_eff['Folding_Containers']['amount']
+    if InputData.Rec_Sorted_material["Folding_Containers"]["amount"] == 1:
+        Fiber_Other[14] = Input[14] * InputData.Rec_Sep_eff["Folding_Containers"]["amount"]
 
     # Separate Paper_Bags index is 15
-    if InputData.Rec_Sorted_material['Paper_Bags']['amount'] == 1:
-        Fiber_Other[15] = Input[15] * InputData.Rec_Sep_eff['Paper_Bags']['amount']
+    if InputData.Rec_Sorted_material["Paper_Bags"]["amount"] == 1:
+        Fiber_Other[15] = Input[15] * InputData.Rec_Sep_eff["Paper_Bags"]["amount"]
 
     # Remaining the mixed Paper
     Mixed_Paper = Input - (ONP + OFF + Fiber_Other)
 
     # Check to not get negative numbers
     if min(Mixed_Paper) < 0:
-        raise ValueError('*** Mass Balance Error *** \n Check the separation efficiencies for secondary separation of Fiber.')
+        raise ValueError(
+            "*** Mass Balance Error *** \n Check the separation efficiencies for secondary separation of Fiber."
+        )
 
     return Mixed_Paper, ONP, OFF, Fiber_Other
 
+
 ### General Electricity
 def Electricity(Input, InputData, LCI):
-    #calculate electricity use in office and floor area
-    elec_office = Input * InputData.Electricity['Area_rate']['amount'] * InputData.Electricity['Frac_office']['amount'] * InputData.Electricity['Elec_office']['amount']
-    elec_floor = Input * InputData.Electricity['Area_rate']['amount'] * (1-InputData.Electricity['Frac_office']['amount']) * InputData.Electricity['Elec_floor']['amount']
-    LCI.add(('Technosphere', 'Electricity_consumption'), elec_office+elec_floor)
+    # calculate electricity use in office and floor area
+    elec_office = (
+        Input
+        * InputData.Electricity["Area_rate"]["amount"]
+        * InputData.Electricity["Frac_office"]["amount"]
+        * InputData.Electricity["Elec_office"]["amount"]
+    )
+    elec_floor = (
+        Input
+        * InputData.Electricity["Area_rate"]["amount"]
+        * (1 - InputData.Electricity["Frac_office"]["amount"])
+        * InputData.Electricity["Elec_floor"]["amount"]
+    )
+    LCI.add(("Technosphere", "Electricity_consumption"), elec_office + elec_floor)
+
 
 ### sterilizing the waste
 def Sterilizer(Input, InputData, LCI):
     # Mass Calculation
     feed = Input
 
     # Equipment input
@@ -816,39 +934,40 @@
 
     # Resource use calculation
     # For Sterilizer removed, remaining and throughput are same.
     calc_resource(Input, Input, Input, Eqpt, InputData, LCI)
 
     return feed
 
+
 ### Dewater
 def Dewater(Input, InputData, MaterialProperties, LCI):
     # Equipment input
     Eqpt = InputData.Eq_Dewater
-    
+
     # Mass Calculation
-    feed_moist = Input * MaterialProperties['Moisture Content'].values / 100
+    feed_moist = Input * MaterialProperties["Moisture Content"].values / 100
     feed_solid = Input - feed_moist
-    product = feed_solid / (1 - InputData.AnF_operation['Dew_moist']['amount'])
+    product = feed_solid / (1 - InputData.AnF_operation["Dew_moist"]["amount"])
     waste_water = Input - product
 
     # Resource use calculation
     calc_resource(Input, product, waste_water, Eqpt, InputData, LCI)
 
     return product, waste_water
 
 
 ### Dryer
 def Dryer(Input, InputData, LCI):
     # Equipment input
     Eqpt = InputData.Eq_Dryer
 
     # Mass Calculation
-    feed_moist = Input * InputData.AnF_operation['Dew_moist']['amount']
+    feed_moist = Input * InputData.AnF_operation["Dew_moist"]["amount"]
     feed_solid = Input - feed_moist
-    product = feed_solid / (1 - InputData.AnF_operation['Dried_moist']['amount'])
+    product = feed_solid / (1 - InputData.AnF_operation["Dried_moist"]["amount"])
     remove = Input - product
 
     # Resource use calculation
     calc_resource(Input, product, remove, Eqpt, InputData, LCI)
 
-    return product
+    return product
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/ProcessModel.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Tue Apr 21 21:31:49 2020
-
-@author: msmsa
-"""
 from abc import ABC, abstractmethod
+
 from swolfpy_inputdata import CommonData
 
 
 class ProcessModel(ABC):
     def __init__(self, process_name, CommonDataObjct):
         if CommonDataObjct:
             self.CommonData = CommonDataObjct
         else:
             self.CommonData = CommonData()
         self.process_name = process_name
 
         # Read Material properties
         self.Material_Properties = self.CommonData.Material_Properties
 
-
         self.Index = self.CommonData.Index
 
     @property
     @abstractmethod
     def Process_Type(self):
         pass
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/ProcessModelsMetaData.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/ProcessModelsMetaData.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 # -*- coding: utf-8 -*-
 
 ProcessModelsMetaData = {}
 
-ProcessModelsMetaData['AD'] = {}
-ProcessModelsMetaData['AD']['Name'] = 'Anaerobic Digestion'
-ProcessModelsMetaData['AD']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['AD']['File'] = 'AD.py'
-ProcessModelsMetaData['AD']['InputType'] = ['Separated_Organics', 'SSO']
-
-ProcessModelsMetaData['Comp'] = {}
-ProcessModelsMetaData['Comp']['Name'] = 'Composting'
-ProcessModelsMetaData['Comp']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['Comp']['File'] = 'Comp.py'
-ProcessModelsMetaData['Comp']['InputType'] = ['SSYW', 'SSO', 'SSYWDO', 'Separated_Organics']
-
-ProcessModelsMetaData['WTE'] = {}
-ProcessModelsMetaData['WTE']['Name'] = 'Waste To Energy'
-ProcessModelsMetaData['WTE']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['WTE']['File'] = 'WTE.py'
-ProcessModelsMetaData['WTE']['InputType'] = ['RWC', 'MRDO', 'Other_Residual']
-
-ProcessModelsMetaData['LF'] = {}
-ProcessModelsMetaData['LF']['Name'] = 'Landfill'
-ProcessModelsMetaData['LF']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['LF']['File'] = 'LF.py'
-ProcessModelsMetaData['LF']['InputType'] = ['RWC', 'MRDO', 'Other_Residual', 'Bottom_Ash',
-                                            'Fly_Ash', 'Unreacted_Ash']
-
-ProcessModelsMetaData['SS_MRF'] = {}
-ProcessModelsMetaData['SS_MRF']['Name'] = 'Single Stream Material Recovery Facility'
-ProcessModelsMetaData['SS_MRF']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['SS_MRF']['File'] = 'SS_MRF.py'
-ProcessModelsMetaData['SS_MRF']['InputType'] = ['SSR', 'Separated_Recyclables']
-
-ProcessModelsMetaData['Reproc'] = {}
-ProcessModelsMetaData['Reproc']['Name'] = 'Reprocessing'
-ProcessModelsMetaData['Reproc']['Process_Type'] = 'Reprocessing'
-ProcessModelsMetaData['Reproc']['File'] = 'Reproc.py'
-ProcessModelsMetaData['Reproc']['InputType'] = ['Al','Fe',
-                                                'OCC', 'Mixed_Paper', 'ONP', 'OFF', 'Fiber_Other',
-                                                'Brown_glass', 'Clear_glass', 'Green_glass', 'Mixed_Glass',
-                                                'PET', 'HDPE_P', 'HDPE_T', 'LDPE_Film']
-
-ProcessModelsMetaData['SF_Col'] = {}
-ProcessModelsMetaData['SF_Col']['Name'] = 'Single Family Collection'
-ProcessModelsMetaData['SF_Col']['Process_Type'] = 'Collection'
-ProcessModelsMetaData['SF_Col']['File'] = 'SF_Col.py'
-ProcessModelsMetaData['SF_Col']['InputType'] = []
-
-ProcessModelsMetaData['MF_Col'] = {}
-ProcessModelsMetaData['MF_Col']['Name'] = 'Multi-Family Collection'
-ProcessModelsMetaData['MF_Col']['Process_Type'] = 'Collection'
-ProcessModelsMetaData['MF_Col']['File'] = 'MF_Col.py'
-ProcessModelsMetaData['MF_Col']['InputType'] = []
-
-ProcessModelsMetaData['COM_Col'] = {}
-ProcessModelsMetaData['COM_Col']['Name'] = 'Commercial Collection'
-ProcessModelsMetaData['COM_Col']['Process_Type'] = 'Collection'
-ProcessModelsMetaData['COM_Col']['File'] = 'COM_Col.py'
-ProcessModelsMetaData['COM_Col']['InputType'] = []
-
-ProcessModelsMetaData['TS'] = {}
-ProcessModelsMetaData['TS']['Name'] = 'Transfer Station'
-ProcessModelsMetaData['TS']['Process_Type'] = 'Transfer_Station'
-ProcessModelsMetaData['TS']['File'] = 'TS.py'
-ProcessModelsMetaData['TS']['InputType'] = ['DryRes', 'WetRes', 'ORG', 'REC']
-
-ProcessModelsMetaData['HC'] = {}
-ProcessModelsMetaData['HC']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['HC']['Name'] = 'Home Composting'
-ProcessModelsMetaData['HC']['File'] = 'HC.py'
-ProcessModelsMetaData['HC']['InputType'] = ['SSO_HC']
-
-ProcessModelsMetaData['GC'] = {}
-ProcessModelsMetaData['GC']['Process_Type'] = 'RDF'
-ProcessModelsMetaData['GC']['Name'] = 'Gasification Syngas Combustion'
-ProcessModelsMetaData['GC']['File'] = 'GC.py'
-ProcessModelsMetaData['GC']['InputType'] = ['RDF']
-
-ProcessModelsMetaData['RDF'] = {}
-ProcessModelsMetaData['RDF']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['RDF']['Name'] = 'Refuse-Derived Fuel'
-ProcessModelsMetaData['RDF']['File'] = 'RDF.py'
-ProcessModelsMetaData['RDF']['InputType'] = ['RWC', 'MRDO']
-
-ProcessModelsMetaData['AnF'] = {}
-ProcessModelsMetaData['AnF']['Process_Type'] = 'Treatment'
-ProcessModelsMetaData['AnF']['Name'] = 'Animal Feed'
-ProcessModelsMetaData['AnF']['File'] = 'AnF.py'
-ProcessModelsMetaData['AnF']['InputType'] = ['SSO_AnF']
-
+ProcessModelsMetaData["AD"] = {}
+ProcessModelsMetaData["AD"]["Name"] = "Anaerobic Digestion"
+ProcessModelsMetaData["AD"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["AD"]["File"] = "AD.py"
+ProcessModelsMetaData["AD"]["InputType"] = ["Separated_Organics", "SSO"]
+
+ProcessModelsMetaData["Comp"] = {}
+ProcessModelsMetaData["Comp"]["Name"] = "Composting"
+ProcessModelsMetaData["Comp"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["Comp"]["File"] = "Comp.py"
+ProcessModelsMetaData["Comp"]["InputType"] = ["SSYW", "SSO", "SSYWDO", "Separated_Organics"]
+
+ProcessModelsMetaData["WTE"] = {}
+ProcessModelsMetaData["WTE"]["Name"] = "Waste To Energy"
+ProcessModelsMetaData["WTE"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["WTE"]["File"] = "WTE.py"
+ProcessModelsMetaData["WTE"]["InputType"] = ["RWC", "MRDO", "Other_Residual"]
+
+ProcessModelsMetaData["LF"] = {}
+ProcessModelsMetaData["LF"]["Name"] = "Landfill"
+ProcessModelsMetaData["LF"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["LF"]["File"] = "LF.py"
+ProcessModelsMetaData["LF"]["InputType"] = [
+    "RWC",
+    "MRDO",
+    "Other_Residual",
+    "Bottom_Ash",
+    "Fly_Ash",
+    "Unreacted_Ash",
+]
+
+ProcessModelsMetaData["SS_MRF"] = {}
+ProcessModelsMetaData["SS_MRF"]["Name"] = "Single Stream Material Recovery Facility"
+ProcessModelsMetaData["SS_MRF"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["SS_MRF"]["File"] = "SS_MRF.py"
+ProcessModelsMetaData["SS_MRF"]["InputType"] = ["SSR", "Separated_Recyclables"]
+
+ProcessModelsMetaData["Reproc"] = {}
+ProcessModelsMetaData["Reproc"]["Name"] = "Reprocessing"
+ProcessModelsMetaData["Reproc"]["Process_Type"] = "Reprocessing"
+ProcessModelsMetaData["Reproc"]["File"] = "Reproc.py"
+ProcessModelsMetaData["Reproc"]["InputType"] = [
+    "Al",
+    "Fe",
+    "OCC",
+    "Mixed_Paper",
+    "ONP",
+    "OFF",
+    "Fiber_Other",
+    "Brown_glass",
+    "Clear_glass",
+    "Green_glass",
+    "Mixed_Glass",
+    "PET",
+    "HDPE_P",
+    "HDPE_T",
+    "LDPE_Film",
+]
+
+ProcessModelsMetaData["SF_Col"] = {}
+ProcessModelsMetaData["SF_Col"]["Name"] = "Single Family Collection"
+ProcessModelsMetaData["SF_Col"]["Process_Type"] = "Collection"
+ProcessModelsMetaData["SF_Col"]["File"] = "SF_Col.py"
+ProcessModelsMetaData["SF_Col"]["InputType"] = []
+
+ProcessModelsMetaData["MF_Col"] = {}
+ProcessModelsMetaData["MF_Col"]["Name"] = "Multi-Family Collection"
+ProcessModelsMetaData["MF_Col"]["Process_Type"] = "Collection"
+ProcessModelsMetaData["MF_Col"]["File"] = "MF_Col.py"
+ProcessModelsMetaData["MF_Col"]["InputType"] = []
+
+ProcessModelsMetaData["COM_Col"] = {}
+ProcessModelsMetaData["COM_Col"]["Name"] = "Commercial Collection"
+ProcessModelsMetaData["COM_Col"]["Process_Type"] = "Collection"
+ProcessModelsMetaData["COM_Col"]["File"] = "COM_Col.py"
+ProcessModelsMetaData["COM_Col"]["InputType"] = []
+
+ProcessModelsMetaData["TS"] = {}
+ProcessModelsMetaData["TS"]["Name"] = "Transfer Station"
+ProcessModelsMetaData["TS"]["Process_Type"] = "Transfer_Station"
+ProcessModelsMetaData["TS"]["File"] = "TS.py"
+ProcessModelsMetaData["TS"]["InputType"] = [
+    "RWC",
+    "SSYW",
+    "SSO",
+    "SSR",
+    "DryRes",
+    "WetRes",
+    "ORG",
+    "REC",
+]
+
+ProcessModelsMetaData["HC"] = {}
+ProcessModelsMetaData["HC"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["HC"]["Name"] = "Home Composting"
+ProcessModelsMetaData["HC"]["File"] = "HC.py"
+ProcessModelsMetaData["HC"]["InputType"] = ["SSO_HC"]
+
+ProcessModelsMetaData["GC"] = {}
+ProcessModelsMetaData["GC"]["Process_Type"] = "RDF"
+ProcessModelsMetaData["GC"]["Name"] = "Gasification Syngas Combustion"
+ProcessModelsMetaData["GC"]["File"] = "GC.py"
+ProcessModelsMetaData["GC"]["InputType"] = ["RDF"]
+
+ProcessModelsMetaData["RDF"] = {}
+ProcessModelsMetaData["RDF"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["RDF"]["Name"] = "Refuse-Derived Fuel"
+ProcessModelsMetaData["RDF"]["File"] = "RDF.py"
+ProcessModelsMetaData["RDF"]["InputType"] = ["RWC", "MRDO"]
+
+ProcessModelsMetaData["AnF"] = {}
+ProcessModelsMetaData["AnF"]["Process_Type"] = "Treatment"
+ProcessModelsMetaData["AnF"]["Name"] = "Animal Feed"
+ProcessModelsMetaData["AnF"]["File"] = "AnF.py"
+ProcessModelsMetaData["AnF"]["InputType"] = ["SSO_AnF"]
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/RDF.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/RDF.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,225 +1,285 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Sep 20 14:39:08 2021
-
-@author: msardar2
-"""
 import numpy as np
 import numpy_financial as npf
 from swolfpy_inputdata import RDF_Input
+
 from .Common_subprocess import LCI
-from .MRF_subprocess import Flail_Mill, Trommel, Sorting, Air_Sep, Shredder, Pelletizer
-from .MRF_subprocess import Optical_sorter, Densimetric_Table, Baler, Magnet_RDF
-from .MRF_subprocess import ECS_RDF, Rolling_Stock, Conveyor, Electricity
+from .MRF_subprocess import (
+    ECS_RDF,
+    Air_Sep,
+    Baler,
+    Conveyor,
+    Densimetric_Table,
+    Electricity,
+    Flail_Mill,
+    Magnet_RDF,
+    Optical_sorter,
+    Pelletizer,
+    Rolling_Stock,
+    Shredder,
+    Sorting,
+    Trommel,
+)
 from .ProcessModel import ProcessModel
 
 
 class RDF(ProcessModel):
-    Process_Type = 'Treatment'
-    def __init__(self, process_name='RDF', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Treatment"
+
+    def __init__(self, process_name="RDF", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = RDF_Input(input_data_path, process_name=self.process_name,
-                                   CommonDataObjct=CommonDataObjct)
+        self.InputData = RDF_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
         self.process_data = self.InputData.process_data
 
-#%% Calc Function
+    # %% Calc Function
     def calc(self):
         self.LCI_Waste = LCI(self.Index)
         self.LCI = LCI(self.Index)
 
         ### Initial mass
-        self._Input = np.array([1/len(self.Index) for _ in range(len(self.Index))])
+        self._Input = np.array([1 / len(self.Index) for _ in range(len(self.Index))])
 
         ### Flail Mill
-        self._FM_feed = Flail_Mill(Input=self._Input,
-                                   InputData=self.InputData,
-                                   LCI=self.LCI)
+        self._FM_feed = Flail_Mill(Input=self._Input, InputData=self.InputData, LCI=self.LCI)
 
         ### Trommel Separating <2"
-        self._Trml_rmnd, self._Trml_rmvd = Trommel(Input=self._FM_feed,
-                                                   sep_eff=self.process_data['Trommel'].values,
-                                                   InputData=self.InputData,
-                                                   LCI=self.LCI)
+        self._Trml_rmnd, self._Trml_rmvd = Trommel(
+            Input=self._FM_feed,
+            sep_eff=self.process_data["Trommel"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
 
         ### Negative Sort  for separating >24"
-        self._NS_rmnd, self._NS_rmvd = Sorting(Input=self._Trml_rmnd,
-                                               sep_eff=self.process_data['Negative Sort'].values,
-                                               InputData=self.InputData,
-                                               Eqpt_data=self.InputData.Eq_Neg_Sort,
-                                               LCI=self.LCI)
+        self._NS_rmnd, self._NS_rmvd = Sorting(
+            Input=self._Trml_rmnd,
+            sep_eff=self.process_data["Negative Sort"].values,
+            InputData=self.InputData,
+            Eqpt_data=self.InputData.Eq_Neg_Sort,
+            LCI=self.LCI,
+        )
 
         ### Air separator for separating Heavy fraction
-        self._AS1_rmnd, self._AS1_rmvd = Air_Sep(Input=self._NS_rmnd,
-                                                 sep_eff=self.process_data['Air Separator'].values,
-                                                 InputData=self.InputData,
-                                                 LCI=self.LCI)
+        self._AS1_rmnd, self._AS1_rmvd = Air_Sep(
+            Input=self._NS_rmnd,
+            sep_eff=self.process_data["Air Separator"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
 
         ### Air separator for separating Medium fraction
-        self._AS2_rmnd, self._AS2_rmvd = Air_Sep(Input=self._AS1_rmnd,
-                                                 sep_eff=self.process_data['Air Separator'].values,
-                                                 InputData=self.InputData,
-                                                 LCI=self.LCI)
+        self._AS2_rmnd, self._AS2_rmvd = Air_Sep(
+            Input=self._AS1_rmnd,
+            sep_eff=self.process_data["Air Separator"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
 
         ### Magnet 1
-        self._Magnet1_rmnd, self._Magnet1_rmvd = Magnet_RDF(Input=self._Trml_rmvd,
-                                                            sep_eff=self.process_data['Magnet'].values,
-                                                            InputData=self.InputData,
-                                                            LCI=self.LCI)
-        self.LCI_Waste.add('Fe', self._Magnet1_rmvd)
+        self._Magnet1_rmnd, self._Magnet1_rmvd = Magnet_RDF(
+            Input=self._Trml_rmvd,
+            sep_eff=self.process_data["Magnet"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
+        self.LCI_Waste.add("Fe", self._Magnet1_rmvd)
 
         ### Optical Sort (separating metals)
-        self._OptSort_rmnd, self._OptSort_rmvd = Optical_sorter(Input=self._AS2_rmvd,
-                                                                sep_eff=self.process_data['Optical Sorter'].values,
-                                                                InputData=self.InputData,
-                                                                LCI=self.LCI)
+        self._OptSort_rmnd, self._OptSort_rmvd = Optical_sorter(
+            Input=self._AS2_rmvd,
+            sep_eff=self.process_data["Optical Sorter"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
 
         ### Magnet 2
-        self._magent_input = self._NS_rmvd +  self._OptSort_rmvd + self._AS1_rmvd
-        self._Magnet2_rmnd, self._Magnet2_rmvd = Magnet_RDF(Input=self._magent_input,
-                                                            sep_eff=self.process_data['Magnet'].values,
-                                                            InputData=self.InputData,
-                                                            LCI=self.LCI)
-        self.LCI_Waste.add('Fe', self._Magnet2_rmvd)
+        self._magent_input = self._NS_rmvd + self._OptSort_rmvd + self._AS1_rmvd
+        self._Magnet2_rmnd, self._Magnet2_rmvd = Magnet_RDF(
+            Input=self._magent_input,
+            sep_eff=self.process_data["Magnet"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
+        self.LCI_Waste.add("Fe", self._Magnet2_rmvd)
 
         ### Positive sort
-        self._PS_rmnd, self._PS_rmvd = Sorting(Input=self._Magnet2_rmnd,
-                                               sep_eff=self.process_data['Positive Sort'].values,
-                                               InputData=self.InputData,
-                                               Eqpt_data=self.InputData.Eq_Pos_Sort,
-                                               LCI=self.LCI)
+        self._PS_rmnd, self._PS_rmvd = Sorting(
+            Input=self._Magnet2_rmnd,
+            sep_eff=self.process_data["Positive Sort"].values,
+            InputData=self.InputData,
+            Eqpt_data=self.InputData.Eq_Pos_Sort,
+            LCI=self.LCI,
+        )
 
         ### ECS
-        self._ECS_rmnd, self._ECS_rmvd = ECS_RDF(Input=self._PS_rmnd,
-                                                 sep_eff=self.process_data['ECS'].values,
-                                                 InputData=self.InputData,
-                                                 Eqpt_data=self.InputData.Eq_ECS,
-                                                 LCI=self.LCI)
-        self.LCI_Waste.add('Al', self._ECS_rmvd)
+        self._ECS_rmnd, self._ECS_rmvd = ECS_RDF(
+            Input=self._PS_rmnd,
+            sep_eff=self.process_data["ECS"].values,
+            InputData=self.InputData,
+            Eqpt_data=self.InputData.Eq_ECS,
+            LCI=self.LCI,
+        )
+        self.LCI_Waste.add("Al", self._ECS_rmvd)
 
         ### Densimetric table
-        self._DMT_rmnd, self._DMT_rmvd = Densimetric_Table(Input=self._Magnet1_rmnd,
-                                                           sep_eff=self.process_data['Densimetric Table'].values,
-                                                           InputData=self.InputData,
-                                                           LCI=self.LCI)
+        self._DMT_rmnd, self._DMT_rmvd = Densimetric_Table(
+            Input=self._Magnet1_rmnd,
+            sep_eff=self.process_data["Densimetric Table"].values,
+            InputData=self.InputData,
+            LCI=self.LCI,
+        )
 
         ### Organics
-        if self.InputData.Products['Sep_org']['amount'] == 0:
+        if self.InputData.Products["Sep_org"]["amount"] == 0:
             self._Organics = np.zeros(len(self.Index))
             self._Organics_RDF = self._DMT_rmnd
         else:
             self._Organics = self._DMT_rmnd
             self._Organics_RDF = np.zeros(len(self.Index))
 
-        self.LCI_Waste.add('Separated_Organics', self._Organics)
+        self.LCI_Waste.add("Separated_Organics", self._Organics)
 
         ### Shredder
-        self._shredder_input = self._AS2_rmnd + self._OptSort_rmnd + self._PS_rmvd + self._Organics_RDF
-        self._Shredded = Shredder(Input=self._shredder_input,
-                                  InputData=self.InputData,
-                                  LCI=self.LCI)
+        self._shredder_input = (
+            self._AS2_rmnd + self._OptSort_rmnd + self._PS_rmvd + self._Organics_RDF
+        )
+        self._Shredded = Shredder(
+            Input=self._shredder_input, InputData=self.InputData, LCI=self.LCI
+        )
 
         ### Pelletizer
-        self._Pelletized = Pelletizer(Input=self._Shredded,
-                                      InputData=self.InputData,
-                                      LCI=self.LCI)
-        self.LCI_Waste.add('RDF', self._Pelletized)
+        self._Pelletized = Pelletizer(Input=self._Shredded, InputData=self.InputData, LCI=self.LCI)
+        self.LCI_Waste.add("RDF", self._Pelletized)
 
         ### Baler
         self._baler_input = self._ECS_rmvd + self._Magnet1_rmvd + self._Magnet2_rmvd
-        self._Baled = Baler(Input=self._baler_input,
-                            InputData=self.InputData,
-                            LCI=self.LCI)
+        self._Baled = Baler(Input=self._baler_input, InputData=self.InputData, LCI=self.LCI)
         #### Residuals
         self._Residuals = self._DMT_rmvd + self._ECS_rmnd
-        self.LCI_Waste.add('Other_Residual', self._Residuals)
+        self.LCI_Waste.add("Other_Residual", self._Residuals)
 
         ### Conveyor
         # Calculate the mass carried by conveyor
         self._Mass_to_Conveyor = (
             self._Input
             + self._FM_feed
-            + self._Trml_rmnd + self._Trml_rmvd
-            + self._NS_rmnd + self._NS_rmvd
-            + self._AS1_rmnd + self._AS1_rmvd
-            + self._AS2_rmnd + self._AS2_rmvd
-            + self._Magnet1_rmnd + self._Magnet1_rmvd
-            + self._PS_rmnd + self._PS_rmvd
-            + self._ECS_rmnd + self._ECS_rmvd
-            + self._DMT_rmnd + self._DMT_rmvd
-            + self._Organics_RDF + self._Organics
+            + self._Trml_rmnd
+            + self._Trml_rmvd
+            + self._NS_rmnd
+            + self._NS_rmvd
+            + self._AS1_rmnd
+            + self._AS1_rmvd
+            + self._AS2_rmnd
+            + self._AS2_rmvd
+            + self._Magnet1_rmnd
+            + self._Magnet1_rmvd
+            + self._PS_rmnd
+            + self._PS_rmvd
+            + self._ECS_rmnd
+            + self._ECS_rmvd
+            + self._DMT_rmnd
+            + self._DMT_rmvd
+            + self._Organics_RDF
+            + self._Organics
             + self._Shredded
-            + self._Pelletized)
+            + self._Pelletized
+        )
 
         # conveyor
         Conveyor(self._Mass_to_Conveyor, self.InputData, self.LCI)
 
         ### Rolling_Stock
         Rolling_Stock(self._Input, self.InputData, self.LCI)
 
         ### General Electricity
         Electricity(self._Input, self.InputData, self.LCI)
 
         ### Capital Cost
-        Land_req = (self.InputData.Electricity['Area_rate']['amount']
-                    * self.InputData.Constr_cost['Land_req_factor']['amount'])
-        Land_cost = Land_req * self.InputData.Constr_cost['Land_rate']['amount'] / 4046.86  # 1acr = 4046.86 m2
-        Constr_cost = Land_req * (self.InputData.Constr_cost['Paving_rate']['amount']
-                                  + self.InputData.Constr_cost['Grading_rate']['amount']) / 10000  # 1ha = 10000m2
-        Constr_cost += (self.InputData.Electricity['Area_rate']['amount']
-                        * self.InputData.Constr_cost['Constr_rate']['amount']
-                        / 0.0929)  # 1ft2 = 0.0929 m2
-        Constr_cost *= (1 + self.InputData.Constr_cost['Eng_rate']['amount'])
+        Land_req = (
+            self.InputData.Electricity["Area_rate"]["amount"]
+            * self.InputData.Constr_cost["Land_req_factor"]["amount"]
+        )
+        Land_cost = (
+            Land_req * self.InputData.Constr_cost["Land_rate"]["amount"] / 4046.86
+        )  # 1acr = 4046.86 m2
+        Constr_cost = (
+            Land_req
+            * (
+                self.InputData.Constr_cost["Paving_rate"]["amount"]
+                + self.InputData.Constr_cost["Grading_rate"]["amount"]
+            )
+            / 10000
+        )  # 1ha = 10000m2
+        Constr_cost += (
+            self.InputData.Electricity["Area_rate"]["amount"]
+            * self.InputData.Constr_cost["Constr_rate"]["amount"]
+            / 0.0929
+        )  # 1ft2 = 0.0929 m2
+        Constr_cost *= 1 + self.InputData.Constr_cost["Eng_rate"]["amount"]
 
         # Add Miscellaneous Costs based on the average size TS: 156 tpd
-        Miscellaneous_Costs = (self.InputData.Constr_cost['Weigh_Station']['amount'] +
-                               self.InputData.Constr_cost['Utility_Connections']['amount']) / 156  # Assume capacity of 1000 tpd
-        Miscellaneous_Costs += (self.InputData.Constr_cost['Landscaping_rate']['amount']
-                                / 10000 * Land_req)  # 1 ha = 10000m2
+        Miscellaneous_Costs = (
+            self.InputData.Constr_cost["Weigh_Station"]["amount"]
+            + self.InputData.Constr_cost["Utility_Connections"]["amount"]
+        ) / 156  # Assume capacity of 1000 tpd
+        Miscellaneous_Costs += (
+            self.InputData.Constr_cost["Landscaping_rate"]["amount"] / 10000 * Land_req
+        )  # 1 ha = 10000m2
         # Assumes fenc along three sides of square
-        Miscellaneous_Costs += (np.sqrt(Land_req * 156) * 3
-                                * self.InputData.Constr_cost['Fencing_Rate']['amount'] / 156)
+        Miscellaneous_Costs += (
+            np.sqrt(Land_req * 156) * 3 * self.InputData.Constr_cost["Fencing_Rate"]["amount"] / 156
+        )
 
         # Total capital cost
-        Unit_capital_cost = Land_cost + Constr_cost +  Miscellaneous_Costs  # $/tpd
-        Unit_capital_cost /= self.InputData.Labor['Day_year']['amount']  # $/t.yr
-        capital_cost = -npf.pmt(rate=self.InputData.Constr_cost['Inerest_rate']['amount'],
-                                nper=self.InputData.Constr_cost['lifetime']['amount'],
-                                pv=Unit_capital_cost)
-        self.LCI.add(('biosphere3', 'Capital_Cost'), capital_cost * self._Input)
+        Unit_capital_cost = Land_cost + Constr_cost + Miscellaneous_Costs  # $/tpd
+        Unit_capital_cost /= self.InputData.Labor["Day_year"]["amount"]  # $/t.yr
+        capital_cost = -npf.pmt(
+            rate=self.InputData.Constr_cost["Interest_rate"]["amount"],
+            nper=self.InputData.Constr_cost["lifetime"]["amount"],
+            pv=Unit_capital_cost,
+        )
+        self.LCI.add(("biosphere3", "Capital_Cost"), capital_cost * self._Input)
 
-#%% Check Mass balance
+        # %% Check Mass balance
         ### Check mass balance:
         mass_out = self.LCI_Waste.lci.sum(axis=1)
         for i in range(len(self.Index)):
             if abs(mass_out[i] - self._Input[i]) > 0.01:
-                raise ValueError('*** Mass Balance Error *** \n Output mass is not equal to input mass!')
+                raise ValueError(
+                    "*** Mass Balance Error *** \n Output mass is not equal to input mass!"
+                )
 
-#%% Report
+    # %% Report
     ### Report
     def report(self):
         ### Output
         self.RDF = {}
         self.RDF["process name"] = (self.process_name, self.Process_Type, self.__class__)
 
         # Waste
         self.RDF["Waste"] = self.LCI_Waste.report(input_mass=self._Input, transpose=True).to_dict()
 
         # Technosphere
-        tech_index = [x for x in self.LCI.col_dict.keys() if 'biosphere3' not in x]
-        self.RDF["Technosphere"] = self.LCI.report(input_mass=self._Input, transpose=True).loc[tech_index, :].to_dict()
-
+        tech_index = [x for x in self.LCI.col_dict.keys() if "biosphere3" not in x]
+        self.RDF["Technosphere"] = (
+            self.LCI.report(input_mass=self._Input, transpose=True).loc[tech_index, :].to_dict()
+        )
 
         # Biosphere
-        bio_index = [x for x in self.LCI.col_dict.keys() if 'biosphere3' in x]
-        self.RDF["Biosphere"] = self.LCI.report(input_mass=self._Input, transpose=True).loc[bio_index, :].to_dict()
+        bio_index = [x for x in self.LCI.col_dict.keys() if "biosphere3" in x]
+        self.RDF["Biosphere"] = (
+            self.LCI.report(input_mass=self._Input, transpose=True).loc[bio_index, :].to_dict()
+        )
         return self.RDF
 
-#%% Monte Carlo
+    # %% Monte Carlo
     ### setup for Monte Carlo simulation
     def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
 
     ### Calculate based on the generated numbers
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/Reproc.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/Reproc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Mar  9 21:46:21 2020
+from swolfpy_inputdata import Reproc_Input
 
-@author: msardar2
-"""
 from .ProcessModel import ProcessModel
-from swolfpy_inputdata import Reproc_Input
 
 
 class Reproc(ProcessModel):
-    Process_Type = 'Reprocessing'
-    def __init__(self,process_name='Reproc', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Reprocessing"
+
+    def __init__(self, process_name="Reproc", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData= Reproc_Input(input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct)
+        self.InputData = Reproc_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
     def calc(self):
         self.Biosphere = {}
         self.Technosphere = {}
-        self.Waste={}
+        self.Waste = {}
 
         for act in self.CommonData.Reprocessing_Index:
             self.Biosphere[act] = {}
             self.Technosphere[act] = {}
             self.Waste[act] = {}
             if act in self.InputData.Input_dict.keys():
                 for exchange in self.InputData.Input_dict[act].keys():
-                    if exchange[0] == 'Technosphere':
-                        self.Technosphere[act][exchange]=self.InputData.Input_dict[act][exchange]['amount']
-                    elif exchange[0] == 'biosphere3':
-                        self.Biosphere[act][exchange]=self.InputData.Input_dict[act][exchange]['amount']
+                    if exchange[0] == "Technosphere":
+                        self.Technosphere[act][exchange] = self.InputData.Input_dict[act][exchange][
+                            "amount"
+                        ]
+                    elif exchange[0] == "biosphere3":
+                        self.Biosphere[act][exchange] = self.InputData.Input_dict[act][exchange][
+                            "amount"
+                        ]
 
-        #self.LCI = self.Reprocessing.read_output_from_SWOLF('ReProc',Path(__file__).parent.parent/"Data/Material_Reprocessing_BW2.csv")
-
-    def setup_MC(self,seed=None):
+    def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
 
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
         self.calc()
-        return(input_list)
-
+        return input_list
 
     def report(self):
         self.REPROC = {}
         self.REPROC["process name"] = (self.process_name, self.Process_Type, self.__class__)
         self.REPROC["Biosphere"] = self.Biosphere
         self.REPROC["Technosphere"] = self.Technosphere
-        self.REPROC["Waste"]= self.Waste
-        return(self.REPROC)
+        self.REPROC["Waste"] = self.Waste
+        return self.REPROC
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/SF_Col.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/SF_Col.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,953 +1,1147 @@
 # -*- coding: utf-8 -*-
-"""
-@author: msardar2
-"""
+import warnings
+
+import numpy as np
+import numpy_financial as npf
 import pandas as pd
 from swolfpy_inputdata import SF_Col_Input
+
 from .ProcessModel import ProcessModel
-import numpy_financial as npf
-import numpy as np
-import warnings
 
 
 class SF_Col(ProcessModel):
-    Process_Type = 'Collection'
-    def __init__(self, process_name, Collection_scheme,
-                 Treatment_processes=None,
-                 Distance=None,
-                 CommonDataObjct=None,
-                 input_data_path=None):
+    Process_Type = "Collection"
+
+    def __init__(
+        self,
+        process_name,
+        Collection_scheme,
+        Treatment_processes=None,
+        Distance=None,
+        CommonDataObjct=None,
+        input_data_path=None,
+    ):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = SF_Col_Input(input_data_path,
-                                      process_name=self.process_name,
-                                      CommonDataObjct=CommonDataObjct)
+        self.InputData = SF_Col_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
         self.process_name = process_name
 
         if Treatment_processes is not None:
             self.Treat_proc = Treatment_processes
             if Distance:
                 self.Distance = Distance
             else:
-                raise Exception('User should define both Distance and Treatment_processes together!')
+                raise ValueError(
+                    "User should define both Distance and Treatment_processes together!"
+                )
         else:
             self.Treat_proc = False
 
         self.process_data = self.InputData.process_data
         self.col_schm = Collection_scheme
 
     @staticmethod
     def scheme():
         """
-        Retrun the dictionary for collection_scheme. all the
-        contributions are zero; user should define them according to his/her case.
+        Return the dictionary for collection_scheme.
+
+        all the contributions are zero; user should define them according to his/her case.
         """
-        SepOrg = ['N/A', 'SSYW', 'SSO', 'SSYWDO']
-        SepRec = ['N/A', 'SSR', 'DSR', 'MSR', 'MSRDO']
+        SepOrg = ["N/A", "SSYW", "SSO", "SSYWDO"]
+        SepRec = ["N/A", "SSR", "DSR", "MSR", "MSRDO"]
         scheme = {}
         for i in SepOrg:
             for j in SepRec:
-                scheme[('RWC', i, j)] = 0
+                scheme[("RWC", i, j)] = 0
         for i in SepOrg:
-            scheme[('REC_WetRes', i, 'REC_WetRes')] = 0
+            scheme[("REC_WetRes", i, "REC_WetRes")] = 0
         for j in SepRec:
-            scheme[('ORG_DryRes', 'ORG_DryRes', j)] = 0
-        for i in ['N/A', 'SSYWDO']:
-            for j in ['N/A', 'MSRDO']:
-                scheme[('MRDO', i, j)] = 0
+            scheme[("ORG_DryRes", "ORG_DryRes", j)] = 0
+        for i in ["N/A", "SSYWDO"]:
+            for j in ["N/A", "MSRDO"]:
+                scheme[("MRDO", i, j)] = 0
         return scheme
 
     def _normalize_scheme(self, DropOff=True, warn=True):
         """
-        Used in optimization. Check that sum of the contributions is 1.
+        Used in optimization.
+
+        Check that sum of the contributions is 1.
         """
         if not DropOff:
             for k in self.col_schm:
-                if 'DO' in k:
+                if "DO" in k:
                     self.col_schm[k] = 0
 
-        contribution =  sum(self.col_schm.values())
+        contribution = sum(self.col_schm.values())
         if abs(contribution - 1) > 0.01:
             if warn:
-                warnings.warn('Error in collection scheme: Sum(Contribution) != 1')
+                warnings.warn("Error in collection scheme: Sum(Contribution) != 1")
             for k, v in self.col_schm.items():
                 self.col_schm[k] = v / contribution
 
     def calc_composition(self):
         # Creating the sel.col Data frame
         col_data = np.zeros((14, 61), dtype=float)
         col_data[:] = np.nan
         col_columns = []
-        col_index = ['RWC', 'SSR', 'DSR', 'MSR', 'LV',
-                                       'SSYW', 'SSO', 'ORG', 'DryRes', 'REC',
-                                        'WetRes', 'MRDO', 'SSYWDO', 'MSRDO']
+        col_index = [
+            "RWC",
+            "SSR",
+            "DSR",
+            "MSR",
+            "LV",
+            "SSYW",
+            "SSO",
+            "ORG",
+            "DryRes",
+            "REC",
+            "WetRes",
+            "MRDO",
+            "SSYWDO",
+            "MSRDO",
+        ]
         col_i = 0
 
         for key, val in self.InputData.den_asmd.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('den_asmd')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("den_asmd")
         col_i += 1
 
         for key, val in self.InputData.Prtcp.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Prtcp')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Prtcp")
         col_i += 1
 
         for key, val in self.InputData.Fr.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Fr')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Fr")
         col_i += 1
 
         for key, val in self.InputData.TL.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('TL')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("TL")
         col_i += 1
 
         for key, val in self.InputData.S.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('S')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("S")
         col_i += 1
 
         for key, val in self.InputData.Nw.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Nw')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Nw")
         col_i += 1
 
         for key, val in self.InputData.Rb.items():
-            col_data[col_index.index(key), col_i] = val['amount']
-        col_columns.append('Rb')
+            col_data[col_index.index(key), col_i] = val["amount"]
+        col_columns.append("Rb")
         col_i += 1
 
         for key, val in self.InputData.Col_Root.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.LCC.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.DropOff.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.Mpg.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
         for key, val in self.InputData.Speed.items():
-            col_data[:, col_i] = val['amount']
+            col_data[:, col_i] = val["amount"]
             col_columns.append(key)
             col_i += 1
 
-        for key in ['CD', 'WV', 'WP', 'wt_lim', 'max_weight', 'F1_', 'F1_idle',
-                    'F2_', 'F2_idle', 'bw', 'bv', 'Lt', 'Ut', 'Vt', 'Fract_CNG',
-                    'grg_area', 'off_area', 'grg_enrg', 'off_enrg', 'Lb']:
-            col_data[:, col_i] = self.InputData.Col[key]['amount']
+        for key in [
+            "CD",
+            "WV",
+            "WP",
+            "wt_lim",
+            "max_weight",
+            "F1_",
+            "F1_idle",
+            "F2_",
+            "F2_idle",
+            "bw",
+            "bv",
+            "Lt",
+            "Ut",
+            "Vt",
+            "Fract_CNG",
+            "grg_area",
+            "off_area",
+            "grg_enrg",
+            "off_enrg",
+            "Lb",
+        ]:
+            col_data[:, col_i] = self.InputData.Col[key]["amount"]
             col_columns.append(key)
             col_i += 1
 
-        self.col = pd.DataFrame(data=col_data,
-                                columns=col_columns,
-                                index=['RWC', 'SSR', 'DSR', 'MSR', 'LV',
-                                       'SSYW', 'SSO', 'ORG', 'DryRes', 'REC',
-                                        'WetRes', 'MRDO', 'SSYWDO', 'MSRDO'],
-                                dtype=float)
+        self.col = pd.DataFrame(
+            data=col_data,
+            columns=col_columns,
+            index=[
+                "RWC",
+                "SSR",
+                "DSR",
+                "MSR",
+                "LV",
+                "SSYW",
+                "SSO",
+                "ORG",
+                "DryRes",
+                "REC",
+                "WetRes",
+                "MRDO",
+                "SSYWDO",
+                "MSRDO",
+            ],
+            dtype=float,
+        )
 
-        self.col['Fract_Dies'] = 1 - self.InputData.Col['Fract_CNG']['amount']
+        self.col["Fract_Dies"] = 1 - self.InputData.Col["Fract_CNG"]["amount"]
 
         self._col_schm = {
-            'RWC': {'Contribution': 0,
-                    'separate_col':{'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSYWDO': 0}},
-            'ORG_DryRes': {'Contribution': 0,
-                           'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSYWDO': 0}},
-            'REC_WetRes': {'Contribution': 0,
-                           'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSYWDO': 0}},
-            'MRDO': {'Contribution': 0,
-                     'separate_col': {'SSR': 0, 'DSR': 0, 'MSR': 0, 'MSRDO': 0, 'SSYW': 0, 'SSO': 0, 'SSYWDO': 0}}}
+            "RWC": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSYWDO": 0,
+                },
+            },
+            "ORG_DryRes": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSYWDO": 0,
+                },
+            },
+            "REC_WetRes": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSYWDO": 0,
+                },
+            },
+            "MRDO": {
+                "Contribution": 0,
+                "separate_col": {
+                    "SSR": 0,
+                    "DSR": 0,
+                    "MSR": 0,
+                    "MSRDO": 0,
+                    "SSYW": 0,
+                    "SSO": 0,
+                    "SSYWDO": 0,
+                },
+            },
+        }
 
         for k, v in self.col_schm.items():
-            if k[0] == 'RWC':
-                self._col_schm['RWC']['Contribution'] += v
-            elif k[0] == 'ORG_DryRes':
-                self._col_schm['ORG_DryRes']['Contribution'] += v
-            elif k[0] == 'REC_WetRes':
-                self._col_schm['REC_WetRes']['Contribution'] += v
-            elif k[0] == 'MRDO':
-                self._col_schm['MRDO']['Contribution'] += v
+            if k[0] == "RWC":
+                self._col_schm["RWC"]["Contribution"] += v
+            elif k[0] == "ORG_DryRes":
+                self._col_schm["ORG_DryRes"]["Contribution"] += v
+            elif k[0] == "REC_WetRes":
+                self._col_schm["REC_WetRes"]["Contribution"] += v
+            elif k[0] == "MRDO":
+                self._col_schm["MRDO"]["Contribution"] += v
             else:
-                raise Exception(f'Error in collection scheme keys: "{k[0]}" is not defined!')
+                raise ValueError(f'Error in collection scheme keys: "{k[0]}" is not defined!')
 
         for k, v in self.col_schm.items():
             if v > 0:
-                if k[1] not in ['N/A', 'ORG_DryRes', 'REC_WetRes']:
-                    self._col_schm[k[0]]['separate_col'][k[1]] += v / self._col_schm[k[0]]['Contribution']
-                if k[2] not in ['N/A', 'ORG_DryRes', 'REC_WetRes']:
-                    self._col_schm[k[0]]['separate_col'][k[2]] += v / self._col_schm[k[0]]['Contribution']
+                if k[1] not in ["N/A", "ORG_DryRes", "REC_WetRes"]:
+                    self._col_schm[k[0]]["separate_col"][k[1]] += (
+                        v / self._col_schm[k[0]]["Contribution"]
+                    )
+                if k[2] not in ["N/A", "ORG_DryRes", "REC_WetRes"]:
+                    self._col_schm[k[0]]["separate_col"][k[2]] += (
+                        v / self._col_schm[k[0]]["Contribution"]
+                    )
 
         # Single Family Residential Waste Generation Rate (kg/household-week)
-        g_res = 7 * self.InputData.Col['res_per_dwel']['amount'] * self.InputData.Col['res_gen']['amount']
-        gen_per_week = g_res * self.process_data['Comp']
+        g_res = (
+            7
+            * self.InputData.Col["res_per_dwel"]["amount"]
+            * self.InputData.Col["res_gen"]["amount"]
+        )
+        gen_per_week = g_res * self.process_data["Comp"]
         total_waste_gen = (
-            g_res
-            * self.InputData.Col['houses_res']['amount']
-            * 365 / 7 / 1000)  # 52 weeks per year & 1000 kg = 1 Mg
+            g_res * self.InputData.Col["houses_res"]["amount"] * 365 / 7 / 1000
+        )  # 52 weeks per year & 1000 kg = 1 Mg
 
         # Check for Leave Vaccum
-        self.process_data['LV'] = 0
-        if self.InputData.Col['Leaf_vacuum']['amount'] == 1:
-            LV_gen = (gen_per_week['Yard_Trimmings_Leaves']
-                      * self.InputData.Col['houses_res']['amount']
-                      * 365 / 7 / 1000)
-            LV_col = self.InputData.Col['Leaf_vacuum_amount']['amount']
+        self.process_data["LV"] = 0
+        if self.InputData.Col["Leaf_vacuum"]["amount"] == 1:
+            LV_gen = (
+                gen_per_week["Yard_Trimmings_Leaves"]
+                * self.InputData.Col["houses_res"]["amount"]
+                * 365
+                / 7
+                / 1000
+            )
+            LV_col = self.InputData.Col["Leaf_vacuum_amount"]["amount"]
 
             if LV_gen <= LV_col:
-                self.process_data.loc['Yard_Trimmings_Leaves', 'LV'] = 1
+                self.process_data.loc["Yard_Trimmings_Leaves", "LV"] = 1
             else:
-                self.process_data.loc['Yard_Trimmings_Leaves', 'LV'] = LV_col / LV_gen
+                self.process_data.loc["Yard_Trimmings_Leaves", "LV"] = LV_col / LV_gen
 
-            for j in ['RWC', 'ORG_DryRes', 'REC_WetRes', 'MRDO']:
-                self._col_schm[j]['separate_col']['LV'] = 1
+            for j in ["RWC", "ORG_DryRes", "REC_WetRes", "MRDO"]:
+                self._col_schm[j]["separate_col"]["LV"] = 1
         else:
-            for j in ['RWC', 'ORG_DryRes', 'REC_WetRes', 'MRDO']:
-                self._col_schm[j]['separate_col']['LV'] = 0
+            for j in ["RWC", "ORG_DryRes", "REC_WetRes", "MRDO"]:
+                self._col_schm[j]["separate_col"]["LV"] = 0
 
-        self.col.loc['LV', 'Fr'] = (
-            self.InputData.Col['LV_serv_times']['amount']
-            / self.InputData.Col['LV_serv_pd']['amount'])
+        self.col.loc["LV", "Fr"] = (
+            self.InputData.Col["LV_serv_times"]["amount"]
+            / self.InputData.Col["LV_serv_pd"]["amount"]
+        )
 
         # Total fraction where this service is offered
         self.col_proc = {
-            'RWC': self._col_schm['RWC']['Contribution'],
-            'ORG': self._col_schm['ORG_DryRes']['Contribution'],
-            'DryRes': self._col_schm['ORG_DryRes']['Contribution'],
-            'REC': self._col_schm['REC_WetRes']['Contribution'],
-            'WetRes': self._col_schm['REC_WetRes']['Contribution'],
-            'MRDO': self._col_schm['MRDO']['Contribution']}
+            "RWC": self._col_schm["RWC"]["Contribution"],
+            "ORG": self._col_schm["ORG_DryRes"]["Contribution"],
+            "DryRes": self._col_schm["ORG_DryRes"]["Contribution"],
+            "REC": self._col_schm["REC_WetRes"]["Contribution"],
+            "WetRes": self._col_schm["REC_WetRes"]["Contribution"],
+            "MRDO": self._col_schm["MRDO"]["Contribution"],
+        }
 
         # SSO_HC contribution
-        for j in ['RWC', 'ORG_DryRes', 'REC_WetRes', 'MRDO']:
-            if self.InputData.Col['HC_partic']['amount'] > 0:
-                self._col_schm[j]['separate_col']['SSO_HC'] = 1
+        for j in ["RWC", "ORG_DryRes", "REC_WetRes", "MRDO"]:
+            if self.InputData.Col["HC_partic"]["amount"] > 0:
+                self._col_schm[j]["separate_col"]["SSO_HC"] = 1
             else:
-                self._col_schm[j]['separate_col']['SSO_HC'] = 0
+                self._col_schm[j]["separate_col"]["SSO_HC"] = 0
 
-        for i in ['LV', 'SSR', 'DSR', 'MSR', 'MSRDO', 'SSYW', 'SSO', 'SSO_HC', 'SSYWDO']:
+        for i in ["LV", "SSR", "DSR", "MSR", "MSRDO", "SSYW", "SSO", "SSO_HC", "SSYWDO"]:
             self.col_proc[i] = 0
-            for j in ['RWC', 'ORG_DryRes', 'REC_WetRes', 'MRDO']:
+            for j in ["RWC", "ORG_DryRes", "REC_WetRes", "MRDO"]:
                 self.col_proc[i] += (
-                    self._col_schm[j]['Contribution']
-                    * self._col_schm[j]['separate_col'][i])
+                    self._col_schm[j]["Contribution"] * self._col_schm[j]["separate_col"][i]
+                )
 
         # Is this collection process offered? (1: in use, 0: not used)
         self.P_use = {}
         for j in self.col_proc.keys():
             self.P_use[j] = 1 if self.col_proc[j] > 0 else 0
 
         # Mass separated by collection process (kg/week.Household)
-        columns = ['RWC', 'SSR', 'DSR', 'MSR', 'LV', 'SSYW', 'SSO',
-                   'SSO_HC', 'ORG', 'DryRes', 'REC', 'WetRes',
-                   'MRDO', 'SSYWDO', 'MSRDO']
-        self.mass = pd.DataFrame(index=self.Index,
-                                 columns=columns,
-                                 data=0.0,
-                                 dtype=float)
-
-        for i in ['SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'ORG', 'REC', 'SSYWDO', 'MSRDO']:
-            self.mass[i] = (
-                gen_per_week.values
-                * self.process_data[i].values
-                * self.P_use[i])
-
-            self.mass.loc['Yard_Trimmings_Leaves', i] *= (1 - self.process_data.loc['Yard_Trimmings_Leaves', 'LV'])
-
-        self.mass['LV'] = (gen_per_week.values
-                           * self.process_data['LV'].values
-                           * self.P_use['LV'])
+        columns = [
+            "RWC",
+            "SSR",
+            "DSR",
+            "MSR",
+            "LV",
+            "SSYW",
+            "SSO",
+            "SSO_HC",
+            "ORG",
+            "DryRes",
+            "REC",
+            "WetRes",
+            "MRDO",
+            "SSYWDO",
+            "MSRDO",
+        ]
+        self.mass = pd.DataFrame(index=self.Index, columns=columns, data=0.0, dtype=float)
+
+        for i in ["SSR", "DSR", "MSR", "SSYW", "SSO", "ORG", "REC", "SSYWDO", "MSRDO"]:
+            self.mass[i] = gen_per_week.values * self.process_data[i].values * self.P_use[i]
+
+            self.mass.loc["Yard_Trimmings_Leaves", i] *= (
+                1 - self.process_data.loc["Yard_Trimmings_Leaves", "LV"]
+            )
+
+        self.mass["LV"] = gen_per_week.values * self.process_data["LV"].values * self.P_use["LV"]
 
         # SSO_HC mass
         """
         For home composting, it is assumed that only yard waste and
         food waste (vegetables) are used.
         """
-        if self.InputData.Col['HC_partic']['amount'] > 0:
-            HC_frac = self.InputData.Col['HC_partic']['amount'] / 100
-            c = ['SSR', 'DSR', 'MSR', 'SSYW', 'SSO', 'ORG', 'REC', 'SSYWDO', 'MSRDO']
-            OFMSW = ['Yard_Trimmings_Leaves',
-                     'Yard_Trimmings_Grass',
-                     'Yard_Trimmings_Branches',
-                     'Food_Waste_Vegetable']
+        if self.InputData.Col["HC_partic"]["amount"] > 0:
+            HC_frac = self.InputData.Col["HC_partic"]["amount"] / 100
+            c = ["SSR", "DSR", "MSR", "SSYW", "SSO", "ORG", "REC", "SSYWDO", "MSRDO"]
+            OFMSW = [
+                "Yard_Trimmings_Leaves",
+                "Yard_Trimmings_Grass",
+                "Yard_Trimmings_Branches",
+                "Food_Waste_Vegetable",
+            ]
+
+            self.mass.loc[OFMSW, "SSO_HC"] = gen_per_week[OFMSW] * HC_frac
+
+            self.mass.loc["Yard_Trimmings_Leaves", "SSO_HC"] *= (
+                1 - self.process_data.loc["Yard_Trimmings_Leaves", "LV"]
+            )
 
-            self.mass.loc[OFMSW, 'SSO_HC'] = (
-                gen_per_week[OFMSW] * HC_frac)
-
-            self.mass.loc['Yard_Trimmings_Leaves', 'SSO_HC'] *= (
-                    1 - self.process_data.loc['Yard_Trimmings_Leaves', 'LV'])
-
-            self.mass.loc[OFMSW, c] *= (1 - HC_frac)
+            self.mass.loc[OFMSW, c] *= 1 - HC_frac
 
         def separate_col_mass(j):
             mass = np.zeros(len(self.CommonData.Index))
-            for i in ['SSR', 'DSR', 'MSR', 'LV', 'SSYW', 'SSO', 'SSO_HC', 'SSYWDO', 'MSRDO']:
-                mass += self.mass[i].values * self._col_schm[j]['separate_col'][i]
+            for i in ["SSR", "DSR", "MSR", "LV", "SSYW", "SSO", "SSO_HC", "SSYWDO", "MSRDO"]:
+                mass += self.mass[i].values * self._col_schm[j]["separate_col"][i]
             return mass
 
         # Calculating the residual waste after separate collection
-        for j in ['RWC', 'MRDO']:
-            self.mass[j]= (
-                gen_per_week.values
-                * self.process_data[j].values
-                - separate_col_mass(j)) * self.P_use[j]
+        for j in ["RWC", "MRDO"]:
+            self.mass[j] = (
+                gen_per_week.values * self.process_data[j].values - separate_col_mass(j)
+            ) * self.P_use[j]
 
         # ORG_DryRes
-        self.mass['DryRes']= (
-            (gen_per_week.values
-             * self.process_data['DryRes'].values
-             - separate_col_mass('ORG_DryRes')
-             - self.mass['ORG'].values) * self.P_use['DryRes'])
+        self.mass["DryRes"] = (
+            gen_per_week.values * self.process_data["DryRes"].values
+            - separate_col_mass("ORG_DryRes")
+            - self.mass["ORG"].values
+        ) * self.P_use["DryRes"]
 
         # REC_WetRes
-        self.mass['WetRes'] = (
-            gen_per_week.values
-            * self.process_data['WetRes'].values
-            - separate_col_mass('REC_WetRes')
-            - self.mass['REC'].values) * self.P_use['WetRes']
+        self.mass["WetRes"] = (
+            gen_per_week.values * self.process_data["WetRes"].values
+            - separate_col_mass("REC_WetRes")
+            - self.mass["REC"].values
+        ) * self.P_use["WetRes"]
 
         # Annual Mass Flows (Mg/yr)
         self.col_massflow = pd.DataFrame(index=self.Index)
         for i in columns:
-            self.col_massflow[i] = (self.mass[i]
-                                    * self.InputData.Col['houses_res']['amount']
-                                    * 365 / 7 / 1000
-                                    * self.col_proc[i])
+            self.col_massflow[i] = (
+                self.mass[i]
+                * self.InputData.Col["houses_res"]["amount"]
+                * 365
+                / 7
+                / 1000
+                * self.col_proc[i]
+            )
 
         # Check for negative mass flows
         if (self.col_massflow.values < 0).any().any():
-            raise Exception(f'Negative mass flows in collection model [{self.process_name}]!')
+            raise ValueError(f"Negative mass flows in collection model [{self.process_name}]!")
             # warnings.warn('Negative mass flows in collection model [{self.process_name}]!')
 
         # Check generated mass = Collected mass
         ratio = self.col_massflow.sum().sum() / total_waste_gen
         if ratio > 1.01 or ratio < 0.99:
-            raise Exception(f'Mass balance error in collection model [{self.process_name}]!')
+            raise ValueError(f"Mass balance error in collection model [{self.process_name}]!")
             # warnings.warn(f'Mass balance error in collection model [{self.process_name}]!')
 
         # Volume Composition of each collection process for each sector
-        mass_to_cyd = (1 / (self.process_data['Bulk_Density'].values + 0.000001)
-                       * 1.30795)  # m3 --> Cubic yard
-        mass_to_cyd[self.process_data['Bulk_Density'].values <= 0] = 0.0
+        mass_to_cyd = (
+            1 / (self.process_data["Bulk_Density"].values + 0.000001) * 1.30795
+        )  # m3 --> Cubic yard
+        mass_to_cyd[self.process_data["Bulk_Density"].values <= 0] = 0.0
 
-        for i in ['RWC', 'SSR', 'DSR', 'MSR', 'LV', 'SSYW', 'SSO', 'MRDO', 'SSYWDO', 'MSRDO']:
+        for i in ["RWC", "SSR", "DSR", "MSR", "LV", "SSYW", "SSO", "MRDO", "SSYWDO", "MSRDO"]:
             vol = (self.mass[i].values * mass_to_cyd).sum()  # Unit kg/cyd
             if vol > 0:
-                self.col.loc[i, 'den_c'] = (self.mass[i].values
-                                            * 2.205 / vol).sum()  # Unit lb/cyd
+                self.col.loc[i, "den_c"] = (self.mass[i].values * 2.205 / vol).sum()  # Unit lb/cyd
             else:
-                self.col.loc[i, 'den_c'] = 0
+                self.col.loc[i, "den_c"] = 0
 
-        for i, j in [('ORG', 'DryRes'), ('REC', 'WetRes')]:
+        for i, j in [("ORG", "DryRes"), ("REC", "WetRes")]:
             m = self.mass[i].values + self.mass[j].values
             vol = (m * mass_to_cyd).sum()  # Unit kg/cyd
             if vol > 0:
-                self.col.loc[i, 'den_c'] = (m * 2.205 / vol).sum()  # Unit lb/cyd
+                self.col.loc[i, "den_c"] = (m * 2.205 / vol).sum()  # Unit lb/cyd
             else:
-                self.col.loc[i, 'den_c'] = 0
+                self.col.loc[i, "den_c"] = 0
 
     def find_destination(self, product, Treatment_processes):
         destination = {}
         for P in Treatment_processes:
-            if product in Treatment_processes[P]['input_type']:
+            if product in Treatment_processes[P]["input_type"]:
                 destination[P] = (
-                    self.Distance.Distance[(self.process_name, P)]['Heavy Duty Truck']
-                    / 1.60934)  # Convert the distance from km to mile
+                    self.Distance.Distance[(self.process_name, P)]["Heavy Duty Truck"] / 1.60934
+                )  # Convert the distance from km to mile
         return destination
 
     # calculating LCI and cost for different locations
     def calc_destin(self):
         if self.Treat_proc:
             self.dest = {}
             self.result_destination = {}
-            for i in ['RWC', 'SSR', 'DSR', 'MSR', 'LV', 'SSYW', 'SSO',
-                      'SSO_HC', 'ORG', 'DryRes', 'REC', 'WetRes',
-                      'MRDO', 'SSYWDO', 'MSRDO']:
+            for i in [
+                "RWC",
+                "SSR",
+                "DSR",
+                "MSR",
+                "LV",
+                "SSYW",
+                "SSO",
+                "SSO_HC",
+                "ORG",
+                "DryRes",
+                "REC",
+                "WetRes",
+                "MRDO",
+                "SSYWDO",
+                "MSRDO",
+            ]:
                 self.dest[i] = self.find_destination(i, self.Treat_proc)
                 self.result_destination[i] = {}
 
             # Number of times we need to run the collection
             n_run = max([len(self.dest[i]) for i in self.dest.keys()])
 
             for i in range(n_run):
-                for j in ['RWC', 'SSR', 'DSR', 'MSR', 'MSRDO', 'LV', 'SSYW',
-                          'SSO', 'SSYWDO', 'MRDO', 'SSYWDO', 'MSRDO', 'ORG', 'REC']:
+                for j in [
+                    "RWC",
+                    "SSR",
+                    "DSR",
+                    "MSR",
+                    "MSRDO",
+                    "LV",
+                    "SSYW",
+                    "SSO",
+                    "SSYWDO",
+                    "MRDO",
+                    "SSYWDO",
+                    "MSRDO",
+                    "ORG",
+                    "REC",
+                ]:
                     if len(self.dest[j]) > i:
                         # Distance btwn collection route and destination
-                        self.col['Drf'][j] = self.dest[j][list(self.dest[j].keys())[i]]
+                        self.col["Drf"][j] = self.dest[j][list(self.dest[j].keys())[i]]
 
                         # Distance between destination and garage
-                        self.col['Dfg'][j] = (
-                            self.dest[j][list(self.dest[j].keys())[i]]
-                            + self.col['Dgr'][j])
+                        self.col["Dfg"][j] = (
+                            self.dest[j][list(self.dest[j].keys())[i]] + self.col["Dgr"][j]
+                        )
 
                 self.calc_lci()
                 for j in self.dest.keys():
                     if len(self.dest[j]) > i:
                         key = list(self.dest[j].keys())[i]
                         self.result_destination[j][key] = {}
 
-                        self.result_destination[j][key][('Technosphere', 'Equipment_Diesel')] = (
-                            self.output['FuelMg'][j]
-                            + self.output['FuelMg_dov'][j])
-
-                        self.result_destination[j][key][('Technosphere', 'Equipment_CNG')] = (
-                            self.output['FuelMg_CNG'][j])
-
-                        self.result_destination[j][key][('Technosphere', 'Electricity_consumption')] = (
-                            self.output['ElecMg'][j])
-
-                        self.result_destination[j][key][('biosphere3', 'Operational_Cost')] = (
-                            self.output['C_collection'][j])
+                        self.result_destination[j][key][("Technosphere", "Equipment_Diesel")] = (
+                            self.output["FuelMg"][j] + self.output["FuelMg_dov"][j]
+                        )
+
+                        self.result_destination[j][key][
+                            ("Technosphere", "Equipment_CNG")
+                        ] = self.output["FuelMg_CNG"][j]
+
+                        self.result_destination[j][key][
+                            ("Technosphere", "Electricity_consumption")
+                        ] = self.output["ElecMg"][j]
+
+                        self.result_destination[j][key][
+                            ("biosphere3", "Operational_Cost")
+                        ] = self.output["C_collection"][j]
         else:
             self.calc_lci()
             self.result_destination = {}
 
     def calc_lci(self):
         # Selected compartment compaction density  (lb/yd3)
         # Override calculated density den_c and use an average assumed in-truck density
-        d_msw = self.col['den_asmd'].values
-        d_msw[d_msw <= 0] = self.col['den_c'].values[d_msw <= 0]
-        self.col['d_msw'] = d_msw
+        d_msw = self.col["den_asmd"].values
+        d_msw[d_msw <= 0] = self.col["den_c"].values[d_msw <= 0]
+        self.col["d_msw"] = d_msw
 
         # Distance between service stops, adjusted (miles)
-        self.col['Dbtw'] = self.col['D100'].values / self.col['Prtcp'].values
+        self.col["Dbtw"] = self.col["D100"].values / self.col["Prtcp"].values
 
         # Travel time between service stops, adjusted based on participation (min/stop)
-        self.col['Tbtw'] = self.col['Dbtw'].values / self.col['Vbet'].values * 60
+        self.col["Tbtw"] = self.col["Dbtw"].values / self.col["Vbet"].values * 60
 
         # Travel time btwn route and disposal fac. (min/trip)
-        self.col['Trf'] = self.col['Drf'].values / self.col['Vrf'].values * 60
+        self.col["Trf"] = self.col["Drf"].values / self.col["Vrf"].values * 60
 
         # Time from grg to 1st collection route (min/day-vehicle)
-        self.col['Tgr'] = self.col['Dgr'].values / self.col['Vgr'].values * 60
+        self.col["Tgr"] = self.col["Dgr"].values / self.col["Vgr"].values * 60
 
         # Time from disposal fac. to garage (min/day-vehicle)
-        self.col['Tfg'] = self.col['Dfg'].values / self.col['Vfg'].values * 60
+        self.col["Tfg"] = self.col["Dfg"].values / self.col["Vfg"].values * 60
 
-        for i in ['RWC', 'SSR', 'DSR', 'MSR', 'LV',
-                  'SSYW', 'SSO', 'MRDO', 'SSYWDO', 'MSRDO']:
-            self.col.loc[i, 'mass'] = self.mass[i].values.sum()
+        for i in ["RWC", "SSR", "DSR", "MSR", "LV", "SSYW", "SSO", "MRDO", "SSYWDO", "MSRDO"]:
+            self.col.loc[i, "mass"] = self.mass[i].values.sum()
 
         # Mass of ORG_DryRes and REC_WetRec
-        for i, j in [('ORG', 'DryRes'), ('REC', 'WetRes')]:
-            self.col.loc[i, 'mass'] = (self.mass[i].values + self.mass[j].values).sum()
+        for i, j in [("ORG", "DryRes"), ("REC", "WetRes")]:
+            self.col.loc[i, "mass"] = (self.mass[i].values + self.mass[j].values).sum()
 
         # Revising mass of LV collection - as it happens only in LV_serv_pd
-        self.col.loc['LV', 'mass'] = (
-            self.col.loc['LV', 'mass'] * 365 / 7
-            / self.InputData.Col['LV_serv_pd']['amount'])
+        self.col.loc["LV", "mass"] = (
+            self.col.loc["LV", "mass"] * 365 / 7 / self.InputData.Col["LV_serv_pd"]["amount"]
+        )
 
         # Calculations for collection vehicle activities
         # Houses per trip (Volume limited) and (mass limited)
         Ht_v = np.zeros(self.col.shape[0])
         Ht_m = np.zeros(self.col.shape[0])
 
-        fltr = self.col['mass'].values > 0
+        fltr = self.col["mass"].values > 0
         Ht_v[fltr] = (
-            self.col['Ut'].values[fltr]
-            * self.col['Vt'].values[fltr]
-            * self.col['d_msw'].values[fltr]
+            self.col["Ut"].values[fltr]
+            * self.col["Vt"].values[fltr]
+            * self.col["d_msw"].values[fltr]
             * 0.4536  # lb to kg
-            * self.col['Fr'].values[fltr]
-            / self.col['mass'].values[fltr])
+            * self.col["Fr"].values[fltr]
+            / self.col["mass"].values[fltr]
+        )
 
         Ht_m[fltr] = (
-            self.col['max_weight'].values[fltr]
-            * self.col['Fr'].values[fltr]
+            self.col["max_weight"].values[fltr]
+            * self.col["Fr"].values[fltr]
             * 1000
-            / self.col['mass'].values[fltr])
+            / self.col["mass"].values[fltr]
+        )
 
-        self.col['Ht_v'] = Ht_v
-        self.col['Ht_m'] = Ht_m
+        self.col["Ht_v"] = Ht_v
+        self.col["Ht_m"] = Ht_m
 
         # Households per trip (limited by mass or volume)
-        Ht = self.col['Ht_v'].values
-        fltr_2 = self.col['wt_lim'].values == 1
-        fltr_3 = Ht[fltr_2] > self.col['Ht_m'].values[fltr_2]
-        Ht[fltr_2][fltr_3] = self.col['Ht_m'].values[fltr_3]
-        self.col['Ht'] = Ht
+        Ht = self.col["Ht_v"].values
+        fltr_2 = self.col["wt_lim"].values == 1
+        fltr_3 = Ht[fltr_2] > self.col["Ht_m"].values[fltr_2]
+        Ht[fltr_2][fltr_3] = self.col["Ht_m"].values[fltr_3]
+        self.col["Ht"] = Ht
 
         # Time per trip (min/trip)
         # Collection
-        self.col['Tc'] = (
-            self.col['Tbtw'].values * (self.col['Ht'].values /self.InputData.Col['HS']['amount'] - 1)  # collection travel
-            + self.col['TL'].values * self.col['Ht'].values / self.InputData.Col['HS']['amount']  # collection loading
-            + 2 * self.col['Trf'].values  # travel
-            + self.col['S'].values)  # unload time
+        self.col["Tc"] = (
+            self.col["Tbtw"].values
+            * (self.col["Ht"].values / self.InputData.Col["HS"]["amount"] - 1)  # collection travel
+            + self.col["TL"].values
+            * self.col["Ht"].values
+            / self.InputData.Col["HS"]["amount"]  # collection loading
+            + 2 * self.col["Trf"].values  # travel
+            + self.col["S"].values
+        )  # unload time
 
         # Trips per day per vehicle (trip/day-vehicle)
-        self.col['RD'] = (
-            self.col['WV'].values * 60
-            - (self.col['F1_'].values + self.col['F2_'].values + self.col['Tfg'].values)
-            - 0.5 * (self.col['Trf'].values + self.col['S'].values)) / self.col['Tc'].values
+        self.col["RD"] = (
+            self.col["WV"].values * 60
+            - (self.col["F1_"].values + self.col["F2_"].values + self.col["Tfg"].values)
+            - 0.5 * (self.col["Trf"].values + self.col["S"].values)
+        ) / self.col["Tc"].values
 
         # Check that the inputs are realistic
-        if any(self.col['RD'].values < 0):
-            raise Exception("Travelling time is too long that the truck cannot make a loop trip in one day!")
+        if any(self.col["RD"].values < 0):
+            raise ValueError(
+                "Traveling time is too long that the truck cannot make a loop trip in one day!"
+            )
 
         # Daily weight of refuse collected per vehicle (Mg/vehicle-day)
-        self.col['RefD'] = (
-            self.col['Ht'].values
-            * self.col['mass'].values / 1000
-            / self.col['Fr'].values
-            * self.col['RD'].values)
+        self.col["RefD"] = (
+            self.col["Ht"].values
+            * self.col["mass"].values
+            / 1000
+            / self.col["Fr"].values
+            * self.col["RD"].values
+        )
 
         # Number of collection stops per day (stops/vehicle-day)
-        self.col['SD'] = (
-            self.col['Ht'].values
-            * self.col['RD'].values
-            / self.InputData.Col['HS']['amount'])
+        self.col["SD"] = (
+            self.col["Ht"].values * self.col["RD"].values / self.InputData.Col["HS"]["amount"]
+        )
 
         # Calculations for collection vehicle activities (Drop off)
-        for i in ['MRDO', 'SSYWDO', 'MSRDO']:
+        for i in ["MRDO", "SSYWDO", "MSRDO"]:
             # volume of recyclables deposited at drop-off site per week (cy/week-house)
-            self.col.loc[i, 'Ht'] = (
+            self.col.loc[i, "Ht"] = (
                 self.mass[i].values.sum()
-                * self.InputData.Col['houses_res']['amount']
+                * self.InputData.Col["houses_res"]["amount"]
                 * self.col_proc[i]
                 / 0.4536  # lb to kg
-                / self.col['d_msw'][i])
+                / self.col["d_msw"][i]
+            )
 
             # collection vehicle trips per week (trips/week)
-            self.col.loc[i, 'DO_trip_week'] = (
-                self.col['Ht'][i]
-                / (self.col['Vt'][i] * self.col['Ut'][i]))
+            self.col.loc[i, "DO_trip_week"] = self.col["Ht"][i] / (
+                self.col["Vt"][i] * self.col["Ut"][i]
+            )
 
             # time per trip (min/trip) -- load+travel+unload time
-            self.col.loc[i, 'Tc'] = (
-                self.col['TL'][i]
-                + 2 * self.col['Trf'][i]
-                + self.col['S'][i])
+            self.col.loc[i, "Tc"] = self.col["TL"][i] + 2 * self.col["Trf"][i] + self.col["S"][i]
 
             # trips per day per vehicle (trip/day-vehicle)
-            self.col.loc[i, 'RD'] = (
-                self.col['WV'][i] * 60
-                - (self.col['F1_'][i]
-                   + self.col['F2_'][i]
-                   + self.col['Tfg'][i]
-                   + self.col['Tgr'][i])
-                + self.col['Trf'][i]) / self.col['Tc'][i]
+            self.col.loc[i, "RD"] = (
+                self.col["WV"][i] * 60
+                - (
+                    self.col["F1_"][i]
+                    + self.col["F2_"][i]
+                    + self.col["Tfg"][i]
+                    + self.col["Tgr"][i]
+                )
+                + self.col["Trf"][i]
+            ) / self.col["Tc"][i]
 
             # daily weight of refuse collected per vehicle (tons/day-vehicle)
-            self.col.loc[i, 'RefD'] = (
-                self.col['Vt'][i]
-                * self.col['Ut'][i]
-                * self.col['d_msw'][i]
+            self.col.loc[i, "RefD"] = (
+                self.col["Vt"][i]
+                * self.col["Ut"][i]
+                * self.col["d_msw"][i]
                 * 0.4536  # lb to kg
                 / 1000  # kg to Mg
-                * self.col['RD'][i])
+                * self.col["RD"][i]
+            )
 
             # number of collection stops per day (stops/vehicle-day) (1 stop per trip)
-            self.col.loc[i, 'SD'] = self.col['RD'][i]
+            self.col.loc[i, "SD"] = self.col["RD"][i]
 
         # Daily collection vehicle activity times
         # loading time at collection stops (min/day-vehicle) & loading time at drop-off site (min/day-vehicle)
-        self.col['LD'] = self.col['SD'].values * self.col['TL'].values
+        self.col["LD"] = self.col["SD"].values * self.col["TL"].values
 
         # travel time between collection stops (min/day-vehicle)
-        fltr_3 = self.col['SD'].values - 1 >= 1
+        fltr_3 = self.col["SD"].values - 1 >= 1
         Tb = np.zeros(self.col.shape[0])
-        Tb[fltr_3] = (self.col['SD'].values[fltr_3] - 1) * self.col['Tbtw'].values[fltr_3]
-        self.col['Tb'] = Tb
+        Tb[fltr_3] = (self.col["SD"].values[fltr_3] - 1) * self.col["Tbtw"].values[fltr_3]
+        self.col["Tb"] = Tb
 
         # travel time between route and disposal facility (min/day-vehicle)
-        self.col['F_R'] = (2 * self.col['RD'].values + 0.5) * self.col['Trf'].values
+        self.col["F_R"] = (2 * self.col["RD"].values + 0.5) * self.col["Trf"].values
 
         # unloading time at disposal facility (min/day-vehicle)
-        self.col['UD'] = (self.col['RD'].values + 0.5) * self.col['S'].values
+        self.col["UD"] = (self.col["RD"].values + 0.5) * self.col["S"].values
 
-        for i in ['MRDO', 'SSYWDO', 'MSRDO']:
-            self.col.loc[i, 'Tb'] = 0
+        for i in ["MRDO", "SSYWDO", "MSRDO"]:
+            self.col.loc[i, "Tb"] = 0
 
             # travel time between disposal facility and drop-off site (min/day-vehicle)
-            self.col.loc[i, 'F_R'] = (2 * self.col['RD'][i] - 1) * self.col['Trf'][i]
+            self.col.loc[i, "F_R"] = (2 * self.col["RD"][i] - 1) * self.col["Trf"][i]
 
             # unloading time at disposal facility (min/day-vehicle)
-            self.col.loc[i, 'UD'] = self.col['RD'][i] * self.col['S'][i]
-
+            self.col.loc[i, "UD"] = self.col["RD"][i] * self.col["S"][i]
 
         # Daily fuel usage - Diesel
-        fltr_4 = self.col['MPG_all'].values != 0
+        fltr_4 = self.col["MPG_all"].values != 0
 
         # from garage to first collection route (gallons/day-vehicle)
         diesel_gr = (
-            self.col['Fract_Dies'].values
-            * self.col['Dgr'].values
-            *((1 - self.col['fDgr'].values)
-              / self.col['MPG_urban'].values
-              + self.col['fDgr'].values
-              /self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["Dgr"].values
+            * (
+                (1 - self.col["fDgr"].values) / self.col["MPG_urban"].values
+                + self.col["fDgr"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_gr[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dgr'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
-
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dgr"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         # break time, if spent idling
         diesel_idl = (
-            self.col['Fract_Dies'].values
-            * (self.col['F1_'].values
-               * self.col['F1_idle'].values
-               + self.col['F2_'].values
-               * self.col['F2_idle'].values)
+            self.col["Fract_Dies"].values
+            * (
+                self.col["F1_"].values * self.col["F1_idle"].values
+                + self.col["F2_"].values * self.col["F2_idle"].values
+            )
             / 60
-            * self.col['GPH_idle_cv'].values)
+            * self.col["GPH_idle_cv"].values
+        )
 
         diesel_idl[fltr_4] = 0
 
         # from first through last collection stop (gallons/day-vehicle)
         diesel_col = (
-            self.col['Fract_Dies'].values
-            * self.col['Dbtw'].values
-            * self.col['SD'].values
-            / self.col['MPG_collection'].values)
+            self.col["Fract_Dies"].values
+            * self.col["Dbtw"].values
+            * self.col["SD"].values
+            / self.col["MPG_collection"].values
+        )
 
         diesel_col[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dbtw'].values[fltr_4]
-            * self.col['SD'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dbtw"].values[fltr_4]
+            * self.col["SD"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
-
-        index_dict = dict(zip(self.col.index,
-                              np.arange(len(self.col.index))))
+        index_dict = dict(zip(self.col.index, np.arange(len(self.col.index))))
         fltr_DO = [False for i in self.col.index]
-        for i in ['MRDO', 'SSYWDO', 'MSRDO']:
+        for i in ["MRDO", "SSYWDO", "MSRDO"]:
             fltr_DO[index_dict[i]] = True
         diesel_col[fltr_DO] = 0
 
-       # between disposal facility and route (gallons/day-vehicle)
+        # between disposal facility and route (gallons/day-vehicle)
         diesel_rf = (
-            self.col['Fract_Dies'].values
-            * self.col['F_R'].values / 60
-            * self.col['Vrf'].values
-            * ((1 - self.col['fDrd'].values) / self.col['MPG_urban'].values
-               + self.col['fDrd'].values / self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["F_R"].values
+            / 60
+            * self.col["Vrf"].values
+            * (
+                (1 - self.col["fDrd"].values) / self.col["MPG_urban"].values
+                + self.col["fDrd"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_rf[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['F_R'].values[fltr_4] / 60
-            * self.col['Vrf'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["F_R"].values[fltr_4]
+            / 60
+            * self.col["Vrf"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         # unloading at disposal facility (gallons/day-vehicle)
         diesel_ud = (
-            self.col['Fract_Dies'].values
-            * self.col['UD'].values / 60
-            * self.col['GPH_idle_cv'].values)
+            self.col["Fract_Dies"].values
+            * self.col["UD"].values
+            / 60
+            * self.col["GPH_idle_cv"].values
+        )
 
         diesel_ud[fltr_4] = 0
 
-       # from disposal facility to garage (gallons/day-vehicle)
+        # from disposal facility to garage (gallons/day-vehicle)
         diesel_fg = (
-            self.col['Fract_Dies'].values
-            * self.col['Dfg'].values
-            * ((1 - self.col['fDfg'].values) / self.col['MPG_urban'].values
-               + self.col['fDfg'].values / self.col['MPG_highway'].values))
+            self.col["Fract_Dies"].values
+            * self.col["Dfg"].values
+            * (
+                (1 - self.col["fDfg"].values) / self.col["MPG_urban"].values
+                + self.col["fDfg"].values / self.col["MPG_highway"].values
+            )
+        )
 
         diesel_fg[fltr_4] = (
-            self.col['Fract_Dies'].values[fltr_4]
-            * self.col['Dfg'].values[fltr_4]
-            / self.col['MPG_all'].values[fltr_4])
+            self.col["Fract_Dies"].values[fltr_4]
+            * self.col["Dfg"].values[fltr_4]
+            / self.col["MPG_all"].values[fltr_4]
+        )
 
         FuelD = pd.Series(
-            (diesel_gr + diesel_idl + diesel_col
-             + diesel_rf + diesel_ud + diesel_fg),
-             index=self.col.index)
+            (diesel_gr + diesel_idl + diesel_col + diesel_rf + diesel_ud + diesel_fg),
+            index=self.col.index,
+        )
 
         for key, val in self.col_proc.items():
             if val == 0:
                 FuelD[key] = 0
 
-        self.col['FuelD'] = FuelD
+        self.col["FuelD"] = FuelD
 
         # Daily fuel usage - CNG - diesel gal equivalent
-        fltr_6 = self.col['MPG_all_CNG'].values != 0
+        fltr_6 = self.col["MPG_all_CNG"].values != 0
 
         # from garage to first collection route ((diesel gal equivalent/day-vehicle)
         CNG_gr = (
-            self.col['Fract_CNG'].values
-            * self.col['Dgr'].values
-            *((1 - self.col['fDgr'].values)
-              / self.col['MPG_urban_CNG'].values
-              + self.col['fDgr'].values
-              /self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["Dgr"].values
+            * (
+                (1 - self.col["fDgr"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDgr"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_gr[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dgr'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
-
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dgr"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         # break time, if spent idling
         CNG_idl = (
-            self.col['Fract_CNG'].values
-            * (self.col['F1_'].values
-               * self.col['F1_idle'].values
-               + self.col['F2_'].values
-               * self.col['F2_idle'].values)
+            self.col["Fract_CNG"].values
+            * (
+                self.col["F1_"].values * self.col["F1_idle"].values
+                + self.col["F2_"].values * self.col["F2_idle"].values
+            )
             / 60
-            * self.col['GPH_idle_CNG'].values)
+            * self.col["GPH_idle_CNG"].values
+        )
 
         CNG_idl[fltr_6] = 0
 
         # from first through last collection stop (diesel gal equivalent/day-vehicle)
         CNG_col = (
-            self.col['Fract_CNG'].values
-            * self.col['Dbtw'].values
-            * self.col['SD'].values
-            / self.col['MPG_col_CNG'].values)
+            self.col["Fract_CNG"].values
+            * self.col["Dbtw"].values
+            * self.col["SD"].values
+            / self.col["MPG_col_CNG"].values
+        )
 
         CNG_col[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dbtw'].values[fltr_6]
-            * self.col['SD'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dbtw"].values[fltr_6]
+            * self.col["SD"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         CNG_col[fltr_DO] = 0
 
-       # between disposal facility and route (diesel gal equivalent/day-vehicle)
+        # between disposal facility and route (diesel gal equivalent/day-vehicle)
         CNG_rf = (
-            self.col['Fract_CNG'].values
-            * self.col['F_R'].values / 60
-            * self.col['Vrf'].values
-            * ((1 - self.col['fDrd'].values) / self.col['MPG_urban_CNG'].values
-               + self.col['fDrd'].values / self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["F_R"].values
+            / 60
+            * self.col["Vrf"].values
+            * (
+                (1 - self.col["fDrd"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDrd"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_rf[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['F_R'].values[fltr_6] / 60
-            * self.col['Vrf'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["F_R"].values[fltr_6]
+            / 60
+            * self.col["Vrf"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         # unloading at disposal facility (diesel gal equivalent/day-vehicle)
         CNG_ud = (
-            self.col['Fract_CNG'].values
-            * self.col['UD'].values / 60
-            * self.col['GPH_idle_CNG'].values)
+            self.col["Fract_CNG"].values
+            * self.col["UD"].values
+            / 60
+            * self.col["GPH_idle_CNG"].values
+        )
 
         CNG_ud[fltr_6] = 0
 
-       # from disposal facility to garage (diesel gal equivalent/day-vehicle)
+        # from disposal facility to garage (diesel gal equivalent/day-vehicle)
         CNG_fg = (
-            self.col['Fract_CNG'].values
-            * self.col['Dfg'].values
-            * ((1 - self.col['fDfg'].values) / self.col['MPG_urban_CNG'].values
-               + self.col['fDfg'].values / self.col['MPG_hwy_CNG'].values))
+            self.col["Fract_CNG"].values
+            * self.col["Dfg"].values
+            * (
+                (1 - self.col["fDfg"].values) / self.col["MPG_urban_CNG"].values
+                + self.col["fDfg"].values / self.col["MPG_hwy_CNG"].values
+            )
+        )
 
         CNG_fg[fltr_6] = (
-            self.col['Fract_CNG'].values[fltr_6]
-            * self.col['Dfg'].values[fltr_6]
-            / self.col['MPG_all_CNG'].values[fltr_6])
+            self.col["Fract_CNG"].values[fltr_6]
+            * self.col["Dfg"].values[fltr_6]
+            / self.col["MPG_all_CNG"].values[fltr_6]
+        )
 
         FuelD_CNG = pd.Series(
-            (CNG_gr + CNG_idl + CNG_col
-             + CNG_rf + CNG_ud + CNG_fg),
-             index=self.col.index)
+            (CNG_gr + CNG_idl + CNG_col + CNG_rf + CNG_ud + CNG_fg), index=self.col.index
+        )
 
         for key, val in self.col_proc.items():
             if val == 0:
                 FuelD_CNG[key] = 0
 
-        self.col['FuelD_CNG'] = FuelD_CNG
+        self.col["FuelD_CNG"] = FuelD_CNG
 
         # ENERGY CONSUMPTION
         # Energy consumption by collection vehicles
         # total coll. vehicle fuel use per Mg of refuse (L/Mg)
         FuelMg = np.zeros(self.col.shape[0])
-        flter_7 = self.col['RefD'].values > 0
+        flter_7 = self.col["RefD"].values > 0
         FuelMg[flter_7] = (
-            self.col['FuelD'].values[flter_7]
+            self.col["FuelD"].values[flter_7]
             * 3.785  # gal to ltr
-            / self.col['RefD'].values[flter_7])
-        self.col['FuelMg'] = FuelMg
+            / self.col["RefD"].values[flter_7]
+        )
+        self.col["FuelMg"] = FuelMg
 
         # total coll. vehicle CNG fuel use per Mg of refuse (diesel L equivalent/Mg)
         FuelMg_CNG = np.zeros(self.col.shape[0])
         FuelMg_CNG[flter_7] = (
-            self.col['FuelD_CNG'].values[flter_7]
+            self.col["FuelD_CNG"].values[flter_7]
             * 3.785  # gal to ltr
-            / self.col['RefD'].values[flter_7])
-        self.col['FuelMg_CNG'] = FuelMg_CNG
+            / self.col["RefD"].values[flter_7]
+        )
+        self.col["FuelMg_CNG"] = FuelMg_CNG
 
         # Energy consumption by drop-off vehicles
         P_use_Seri = pd.Series(index=self.col.index)
         col_proc_Seri = pd.Series(index=self.col.index)
-        self.col_proc
+
         for key, val in index_dict.items():
             P_use_Seri[val] = self.P_use[key]
             col_proc_Seri[val] = self.col_proc[key]
 
         # fuel usage per trip to drop-off site (gallons/trip)
         FuelT = np.zeros(self.col.shape[0])
         FuelT[fltr_DO] = (
             P_use_Seri.values[fltr_DO]
-            * self.col['RTDdos'].values[fltr_DO]
-            * self.col['DED'].values[fltr_DO]
-            / self.col['dropoff_MPG'].values[fltr_DO] )
-        self.col['FuelT'] = FuelT
+            * self.col["RTDdos"].values[fltr_DO]
+            * self.col["DED"].values[fltr_DO]
+            / self.col["dropoff_MPG"].values[fltr_DO]
+        )
+        self.col["FuelT"] = FuelT
 
-        for i in ['MRDO', 'SSYWDO', 'MSRDO']:
+        for i in ["MRDO", "SSYWDO", "MSRDO"]:
             # weight of refuse delivered per trip (kg/trip)
-            self.col.loc[i, 'RefT'] = (
+            self.col.loc[i, "RefT"] = (
                 self.mass[i].values.sum()
-                * self.col['Prtcp'][i]
-                * 365 / 7
-                / (self.col['FREQdos'][i] * 12))
+                * self.col["Prtcp"][i]
+                * 365
+                / 7
+                / (self.col["FREQdos"][i] * 12)
+            )
 
         # total dropoff vehicle  fuel use per Mg of refuse (L/Mg)
         FuelMg_dov = np.zeros(self.col.shape[0])
-        flter_8 = self.col['RefT'].values > 0
+        flter_8 = self.col["RefT"].values > 0
         FuelMg_dov[flter_8] = (
-            self.col['FuelT'].values[flter_8]
+            self.col["FuelT"].values[flter_8]
             * 3.785  # gal to ltr
-            / (self.col['RefT'].values[flter_8] / 1000))
-        self.col['FuelMg_dov'] = FuelMg_dov
+            / (self.col["RefT"].values[flter_8] / 1000)
+        )
+        self.col["FuelMg_dov"] = FuelMg_dov
 
         # Energy consumption by garage
         # daily electricity usage per vehicle  (kWh/vehicle-day)
-        self.col['ElecD'] = (
-            P_use_Seri.values
-            * (self.col['grg_area'].values * self.col['grg_enrg'].values
-               + self.col['off_area'].values * self.col['off_enrg'].values))
+        self.col["ElecD"] = P_use_Seri.values * (
+            self.col["grg_area"].values * self.col["grg_enrg"].values
+            + self.col["off_area"].values * self.col["off_enrg"].values
+        )
 
         # electricity usage per Mg of refuse  (kWh/Mg)
         ElecMg = np.zeros(self.col.shape[0])
-        ElecMg[flter_7] = (
-            self.col['ElecD'].values[flter_7]
-            / self.col['RefD'].values[flter_7])
-        self.col['ElecMg'] =  ElecMg
+        ElecMg[flter_7] = self.col["ElecD"].values[flter_7] / self.col["RefD"].values[flter_7]
+        self.col["ElecMg"] = ElecMg
 
         # Mass
         # total mass of refuse collected per year (Mg)
-        self.col['TotalMass'] = self.col_massflow.sum()
+        self.col["TotalMass"] = self.col_massflow.sum()
 
         # COLLECTION COSTS
         # Breakdown of capital costs
 
         # annual capital cost per vehicle ($/vehicle-year)
-        self.col['C_cap_v'] = (
-            (1 + self.col['e'].values)
-            * npf.pmt(self.InputData.LCC['Discount_rate']['amount'],
-                      self.col['Lt'].values,
-                      -self.col['Pt'].values))
+        self.col["C_cap_v"] = (1 + self.col["e"].values) * npf.pmt(
+            self.InputData.LCC["Discount_rate"]["amount"],
+            self.col["Lt"].values,
+            -self.col["Pt"].values,
+        )
 
         # number of collection vehicles (vehicles)
-        self.col['Nt'] = (
-            self.InputData.Col['houses_res']['amount']
+        self.col["Nt"] = (
+            self.InputData.Col["houses_res"]["amount"]
             * col_proc_Seri.values
-            * self.col['Fr'].values
-            / (self.col['Ht'].values
-               * self.col['RD'].values
-               * self.col['CD'].values))
+            * self.col["Fr"].values
+            / (self.col["Ht"].values * self.col["RD"].values * self.col["CD"].values)
+        )
 
         # annualized capital cost per bin ($/bin-year)
-        self.col['Cb'] = (
-            (1 + self.col['e'].values)
-            * npf.pmt(self.InputData.LCC['Discount_rate']['amount'],
-                      self.col['Lb'].values,
-                      -self.col['Pb'].values))
+        self.col["Cb"] = (1 + self.col["e"].values) * npf.pmt(
+            self.InputData.LCC["Discount_rate"]["amount"],
+            self.col["Lb"].values,
+            -self.col["Pb"].values,
+        )
 
         # no. of bins per vehicle (bins/vehicle)
-        self.col['Nb'] = (
-            self.col['Rb'].values
-            * (self.col['Ht'].values / self.col['Prtcp'].values)
-            * self.col['RD'].values
-            * self.col['CD'].values
-            / self.col['Fr'].values)
+        self.col["Nb"] = (
+            self.col["Rb"].values
+            * (self.col["Ht"].values / self.col["Prtcp"].values)
+            * self.col["RD"].values
+            * self.col["CD"].values
+            / self.col["Fr"].values
+        )
 
         # bin annual cost per vehicle ($/vehicle-year)
-        self.col['C_cap_b'] = (
-            self.col['Cb'].values * self.col['Nb'].values)
+        self.col["C_cap_b"] = self.col["Cb"].values * self.col["Nb"].values
 
         # Breakdown of operating costs
         # labor cost per vehicle ($/vehicle-year)
-        self.col['Cw'] = (
-            (1 + self.col['a'].values)
-            * ((1 + self.col['bw'].values)
-               * (self.col['Wa'].values * self.col['Nw'].values
-                  + self.col['Wd'].values)
-               * self.col['WP'].values
-               * self.col['CD'].values
-               * 365 / 7))
+        self.col["Cw"] = (1 + self.col["a"].values) * (
+            (1 + self.col["bw"].values)
+            * (self.col["Wa"].values * self.col["Nw"].values + self.col["Wd"].values)
+            * self.col["WP"].values
+            * self.col["CD"].values
+            * 365
+            / 7
+        )
 
         # O&M cost per vehicle ($/vehicle-year)
-        self.col['Cvo'] = self.col['c'].values
+        self.col["Cvo"] = self.col["c"].values
 
         # other expenses per vehicle ($/vehicle-year)
-        self.col['Coe'] = self.col['d'].values * (self.col['Nw'].values + 1)
+        self.col["Coe"] = self.col["d"].values * (self.col["Nw"].values + 1)
 
         # Annual operating cost ($/vehicle-year)
-        self.col['C_op'] = (
-            (1 + self.col['e'].values)
-            * (self.col['Cw'].values
-               + self.col['Cvo'].values
-               + self.col['Coe'].values))
+        self.col["C_op"] = (1 + self.col["e"].values) * (
+            self.col["Cw"].values + self.col["Cvo"].values + self.col["Coe"].values
+        )
 
         # Total annual cost per vehicle -- cap + O&M ($/vehicle-year)
-        self.col['C_vehicle'] = (
-            (1 + self.col['bv'].values)
-            * self.col['C_cap_v'].values
-            + self.col['C_op'].values)
+        self.col["C_vehicle"] = (1 + self.col["bv"].values) * self.col["C_cap_v"].values + self.col[
+            "C_op"
+        ].values
 
         # Total annual cost per house, including bins ($/house-year)
         # Includes all houses provided service, even if not participating
-        hpdv = (self.col['Ht'].values
-                * self.col['RD'].values
-                * self.col['CD'].values
-                / self.col['Fr'].values)
+        hpdv = (
+            self.col["Ht"].values
+            * self.col["RD"].values
+            * self.col["CD"].values
+            / self.col["Fr"].values
+        )
 
         fltr_9 = hpdv > 0.0
 
         C_house = np.zeros(self.col.shape[0])
 
         C_house[fltr_9] = (
-            self.col['C_vehicle'].values[fltr_9]
-            / hpdv[fltr_9]
-            * self.col['Prtcp'].values[fltr_9])
+            self.col["C_vehicle"].values[fltr_9] / hpdv[fltr_9] * self.col["Prtcp"].values[fltr_9]
+        )
 
-        C_house += (self.col['Cb'].values * self.col['Rb'].values)
+        C_house += self.col["Cb"].values * self.col["Rb"].values
         C_house[np.isnan(C_house)] = 0.0
-        self.col['C_house'] = C_house
+        self.col["C_house"] = C_house
 
         # Cost per ton of refuse collected - Cap+OM+bins ($/Mg)
-        self.col['C_collection'] = (
-            (self.col['C_house'] * 7 / 365)
-            / (self.mass.sum() / 1000)).replace([np.inf, np.nan], 0)
+        self.col["C_collection"] = (
+            (self.col["C_house"] * 7 / 365) / (self.mass.sum() / 1000)
+        ).replace([np.inf, np.nan], 0)
 
         # OUTPUT
-        # Energy use is calculated for ORG and it is same with Dryres
-        self.col.loc['DryRes', 'FuelMg'] = self.col['FuelMg']['ORG']
-        self.col.loc['DryRes', 'FuelMg_CNG'] = self.col['FuelMg_CNG']['ORG']
-        self.col.loc['DryRes', 'ElecMg'] = self.col['ElecMg']['ORG']
+        # Energy use is calculated for ORG and it is same with Dryers
+        self.col.loc["DryRes", "FuelMg"] = self.col["FuelMg"]["ORG"]
+        self.col.loc["DryRes", "FuelMg_CNG"] = self.col["FuelMg_CNG"]["ORG"]
+        self.col.loc["DryRes", "ElecMg"] = self.col["ElecMg"]["ORG"]
 
         # Energy use is calculated for REC and it is same with WetRes
-        self.col.loc['WetRes', 'FuelMg'] = self.col['FuelMg']['REC']
-        self.col.loc['WetRes', 'FuelMg_CNG'] = self.col['FuelMg_CNG']['REC']
-        self.col.loc['WetRes', 'ElecMg'] = self.col['ElecMg']['REC']
-
-
-        self.output = self.col[['TotalMass', 'FuelMg', 'FuelMg_CNG',
-                                'ElecMg', 'FuelMg_dov', 'C_collection']]
+        self.col.loc["WetRes", "FuelMg"] = self.col["FuelMg"]["REC"]
+        self.col.loc["WetRes", "FuelMg_CNG"] = self.col["FuelMg_CNG"]["REC"]
+        self.col.loc["WetRes", "ElecMg"] = self.col["ElecMg"]["REC"]
+
+        self.output = self.col[
+            ["TotalMass", "FuelMg", "FuelMg_CNG", "ElecMg", "FuelMg_dov", "C_collection"]
+        ]
         self.output = self.output.fillna(0.0)
-        self.output.loc['SSO_HC', :] = 0.0
+        self.output.loc["SSO_HC", :] = 0.0
 
     def calc(self):
         self.calc_composition()
         self.calc_destin()
 
     # setup for Monte Carlo simulation
     def setup_MC(self, seed=None):
@@ -961,21 +1155,19 @@
 
     def report(self):
         # report
         self.collection = {}
         Waste = {}
         Technosphere = {}
         Biosphere = {}
-        self.collection["process name"] = (self.process_name,
-                                           self.Process_Type,
-                                           self.__class__)
+        self.collection["process name"] = (self.process_name, self.Process_Type, self.__class__)
         self.collection["Waste"] = Waste
         self.collection["Technosphere"] = Technosphere
         self.collection["Biosphere"] = Biosphere
-        self.collection['LCI'] = self.result_destination
+        self.collection["LCI"] = self.result_destination
 
         for x in [Waste, Technosphere, Biosphere]:
             for y in self.Index:
                 x[y] = {}
 
         for y in self.Index:
             for x in self.col_massflow.columns:
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/TS.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,134 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Apr 29 11:51:31 2021
-
-@author: msardar2
-"""
 import numpy as np
 import numpy_financial as npf
 from swolfpy_inputdata import TS_Input
-from .TS_subprocess import LCI, Electricity, Rolling_Stock
+
 from .ProcessModel import ProcessModel
+from .TS_subprocess import LCI, Electricity, Rolling_Stock
 
 
 class TS(ProcessModel):
-    Process_Type = 'Transfer_Station'
-    def __init__(self,process_name='TS', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Transfer_Station"
+
+    def __init__(self, process_name="TS", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData= TS_Input(input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct)
+        self.InputData = TS_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
-        self._Extened_Index = []
-        for i in ['ORG', 'DryRes', 'REC', 'WetRes']:
+        self._Extended_Index = []
+        for i in ["RWC", "SSR", "SSYW", "SSO", "ORG", "DryRes", "REC", "WetRes"]:
             for j in self.Index:
-                self._Extened_Index.append(i + '_' + j)
+                self._Extended_Index.append(i + "_" + j)
 
-#%% Calc Function
+    # %% Calc Function
     def calc(self):
-        n = len(self._Extened_Index)
-        self.LCI_Waste = LCI(self._Extened_Index)
-        self.LCI = LCI(self._Extened_Index)
+        n = len(self._Extended_Index)
+        self.LCI_Waste = LCI(self._Extended_Index)
+        self.LCI = LCI(self._Extended_Index)
 
         ### Initial mass
-        self._Input = np.array([1/n] * n)
+        self._Input = np.array([1 / n] * n)
 
         ### Rolling_Stock
         Rolling_Stock(self._Input, self.InputData, self.LCI)
 
         self._organics = np.zeros(n)
         self._residuals = np.zeros(n)
         self._recyclables = np.zeros(n)
-        for i, j in enumerate(self._Extened_Index):
-            if 'DryRes' == j[0:6] or 'WetRes' == j[0:6]:
+        for i, j in enumerate(self._Extended_Index):
+            if "DryRes" == j[0:6] or "WetRes" == j[0:6] or "RWC" == j[0:3]:
                 self._residuals[i] = 1 / n
-            elif 'ORG'==j[0:3]:
+            elif "ORG" == j[0:3] or "SSYW" == j[0:4] or "SSO" == j[0:3]:
                 self._organics[i] = 1 / n
-            elif 'REC'==j[0:3]:
+            elif "REC" == j[0:3] or "SSR" == j[0:3]:
                 self._recyclables[i] = 1 / n
 
-        self.LCI_Waste.add('Other_Residual', self._residuals)
-        self.LCI_Waste.add('Separated_Organics', self._organics)
-        self.LCI_Waste.add('Separated_Recyclables', self._recyclables)
+        self.LCI_Waste.add("Other_Residual", self._residuals)
+        self.LCI_Waste.add("Separated_Organics", self._organics)
+        self.LCI_Waste.add("Separated_Recyclables", self._recyclables)
 
         ### General Electricity
         Electricity(self._Input, self.InputData, self.LCI)
 
         ### Capital Cost
-        Land_req =  self.InputData.Electricity['Area_rate']['amount'] * self.InputData.Constr_cost['Land_req_factor']['amount']
-        Land_cost = Land_req * self.InputData.Constr_cost['Land_rate']['amount'] / 4046.86  # 1acr = 4046.86 m2
-        Constr_cost =  Land_req * (self.InputData.Constr_cost['Paving_rate']['amount'] +
-                                   self.InputData.Constr_cost['Grading_rate']['amount']) / 10000  # 1ha = 10000m2
-        Constr_cost += (self.InputData.Electricity['Area_rate']['amount'] * self.InputData.Constr_cost['Constr_rate']['amount'] / 0.0929)  # 1ft2 = 0.0929 m2
-        Constr_cost *= (1 + self.InputData.Constr_cost['Eng_rate']['amount'])
+        Land_req = (
+            self.InputData.Electricity["Area_rate"]["amount"]
+            * self.InputData.Constr_cost["Land_req_factor"]["amount"]
+        )
+        Land_cost = (
+            Land_req * self.InputData.Constr_cost["Land_rate"]["amount"] / 4046.86
+        )  # 1acr = 4046.86 m2
+        Constr_cost = (
+            Land_req
+            * (
+                self.InputData.Constr_cost["Paving_rate"]["amount"]
+                + self.InputData.Constr_cost["Grading_rate"]["amount"]
+            )
+            / 10000
+        )  # 1ha = 10000m2
+        Constr_cost += (
+            self.InputData.Electricity["Area_rate"]["amount"]
+            * self.InputData.Constr_cost["Constr_rate"]["amount"]
+            / 0.0929
+        )  # 1ft2 = 0.0929 m2
+        Constr_cost *= 1 + self.InputData.Constr_cost["Eng_rate"]["amount"]
 
         # Add Miscellaneous Costs based on the average size TS: 1000 tpd
-        Miscellaneous_Costs = (self.InputData.Constr_cost['Weigh_Station']['amount'] +
-                               self.InputData.Constr_cost['Utility_Connections']['amount']) / 1000  # Assume capacity of 1000 tpd
-        Miscellaneous_Costs += (self.InputData.Constr_cost['Landscaping_rate']['amount'] / 10000 * Land_req) # 1 ha = 10000m2
-        # Assumes fenc along three sides of square
-        Miscellaneous_Costs += np.sqrt(Land_req * 1000) * 3 * self.InputData.Constr_cost['Fencing_Rate']['amount'] / 1000
+        Miscellaneous_Costs = (
+            self.InputData.Constr_cost["Weigh_Station"]["amount"]
+            + self.InputData.Constr_cost["Utility_Connections"]["amount"]
+        ) / 1000  # Assume capacity of 1000 tpd
+        Miscellaneous_Costs += (
+            self.InputData.Constr_cost["Landscaping_rate"]["amount"] / 10000 * Land_req
+        )  # 1 ha = 10000m2
+        # Assumes fence along three sides of square
+        Miscellaneous_Costs += (
+            np.sqrt(Land_req * 1000)
+            * 3
+            * self.InputData.Constr_cost["Fencing_Rate"]["amount"]
+            / 1000
+        )
 
         # Total capital cost
-        Unit_capital_cost = Land_cost + Constr_cost +  Miscellaneous_Costs  # $/tpd
-        Unit_capital_cost /= self.InputData.Labor['Day_year']['amount']  # $/t.yr
-        capital_cost = -npf.pmt(rate=self.InputData.Constr_cost['Inerest_rate']['amount'],
-                        nper=self.InputData.Constr_cost['lifetime']['amount'],
-                        pv=Unit_capital_cost)
-        self.LCI.add(('biosphere3', 'Capital_Cost'), capital_cost * self._Input)
-
+        Unit_capital_cost = Land_cost + Constr_cost + Miscellaneous_Costs  # $/tpd
+        Unit_capital_cost /= self.InputData.Labor["Day_year"]["amount"]  # $/t.yr
+        capital_cost = -npf.pmt(
+            rate=self.InputData.Constr_cost["Interest_rate"]["amount"],
+            nper=self.InputData.Constr_cost["lifetime"]["amount"],
+            pv=Unit_capital_cost,
+        )
+        self.LCI.add(("biosphere3", "Capital_Cost"), capital_cost * self._Input)
 
-#%% Report
+    # %% Report
     ### Report
     def report(self):
         ### Output
         self.SS_MRF = {}
         self.SS_MRF["process name"] = (self.process_name, self.Process_Type, self.__class__)
 
         # Waste
-        #self.waste_DF = self.LCI_Waste.report(self._Input)
-        #self.SS_MRF["Waste"] = self.waste_DF.transpose().to_dict()
+        # self.waste_DF = self.LCI_Waste.report(self._Input)
+        # self.SS_MRF["Waste"] = self.waste_DF.transpose().to_dict()
         self.SS_MRF["Waste"] = self.LCI_Waste.report_T(self._Input).to_dict()
 
         # Technosphere
-        tech_index = [x for x in self.LCI.ColDict.keys() if 'biosphere3' not in x]
-        self.SS_MRF["Technosphere"] = self.LCI.report_T(self._Input).loc[tech_index,:].to_dict()
-
+        tech_index = [x for x in self.LCI.ColDict.keys() if "biosphere3" not in x]
+        self.SS_MRF["Technosphere"] = self.LCI.report_T(self._Input).loc[tech_index, :].to_dict()
 
         # Biosphere
-        bio_index = [x for x in self.LCI.ColDict.keys() if 'biosphere3' in x]
-        self.SS_MRF["Biosphere"] = self.LCI.report_T(self._Input).loc[bio_index,:].to_dict()
-        return(self.SS_MRF)
+        bio_index = [x for x in self.LCI.ColDict.keys() if "biosphere3" in x]
+        self.SS_MRF["Biosphere"] = self.LCI.report_T(self._Input).loc[bio_index, :].to_dict()
+        return self.SS_MRF
 
-#%% Monte Carlo
+    # %% Monte Carlo
     ### setup for Monte Carlo simulation
-    def setup_MC(self,seed=None):
+    def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
 
     ### Calculate based on the generated numbers
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
         self.calc()
-        return(input_list)
+        return input_list
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/TS_subprocess.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/TS_subprocess.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,133 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Tue Jan  7 11:12:21 2020
+from copy import deepcopy
 
-@author: msardar2
-"""
-import pandas as pd
 import numpy as np
-from copy import deepcopy
 import numpy_financial as npf
+import pandas as pd
 
 
-class LCI():
+class LCI:
     """
     This class store the LCI data in numpy.ndarray instead of pandas for speedup.
-    Report function create pandas DataFrame and return it
-    Column names are stored in self.ColDict
+
+    Report function create pandas DataFrame and return it Column names are stored in
+    self.ColDict
     """
-    def __init__(self,Index):
+
+    def __init__(self, Index):
         self.Index = Index
-        self.LCI = np.zeros((len(Index),20))
-        self.ColDict={}
-        self.ColNumber=0
+        self.LCI = np.zeros((len(Index), 20))
+        self.ColDict = {}
+        self.ColNumber = 0
 
-    def add(self,name,flow):
+    def add(self, name, flow):
         if name not in self.ColDict:
-            self.ColDict[name]=self.ColNumber
-            self.ColNumber+=1
-        self.LCI[:,self.ColDict[name]]+=flow
+            self.ColDict[name] = self.ColNumber
+            self.ColNumber += 1
+        self.LCI[:, self.ColDict[name]] += flow
 
-    def report(self,InputMass):
+    def report(self, InputMass):
         LCI_normal = deepcopy(self.LCI)
         for j in range(len(self.ColDict)):
-            LCI_normal[:,j]=self.LCI[:,j]/InputMass
-        return(pd.DataFrame(LCI_normal[:,:len(self.ColDict)],columns=list(self.ColDict.keys()),index=self.Index))
+            LCI_normal[:, j] = self.LCI[:, j] / InputMass
+        return pd.DataFrame(
+            LCI_normal[:, : len(self.ColDict)], columns=list(self.ColDict.keys()), index=self.Index
+        )
 
-    def report_T(self,InputMass):
+    def report_T(self, InputMass):
         LCI_normal = deepcopy(self.LCI)
         for j in range(len(self.ColDict)):
-            LCI_normal[:,j]=self.LCI[:,j]/InputMass
-        return(pd.DataFrame(LCI_normal[:,:len(self.ColDict)].transpose(),index=list(self.ColDict.keys()),columns=self.Index))
+            LCI_normal[:, j] = self.LCI[:, j] / InputMass
+        return pd.DataFrame(
+            LCI_normal[:, : len(self.ColDict)].transpose(),
+            index=list(self.ColDict.keys()),
+            columns=self.Index,
+        )
+
 
 ### Resource use calculation for equipments
 def calc_resource(total_throughput, remaining, removed, Eq, InputData, LCI):
-    #Calculating resource use
-    #Elec use = (motor_size*Frac_motor)/(max_input*frac_input)  --> unit: kW/Mg
-    elec = Eq['motor']['amount'] * Eq['frac_motor']['amount']/ \
-                (Eq['Max_input']['amount']*Eq['frac_MaxInput']['amount'])
-
-    if Eq['Calc_base']['amount']==0: # 0: calculation based on the removed mass
-        Aloc = (removed/sum(removed) if sum(removed)>0 else 0)
-    elif Eq['Calc_base']['amount']==1: # 1: calculation based on the remaining mass
-        Aloc = (remaining/sum(remaining) if sum(remaining)>0 else 0)
-    elif Eq['Calc_base']['amount']==2:  # 2: calculation based on the total throughput mass
-        Aloc = (total_throughput/sum(total_throughput) if sum(total_throughput)>0 else 0)
+    # Calculating resource use
+    # Elec use = (motor_size*Frac_motor)/(max_input*frac_input)  --> unit: kW/Mg
+    elec = (
+        Eq["motor"]["amount"]
+        * Eq["frac_motor"]["amount"]
+        / (Eq["Max_input"]["amount"] * Eq["frac_MaxInput"]["amount"])
+    )
+
+    if Eq["Calc_base"]["amount"] == 0:  # 0: calculation based on the removed mass
+        Aloc = removed / sum(removed) if sum(removed) > 0 else 0
+    elif Eq["Calc_base"]["amount"] == 1:  # 1: calculation based on the remaining mass
+        Aloc = remaining / sum(remaining) if sum(remaining) > 0 else 0
+    elif Eq["Calc_base"]["amount"] == 2:  # 2: calculation based on the total throughput mass
+        Aloc = total_throughput / sum(total_throughput) if sum(total_throughput) > 0 else 0
     else:
-        raise ValueError('Input parameter [Calc_base] is not valid')
+        raise ValueError("Input parameter [Calc_base] is not valid")
 
-    elec_use =  sum(total_throughput) * elec *  Aloc
-    dsl_use = sum(total_throughput) * Eq['diesel_use']['amount'] * Aloc
-    LPG_use = sum(total_throughput) * Eq['LPG_use']['amount'] * Aloc
-
-    Cap = Eq['Investment_cost']['amount'] + Eq['Installation_cost']['amount']
-    Rate = InputData.Constr_cost['Inerest_rate']['amount']
-    Lftime = Eq['LifeTime']['amount']
-    TotalHour = InputData.Labor['Hr_shift']['amount'] * InputData.Labor['Shift_day']['amount'] * InputData.Labor['Day_year']['amount']
+    elec_use = sum(total_throughput) * elec * Aloc
+    dsl_use = sum(total_throughput) * Eq["diesel_use"]["amount"] * Aloc
+    LPG_use = sum(total_throughput) * Eq["LPG_use"]["amount"] * Aloc
+
+    Cap = Eq["Investment_cost"]["amount"] + Eq["Installation_cost"]["amount"]
+    Rate = InputData.Constr_cost["Interest_rate"]["amount"]
+    LifeTime = Eq["LifeTime"]["amount"]
+    TotalHour = (
+        InputData.Labor["Hr_shift"]["amount"]
+        * InputData.Labor["Shift_day"]["amount"]
+        * InputData.Labor["Day_year"]["amount"]
+    )
     # Average Cost of Ownership ($/Mg)
-    AveCostOwner = (npf.pmt(Rate, Lftime, -Cap) + Eq['O&M']['amount']) / (TotalHour * Eq['Max_input']['amount']*Eq['frac_MaxInput']['amount'])
-
-    #Laborers Required (Sorter*hours/Mg)
-    LaborReq = Eq['N_Labor']['amount'] / (Eq['Max_input']['amount'] * Eq['frac_MaxInput']['amount'])
-    #Drivers Required (Driver*hours/Mg)
-    DriverReq = Eq['N_Driver']['amount'] / (Eq['Max_input']['amount'] * Eq['frac_MaxInput']['amount'])
-    #Labor (sorter+Driver) Cost ($/Mg input)
-    LaborCost = (LaborReq * InputData.Labor['Labor_rate']['amount'] + DriverReq * InputData.Labor['Driver_rate']['amount'] ) *\
-                (1 + InputData.Labor['Fringe_rate']['amount']) * (1 + InputData.Labor['Management_rate']['amount'])
+    AveCostOwner = (npf.pmt(Rate, LifeTime, -Cap) + Eq["O&M"]["amount"]) / (
+        TotalHour * Eq["Max_input"]["amount"] * Eq["frac_MaxInput"]["amount"]
+    )
+
+    # Laborers Required (Sorter*hours/Mg)
+    LaborReq = Eq["N_Labor"]["amount"] / (Eq["Max_input"]["amount"] * Eq["frac_MaxInput"]["amount"])
+    # Drivers Required (Driver*hours/Mg)
+    DriverReq = Eq["N_Driver"]["amount"] / (
+        Eq["Max_input"]["amount"] * Eq["frac_MaxInput"]["amount"]
+    )
+    # Labor (sorter+Driver) Cost ($/Mg input)
+    LaborCost = (
+        (
+            LaborReq * InputData.Labor["Labor_rate"]["amount"]
+            + DriverReq * InputData.Labor["Driver_rate"]["amount"]
+        )
+        * (1 + InputData.Labor["Fringe_rate"]["amount"])
+        * (1 + InputData.Labor["Management_rate"]["amount"])
+    )
 
     TotalOMcost = sum(total_throughput) * Aloc * (AveCostOwner + LaborCost)
 
     # adding the resource use
-    LCI.add(('Technosphere', 'Electricity_consumption'), elec_use)
-    LCI.add(('Technosphere', 'Equipment_Diesel'), dsl_use)
-    LCI.add(('Technosphere', 'Equipment_LPG'), LPG_use)
-    LCI.add(('biosphere3', 'Operational_Cost'), TotalOMcost)
+    LCI.add(("Technosphere", "Electricity_consumption"), elec_use)
+    LCI.add(("Technosphere", "Equipment_Diesel"), dsl_use)
+    LCI.add(("Technosphere", "Equipment_LPG"), LPG_use)
+    LCI.add(("biosphere3", "Operational_Cost"), TotalOMcost)
+
 
 ### Rolling_Stock
-def Rolling_Stock(Input,InputData,LCI):
-    #Equipment input
-    Eq=InputData.Eq_Rolling_Stock
-    #Resource use calculation
-    calc_resource(Input,Input,Input,Eq,InputData,LCI)
-    return(None)
+def Rolling_Stock(Input, InputData, LCI):
+    # Equipment input
+    Eq = InputData.Eq_Rolling_Stock
+    # Resource use calculation
+    calc_resource(Input, Input, Input, Eq, InputData, LCI)
+    return None
 
 
 ### General Electricity
 def Electricity(Input, InputData, LCI):
-    #calculate electricity use in office and floor area
-    elec_office = (Input *
-                   InputData.Electricity['Area_rate']['amount'] *
-                   InputData.Electricity['Frac_office']['amount'] *
-                   InputData.Electricity['Elec_office']['amount'])
-    elec_floor = (Input *
-                  InputData.Electricity['Area_rate']['amount'] *
-                  (1 - InputData.Electricity['Frac_office']['amount']) *
-                  InputData.Electricity['Elec_floor']['amount'])
-    LCI.add(('Technosphere', 'Electricity_consumption'), elec_office + elec_floor)
+    # calculate electricity use in office and floor area
+    elec_office = (
+        Input
+        * InputData.Electricity["Area_rate"]["amount"]
+        * InputData.Electricity["Frac_office"]["amount"]
+        * InputData.Electricity["Elec_office"]["amount"]
+    )
+    elec_floor = (
+        Input
+        * InputData.Electricity["Area_rate"]["amount"]
+        * (1 - InputData.Electricity["Frac_office"]["amount"])
+        * InputData.Electricity["Elec_floor"]["amount"]
+    )
+    LCI.add(("Technosphere", "Electricity_consumption"), elec_office + elec_floor)
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/WTE.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/WTE.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,253 +1,306 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Jun 13 15:10:31 2019
-
-@author: msmsa
-"""
+import numpy_financial as npf
 import pandas as pd
 from swolfpy_inputdata import WTE_Input
+
 from .ProcessModel import ProcessModel
-import numpy_financial as npf
 
 
 class WTE(ProcessModel):
-    Process_Type = 'Treatment'
-    def __init__(self, process_name='WTE', input_data_path=None, CommonDataObjct=None):
+    Process_Type = "Treatment"
+
+    def __init__(self, process_name="WTE", input_data_path=None, CommonDataObjct=None):
         super().__init__(process_name, CommonDataObjct)
 
-        self.InputData = WTE_Input(input_data_path,
-                                   process_name=self.process_name,
-                                   CommonDataObjct=CommonDataObjct)
+        self.InputData = WTE_Input(
+            input_data_path, process_name=self.process_name, CommonDataObjct=CommonDataObjct
+        )
 
         self.process_data = self.InputData.process_data
 
     def calc(self):
         self.LCI_index = False
 
         ### Energy Calculations
         self.Energy_Calculations = pd.DataFrame(index=self.Index)
 
         # MJ/Mg
-        self.Energy_Calculations['Energy_Loss_Due_to_Water'] = (
-            -1 * self.Material_Properties['Moisture Content'].values / 100
-            * self.CommonData.Evap_heat['water']['amount'] * 1000)
+        self.Energy_Calculations["Energy_Loss_Due_to_Water"] = (
+            -1
+            * self.Material_Properties["Moisture Content"].values
+            / 100
+            * self.CommonData.Evap_heat["water"]["amount"]
+            * 1000
+        )
 
         # MJ/Mg
-        self.Energy_Calculations['Energy_Loss_Due_to_Ashes'] = (
-            -1 * self.process_data['Ash_Cp'].values
-            * self.process_data['Delta T'].values
-            * (self.Material_Properties['Ash Content'].values / 100
-               + self.Material_Properties['Volatile Solids'].values / 100
-               * (1 - self.process_data['Comb_eff'].values / 100))
-            * (1 - self.Material_Properties['Moisture Content'].values/100))
+        self.Energy_Calculations["Energy_Loss_Due_to_Ashes"] = (
+            -1
+            * self.process_data["Ash_Cp"].values
+            * self.process_data["Delta T"].values
+            * (
+                self.Material_Properties["Ash Content"].values / 100
+                + self.Material_Properties["Volatile Solids"].values
+                / 100
+                * (1 - self.process_data["Comb_eff"].values / 100)
+            )
+            * (1 - self.Material_Properties["Moisture Content"].values / 100)
+        )
 
         # MJ/Mg
-        self.Energy_Calculations['Energy_Produced'] = (
-            self.Material_Properties['Lower Heating Value'].values
-            * self.process_data['Comb_eff'].values / 100
-            * (100 - self.Material_Properties['Moisture Content'].values)
-            / 100 * 1000)
-
+        self.Energy_Calculations["Energy_Produced"] = (
+            self.Material_Properties["Lower Heating Value"].values
+            * self.process_data["Comb_eff"].values
+            / 100
+            * (100 - self.Material_Properties["Moisture Content"].values)
+            / 100
+            * 1000
+        )
 
         # MJ/Mg
-        self.Energy_Calculations['Net_Energy_Produced'] = (
-            self.Energy_Calculations['Energy_Produced'].values
-            + self.Energy_Calculations['Energy_Loss_Due_to_Ashes'].values
-            + self.Energy_Calculations['Energy_Loss_Due_to_Water'].values)
+        self.Energy_Calculations["Net_Energy_Produced"] = (
+            self.Energy_Calculations["Energy_Produced"].values
+            + self.Energy_Calculations["Energy_Loss_Due_to_Ashes"].values
+            + self.Energy_Calculations["Energy_Loss_Due_to_Water"].values
+        )
 
         # kWh/Mg
-        self.Energy_Calculations['Energy_Recovered_as_Electricity'] = (
-            self.Energy_Calculations['Net_Energy_Produced'].values
-            * self.InputData.Elec_Prod_Eff['Gross_Efficiency']['amount'] / 3.6)
+        self.Energy_Calculations["Energy_Recovered_as_Electricity"] = (
+            self.Energy_Calculations["Net_Energy_Produced"].values
+            * self.InputData.Elec_Prod_Eff["Gross_Efficiency"]["amount"]
+            / 3.6
+        )
 
         # kWh/Mg
-        self.Energy_Calculations['Electricity_Use'] = (
-            self.Energy_Calculations['Energy_Recovered_as_Electricity'].values
-            * self.InputData.Elec_Prod_Eff['Internal_use']['amount'])
+        self.Energy_Calculations["Electricity_Use"] = (
+            self.Energy_Calculations["Energy_Recovered_as_Electricity"].values
+            * self.InputData.Elec_Prod_Eff["Internal_use"]["amount"]
+        )
 
         # kWh/Mg
-        self.Energy_Calculations['Net_Electricity_Produced'] = (
-            self.Energy_Calculations['Energy_Recovered_as_Electricity'].values
-            - self.Energy_Calculations['Electricity_Use'].values)
+        self.Energy_Calculations["Net_Electricity_Produced"] = (
+            self.Energy_Calculations["Energy_Recovered_as_Electricity"].values
+            - self.Energy_Calculations["Electricity_Use"].values
+        )
 
         #'MJ/Mg'
-        self.Energy_Calculations['Heat_Recovered'] = (
-            self.Energy_Calculations['Net_Energy_Produced'].values
-            * self.InputData.Elec_Prod_Eff['Heat_prod_Eff']['amount'])
+        self.Energy_Calculations["Heat_Recovered"] = (
+            self.Energy_Calculations["Net_Energy_Produced"].values
+            * self.InputData.Elec_Prod_Eff["Heat_prod_Eff"]["amount"]
+        )
 
         ### Combustion Emission
         self.Combustion_Emission = pd.DataFrame(index=self.Index)
 
         #'kg/kgww'
-        self.Combustion_Emission['CO2_fossil'] = (
-            self.Material_Properties['Fossil Carbon Content'].values / 100
-            * self.process_data['Comb_eff'].values / 100
-            * (1 - self.Material_Properties['Moisture Content'].values / 100)
-            * self.CommonData.MW['CO2']['amount']
-            / self.CommonData.MW['C']['amount'])
+        self.Combustion_Emission["CO2_fossil"] = (
+            self.Material_Properties["Fossil Carbon Content"].values
+            / 100
+            * self.process_data["Comb_eff"].values
+            / 100
+            * (1 - self.Material_Properties["Moisture Content"].values / 100)
+            * self.CommonData.MW["CO2"]["amount"]
+            / self.CommonData.MW["C"]["amount"]
+        )
 
         #'kg/kgww'
-        self.Combustion_Emission['CO2_biogenic'] = (
-            self.Material_Properties['Biogenic Carbon Content'].values / 100
-            * self.process_data['Comb_eff'].values / 100
-            * (1 - self.Material_Properties['Moisture Content'].values / 100)
-            * self.CommonData.MW['CO2']['amount']
-            / self.CommonData.MW['C']['amount'])
+        self.Combustion_Emission["CO2_biogenic"] = (
+            self.Material_Properties["Biogenic Carbon Content"].values
+            / 100
+            * self.process_data["Comb_eff"].values
+            / 100
+            * (1 - self.Material_Properties["Moisture Content"].values / 100)
+            * self.CommonData.MW["CO2"]["amount"]
+            / self.CommonData.MW["C"]["amount"]
+        )
 
         ### Stack metal emissions
-        key1 = {'As': 'Arsenic',
-                'Ba': 'Barium',
-                'Cd': 'Cadmium',
-                'Cr': 'Chromium',
-                'Cu': 'Copper',
-                'Hg': 'Mercury',
-                'Ni': 'Nickel',
-                'Pb': 'Lead',
-                'Sb': 'Antimony',
-                'Se': 'Selenium',
-                'Zn': 'Zinc'}
+        key1 = {
+            "As": "Arsenic",
+            "Ba": "Barium",
+            "Cd": "Cadmium",
+            "Cr": "Chromium",
+            "Cu": "Copper",
+            "Hg": "Mercury",
+            "Ni": "Nickel",
+            "Pb": "Lead",
+            "Sb": "Antimony",
+            "Se": "Selenium",
+            "Zn": "Zinc",
+        }
 
         for m in key1.keys():
             # 'kg/kgww'
             self.Combustion_Emission[m] = (
-                self.Material_Properties[key1[m]].values / 100
-                * self.InputData.Stack_metal_emission[m]['amount']
-                * (1 - self.Material_Properties['Moisture Content'].values / 100))
+                self.Material_Properties[key1[m]].values
+                / 100
+                * self.InputData.Stack_metal_emission[m]["amount"]
+                * (1 - self.Material_Properties["Moisture Content"].values / 100)
+            )
 
         ### mole content of input waste
         #'Moles per dry kg'
-        self.Combustion_Emission['C_mole'] = (
-            (self.Material_Properties['Biogenic Carbon Content'].values
-             + self.Material_Properties['Fossil Carbon Content'].values) / 100
-            / self.CommonData.MW['C']['amount'] * 1000)
-
-
-        key2 = {'Hydrogen Content': ('H', 'H_mole'),
-                'Oxygen Content': ('O', 'O_mole'),
-                'Nitrogen Content': ('N', 'N_mole'),
-                'Chlorine': ('Cl', 'Cl_mole'),
-                'Sulphur': ('S', 'S_mole')}
+        self.Combustion_Emission["C_mole"] = (
+            (
+                self.Material_Properties["Biogenic Carbon Content"].values
+                + self.Material_Properties["Fossil Carbon Content"].values
+            )
+            / 100
+            / self.CommonData.MW["C"]["amount"]
+            * 1000
+        )
+
+        key2 = {
+            "Hydrogen Content": ("H", "H_mole"),
+            "Oxygen Content": ("O", "O_mole"),
+            "Nitrogen Content": ("N", "N_mole"),
+            "Chlorine": ("Cl", "Cl_mole"),
+            "Sulphur": ("S", "S_mole"),
+        }
 
         for m in key2.keys():
             #'Moles per dry kg'
             self.Combustion_Emission[key2[m][1]] = (
-                self.Material_Properties[m].values / 100
-                / self.CommonData.MW[key2[m][0]]['amount'] * 1000)
-
-
-        self.Combustion_Emission['alpha'] = (
-            -0.699 * self.Combustion_Emission['O_mole'].values
-            + 1.5 * self.Combustion_Emission['C_mole'].values
-            + 0.35 * self.Combustion_Emission['H_mole'].values
-            - 0.244 * self.Combustion_Emission['Cl_mole'].values
-            + 1.5 * self.Combustion_Emission['S_mole'].values
-            + 0.53 * self.Combustion_Emission['N_mole'].values)
-
+                self.Material_Properties[m].values
+                / 100
+                / self.CommonData.MW[key2[m][0]]["amount"]
+                * 1000
+            )
+
+        self.Combustion_Emission["alpha"] = (
+            -0.699 * self.Combustion_Emission["O_mole"].values
+            + 1.5 * self.Combustion_Emission["C_mole"].values
+            + 0.35 * self.Combustion_Emission["H_mole"].values
+            - 0.244 * self.Combustion_Emission["Cl_mole"].values
+            + 1.5 * self.Combustion_Emission["S_mole"].values
+            + 0.53 * self.Combustion_Emission["N_mole"].values
+        )
 
         #'mole/kgDryFlueGas'
-        self.Combustion_Emission['Moles_per_dry_flue_gas'] = (
-            self.Combustion_Emission['O_mole'].values / 2
-            + self.Combustion_Emission['alpha'].values * 4.78
-            - self.Combustion_Emission['H_mole'].values / 4
-            + 5 * self.Combustion_Emission['Cl_mole'].values / 4
-            + self.Combustion_Emission['N_mole'].values / 2)
+        self.Combustion_Emission["Moles_per_dry_flue_gas"] = (
+            self.Combustion_Emission["O_mole"].values / 2
+            + self.Combustion_Emission["alpha"].values * 4.78
+            - self.Combustion_Emission["H_mole"].values / 4
+            + 5 * self.Combustion_Emission["Cl_mole"].values / 4
+            + self.Combustion_Emission["N_mole"].values / 2
+        )
 
         #'dscm FlueGas/kgww'   #Dry Standard Cubic meter
-        self.Combustion_Emission['Flue_gas'] = (
-            self.Combustion_Emission['Moles_per_dry_flue_gas'].values
-            * self.CommonData.STP['Density_Air']['amount'] / 1000
-            * (1 - self.Material_Properties['Moisture Content'].values / 100))
-
-
-        key3 = {'Stack_SO2': ('Sulfur_dioxide', self.CommonData.MW['SO2']['amount']),
-                'Stack_HCl': ('HCl', self.CommonData.MW['HCl']['amount']),
-                'Stack_NOx': ('NOx', self.CommonData.MW['NOx']['amount']),
-                'Stack_CO': ('CO', self.CommonData.MW['CO']['amount']),
-                'Stack_Methane': ('Methane', self.CommonData.MW['CH4']['amount']),
-                'Stack_Nitrous_Oxide': ('Nitrous_Oxide', self.CommonData.MW['Nitrous_Oxide']['amount']),
-                'Stack_Ammonia': ('Ammonia', self.CommonData.MW['Ammonia']['amount']),
-                'Stack_Hydrocarbons': ('Hydrocarbons', self.CommonData.MW['Hydrocarbons']['amount'])}
+        self.Combustion_Emission["Flue_gas"] = (
+            self.Combustion_Emission["Moles_per_dry_flue_gas"].values
+            * self.CommonData.STP["Density_Air"]["amount"]
+            / 1000
+            * (1 - self.Material_Properties["Moisture Content"].values / 100)
+        )
+
+        key3 = {
+            "Stack_SO2": ("Sulfur_dioxide", self.CommonData.MW["SO2"]["amount"]),
+            "Stack_HCl": ("HCl", self.CommonData.MW["HCl"]["amount"]),
+            "Stack_NOx": ("NOx", self.CommonData.MW["NOx"]["amount"]),
+            "Stack_CO": ("CO", self.CommonData.MW["CO"]["amount"]),
+            "Stack_Methane": ("Methane", self.CommonData.MW["CH4"]["amount"]),
+            "Stack_Nitrous_Oxide": ("Nitrous_Oxide", self.CommonData.MW["Nitrous_Oxide"]["amount"]),
+            "Stack_Ammonia": ("Ammonia", self.CommonData.MW["Ammonia"]["amount"]),
+            "Stack_Hydrocarbons": ("Hydrocarbons", self.CommonData.MW["Hydrocarbons"]["amount"]),
+        }
 
         for m in key3.keys():
             #'kg/kg ww'
             self.Combustion_Emission[m] = (
-                self.InputData.Stack_Gas_Conc_Non_metal[key3[m][0]]['amount'] / 10**6
-                * key3[m][1] / 1000
-                / (self.CommonData.STP['Density_Air']['amount'] / 1000)
-                * self.Combustion_Emission['Flue_gas'].values)
+                self.InputData.Stack_Gas_Conc_Non_metal[key3[m][0]]["amount"]
+                / 10**6
+                * key3[m][1]
+                / 1000
+                / (self.CommonData.STP["Density_Air"]["amount"] / 1000)
+                * self.Combustion_Emission["Flue_gas"].values
+            )
 
         #'kg/kg ww'
-        self.Combustion_Emission['Stack_PM'] = (
-            self.InputData.Stack_Gas_Conc_Non_metal['PM']['amount'] / 10**6
-            * self.Combustion_Emission['Flue_gas'].values)
+        self.Combustion_Emission["Stack_PM"] = (
+            self.InputData.Stack_Gas_Conc_Non_metal["PM"]["amount"]
+            / 10**6
+            * self.Combustion_Emission["Flue_gas"].values
+        )
 
         #'kg/kg ww'
-        self.Combustion_Emission['Stack_Dioxins_Furans'] = (
-            self.InputData.Stack_Gas_Conc_Non_metal['Dioxins_Furans']['amount'] / 10**12
-            * self.Combustion_Emission['Flue_gas'].values)
+        self.Combustion_Emission["Stack_Dioxins_Furans"] = (
+            self.InputData.Stack_Gas_Conc_Non_metal["Dioxins_Furans"]["amount"]
+            / 10**12
+            * self.Combustion_Emission["Flue_gas"].values
+        )
 
         ### Post_Combustion Solids
-        self.Post_Combustion_Solids = pd.DataFrame(index = self.Index)
+        self.Post_Combustion_Solids = pd.DataFrame(index=self.Index)
 
         #'kg/kg ww'
-        self.Post_Combustion_Solids['Total_Post_Combustion_Solids'] = (
-            self.Material_Properties['Ash Content'].values / 100)
-
-        self.Post_Combustion_Solids['Unreacted_Ash'] = (
-            (1 - self.Material_Properties['Moisture Content'].values / 100)
-            * self.Material_Properties['Volatile Solids'].values
-            * (1 - self.process_data['Comb_eff'].values / 100))
+        self.Post_Combustion_Solids["Total_Post_Combustion_Solids"] = (
+            self.Material_Properties["Ash Content"].values / 100
+        )
+
+        self.Post_Combustion_Solids["Unreacted_Ash"] = (
+            (1 - self.Material_Properties["Moisture Content"].values / 100)
+            * self.Material_Properties["Volatile Solids"].values
+            * (1 - self.process_data["Comb_eff"].values / 100)
+        )
 
         # 'kg/kg ww'
-        self.Post_Combustion_Solids['Fly_Ash'] = (
-            self.InputData.Metals_Recovery['Fly_ash_frac']['amount']
-            * self.Post_Combustion_Solids['Total_Post_Combustion_Solids'].values)
+        self.Post_Combustion_Solids["Fly_Ash"] = (
+            self.InputData.Metals_Recovery["Fly_ash_frac"]["amount"]
+            * self.Post_Combustion_Solids["Total_Post_Combustion_Solids"].values
+        )
 
         #'kg/kg ww'
-        self.Post_Combustion_Solids['Bottom_Ash_with_Metals'] = (
-            self.Post_Combustion_Solids['Total_Post_Combustion_Solids']
-            - self.Post_Combustion_Solids['Fly_Ash'])
+        self.Post_Combustion_Solids["Bottom_Ash_with_Metals"] = (
+            self.Post_Combustion_Solids["Total_Post_Combustion_Solids"]
+            - self.Post_Combustion_Solids["Fly_Ash"]
+        )
 
         #'kg/kg ww'
-        self.Post_Combustion_Solids['Ferrous_Recovery'] = (
-            self.process_data['Frac_recoverable_Fe'].values
-            * (1 - self.process_data['Fe_frac_oxidized'].values)
-            * self.InputData.Metals_Recovery['Fe_Rec_Rate']['amount'])
+        self.Post_Combustion_Solids["Ferrous_Recovery"] = (
+            self.process_data["Frac_recoverable_Fe"].values
+            * (1 - self.process_data["Fe_frac_oxidized"].values)
+            * self.InputData.Metals_Recovery["Fe_Rec_Rate"]["amount"]
+        )
 
         #'kg/kg ww'
-        self.Post_Combustion_Solids['Aluminum_Recovery'] = (
-            self.process_data['Frac_recoverable_Al'].values
-            * (1 - self.process_data['Al_frac_oxidized'].values)
-            * self.InputData.Metals_Recovery['Al_Rec_Rate']['amount'])
+        self.Post_Combustion_Solids["Aluminum_Recovery"] = (
+            self.process_data["Frac_recoverable_Al"].values
+            * (1 - self.process_data["Al_frac_oxidized"].values)
+            * self.InputData.Metals_Recovery["Al_Rec_Rate"]["amount"]
+        )
 
         #'kg/kg ww'
-        self.Post_Combustion_Solids['Bottom_Ash_without_Metals'] = (
-            self.Post_Combustion_Solids['Bottom_Ash_with_Metals'].values
-            - self.Post_Combustion_Solids['Ferrous_Recovery'].values
-            - self.Post_Combustion_Solids['Aluminum_Recovery'].values)
+        self.Post_Combustion_Solids["Bottom_Ash_without_Metals"] = (
+            self.Post_Combustion_Solids["Bottom_Ash_with_Metals"].values
+            - self.Post_Combustion_Solids["Ferrous_Recovery"].values
+            - self.Post_Combustion_Solids["Aluminum_Recovery"].values
+        )
 
         ### APC_Consumption
         self.APC_Consumption = pd.DataFrame(index=self.Index)
-        for x in ['lime', 'carbon', 'ammonia']:
+        for x in ["lime", "carbon", "ammonia"]:
             #'kg/Mg ww'
-            self.APC_Consumption[x] = self.InputData.Material_Consumption[x]['amount']*1000
+            self.APC_Consumption[x] = self.InputData.Material_Consumption[x]["amount"] * 1000
 
-### Cost Calculation
+        ### Cost Calculation
         self.add_cost()
 
-### Add economic data
+    ### Add economic data
     def add_cost(self):
-        self.Cost=pd.DataFrame(index=self.Index)
-        self.Cost[('biosphere3', 'Capital_Cost')] = -npf.pmt(
-            rate=self.InputData.Economic_parameters['Inerest_rate']['amount'],
-            nper=self.InputData.Economic_parameters['WTE_lifetime']['amount'],
-            pv=self.InputData.Economic_parameters['Capital_cost']['amount'])
-
-        self.Cost[('biosphere3', 'Operational_Cost')] = self.InputData.Economic_parameters['O_M_cost']['amount']
+        self.Cost = pd.DataFrame(index=self.Index)
+        self.Cost[("biosphere3", "Capital_Cost")] = -npf.pmt(
+            rate=self.InputData.Economic_parameters["Interest_rate"]["amount"],
+            nper=self.InputData.Economic_parameters["WTE_lifetime"]["amount"],
+            pv=self.InputData.Economic_parameters["Capital_cost"]["amount"],
+        )
+
+        self.Cost[("biosphere3", "Operational_Cost")] = self.InputData.Economic_parameters[
+            "O_M_cost"
+        ]["amount"]
 
     def setup_MC(self, seed=None):
         self.InputData.setup_MC(seed)
 
     def MC_calc(self):
         input_list = self.InputData.gen_MC()
         self.calc()
@@ -264,82 +317,96 @@
 
         for x in [Waste, Technosphere]:
             for y in self.Index:
                 x[y] = {}
 
         ### Output Waste Database
         for y in self.Index:
-            Waste[y]['Bottom_Ash'] = self.Post_Combustion_Solids['Bottom_Ash_without_Metals'][y]
-
-            Waste[y]['Fly_Ash'] = (
-                self.Post_Combustion_Solids['Fly_Ash'][y]
-                + self.InputData.Material_Consumption['ammonia']['amount']
-                + self.InputData.Material_Consumption['lime']['amount']
-                + self.InputData.Material_Consumption['carbon']['amount'])
-
-            Waste[y]['Unreacted_Ash'] = self.Post_Combustion_Solids['Unreacted_Ash'][y]
-
-            Waste[y]['Al'] = self.Post_Combustion_Solids['Aluminum_Recovery'][y]
-
-            Waste[y]['Fe'] = self.Post_Combustion_Solids['Ferrous_Recovery'][y]
-
-        ### Output Technospphere Database
-            Technosphere[y][('Technosphere', 'Electricity_production')] = self.Energy_Calculations['Net_Electricity_Produced'][y]
-
-            Technosphere[y][('Technosphere', 'Heat_Steam')] = self.Energy_Calculations['Heat_Recovered'][y]
-
-            Technosphere[y][('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck')] = (
-                self.InputData.Material_Consumption['ammonia']['amount']
-                * self.InputData.Material_Consumption['Distance_from_prod_fac']['amount']
-                + self.InputData.Material_Consumption['lime']['amount']
-                * self.InputData.Material_Consumption['Distance_from_prod_fac']['amount']
-                + self.InputData.Material_Consumption['carbon']['amount']
-                * self.InputData.Material_Consumption['Distance_from_prod_fac']['amount'])
-
-            Technosphere[y][('Technosphere', 'Empty_Return_Heavy_Duty_Diesel_Truck')] = (
-                self.InputData.Material_Consumption['Distance_from_prod_fac']['amount']
-                * self.InputData.Material_Consumption['Empty_Return_Truck']['amount']
-                + self.InputData.Material_Consumption['Distance_from_prod_fac']['amount']
-                * self.InputData.Material_Consumption['Empty_Return_Truck']['amount']
-                + self.InputData.Material_Consumption['Distance_from_prod_fac']['amount']
-                * self.InputData.Material_Consumption['Empty_Return_Truck']['amount']) / 23 # 23 is the heavy duty truck payload
-
-            Technosphere[y][('Technosphere', 'lime_hydrated_loose_weight_RoW_lime_production')] = (
-                self.APC_Consumption['lime'][y])
-
-            Technosphere[y][('Technosphere', 'ammonia_liquid_RoW_ammonia_production_steam_reforming_liquid')] = (
-                self.APC_Consumption['ammonia'][y])
+            Waste[y]["Bottom_Ash"] = self.Post_Combustion_Solids["Bottom_Ash_without_Metals"][y]
 
-            Technosphere[y][('Technosphere', 'charcoal_GLO_charcoal_production')] = self.APC_Consumption['carbon'][y]
+            Waste[y]["Fly_Ash"] = (
+                self.Post_Combustion_Solids["Fly_Ash"][y]
+                + self.InputData.Material_Consumption["ammonia"]["amount"]
+                + self.InputData.Material_Consumption["lime"]["amount"]
+                + self.InputData.Material_Consumption["carbon"]["amount"]
+            )
+
+            Waste[y]["Unreacted_Ash"] = self.Post_Combustion_Solids["Unreacted_Ash"][y]
+
+            Waste[y]["Al"] = self.Post_Combustion_Solids["Aluminum_Recovery"][y]
+
+            Waste[y]["Fe"] = self.Post_Combustion_Solids["Ferrous_Recovery"][y]
+
+            ### Output Technosphere Database
+            Technosphere[y][("Technosphere", "Electricity_production")] = self.Energy_Calculations[
+                "Net_Electricity_Produced"
+            ][y]
+
+            Technosphere[y][("Technosphere", "Heat_Steam")] = self.Energy_Calculations[
+                "Heat_Recovered"
+            ][y]
+
+            Technosphere[y][
+                ("Technosphere", "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck")
+            ] = (
+                self.InputData.Material_Consumption["ammonia"]["amount"]
+                * self.InputData.Material_Consumption["Distance_from_prod_fac"]["amount"]
+                + self.InputData.Material_Consumption["lime"]["amount"]
+                * self.InputData.Material_Consumption["Distance_from_prod_fac"]["amount"]
+                + self.InputData.Material_Consumption["carbon"]["amount"]
+                * self.InputData.Material_Consumption["Distance_from_prod_fac"]["amount"]
+            )
+
+            Technosphere[y][("Technosphere", "Empty_Return_Heavy_Duty_Diesel_Truck")] = (
+                self.InputData.Material_Consumption["Distance_from_prod_fac"]["amount"]
+                * self.InputData.Material_Consumption["Empty_Return_Truck"]["amount"]
+                + self.InputData.Material_Consumption["Distance_from_prod_fac"]["amount"]
+                * self.InputData.Material_Consumption["Empty_Return_Truck"]["amount"]
+                + self.InputData.Material_Consumption["Distance_from_prod_fac"]["amount"]
+                * self.InputData.Material_Consumption["Empty_Return_Truck"]["amount"]
+            ) / 23  # 23 is the heavy duty truck payload
+
+            Technosphere[y][
+                ("Technosphere", "lime_hydrated_loose_weight_RoW_lime_production")
+            ] = self.APC_Consumption["lime"][y]
+
+            Technosphere[y][
+                ("Technosphere", "ammonia_liquid_RoW_ammonia_production_steam_reforming_liquid")
+            ] = self.APC_Consumption["ammonia"][y]
+
+            Technosphere[y][
+                ("Technosphere", "charcoal_GLO_charcoal_production")
+            ] = self.APC_Consumption["carbon"][y]
 
         ### Output Biosphere Database
         bio_rename_dict = {
-            'Stack_Ammonia':('biosphere3', '87883a4e-1e3e-4c9d-90c0-f1bea36f8014'),
-            'Sb':('biosphere3', '77927dac-dea3-429d-a434-d5a71d92c4f7'),
-            'As':('biosphere3', 'dc6dbdaa-9f13-43a8-8af5-6603688c6ad0'),
-            'Ba':('biosphere3', '7e246e3a-5cff-43fc-a8e6-02d191424559'),
-            'Cd':('biosphere3', '1c5a7322-9261-4d59-a692-adde6c12de92'),
-            'CO2_fossil':('biosphere3', '349b29d1-3e58-4c66-98b9-9d1a076efd2e'),
-            'CO2_biogenic':('biosphere3', 'eba59fd6-f37e-41dc-9ca3-c7ea22d602c7'),
-            'Stack_CO':('biosphere3', 'ba2f3f82-c93a-47a5-822a-37ec97495275'),
-            'Cr':('biosphere3', 'e142b577-e934-4085-9a07-3983d4d92afb'),
-            'Cu':('biosphere3', 'ec8144d6-d123-43b1-9c17-a295422a0498'),
-            'Stack_Nitrous_Oxide':('biosphere3', '20185046-64bb-4c09-a8e7-e8a9e144ca98'),
-            'Stack_Dioxins_Furans':('biosphere3', '082903e4-45d8-4078-94cb-736b15279277'),
-            'Stack_Hydrocarbons':('biosphere3', 'f9abb851-8731-4c5b-b057-863996a1f94a'),
-            'Stack_HCl':('biosphere3', 'c941d6d0-a56c-4e6c-95de-ac685635218d'),
-            'Pb':('biosphere3', '8e123669-94d3-41d8-9480-a79211fe7c43'),
-            'Hg':('biosphere3', '71234253-b3a7-4dfe-b166-a484ad15bee7'),
-            'Stack_Methane':('biosphere3', 'b53d3744-3629-4219-be20-980865e54031'),
-            'Ni':('biosphere3', 'a5506f4b-113f-4713-95c3-c819dde6e48b'),
-            'Stack_NOx':('biosphere3', 'c1b91234-6f24-417b-8309-46111d09c457'),
-            'Stack_PM':('biosphere3', '21e46cb8-6233-4c99-bac3-c41d2ab99498'),
-            'Se':('biosphere3', '454c61fd-c52b-4a04-9731-f141bb7b5264'),
-            'Stack_SO2':('biosphere3', 'fd7aa71c-508c-480d-81a6-8052aad92646'),
-            'Zn':('biosphere3', '5ce378a0-b48d-471c-977d-79681521efde')}
+            "Stack_Ammonia": ("biosphere3", "87883a4e-1e3e-4c9d-90c0-f1bea36f8014"),
+            "Sb": ("biosphere3", "77927dac-dea3-429d-a434-d5a71d92c4f7"),
+            "As": ("biosphere3", "dc6dbdaa-9f13-43a8-8af5-6603688c6ad0"),
+            "Ba": ("biosphere3", "7e246e3a-5cff-43fc-a8e6-02d191424559"),
+            "Cd": ("biosphere3", "1c5a7322-9261-4d59-a692-adde6c12de92"),
+            "CO2_fossil": ("biosphere3", "349b29d1-3e58-4c66-98b9-9d1a076efd2e"),
+            "CO2_biogenic": ("biosphere3", "eba59fd6-f37e-41dc-9ca3-c7ea22d602c7"),
+            "Stack_CO": ("biosphere3", "ba2f3f82-c93a-47a5-822a-37ec97495275"),
+            "Cr": ("biosphere3", "e142b577-e934-4085-9a07-3983d4d92afb"),
+            "Cu": ("biosphere3", "ec8144d6-d123-43b1-9c17-a295422a0498"),
+            "Stack_Nitrous_Oxide": ("biosphere3", "20185046-64bb-4c09-a8e7-e8a9e144ca98"),
+            "Stack_Dioxins_Furans": ("biosphere3", "082903e4-45d8-4078-94cb-736b15279277"),
+            "Stack_Hydrocarbons": ("biosphere3", "f9abb851-8731-4c5b-b057-863996a1f94a"),
+            "Stack_HCl": ("biosphere3", "c941d6d0-a56c-4e6c-95de-ac685635218d"),
+            "Pb": ("biosphere3", "8e123669-94d3-41d8-9480-a79211fe7c43"),
+            "Hg": ("biosphere3", "71234253-b3a7-4dfe-b166-a484ad15bee7"),
+            "Stack_Methane": ("biosphere3", "b53d3744-3629-4219-be20-980865e54031"),
+            "Ni": ("biosphere3", "a5506f4b-113f-4713-95c3-c819dde6e48b"),
+            "Stack_NOx": ("biosphere3", "c1b91234-6f24-417b-8309-46111d09c457"),
+            "Stack_PM": ("biosphere3", "21e46cb8-6233-4c99-bac3-c41d2ab99498"),
+            "Se": ("biosphere3", "454c61fd-c52b-4a04-9731-f141bb7b5264"),
+            "Stack_SO2": ("biosphere3", "fd7aa71c-508c-480d-81a6-8052aad92646"),
+            "Zn": ("biosphere3", "5ce378a0-b48d-471c-977d-79681521efde"),
+        }
 
         # report function rename the LCI dataframe, so we use the self.LCI_index to rename LCI only one time
         # unless the we call the calc function
         if not self.LCI_index:
             self.Combustion_Emission = self.Combustion_Emission.rename(columns=bio_rename_dict)
             self.LCI_index = True
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels/__init__.py` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 # -*- coding: utf-8 -*-
 """
-@author: Mojtaba Sardarmehni
-
-Life_cycle process models for the swolfpy
+Life_cycle process models for the swolfpy.
 """
-from .ProcessModel import ProcessModel
+from .AD import AD
+from .AnF import AnF
+from .COM_Col import COM_Col
+from .Comp import Comp
 from .Distance import Distance
+from .GC import GC
+from .HC import HC
 from .LF import LF
-from .WTE import WTE
-from .Comp import Comp
-from .AD import AD
-from .SS_MRF import SS_MRF
+from .MF_Col import MF_Col
+from .ProcessModel import ProcessModel
+from .RDF import RDF
 from .Reproc import Reproc
 from .SF_Col import SF_Col
-from .MF_Col import MF_Col
-from .COM_Col import COM_Col
+from .SS_MRF import SS_MRF
 from .TS import TS
-from .HC import HC
-from .GC import GC
-from .RDF import RDF
-from .AnF import AnF
-
+from .WTE import WTE
 
-__all__ = ['ProcessModel',
-           'Distance',
-           'LF',
-           'WTE',
-           'Comp',
-           'AD',
-           'SS_MRF',
-           'Reproc',
-           'SF_Col',
-           'MF_Col',
-           'COM_Col',
-           'TS',
-           'HC',
-           'GC',
-           'RDF',
-           'AnF',
-           ]
+__all__ = [
+    "ProcessModel",
+    "Distance",
+    "LF",
+    "WTE",
+    "Comp",
+    "AD",
+    "SS_MRF",
+    "Reproc",
+    "SF_Col",
+    "MF_Col",
+    "COM_Col",
+    "TS",
+    "HC",
+    "GC",
+    "RDF",
+    "AnF",
+]
 
-__version__ = '0.1.9'
+__version__ = "1.0.0"
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/PKG-INFO` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,201 +1,210 @@
 Metadata-Version: 2.1
 Name: swolfpy-processmodels
-Version: 0.1.9
-Summary: Life-Cylce Process Models for swolfpy (swolfpy_processmodels)
-Home-page: https://github.com/SwolfPy-Project/swolfpy-processmodels
-Author: Mojtaba Sardarmehni
-Author-email: msardar2@ncsu.edu
+Version: 1.0.0
+Summary: Life-Cylce Process Models for swolfpy (swolfpy_processmodels).
+Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
+Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
-Description: .. General
-        
-        ==============================================================
-        Life-Cycle Process Models for SwolfPy (swolfpy_processmodels)
-        ==============================================================
-        
-        .. image:: https://img.shields.io/pypi/v/swolfpy_processmodels.svg
-                :target: https://pypi.python.org/pypi/swolfpy_processmodels
-                
-        .. image:: https://img.shields.io/pypi/pyversions/swolfpy_processmodels.svg
-            :target: https://pypi.org/project/swolfpy_processmodels/
-            :alt: Supported Python Versions
-        
-        .. image:: https://img.shields.io/pypi/l/swolfpy_processmodels.svg
-            :target: https://pypi.org/project/swolfpy_processmodels/
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/dm/swolfpy-processmodels.svg?label=Pypi%20downloads
-            :target: https://pypi.org/project/swolfpy-processmodels/
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/format/swolfpy_processmodels.svg
-            :target: https://pypi.org/project/swolfpy_processmodels/
-            :alt: Format
-        
-        .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
-                :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml/badge.svg?branch=master
-                :target: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml
-                :alt: Test
-        
-        .. image:: https://zenodo.org/badge/395802174.svg
-                :target: https://zenodo.org/badge/latestdoi/395802174
-                :alt: DOI
-        
-        .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
-           :target: https://doi.org/10.1111/jiec.13236
-           :alt: JIE DOI
-        
-        
-        * Free software: GNU GENERAL PUBLIC LICENSE V2
-        * Website: https://swolfpy-project.github.io
-        * Documentation: https://swolfpy.readthedocs.io.
-        * Repository: https://github.com/SwolfPy-Project/swolfpy-processmodels
-        
-        
-        Features
-        --------
-        * Life-cycle process models for solid waste management (SWM) processes.
-        * Built-in Monte Carlo simulation
-        
-        .. list-table:: **Life-cycle process models**
-           :widths: auto
-           :header-rows: 1
-        
-           * - 
-             - Process model 
-             - Description
-           * - 1
-             - Landfill (**LF**)
-             - Calculates emissions, material use, and energy use associated with construction, operations, 
-               closure and post-closure activities, landfill gas and leachate management, and carbon storage.
-           * - 2
-             - Waste-to-Energy (**WTE**)
-             - Calculates emissions, mass flows, and resource use and recovery for the mass burn WTE process.
-           * - 3
-             - Gasification & Syngas Combustion (**GC**)
-             - Calculates emissions, mass flows, and resource use and recovery for the GC process (Produced syngas from
-               gasification is combusted to produce electricity by steam turbine). 
-           * - 4
-             - Composting (**Comp**)
-             - Calculates emissions, mass flows, and resource use and recovery for aerobic composting process and final use of compost.
-           * - 5
-             - Home Composting (**HC**)
-             - Calculates emissions, mass flows, and resource use and recovery for home composting process and final use of compost.
-           * - 6
-             - Anaerobic Digestion (**AD**)
-             - Calculates emissions, mass flows, and resource use and recovery for anaerobic digestion process and final use of compost.
-           * - 7
-             - Single-Stream Material Recovery facility (**SS_MRF**)
-             - Calculates cost, emissions, and energy use associated with material recovery facilities.
-           * - 8
-             - Refuse-Derived Fuel (**RDF**)
-             - Calculates cost, emissions, and energy use associated with RDF production facilities.
-           * - 9
-             - Reprocessing (**Reproc**)
-             - Calculates emissions, mass flows, and resource use and recovery associated with recycling materials.	 
-           * - 10
-             - Transfer Station (**TS**)
-             - Calculates cost, emissions, and energy use associated with Transfer Stations.
-           * - 11
-             - Single Family Collection (**SF_Col**)
-             - Calculates cost, emissions, and fossil fuel use associated with MSW collection from single family sector.
-           * - 12
-             - Multi Family Collection (**MF_Col**)
-             - Calculates cost, emissions, and fossil fuel use associated with MSW collection from multi-family sector.
-           * - 13
-             - Collection (**COM_Col**)
-             - Calculates cost, emissions, and fossil fuel use associated with MSW collection from commercial sector.
-           * - 14
-             - Animal Feed (**AnF**)
-             - Calculates cost, emissions, and energy use associated with conversion of food waste to animal feed and final use of produced feed.
-          
-        .. Installation
-        
-        Installation
-        ------------
-        1- Download and install miniconda from:  https://docs.conda.io/en/latest/miniconda.html
-        
-        2- Update conda in a terminal window or anaconda prompt::
-        
-                conda update conda
-        
-        3- Create a new environment for swolfpy::
-        
-                conda create --name swolfpy python=3.7
-        
-        4- Activate the environment::
-        
-                conda activate swolfpy
-        
-        5- Install swolfpy_processmodels in the environment::
-        
-                pip install swolfpy_processmodels
-        
-        6- Use in python (e.g., Landfill model)::
-        
-                import swolfpy_processmodels as sppm 
-                model = sppm.LF()
-                model.calc()
-                LCI_report = model.report()
-                LCI_report
-        
-        .. endInstallation
-        
-        
-        =======
-        History
-        =======
-        
-        0.1.9 (2022-04-06)
-        ------------------
-        * Add Multi-family and commercial Waste collection
-        * Add Animal feed production
-        * Refactor SF-collection model
-        
-        
-        0.1.8 (2021-11-25)
-        ------------------
-        
-        * Update Landfill model.
-        
-        
-        0.1.6 (2021-10-02)
-        ------------------
-        
-        * Add Home Composting (HC)
-        * Add Gasification & Syngas combustion (GC)
-        * Add Refuse-derived fuel (RDF)
-        
-        
-        0.1.4 (2021-05-10)
-        ------------------
-        
-        * New Life-cyle model: TS
-        * Add Cost calculations
-        
-        
-        
-        0.1.0 (2020-05-06)
-        ------------------
-        
-        * First release on PyPI. Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
-        
-Keywords: swolfpy_processmodels
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://swolfpy-project.github.io/
+Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-processmodels
+Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE.md
+License-File: AUTHORS.rst
+
+.. General
+
+==============================================================
+Life-Cycle Process Models for SwolfPy (swolfpy_processmodels)
+==============================================================
+
+.. image:: https://img.shields.io/pypi/v/swolfpy_processmodels.svg
+        :target: https://pypi.python.org/pypi/swolfpy_processmodels
+
+.. image:: https://img.shields.io/pypi/pyversions/swolfpy_processmodels.svg
+    :target: https://pypi.org/project/swolfpy_processmodels/
+    :alt: Supported Python Versions
+
+.. image:: https://img.shields.io/pypi/l/swolfpy_processmodels.svg
+    :target: https://pypi.org/project/swolfpy_processmodels/
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/swolfpy-processmodels.svg?label=Pypi%20downloads
+    :target: https://pypi.org/project/swolfpy-processmodels/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/format/swolfpy_processmodels.svg
+    :target: https://pypi.org/project/swolfpy_processmodels/
+    :alt: Format
+
+.. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
+        :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml/badge.svg?branch=master
+        :target: https://github.com/SwolfPy-Project/swolfpy-processmodels/actions/workflows/python-app.yml
+        :alt: Test
+
+.. image:: https://zenodo.org/badge/395802174.svg
+        :target: https://zenodo.org/badge/latestdoi/395802174
+        :alt: DOI
+
+.. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
+   :target: https://doi.org/10.1111/jiec.13236
+   :alt: JIE DOI
+
+
+* Free software: GNU GENERAL PUBLIC LICENSE V2
+* Website: https://swolfpy-project.github.io
+* Documentation: https://swolfpy.readthedocs.io.
+* Repository: https://github.com/SwolfPy-Project/swolfpy-processmodels
+
+
+Features
+--------
+* Life-cycle process models for solid waste management (SWM) processes.
+* Built-in Monte Carlo simulation
+
+.. list-table:: **Life-cycle process models**
+   :widths: auto
+   :header-rows: 1
+
+   * -
+     - Process model
+     - Description
+   * - 1
+     - Landfill (**LF**)
+     - Calculates emissions, material use, and energy use associated with construction, operations,
+       closure and post-closure activities, landfill gas and leachate management, and carbon storage.
+   * - 2
+     - Waste-to-Energy (**WTE**)
+     - Calculates emissions, mass flows, and resource use and recovery for the mass burn WTE process.
+   * - 3
+     - Gasification & Syngas Combustion (**GC**)
+     - Calculates emissions, mass flows, and resource use and recovery for the GC process (Produced syngas from
+       gasification is combusted to produce electricity by steam turbine).
+   * - 4
+     - Composting (**Comp**)
+     - Calculates emissions, mass flows, and resource use and recovery for aerobic composting process and final use of compost.
+   * - 5
+     - Home Composting (**HC**)
+     - Calculates emissions, mass flows, and resource use and recovery for home composting process and final use of compost.
+   * - 6
+     - Anaerobic Digestion (**AD**)
+     - Calculates emissions, mass flows, and resource use and recovery for anaerobic digestion process and final use of compost.
+   * - 7
+     - Single-Stream Material Recovery facility (**SS_MRF**)
+     - Calculates cost, emissions, and energy use associated with material recovery facilities.
+   * - 8
+     - Refuse-Derived Fuel (**RDF**)
+     - Calculates cost, emissions, and energy use associated with RDF production facilities.
+   * - 9
+     - Reprocessing (**Reproc**)
+     - Calculates emissions, mass flows, and resource use and recovery associated with recycling materials.
+   * - 10
+     - Transfer Station (**TS**)
+     - Calculates cost, emissions, and energy use associated with Transfer Stations.
+   * - 11
+     - Single Family Collection (**SF_Col**)
+     - Calculates cost, emissions, and fossil fuel use associated with MSW collection from single family sector.
+   * - 12
+     - Multi Family Collection (**MF_Col**)
+     - Calculates cost, emissions, and fossil fuel use associated with MSW collection from multi-family sector.
+   * - 13
+     - Commercial Collection (**COM_Col**)
+     - Calculates cost, emissions, and fossil fuel use associated with MSW collection from commercial sector.
+   * - 14
+     - Animal Feed (**AnF**)
+     - Calculates cost, emissions, and energy use associated with conversion of food waste to animal feed and final use of produced feed.
+
+.. Installation
+
+Installation
+------------
+1- Download and install miniconda from:  https://docs.conda.io/en/latest/miniconda.html
+
+2- Update conda in a terminal window or anaconda prompt::
+
+        conda update conda
+
+3- Create a new environment for swolfpy::
+
+        conda create --name swolfpy python=3.10
+
+4- Activate the environment::
+
+        conda activate swolfpy
+
+5- Install swolfpy_processmodels in the environment::
+
+        pip install swolfpy_processmodels
+
+6- Use in python (e.g., Landfill model)::
+
+        import swolfpy_processmodels as sppm
+        model = sppm.LF()
+        model.calc()
+        LCI_report = model.report()
+        LCI_report
+
+.. endInstallation
+
+=======
+History
+=======
+
+1.0.0 (2023-06-03)
+------------------
+
+* Upgrade to Python 3.10
+* Add PreCommit
+
+
+0.1.9 (2022-04-06)
+------------------
+
+* Add Multi-family and commercial Waste collection
+* Add Animal feed production
+* Refactor SF-collection model
+
+
+0.1.8 (2021-11-25)
+------------------
+
+* Update Landfill model.
+
+
+0.1.6 (2021-10-02)
+------------------
+
+* Add Home Composting (HC)
+* Add Gasification & Syngas combustion (GC)
+* Add Refuse-derived fuel (RDF)
+
+
+0.1.4 (2021-05-10)
+------------------
+
+* New Life-cycle model: TS
+* Add Cost calculations
+
+
+
+0.1.0 (2020-05-06)
+------------------
+
+* First release on PyPI. Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
```

### Comparing `swolfpy_processmodels-0.1.9/swolfpy_processmodels.egg-info/SOURCES.txt` & `swolfpy_processmodels-1.0.0/swolfpy_processmodels.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE.md
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
+requirements.txt
 swolfpy_processmodels/AD.py
 swolfpy_processmodels/AD_subprocess.py
 swolfpy_processmodels/AnF.py
 swolfpy_processmodels/COM_Col.py
 swolfpy_processmodels/Common_subprocess.py
 swolfpy_processmodels/Comp.py
 swolfpy_processmodels/Comp_subprocess.py
@@ -28,12 +29,11 @@
 swolfpy_processmodels/TS.py
 swolfpy_processmodels/TS_subprocess.py
 swolfpy_processmodels/WTE.py
 swolfpy_processmodels/__init__.py
 swolfpy_processmodels.egg-info/PKG-INFO
 swolfpy_processmodels.egg-info/SOURCES.txt
 swolfpy_processmodels.egg-info/dependency_links.txt
-swolfpy_processmodels.egg-info/not-zip-safe
 swolfpy_processmodels.egg-info/requires.txt
 swolfpy_processmodels.egg-info/top_level.txt
 tests/__init__.py
 tests/test_processmodels.py
```

### Comparing `swolfpy_processmodels-0.1.9/tests/test_processmodels.py` & `swolfpy_processmodels-1.0.0/tests/test_processmodels.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,158 @@
 # -*- coding: utf-8 -*-
 """
-Created on Sat May  9 17:43:11 2020
-
-@author: Mojtaba Sardarmehni
-
-Tests for `swolfpy_processmodels` package
+Tests for `swolfpy_processmodels` package.
 """
-import swolfpy_processmodels as sp
-from swolfpy_inputdata import CommonData
 import numpy as np
+from swolfpy_inputdata import CommonData
+
+import swolfpy_processmodels as sp
 
 
 def LCA_model_helper(model):
     commondata = CommonData()
     Index = set(commondata.Index)
     Reprocessing_Index = set(commondata.Reprocessing_Index)
 
     model.calc()
     report = model.report()
 
     assert isinstance(report, dict)
-    assert 'process name' in report.keys()
+    assert "process name" in report.keys()
 
-    assert 'Waste' in report.keys()
-    assert 'Technosphere' in report.keys()
-    assert 'Biosphere' in report.keys()
-
-    if model.Process_Type == 'Reprocessing':
-        assert Reprocessing_Index.issubset(report['Waste'])
-        assert len(Reprocessing_Index) == len(report['Waste'])
+    assert "Waste" in report.keys()
+    assert "Technosphere" in report.keys()
+    assert "Biosphere" in report.keys()
+
+    if model.Process_Type == "Reprocessing":
+        assert Reprocessing_Index.issubset(report["Waste"])
+        assert len(Reprocessing_Index) == len(report["Waste"])
         for x in Reprocessing_Index:
-            for y in report['Waste'][x]:
-                assert not np.isnan(report['Waste'][x][y])
+            for y in report["Waste"][x]:
+                assert not np.isnan(report["Waste"][x][y])
 
-        assert Reprocessing_Index.issubset(report['Technosphere'])
-        assert len(Reprocessing_Index) == len(report['Technosphere'])
+        assert Reprocessing_Index.issubset(report["Technosphere"])
+        assert len(Reprocessing_Index) == len(report["Technosphere"])
         for x in Reprocessing_Index:
-            for y in report['Technosphere'][x]:
-                assert not np.isnan(report['Technosphere'][x][y])
+            for y in report["Technosphere"][x]:
+                assert not np.isnan(report["Technosphere"][x][y])
 
-        assert Reprocessing_Index.issubset(report['Biosphere'])
-        assert len(Reprocessing_Index) == len(report['Biosphere'])
+        assert Reprocessing_Index.issubset(report["Biosphere"])
+        assert len(Reprocessing_Index) == len(report["Biosphere"])
         for x in Reprocessing_Index:
-            for y in report['Biosphere'][x]:
-                assert not np.isnan(report['Biosphere'][x][y])
+            for y in report["Biosphere"][x]:
+                assert not np.isnan(report["Biosphere"][x][y])
 
-    elif model.Process_Type == 'Treatment' or model.Process_Type == 'Collection':
-        assert Index.issubset(report['Waste'])
-        assert len(Index) == len(report['Waste'])
+    elif model.Process_Type in ["Treatment", "Collection"]:
+        assert Index.issubset(report["Waste"])
+        assert len(Index) == len(report["Waste"])
         for x in Index:
-            for y in report['Waste'][x]:
-                assert not np.isnan(report['Waste'][x][y])
+            for y in report["Waste"][x]:
+                assert not np.isnan(report["Waste"][x][y])
 
-        assert Index.issubset(report['Technosphere'])
-        assert len(Index) == len(report['Technosphere'])
+        assert Index.issubset(report["Technosphere"])
+        assert len(Index) == len(report["Technosphere"])
         for x in Index:
-            for y in report['Technosphere'][x]:
-                assert not np.isnan(report['Technosphere'][x][y])
+            for y in report["Technosphere"][x]:
+                assert not np.isnan(report["Technosphere"][x][y])
 
-        assert Index.issubset(report['Biosphere'])
-        assert len(Index) == len(report['Biosphere'])
+        assert Index.issubset(report["Biosphere"])
+        assert len(Index) == len(report["Biosphere"])
         for x in Index:
-            for y in report['Biosphere'][x]:
-                assert not np.isnan(report['Biosphere'][x][y])
+            for y in report["Biosphere"][x]:
+                assert not np.isnan(report["Biosphere"][x][y])
 
     model.setup_MC()
     model.MC_calc()
     report = model.report()
     report1 = model.report()
     assert report == report1
 
 
 def test_LF():
-    assert sp.LF.Process_Type == 'Treatment'
+    assert sp.LF.Process_Type == "Treatment"
     LCA_model_helper(sp.LF())
 
 
 def test_WTE():
-    assert sp.WTE.Process_Type == 'Treatment'
+    assert sp.WTE.Process_Type == "Treatment"
     LCA_model_helper(sp.WTE())
 
 
 def test_Composting():
-    assert sp.Comp.Process_Type == 'Treatment'
+    assert sp.Comp.Process_Type == "Treatment"
     LCA_model_helper(sp.Comp())
 
 
 def test_AD():
-    assert sp.AD.Process_Type == 'Treatment'
+    assert sp.AD.Process_Type == "Treatment"
     LCA_model_helper(sp.AD())
 
 
 def test_SS_MRF():
-    assert sp.SS_MRF.Process_Type == 'Treatment'
+    assert sp.SS_MRF.Process_Type == "Treatment"
     LCA_model_helper(sp.SS_MRF())
 
 
 def test_HC():
-    assert sp.HC.Process_Type == 'Treatment'
+    assert sp.HC.Process_Type == "Treatment"
     LCA_model_helper(sp.HC())
 
 
 def test_AnF():
-    assert sp.AnF.Process_Type == 'Treatment'
+    assert sp.AnF.Process_Type == "Treatment"
     LCA_model_helper(sp.AnF())
 
 
 def test_Reproc():
-    assert sp.Reproc.Process_Type == 'Reprocessing'
+    assert sp.Reproc.Process_Type == "Reprocessing"
     LCA_model_helper(sp.Reproc())
 
 
 def test_TS():
-    assert sp.TS.Process_Type == 'Transfer_Station'
+    assert sp.TS.Process_Type == "Transfer_Station"
     LCA_model_helper(sp.TS())
 
 
 def test_GC():
-    assert sp.GC.Process_Type == 'RDF'
+    assert sp.GC.Process_Type == "RDF"
     LCA_model_helper(sp.GC())
 
 
 def test_RDF():
-    assert sp.RDF.Process_Type == 'Treatment'
+    assert sp.RDF.Process_Type == "Treatment"
     LCA_model_helper(sp.RDF())
 
 
 def test_SF_Col():
-    assert sp.SF_Col.Process_Type == 'Collection'
+    assert sp.SF_Col.Process_Type == "Collection"
     col_scheme = sp.SF_Col.scheme()
-    col_scheme[('RWC', 'SSYW', 'SSR')] = 1
-    LCA_model_helper(sp.SF_Col('SF_test', Collection_scheme=col_scheme))
+    col_scheme[("RWC", "SSYW", "SSR")] = 1
+    LCA_model_helper(sp.SF_Col("SF_test", Collection_scheme=col_scheme))
 
 
 def test_MF_Col():
-    assert sp.MF_Col.Process_Type == 'Collection'
+    assert sp.MF_Col.Process_Type == "Collection"
     col_scheme = sp.MF_Col.scheme()
-    col_scheme[('RWC', 'SSYW', 'SSR')] = 1
-    LCA_model_helper(sp.MF_Col('MF_test', Collection_scheme=col_scheme))
+    col_scheme[("RWC", "SSYW", "SSR")] = 1
+    LCA_model_helper(sp.MF_Col("MF_test", Collection_scheme=col_scheme))
 
 
 def test_COM_Col():
-    assert sp.COM_Col.Process_Type == 'Collection'
+    assert sp.COM_Col.Process_Type == "Collection"
     col_scheme = sp.COM_Col.scheme()
-    col_scheme[('RWC', 'SSYW', 'SSR')] = 1
-    LCA_model_helper(sp.COM_Col('COM_test', Collection_scheme=col_scheme))
+    col_scheme[("RWC", "SSYW", "SSR")] = 1
+    LCA_model_helper(sp.COM_Col("COM_test", Collection_scheme=col_scheme))
 
 
 def test_Distance():
-    dist_data = sp.Distance.create_distance_table(['P1', 'P2', 'P3'], ['Heavy Duty Truck'])
-    dist_data['Heavy Duty Truck']['P1']['P2'] = 20
-    dist_data['Heavy Duty Truck']['P3']['P1'] = 30
-    dist_data['Heavy Duty Truck']['P3']['P2'] = 20
+    dist_data = sp.Distance.create_distance_table(["P1", "P2", "P3"], ["Heavy Duty Truck"])
+    dist_data["Heavy Duty Truck"]["P1"]["P2"] = 20
+    dist_data["Heavy Duty Truck"]["P3"]["P1"] = 30
+    dist_data["Heavy Duty Truck"]["P3"]["P2"] = 20
     dist = sp.Distance(dist_data)
-    assert dist.Distance[('P1', 'P2')]['Heavy Duty Truck'] == 20
-    assert dist.Distance[('P3', 'P1')]['Heavy Duty Truck'] == 30
-    assert dist.Distance[('P2', 'P3')]['Heavy Duty Truck'] == dist.Distance[('P3', 'P2')]['Heavy Duty Truck']
+    assert dist.Distance[("P1", "P2")]["Heavy Duty Truck"] == 20
+    assert dist.Distance[("P3", "P1")]["Heavy Duty Truck"] == 30
+    assert (
+        dist.Distance[("P2", "P3")]["Heavy Duty Truck"]
+        == dist.Distance[("P3", "P2")]["Heavy Duty Truck"]
+    )
```

