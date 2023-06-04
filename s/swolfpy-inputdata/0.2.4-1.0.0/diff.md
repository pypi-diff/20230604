# Comparing `tmp/swolfpy_inputdata-0.2.4.tar.gz` & `tmp/swolfpy_inputdata-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\swolfpy_inputdata-0.2.4.tar", last modified: Wed Apr  6 03:29:30 2022, max compression
+gzip compressed data, was "swolfpy_inputdata-1.0.0.tar", last modified: Sun Jun  4 17:38:05 2023, max compression
```

## Comparing `swolfpy_inputdata-0.2.4.tar` & `swolfpy_inputdata-1.0.0.tar`

### file list

```diff
@@ -1,48 +1,93 @@
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:30.000000 swolfpy_inputdata-0.2.4/
--rw-rw-rw-   0        0        0      749 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     1629 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      650 2022-04-06 03:25:46.000000 swolfpy_inputdata-0.2.4/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2021-10-02 16:34:47.000000 swolfpy_inputdata-0.2.4/LICENSE.md
--rw-rw-rw-   0        0        0      273 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7687 2022-04-06 03:29:30.000000 swolfpy_inputdata-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4571 2022-04-06 03:25:46.000000 swolfpy_inputdata-0.2.4/README.rst
--rw-rw-rw-   0        0        0       42 2022-04-06 03:29:30.000000 swolfpy_inputdata-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2216 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:29.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/
--rw-rw-rw-   0        0        0      969 2021-10-02 16:52:49.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/AD_Input.py
--rw-rw-rw-   0        0        0      983 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/AnF_Input.py
--rw-rw-rw-   0        0        0      988 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/COM_Col_Input.py
--rw-rw-rw-   0        0        0     3175 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/CommonData.py
--rw-rw-rw-   0        0        0      985 2021-10-02 16:54:39.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Comp_Input.py
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:29.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Data/
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:29.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Data/LCIA_Methods/
--rw-rw-rw-   0        0        0        0 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Data/LCIA_Methods/__init__.py
--rw-rw-rw-   0        0        0        0 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:29.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Ecospold2/
--rw-rw-rw-   0        0        0       90 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Ecospold2/__init__.py
--rw-rw-rw-   0        0        0      969 2021-10-02 16:56:40.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/GC_Input.py
--rw-rw-rw-   0        0        0      984 2021-10-02 16:57:33.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/HC_Input.py
--rw-rw-rw-   0        0        0     4056 2021-08-30 21:04:49.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/InputData.py
--rw-rw-rw-   0        0        0     1637 2021-11-25 12:17:29.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/LF_Input.py
--rw-rw-rw-   0        0        0     6982 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/MC.py
--rw-rw-rw-   0        0        0      984 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/MF_Col_Input.py
--rw-rw-rw-   0        0        0      981 2021-10-02 22:31:34.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/RDF_Input.py
--rw-rw-rw-   0        0        0      586 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Reproc_Input.py
--rw-rw-rw-   0        0        0      984 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/SF_Col_Input.py
--rw-rw-rw-   0        0        0      987 2021-10-02 16:59:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/SS_MRF_Input.py
--rw-rw-rw-   0        0        0      665 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/TS_Input.py
--rw-rw-rw-   0        0        0     1439 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/Technosphere_Input.py
--rw-rw-rw-   0        0        0      973 2021-10-02 17:00:56.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/WTE_Input.py
--rw-rw-rw-   0        0        0     1148 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:29.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/
--rw-rw-rw-   0        0        0     7687 2022-04-06 03:29:27.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1137 2022-04-06 03:29:27.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-06 03:29:27.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-04-06 03:29:27.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       81 2022-04-06 03:29:27.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-04-06 03:29:27.000000 swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-06 03:29:30.000000 swolfpy_inputdata-0.2.4/tests/
--rw-rw-rw-   0        0        0      373 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/tests/Test_Input.csv
--rw-rw-rw-   0        0        0       50 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1786 2021-08-24 20:23:56.000000 swolfpy_inputdata-0.2.4/tests/test_inputdata.py
--rw-rw-rw-   0        0        0      690 2022-02-03 21:42:05.000000 swolfpy_inputdata-0.2.4/tests/test_inputs.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.599866 swolfpy_inputdata-1.0.0/
+-rw-rw-rw-   0        0        0      748 2023-06-04 17:34:09.000000 swolfpy_inputdata-1.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1629 2022-11-26 02:47:46.000000 swolfpy_inputdata-1.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      739 2023-06-04 17:34:09.000000 swolfpy_inputdata-1.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    18431 2022-11-25 05:19:43.000000 swolfpy_inputdata-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0      319 2023-06-04 17:34:09.000000 swolfpy_inputdata-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6878 2023-06-04 17:38:05.597895 swolfpy_inputdata-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4773 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/README.rst
+-rw-rw-rw-   0        0        0    10351 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      109 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:38:05.599866 swolfpy_inputdata-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 17:38:04.698908 swolfpy_inputdata-1.0.0/swolfpy_inputdata/
+-rw-rw-rw-   0        0        0      845 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/AD_Input.py
+-rw-rw-rw-   0        0        0      896 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/AnF_Input.py
+-rw-rw-rw-   0        0        0      904 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/COM_Col_Input.py
+-rw-rw-rw-   0        0        0     3393 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/CommonData.py
+-rw-rw-rw-   0        0        0      898 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/Comp_Input.py
+-rw-rw-rw-   0        0        0      845 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/GC_Input.py
+-rw-rw-rw-   0        0        0      897 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/HC_Input.py
+-rw-rw-rw-   0        0        0     4142 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/InputData.py
+-rw-rw-rw-   0        0        0     1505 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/LF_Input.py
+-rw-rw-rw-   0        0        0     4213 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/MC.py
+-rw-rw-rw-   0        0        0      900 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/MF_Col_Input.py
+-rw-rw-rw-   0        0        0      851 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/RDF_Input.py
+-rw-rw-rw-   0        0        0      537 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/Reproc_Input.py
+-rw-rw-rw-   0        0        0      900 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/SF_Col_Input.py
+-rw-rw-rw-   0        0        0      900 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/SS_MRF_Input.py
+-rw-rw-rw-   0        0        0      574 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/TS_Input.py
+-rw-rw-rw-   0        0        0     1400 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/Technosphere_Input.py
+-rw-rw-rw-   0        0        0      849 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/WTE_Input.py
+-rw-rw-rw-   0        0        0     1147 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.322090 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/
+-rw-rw-rw-   0        0        0    13013 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AD_Input.csv
+-rw-rw-rw-   0        0        0     4069 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AD_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    13078 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AnF_Input.csv
+-rw-rw-rw-   0        0        0     1313 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/AnF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    11442 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/COM_Col_Input.csv
+-rw-rw-rw-   0        0        0     2734 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/COM_Col_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     5998 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/CommonData.csv
+-rw-rw-rw-   0        0        0    10725 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Comp_Input.csv
+-rw-rw-rw-   0        0        0     4136 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Comp_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0       75 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Distance.csv
+-rw-rw-rw-   0        0        0     3040 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/GC_Input.csv
+-rw-rw-rw-   0        0        0     1023 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/GC_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     1679 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/HC_Input.csv
+-rw-rw-rw-   0        0        0     1739 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/HC_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0      505 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_GasColPlan.csv
+-rw-rw-rw-   0        0        0     8510 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Gas_emission_factors.csv
+-rw-rw-rw-   0        0        0    10918 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Input.csv
+-rw-rw-rw-   0        0        0     1239 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     5508 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/LF_Leachate_Quality.csv
+-rw-rw-rw-   0        0        0    11011 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/MF_Col_Input.csv
+-rw-rw-rw-   0        0        0     2614 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/MF_Col_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    10890 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Material properties.csv
+-rw-rw-rw-   0        0        0    18551 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/RDF_Input.csv
+-rw-rw-rw-   0        0        0     1635 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/RDF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     3343 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/References.csv
+-rw-rw-rw-   0        0        0    53452 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Reprocessing_Input.csv
+-rw-rw-rw-   0        0        0    10939 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SF_Col_Input.csv
+-rw-rw-rw-   0        0        0     2821 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SF_Col_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0    48925 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SS_MRF_Input.csv
+-rw-rw-rw-   0        0        0     3824 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/SS_MRF_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0     3206 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/TS_Input.csv
+-rw-rw-rw-   0        0        0   781594 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Technosphere_LCI.csv
+-rw-rw-rw-   0        0        0     2126 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/Technosphere_References.csv
+-rw-rw-rw-   0        0        0     5618 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/WTE_Input.csv
+-rw-rw-rw-   0        0        0     2092 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/WTE_Input_MaterialDependent.csv
+-rw-rw-rw-   0        0        0   230942 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/keys.csv
+drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.550862 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/
+-rw-rw-rw-   0        0        0    13531 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('CML (v4.4) SwolfPy', 'resources', 'depletion of abiotic resources - elements, ultimate reserves').csv
+-rw-rw-rw-   0        0        0    30907 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
+-rw-rw-rw-   0        0        0    30899 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2007, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
+-rw-rw-rw-   0        0        0    32831 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0').csv
+-rw-rw-rw-   0        0        0    32831 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=0, C1_36').csv
+-rw-rw-rw-   0        0        0    32828 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1').csv
+-rw-rw-rw-   0        0        0    32828 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('IPCC 2013, Ecoinvent V3.5', 'climate change', 'GWP 100a, bioCO2=1, C1_36').csv
+-rw-rw-rw-   0        0        0      101 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Capital_Cost', 'SwolfPy').csv
+-rw-rw-rw-   0        0        0      472 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Operational_Cost', 'SwolfPy').csv
+-rw-rw-rw-   0        0        0      541 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('SwolfPy_Total_Cost', 'SwolfPy').csv
+-rw-rw-rw-   0        0        0     5933 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'acidification').csv
+-rw-rw-rw-   0        0        0     4899 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'eutrophication').csv
+-rw-rw-rw-   0        0        0    16120 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata/data/lcia_methods/('TRACI (2.1) SwolfPy', 'environmental impact', 'photochemical smog').csv
+drwxrwxrwx   0        0        0        0 2023-06-04 17:38:04.734859 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/
+-rw-rw-rw-   0        0        0     6878 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-04 17:38:04.000000 swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 17:38:05.594875 swolfpy_inputdata-1.0.0/tests/
+-rw-rw-rw-   0        0        0      373 2022-11-26 05:55:39.000000 swolfpy_inputdata-1.0.0/tests/Test_Input.csv
+-rw-rw-rw-   0        0        0       50 2022-11-25 05:49:34.000000 swolfpy_inputdata-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     1811 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/tests/test_inputdata.py
+-rw-rw-rw-   0        0        0      600 2023-06-04 17:34:10.000000 swolfpy_inputdata-1.0.0/tests/test_inputs.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swolfpy_inputdata-0.2.4/AUTHORS.rst` & `swolfpy_inputdata-1.0.0/AUTHORS.rst`

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

### Comparing `swolfpy_inputdata-0.2.4/CONTRIBUTING.rst` & `swolfpy_inputdata-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-0.2.4/HISTORY.rst` & `swolfpy_inputdata-1.0.0/HISTORY.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,40 @@
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
 0.2.4 (2022-04-05)
 ------------------
+
 * Add Multi-family and commercial Waste collection
 * Add Animal feed production (AnF)
 
 
 0.2.3 (2021-11-24)
 ------------------
 
 * Update Landfill
 
 
 0.2.1 (2021-10-02)
 ------------------
 
-* New models: Gasification & Syngas combustion (GC), Refuse-Derived Fuel (RDF), Home composting (HC) 
+* New models: Gasification & Syngas combustion (GC), Refuse-Derived Fuel (RDF), Home composting (HC)
 
 
 0.1.9 (2021-05-10)
 ------------------
 
-* Life cycle cost, input data for TS, References 
+* Life cycle cost, input data for TS, References
 
 
 0.1.0 (2020-05-06)
 ------------------
 
 * First release on PyPI. Data for the Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
```

### Comparing `swolfpy_inputdata-0.2.4/LICENSE.md` & `swolfpy_inputdata-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swolfpy_inputdata-0.2.4/PKG-INFO` & `swolfpy_inputdata-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,192 +1,207 @@
 Metadata-Version: 2.1
 Name: swolfpy_inputdata
-Version: 0.2.4
-Summary: Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
-Home-page: https://github.com/SwolfPy-Project/swolfpy-inputdata
-Author: Mojtaba Sardarmehni
-Author-email: msardar2@ncsu.edu
+Version: 1.0.0
+Summary: Input data for swolfpy's life-cycle process models (swolfpy_inputdata).
+Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
+Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
-Description: .. General
-        
-        ======================================================================
-        Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
-        ======================================================================
-        
-        .. image:: https://img.shields.io/pypi/v/swolfpy_inputdata.svg
-                :target: https://pypi.python.org/pypi/swolfpy_inputdata
-                
-        .. image:: https://img.shields.io/pypi/pyversions/swolfpy_inputdata.svg
-            :target: https://pypi.org/project/swolfpy_inputdata/
-            :alt: Supported Python Versions
-        
-        .. image:: https://img.shields.io/pypi/l/swolfpy_inputdata.svg
-            :target: https://pypi.org/project/swolfpy_inputdata/
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/dm/swolfpy-inputdata.svg?label=Pypi%20downloads
-            :target: https://pypi.org/project/swolfpy-inputdata/
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/format/swolfpy_inputdata.svg
-            :target: https://pypi.org/project/swolfpy_inputdata/
-            :alt: Format
-        
-        .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
-                :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml/badge.svg?branch=master
-                :target: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml
-                :alt: Test
-        
-        .. image:: https://zenodo.org/badge/395800995.svg
-                :target: https://zenodo.org/badge/latestdoi/395800995
-                :alt: DOI
-            
-        .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
-           :target: https://doi.org/10.1111/jiec.13236
-           :alt: JIE DOI
-        
-        * Free software: GNU GENERAL PUBLIC LICENSE V2
-        * Website: https://swolfpy-project.github.io
-        * Documentation: https://swolfpy.readthedocs.io.
-        * Repository: https://github.com/SwolfPy-Project/swolfpy-inputdata
-        
-        
-        
-        Features
-        --------
-        * Input data for Life-cycle process models of swolfpy
-        
-          * Common data (e.g., molecular weights, heating values) 
-          * Material properties (46 common waste fractions; e.g., Food waste, Yard waste)
-          
-            * Chemical properties (e.g., carbon content, methane yield)
-            * Physical properties (e.g., moisture content, density) 
-          * Material dependent process model inputs (e.g., separation efficiency for each waste fraction in the trommel) 
-          * Material indepent process model inputs
-          
-        * Built-in Monte Carlo simulation
-        
-        
-        .. list-table:: **Description of columns in the csv file for input data**
-           :widths: auto
-           :header-rows: 1
-        
-           * - Field 
-             - Description
-           * - Category
-             - Category of the input (e.g., energy recovery, post closure)
-           * - Dictonary_Name
-             - Name of the dictionary and attribute (whitespace is not allowed)
-           * - Parameter Name
-             - Short name of the parameter (whitespace is not allowed)
-           * - Parameter Description
-             - Longer description of the parameter
-           * - Amount
-             - Default value for the parameter
-           * - Unit
-             - Unit of the parameter (e.g., MJ/Mg, kW, hours/day)
-           * - Uncertainty_type
-             - 0: Undefined, 2: Lognormal, 3: normal, 4: Uniform, 5: Triangular, 7: Discrete Uniform
-           * - Loc
-             - Mean for lognormal and normal distribution
-           * - scale
-             - Standard deviation for lognormal and normal distribution
-           * - shape
-             - Shape parameter for Weibull, Gamma or Beta distributions     
-           * - Minimum
-             - Lower bound/minimum for lognormal, normal, uniform, triangular, and discrete uniform distributions
-           * - maximum
-             - Upper bound/maximum for lognormal, normal, uniform, triangular, and discrete uniform distributions
-           * - Reference
-             - 
-           * - Comment
-             -
-             
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
-        5- Install swolfpy_inputdata in the environment::
-        
-                pip install swolfpy_inputdata
-        
-        6- Use in python (e.g., Landfill model)::
-        
-                import swolfpy_inputdata as spid 
-                data = spid.LF_Input()
-                model.calc()
-                #Example: Returs the actk parameter in landfill
-                data.LF_gas['actk']
-                #Example: Returns input data in dataframe format
-                data.Data
-        
-        .. endInstallation
-        
-        
-        =======
-        History
-        =======
-        
-        0.2.4 (2022-04-05)
-        ------------------
-        * Add Multi-family and commercial Waste collection
-        * Add Animal feed production (AnF)
-        
-        
-        0.2.3 (2021-11-24)
-        ------------------
-        
-        * Update Landfill
-        
-        
-        0.2.1 (2021-10-02)
-        ------------------
-        
-        * New models: Gasification & Syngas combustion (GC), Refuse-Derived Fuel (RDF), Home composting (HC) 
-        
-        
-        0.1.9 (2021-05-10)
-        ------------------
-        
-        * Life cycle cost, input data for TS, References 
-        
-        
-        0.1.0 (2020-05-06)
-        ------------------
-        
-        * First release on PyPI. Data for the Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
-        
-Keywords: swolfpy_inputdata
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://swolfpy-project.github.io/
+Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-inputdata
+Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
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
+======================================================================
+Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
+======================================================================
+
+.. image:: https://img.shields.io/pypi/v/swolfpy_inputdata.svg
+        :target: https://pypi.python.org/pypi/swolfpy_inputdata
+
+.. image:: https://img.shields.io/pypi/pyversions/swolfpy_inputdata.svg
+    :target: https://pypi.org/project/swolfpy_inputdata/
+    :alt: Supported Python Versions
+
+.. image:: https://img.shields.io/pypi/l/swolfpy_inputdata.svg
+    :target: https://pypi.org/project/swolfpy_inputdata/
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/swolfpy-inputdata.svg?label=Pypi%20downloads
+    :target: https://pypi.org/project/swolfpy-inputdata/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/format/swolfpy_inputdata.svg
+    :target: https://pypi.org/project/swolfpy_inputdata/
+    :alt: Format
+
+.. image:: https://img.shields.io/badge/linting-pylint-yellowgreen
+    :target: https://github.com/PyCQA/pylint
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+
+.. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
+        :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml/badge.svg?branch=master
+        :target: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml
+        :alt: Test
+
+.. image:: https://zenodo.org/badge/395800995.svg
+        :target: https://zenodo.org/badge/latestdoi/395800995
+        :alt: DOI
+
+.. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
+   :target: https://doi.org/10.1111/jiec.13236
+   :alt: JIE DOI
+
+* Free software: GNU GENERAL PUBLIC LICENSE V2
+* Website: https://swolfpy-project.github.io
+* Documentation: https://swolfpy.readthedocs.io.
+* Repository: https://github.com/SwolfPy-Project/swolfpy-inputdata
+
+
+
+Features
+--------
+* Input data for Life-cycle process models of swolfpy
+
+  * Common data (e.g., molecular weights, heating values)
+  * Material properties (46 common waste fractions; e.g., Food waste, Yard waste)
+
+    * Chemical properties (e.g., carbon content, methane yield)
+    * Physical properties (e.g., moisture content, density)
+  * Material dependent process model inputs (e.g., separation efficiency for each waste fraction in the trommel)
+  * Material indepent process model inputs
+
+* Built-in Monte Carlo simulation
+
+
+.. list-table:: **Description of columns in the csv file for input data**
+   :widths: auto
+   :header-rows: 1
+
+   * - Field
+     - Description
+   * - Category
+     - Category of the input (e.g., energy recovery, post closure)
+   * - Dictonary_Name
+     - Name of the dictionary and attribute (whitespace is not allowed)
+   * - Parameter Name
+     - Short name of the parameter (whitespace is not allowed)
+   * - Parameter Description
+     - Longer description of the parameter
+   * - Amount
+     - Default value for the parameter
+   * - Unit
+     - Unit of the parameter (e.g., MJ/Mg, kW, hours/day)
+   * - Uncertainty_type
+     - 0: Undefined, 2: Lognormal, 3: normal, 4: Uniform, 5: Triangular, 7: Discrete Uniform
+   * - Loc
+     - Mean for lognormal and normal distribution
+   * - scale
+     - Standard deviation for lognormal and normal distribution
+   * - shape
+     - Shape parameter for Weibull, Gamma or Beta distributions
+   * - Minimum
+     - Lower bound/minimum for lognormal, normal, uniform, triangular, and discrete uniform distributions
+   * - maximum
+     - Upper bound/maximum for lognormal, normal, uniform, triangular, and discrete uniform distributions
+   * - Reference
+     -
+   * - Comment
+     -
+
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
+5- Install swolfpy_inputdata in the environment::
+
+        pip install swolfpy_inputdata
+
+6- Use in python (e.g., Landfill model)::
+
+        import swolfpy_inputdata as spid
+        data = spid.LF_Input()
+        model.calc()
+        #Example: Returs the actk parameter in landfill
+        data.LF_gas['actk']
+        #Example: Returns input data in dataframe format
+        data.Data
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
+0.2.4 (2022-04-05)
+------------------
+
+* Add Multi-family and commercial Waste collection
+* Add Animal feed production (AnF)
+
+
+0.2.3 (2021-11-24)
+------------------
+
+* Update Landfill
+
+
+0.2.1 (2021-10-02)
+------------------
+
+* New models: Gasification & Syngas combustion (GC), Refuse-Derived Fuel (RDF), Home composting (HC)
+
+
+0.1.9 (2021-05-10)
+------------------
+
+* Life cycle cost, input data for TS, References
+
+
+0.1.0 (2020-05-06)
+------------------
+
+* First release on PyPI. Data for the Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
```

### Comparing `swolfpy_inputdata-0.2.4/README.rst` & `swolfpy_inputdata-1.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ======================================================================
 Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
 ======================================================================
 
 .. image:: https://img.shields.io/pypi/v/swolfpy_inputdata.svg
         :target: https://pypi.python.org/pypi/swolfpy_inputdata
-        
+
 .. image:: https://img.shields.io/pypi/pyversions/swolfpy_inputdata.svg
     :target: https://pypi.org/project/swolfpy_inputdata/
     :alt: Supported Python Versions
 
 .. image:: https://img.shields.io/pypi/l/swolfpy_inputdata.svg
     :target: https://pypi.org/project/swolfpy_inputdata/
     :alt: License
@@ -19,26 +19,32 @@
     :target: https://pypi.org/project/swolfpy-inputdata/
     :alt: Downloads
 
 .. image:: https://img.shields.io/pypi/format/swolfpy_inputdata.svg
     :target: https://pypi.org/project/swolfpy_inputdata/
     :alt: Format
 
+.. image:: https://img.shields.io/badge/linting-pylint-yellowgreen
+    :target: https://github.com/PyCQA/pylint
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+
 .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
         :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml/badge.svg?branch=master
         :target: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml
         :alt: Test
 
 .. image:: https://zenodo.org/badge/395800995.svg
         :target: https://zenodo.org/badge/latestdoi/395800995
         :alt: DOI
-    
+
 .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
    :target: https://doi.org/10.1111/jiec.13236
    :alt: JIE DOI
 
 * Free software: GNU GENERAL PUBLIC LICENSE V2
 * Website: https://swolfpy-project.github.io
 * Documentation: https://swolfpy.readthedocs.io.
@@ -46,30 +52,30 @@
 
 
 
 Features
 --------
 * Input data for Life-cycle process models of swolfpy
 
-  * Common data (e.g., molecular weights, heating values) 
+  * Common data (e.g., molecular weights, heating values)
   * Material properties (46 common waste fractions; e.g., Food waste, Yard waste)
-  
+
     * Chemical properties (e.g., carbon content, methane yield)
-    * Physical properties (e.g., moisture content, density) 
-  * Material dependent process model inputs (e.g., separation efficiency for each waste fraction in the trommel) 
+    * Physical properties (e.g., moisture content, density)
+  * Material dependent process model inputs (e.g., separation efficiency for each waste fraction in the trommel)
   * Material indepent process model inputs
-  
+
 * Built-in Monte Carlo simulation
 
 
 .. list-table:: **Description of columns in the csv file for input data**
    :widths: auto
    :header-rows: 1
 
-   * - Field 
+   * - Field
      - Description
    * - Category
      - Category of the input (e.g., energy recovery, post closure)
    * - Dictonary_Name
      - Name of the dictionary and attribute (whitespace is not allowed)
    * - Parameter Name
      - Short name of the parameter (whitespace is not allowed)
@@ -82,50 +88,50 @@
    * - Uncertainty_type
      - 0: Undefined, 2: Lognormal, 3: normal, 4: Uniform, 5: Triangular, 7: Discrete Uniform
    * - Loc
      - Mean for lognormal and normal distribution
    * - scale
      - Standard deviation for lognormal and normal distribution
    * - shape
-     - Shape parameter for Weibull, Gamma or Beta distributions     
+     - Shape parameter for Weibull, Gamma or Beta distributions
    * - Minimum
      - Lower bound/minimum for lognormal, normal, uniform, triangular, and discrete uniform distributions
    * - maximum
      - Upper bound/maximum for lognormal, normal, uniform, triangular, and discrete uniform distributions
    * - Reference
-     - 
+     -
    * - Comment
      -
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
 
 5- Install swolfpy_inputdata in the environment::
 
         pip install swolfpy_inputdata
 
 6- Use in python (e.g., Landfill model)::
 
-        import swolfpy_inputdata as spid 
+        import swolfpy_inputdata as spid
         data = spid.LF_Input()
         model.calc()
         #Example: Returs the actk parameter in landfill
         data.LF_gas['actk']
         #Example: Returns input data in dataframe format
         data.Data
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/AD_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/SS_MRF_Input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Nov 22 11:16:05 2019
+from pathlib import Path
 
-@author: msardar2
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
-class AD_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='AD', CommonDataObjct=None):
+class SS_MRF_Input(InputData):
+    def __init__(
+        self,
+        input_data_path=None,
+        process_data_path=None,
+        process_name="SS_MRF",
+        CommonDataObjct=None,
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/AD_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/SS_MRF_Input.csv"
+
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/AD_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/SS_MRF_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/AnF_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/HC_Input.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Thu Jan  6 12:42:59 2022
+from pathlib import Path
 
-@author: msardar2
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
-class AnF_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='Animal Feed', CommonDataObjct=None):
+class HC_Input(InputData):
+    def __init__(
+        self,
+        input_data_path=None,
+        process_data_path=None,
+        process_name="Home Composting",
+        CommonDataObjct=None,
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/AnF_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/HC_Input.csv"
 
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/AnF_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/HC_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/COM_Col_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/MF_Col_Input.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Oct 21 22:52:32 2019
+from pathlib import Path
 
-@author: msmsa
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
-class COM_Col_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='COM_Col', CommonDataObjct=None):
+class MF_Col_Input(InputData):
+    def __init__(
+        self,
+        input_data_path=None,
+        process_data_path=None,
+        process_name="MF_Col",
+        CommonDataObjct=None,
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/COM_Col_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/MF_Col_Input.csv"
 
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/COM_Col_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/MF_Col_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/Comp_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/SF_Col_Input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Nov 22 11:56:34 2019
+from pathlib import Path
 
-@author: msardar2
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
-class Comp_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='Composting', CommonDataObjct=None):
+class SF_Col_Input(InputData):
+    def __init__(
+        self,
+        input_data_path=None,
+        process_data_path=None,
+        process_name="SF_Col",
+        CommonDataObjct=None,
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/Comp_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/SF_Col_Input.csv"
 
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/Comp_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/SF_Col_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/InputData.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/InputData.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,110 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Apr 21 20:45:14 2020
+import ast
 
-@author: msmsa
-"""
 import pandas as pd
+
 from .MC import MC
-import ast
 
 
 class InputData(MC):
     """
-    ``InputData`` class reads the input data from the csv file and load them as class attributes. This class is inherited from the ``MC`` class.
+    ``InputData`` class reads the input data from the csv file and load them as class
+    attributes. This class is inherited from the ``MC`` class.
 
     Main functionalities include:
-    loading data, updating data and generating random number for data based on the defined probabiliy distributions.
+    loading data, updating data and generating random number for data based on the defined probability distributions.
 
     :param input_data_path: absolute path to the input data file
     :type input_data_path: str
-    :param eval_parameter: If the parameters are tuple instead of str, it will evalute their real value.
+    :param eval_parameter: If the parameters are tuple instead of str, it will evaluate their real value.
     :type eval_parameter: bool, optional
-
     """
+
     def __init__(self, input_data_path, process_name, eval_parameter=False):
-        """Initialize ``InputData`` class
+        """
+        Initialize ``InputData`` class.
         """
         self.input_data_path = input_data_path
         self.process_name = process_name
-        self.Data = pd.read_csv(self.input_data_path, dtype={'amount': float, 'uncertainty_type': float, 'loc': float,
-                                                             'scale': float, 'shape': float, 'minimum': float, 'maximum': float})
+        self.Data = pd.read_csv(
+            self.input_data_path,
+            dtype={
+                "amount": float,
+                "uncertainty_type": float,
+                "loc": float,
+                "scale": float,
+                "shape": float,
+                "minimum": float,
+                "maximum": float,
+            },
+        )
 
         if eval_parameter:
-            self.Data['Parameter Name'] = self.Data['Parameter Name'].apply(ast.literal_eval)
+            self.Data["Parameter Name"] = self.Data["Parameter Name"].apply(ast.literal_eval)
 
         # Setting uncertainty type to 0 : Undefined ; when it is not defined
-        self.Data['uncertainty_type'].fillna(0, inplace=True)
+        self.Data["uncertainty_type"].fillna(0, inplace=True)
         # self.Data=self.Data.where((pd.notnull(self.Data)), None)
         self.Input_dict = {}
         self.keys = self.Data.columns[3:]
         for i in range(len(self.Data)):
             if self.Data.Category[i] not in self.Input_dict.keys():
                 exec("self.%s = {}" % self.Data.Dictonary_Name[i])
-                exec("self.Input_dict[self.Data.Category[i]] = self.%s" % self.Data.Dictonary_Name[i])
-                exec("self.%s[self.Data['Parameter Name'][i]] = dict(zip(self.keys,self.Data.loc[i,'Parameter Description':]))" %
-                     self.Data.Dictonary_Name[i])
+                exec(
+                    "self.Input_dict[self.Data.Category[i]] = self.%s" % self.Data.Dictonary_Name[i]
+                )
+                exec(
+                    "self.%s[self.Data['Parameter Name'][i]] = dict(zip(self.keys,self.Data.loc[i,'Parameter Description':]))"
+                    % self.Data.Dictonary_Name[i]
+                )
             else:
-                exec("self.%s[self.Data['Parameter Name'][i]] = dict(zip(self.keys,self.Data.loc[i,'Parameter Description':]))" %
-                     self.Data.Dictonary_Name[i])
+                exec(
+                    "self.%s[self.Data['Parameter Name'][i]] = dict(zip(self.keys,self.Data.loc[i,'Parameter Description':]))"
+                    % self.Data.Dictonary_Name[i]
+                )
 
-### Add process data
+    ### Add process data
     def add_process_data(self, process_data_path, index):
-        self.process_data = pd.read_csv(process_data_path,
-                                        index_col=0,
-                                        header=0,
-                                        skiprows=[1, 2, 3]).loc[index].astype(float)
+        self.process_data = (
+            pd.read_csv(process_data_path, index_col=0, header=0, skiprows=[1, 2, 3])
+            .loc[index]
+            .astype(float)
+        )
         self.process_data.fillna(0, inplace=True)
-        self.process_data_info = pd.read_csv(process_data_path,
-                                             index_col=0,
-                                             header=0,
-                                             nrows=3)
+        self.process_data_info = pd.read_csv(process_data_path, index_col=0, header=0, nrows=3)
 
-### Update_Input
+    ### Update_Input
     def Update_input(self, NewData):
-        """ Get a new DataFrame and update the ``data`` in ``InputData`` class.
+        """
+        Get a new DataFrame and update the ``data`` in ``InputData`` class.
 
         :param NewData:
         :type NewData: 'pandas.DataFrame'
         """
         for i in NewData.index:
-            exec("self.%s[NewData['Parameter Name'][i]] = dict(zip(self.keys,NewData.loc[i,'Parameter Description':]))" % NewData.Dictonary_Name[i])
+            exec(
+                "self.%s[NewData['Parameter Name'][i]] = dict(zip(self.keys,NewData.loc[i,'Parameter Description':]))"
+                % NewData.Dictonary_Name[i]
+            )
             self.Data.loc[i] = NewData.loc[i]
 
-### Monte_carlo
+    ### Monte_carlo
     def setup_MC(self, seed=None):
-        """ Initialize the parent class (``MC``) and create ``MCRandomNumberGenerator`` based on the data for uncertainty distributions via
-        calling ``MC.setupMC()`` method.
+        """
+        Initialize the parent class (``MC``) and create ``MCRandomNumberGenerator`` based
+        on the data for uncertainty distributions via calling ``MC.setupMC()`` method.
 
         :param seed: seed for random number generation
         :type seed: int, optional
 
         .. seealso:: Class_MC_
         """
         super().__init__(self.Input_dict, self.process_name)
         super().setup_MC(seed)
 
-### Reset static Values
+    ### Reset static Values
     def reset_static_vals(self):
         for i in self.Data.index:
-            exec("self.%s[self.Data['Parameter Name'][i]]['amount'] = self.Data.loc[i,'amount']" % self.Data.Dictonary_Name[i])
+            exec(
+                "self.%s[self.Data['Parameter Name'][i]]['amount'] = self.Data.loc[i,'amount']"
+                % self.Data.Dictonary_Name[i]
+            )
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/MF_Col_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/Reproc_Input.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,15 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Oct 21 22:52:32 2019
+from pathlib import Path
 
-@author: msmsa
-"""
 from .InputData import InputData
-from .CommonData import CommonData
-from pathlib import Path
 
 
-class MF_Col_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='MF_Col', CommonDataObjct=None):
+class Reproc_Input(InputData):
+    # pylint: disable=unused-argument
+    def __init__(self, input_data_path=None, process_name="Reproc", CommonDataObjct=None):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/MF_Col_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/Reprocessing_Input.csv"
 
         # Initialize the superclass
-        super().__init__(self.input_data_path, process_name)
-
-        if not CommonDataObjct:
-            CommonDataObjct = CommonData()
-
-        if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/MF_Col_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+        super().__init__(self.input_data_path, process_name, eval_parameter=True)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/RDF_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/RDF_Input.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Sep 20 14:37:35 2021
+from pathlib import Path
 
-@author: mojtaba sardar
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
 class RDF_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='RDF', CommonDataObjct=None):
+    def __init__(
+        self, input_data_path=None, process_data_path=None, process_name="RDF", CommonDataObjct=None
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/RDF_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/RDF_Input.csv"
 
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/RDF_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/RDF_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/SS_MRF_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/AnF_Input.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Jan  7 11:11:58 2020
+from pathlib import Path
 
-@author: msardar2
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
-class SS_MRF_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='SS_MRF', CommonDataObjct=None):
+class AnF_Input(InputData):
+    def __init__(
+        self,
+        input_data_path=None,
+        process_data_path=None,
+        process_name="Animal Feed",
+        CommonDataObjct=None,
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/SS_MRF_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/AnF_Input.csv"
 
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/SS_MRF_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/AnF_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/TS_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/TS_Input.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Jan  7 11:11:58 2020
+from pathlib import Path
 
-@author: msardar2
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
 class TS_Input(InputData):
-    def __init__(self, input_data_path=None, process_name='TS', CommonDataObjct=None):
+    def __init__(self, input_data_path=None, process_name="TS", CommonDataObjct=None):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/TS_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/TS_Input.csv"
 
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/Technosphere_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/Technosphere_Input.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Fri Nov 22 11:16:05 2019
-
-@author: msardar2
-"""
 from pathlib import Path
+
 import pandas as pd
 
 
-class Technosphere_Input():
+class Technosphere_Input:
     def __init__(self, LCI_path=None, LCI_Reference_path=None, Ecospold2_Path=None):
-
         # Checking the path for technosphere LCI data and writing the technophere database
         if LCI_path:
             self.technosphere_path = LCI_path
         else:
-            self.technosphere_path = Path(__file__).parent / 'Data/Technosphere_LCI.csv'
+            self.technosphere_path = Path(__file__).parent / "data/Technosphere_LCI.csv"
 
         # Checking the path for technosphere LCI references
         if LCI_Reference_path:
             self.LCI_Reference_path = LCI_Reference_path
         else:
-            self.LCI_Reference_path = Path(__file__).parent / 'Data/Technosphere_References.csv'
+            self.LCI_Reference_path = Path(__file__).parent / "data/Technosphere_References.csv"
 
         # Checking the path for Ecospold2
         if Ecospold2_Path:
             self.Ecospold2_Path = Ecospold2_Path
         else:
-            self.Ecospold2_Path = Path(__file__).parent / 'Data/Ecospold2'
+            self.Ecospold2_Path = Path(__file__).parent / "data/Ecospold2"
 
         # Read the data
         self.LCI_swolfpy_data = pd.read_csv(self.technosphere_path)
-        self.LCI_reference = pd.read_csv(self.LCI_Reference_path, index_col='swolfpy_technosphere_name')
-
-        if self.LCI_reference['Reference_activity_id'].count() > 0 and self.Ecospold2_Path is None:
-            raise ValueError('User should select the path to ecospold files, because of keys in Technosphere_References.csv')
+        self.LCI_reference = pd.read_csv(
+            self.LCI_Reference_path, index_col="swolfpy_technosphere_name"
+        )
+
+        if self.LCI_reference["Reference_activity_id"].count() > 0 and self.Ecospold2_Path is None:
+            raise ValueError(
+                "User should select the path to ecospold files, because of keys in Technosphere_References.csv"
+            )
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/WTE_Input.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/COM_Col_Input.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Wed Mar 27 12:25:05 2019
+from pathlib import Path
 
-@author: msardar2
-"""
-from .InputData import InputData
 from .CommonData import CommonData
-from pathlib import Path
+from .InputData import InputData
 
 
-class WTE_Input(InputData):
-    def __init__(self, input_data_path=None, process_data_path=None,
-                 process_name='WTE', CommonDataObjct=None):
+class COM_Col_Input(InputData):
+    def __init__(
+        self,
+        input_data_path=None,
+        process_data_path=None,
+        process_name="COM_Col",
+        CommonDataObjct=None,
+    ):
         if input_data_path:
             self.input_data_path = input_data_path
         else:
-            self.input_data_path = Path(__file__).parent / 'Data/WTE_Input.csv'
+            self.input_data_path = Path(__file__).parent / "data/COM_Col_Input.csv"
+
         # Initialize the superclass
         super().__init__(self.input_data_path, process_name)
 
         if not CommonDataObjct:
             CommonDataObjct = CommonData()
 
         if process_data_path is None:
-            process_data_path = Path(__file__).parent / "Data/WTE_Input_MaterialDependent.csv"
-        self.add_process_data(process_data_path=process_data_path,
-                              index=CommonDataObjct.Index)
+            process_data_path = Path(__file__).parent / "data/COM_Col_Input_MaterialDependent.csv"
+        self.add_process_data(process_data_path=process_data_path, index=CommonDataObjct.Index)
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata/__init__.py` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 # -*- coding: utf-8 -*-
 """
 @author: Mojtaba Sardarmehni
 
 Input data for the swolfpy's life_cycle process models
 """
-from .MC import MC
-from .InputData import InputData
+from .AD_Input import AD_Input
+from .AnF_Input import AnF_Input
+from .COM_Col_Input import COM_Col_Input
 from .CommonData import CommonData
-from .Technosphere_Input import Technosphere_Input
-from .LF_Input import LF_Input
-from .WTE_Input import WTE_Input
 from .Comp_Input import Comp_Input
-from .AD_Input import AD_Input
-from .SS_MRF_Input import SS_MRF_Input
+from .GC_Input import GC_Input
+from .HC_Input import HC_Input
+from .InputData import InputData
+from .LF_Input import LF_Input
+from .MC import MC
+from .MF_Col_Input import MF_Col_Input
+from .RDF_Input import RDF_Input
 from .Reproc_Input import Reproc_Input
 from .SF_Col_Input import SF_Col_Input
-from .MF_Col_Input import MF_Col_Input
-from .COM_Col_Input import COM_Col_Input
+from .SS_MRF_Input import SS_MRF_Input
+from .Technosphere_Input import Technosphere_Input
 from .TS_Input import TS_Input
-from .HC_Input import HC_Input
-from .GC_Input import GC_Input
-from .RDF_Input import RDF_Input
-from .AnF_Input import AnF_Input
-
+from .WTE_Input import WTE_Input
 
 __all__ = [
-    'MC',
-    'InputData',
-    'CommonData',
-    'Technosphere_Input',
-    'LF_Input',
-    'WTE_Input',
-    'Comp_Input',
-    'AD_Input',
-    'SS_MRF_Input',
-    'Reproc_Input',
-    'SF_Col_Input',
-    'MF_Col_Input',
-    'COM_Col_Input',
-    'TS_Input',
-    'HC_Input',
-    'GC_Input',
-    'RDF_Input',
-    'AnF_Input'
+    "MC",
+    "InputData",
+    "CommonData",
+    "Technosphere_Input",
+    "LF_Input",
+    "WTE_Input",
+    "Comp_Input",
+    "AD_Input",
+    "SS_MRF_Input",
+    "Reproc_Input",
+    "SF_Col_Input",
+    "MF_Col_Input",
+    "COM_Col_Input",
+    "TS_Input",
+    "HC_Input",
+    "GC_Input",
+    "RDF_Input",
+    "AnF_Input",
 ]
 
-__version__ = '0.2.4'
+__version__ = "1.0.0"
```

### Comparing `swolfpy_inputdata-0.2.4/swolfpy_inputdata.egg-info/PKG-INFO` & `swolfpy_inputdata-1.0.0/swolfpy_inputdata.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,192 +1,207 @@
 Metadata-Version: 2.1
 Name: swolfpy-inputdata
-Version: 0.2.4
-Summary: Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
-Home-page: https://github.com/SwolfPy-Project/swolfpy-inputdata
-Author: Mojtaba Sardarmehni
-Author-email: msardar2@ncsu.edu
+Version: 1.0.0
+Summary: Input data for swolfpy's life-cycle process models (swolfpy_inputdata).
+Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
+Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
-Description: .. General
-        
-        ======================================================================
-        Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
-        ======================================================================
-        
-        .. image:: https://img.shields.io/pypi/v/swolfpy_inputdata.svg
-                :target: https://pypi.python.org/pypi/swolfpy_inputdata
-                
-        .. image:: https://img.shields.io/pypi/pyversions/swolfpy_inputdata.svg
-            :target: https://pypi.org/project/swolfpy_inputdata/
-            :alt: Supported Python Versions
-        
-        .. image:: https://img.shields.io/pypi/l/swolfpy_inputdata.svg
-            :target: https://pypi.org/project/swolfpy_inputdata/
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/dm/swolfpy-inputdata.svg?label=Pypi%20downloads
-            :target: https://pypi.org/project/swolfpy-inputdata/
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/format/swolfpy_inputdata.svg
-            :target: https://pypi.org/project/swolfpy_inputdata/
-            :alt: Format
-        
-        .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
-                :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml/badge.svg?branch=master
-                :target: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml
-                :alt: Test
-        
-        .. image:: https://zenodo.org/badge/395800995.svg
-                :target: https://zenodo.org/badge/latestdoi/395800995
-                :alt: DOI
-            
-        .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
-           :target: https://doi.org/10.1111/jiec.13236
-           :alt: JIE DOI
-        
-        * Free software: GNU GENERAL PUBLIC LICENSE V2
-        * Website: https://swolfpy-project.github.io
-        * Documentation: https://swolfpy.readthedocs.io.
-        * Repository: https://github.com/SwolfPy-Project/swolfpy-inputdata
-        
-        
-        
-        Features
-        --------
-        * Input data for Life-cycle process models of swolfpy
-        
-          * Common data (e.g., molecular weights, heating values) 
-          * Material properties (46 common waste fractions; e.g., Food waste, Yard waste)
-          
-            * Chemical properties (e.g., carbon content, methane yield)
-            * Physical properties (e.g., moisture content, density) 
-          * Material dependent process model inputs (e.g., separation efficiency for each waste fraction in the trommel) 
-          * Material indepent process model inputs
-          
-        * Built-in Monte Carlo simulation
-        
-        
-        .. list-table:: **Description of columns in the csv file for input data**
-           :widths: auto
-           :header-rows: 1
-        
-           * - Field 
-             - Description
-           * - Category
-             - Category of the input (e.g., energy recovery, post closure)
-           * - Dictonary_Name
-             - Name of the dictionary and attribute (whitespace is not allowed)
-           * - Parameter Name
-             - Short name of the parameter (whitespace is not allowed)
-           * - Parameter Description
-             - Longer description of the parameter
-           * - Amount
-             - Default value for the parameter
-           * - Unit
-             - Unit of the parameter (e.g., MJ/Mg, kW, hours/day)
-           * - Uncertainty_type
-             - 0: Undefined, 2: Lognormal, 3: normal, 4: Uniform, 5: Triangular, 7: Discrete Uniform
-           * - Loc
-             - Mean for lognormal and normal distribution
-           * - scale
-             - Standard deviation for lognormal and normal distribution
-           * - shape
-             - Shape parameter for Weibull, Gamma or Beta distributions     
-           * - Minimum
-             - Lower bound/minimum for lognormal, normal, uniform, triangular, and discrete uniform distributions
-           * - maximum
-             - Upper bound/maximum for lognormal, normal, uniform, triangular, and discrete uniform distributions
-           * - Reference
-             - 
-           * - Comment
-             -
-             
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
-        5- Install swolfpy_inputdata in the environment::
-        
-                pip install swolfpy_inputdata
-        
-        6- Use in python (e.g., Landfill model)::
-        
-                import swolfpy_inputdata as spid 
-                data = spid.LF_Input()
-                model.calc()
-                #Example: Returs the actk parameter in landfill
-                data.LF_gas['actk']
-                #Example: Returns input data in dataframe format
-                data.Data
-        
-        .. endInstallation
-        
-        
-        =======
-        History
-        =======
-        
-        0.2.4 (2022-04-05)
-        ------------------
-        * Add Multi-family and commercial Waste collection
-        * Add Animal feed production (AnF)
-        
-        
-        0.2.3 (2021-11-24)
-        ------------------
-        
-        * Update Landfill
-        
-        
-        0.2.1 (2021-10-02)
-        ------------------
-        
-        * New models: Gasification & Syngas combustion (GC), Refuse-Derived Fuel (RDF), Home composting (HC) 
-        
-        
-        0.1.9 (2021-05-10)
-        ------------------
-        
-        * Life cycle cost, input data for TS, References 
-        
-        
-        0.1.0 (2020-05-06)
-        ------------------
-        
-        * First release on PyPI. Data for the Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
-        
-Keywords: swolfpy_inputdata
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://swolfpy-project.github.io/
+Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy-inputdata
+Keywords: LCA,solid_waste,waste_management,swolfpy,brightway2
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
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
+======================================================================
+Input data for swolfpy's life-cycle process models (swolfpy_inputdata)
+======================================================================
+
+.. image:: https://img.shields.io/pypi/v/swolfpy_inputdata.svg
+        :target: https://pypi.python.org/pypi/swolfpy_inputdata
+
+.. image:: https://img.shields.io/pypi/pyversions/swolfpy_inputdata.svg
+    :target: https://pypi.org/project/swolfpy_inputdata/
+    :alt: Supported Python Versions
+
+.. image:: https://img.shields.io/pypi/l/swolfpy_inputdata.svg
+    :target: https://pypi.org/project/swolfpy_inputdata/
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/swolfpy-inputdata.svg?label=Pypi%20downloads
+    :target: https://pypi.org/project/swolfpy-inputdata/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/format/swolfpy_inputdata.svg
+    :target: https://pypi.org/project/swolfpy_inputdata/
+    :alt: Format
+
+.. image:: https://img.shields.io/badge/linting-pylint-yellowgreen
+    :target: https://github.com/PyCQA/pylint
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/ambv/black
+
+.. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
+        :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml/badge.svg?branch=master
+        :target: https://github.com/SwolfPy-Project/swolfpy-inputdata/actions/workflows/python-app.yml
+        :alt: Test
+
+.. image:: https://zenodo.org/badge/395800995.svg
+        :target: https://zenodo.org/badge/latestdoi/395800995
+        :alt: DOI
+
+.. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
+   :target: https://doi.org/10.1111/jiec.13236
+   :alt: JIE DOI
+
+* Free software: GNU GENERAL PUBLIC LICENSE V2
+* Website: https://swolfpy-project.github.io
+* Documentation: https://swolfpy.readthedocs.io.
+* Repository: https://github.com/SwolfPy-Project/swolfpy-inputdata
+
+
+
+Features
+--------
+* Input data for Life-cycle process models of swolfpy
+
+  * Common data (e.g., molecular weights, heating values)
+  * Material properties (46 common waste fractions; e.g., Food waste, Yard waste)
+
+    * Chemical properties (e.g., carbon content, methane yield)
+    * Physical properties (e.g., moisture content, density)
+  * Material dependent process model inputs (e.g., separation efficiency for each waste fraction in the trommel)
+  * Material indepent process model inputs
+
+* Built-in Monte Carlo simulation
+
+
+.. list-table:: **Description of columns in the csv file for input data**
+   :widths: auto
+   :header-rows: 1
+
+   * - Field
+     - Description
+   * - Category
+     - Category of the input (e.g., energy recovery, post closure)
+   * - Dictonary_Name
+     - Name of the dictionary and attribute (whitespace is not allowed)
+   * - Parameter Name
+     - Short name of the parameter (whitespace is not allowed)
+   * - Parameter Description
+     - Longer description of the parameter
+   * - Amount
+     - Default value for the parameter
+   * - Unit
+     - Unit of the parameter (e.g., MJ/Mg, kW, hours/day)
+   * - Uncertainty_type
+     - 0: Undefined, 2: Lognormal, 3: normal, 4: Uniform, 5: Triangular, 7: Discrete Uniform
+   * - Loc
+     - Mean for lognormal and normal distribution
+   * - scale
+     - Standard deviation for lognormal and normal distribution
+   * - shape
+     - Shape parameter for Weibull, Gamma or Beta distributions
+   * - Minimum
+     - Lower bound/minimum for lognormal, normal, uniform, triangular, and discrete uniform distributions
+   * - maximum
+     - Upper bound/maximum for lognormal, normal, uniform, triangular, and discrete uniform distributions
+   * - Reference
+     -
+   * - Comment
+     -
+
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
+5- Install swolfpy_inputdata in the environment::
+
+        pip install swolfpy_inputdata
+
+6- Use in python (e.g., Landfill model)::
+
+        import swolfpy_inputdata as spid
+        data = spid.LF_Input()
+        model.calc()
+        #Example: Returs the actk parameter in landfill
+        data.LF_gas['actk']
+        #Example: Returns input data in dataframe format
+        data.Data
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
+0.2.4 (2022-04-05)
+------------------
+
+* Add Multi-family and commercial Waste collection
+* Add Animal feed production (AnF)
+
+
+0.2.3 (2021-11-24)
+------------------
+
+* Update Landfill
+
+
+0.2.1 (2021-10-02)
+------------------
+
+* New models: Gasification & Syngas combustion (GC), Refuse-Derived Fuel (RDF), Home composting (HC)
+
+
+0.1.9 (2021-05-10)
+------------------
+
+* Life cycle cost, input data for TS, References
+
+
+0.1.0 (2020-05-06)
+------------------
+
+* First release on PyPI. Data for the Life-cycle process models include: LF, WTE, Composting, AD, SS_MRF, reprocessing and Collection.
```

