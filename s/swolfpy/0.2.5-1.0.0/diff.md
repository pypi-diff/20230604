# Comparing `tmp/swolfpy-0.2.5.tar.gz` & `tmp/swolfpy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\swolfpy-0.2.5.tar", last modified: Thu Apr  7 13:42:46 2022, max compression
+gzip compressed data, was "swolfpy-1.0.0.tar", last modified: Sun Jun  4 18:03:00 2023, max compression
```

## Comparing `swolfpy-0.2.5.tar` & `swolfpy-1.0.0.tar`

### file list

```diff
@@ -1,78 +1,68 @@
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:46.000000 swolfpy-0.2.5/
--rw-rw-rw-   0        0        0      803 2021-08-24 20:23:22.000000 swolfpy-0.2.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     1586 2021-11-15 21:16:01.000000 swolfpy-0.2.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1033 2022-04-07 13:39:41.000000 swolfpy-0.2.5/HISTORY.rst
--rw-rw-rw-   0        0        0    18431 2021-10-02 16:33:29.000000 swolfpy-0.2.5/LICENSE.md
--rw-rw-rw-   0        0        0      273 2021-08-24 20:23:23.000000 swolfpy-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     9538 2022-04-07 13:42:46.000000 swolfpy-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     5699 2022-04-07 13:37:02.000000 swolfpy-0.2.5/README.rst
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:44.000000 swolfpy-0.2.5/docs/
--rw-rw-rw-   0        0        0     9752 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Getting_started.rst
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:45.000000 swolfpy-0.2.5/docs/Images/
--rw-rw-rw-   0        0        0   119274 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/AddCol.png
--rw-rw-rw-   0        0        0   131147 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/AddTreat.png
--rw-rw-rw-   0        0        0   154839 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/CreateScen.png
--rw-rw-rw-   0        0        0   192895 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/DefSys.png
--rw-rw-rw-   0        0        0    33184 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/IPM_CommonData.png
--rw-rw-rw-   0        0        0    63578 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/IPM_Tech.png
--rw-rw-rw-   0        0        0   154988 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/ImportPM.png
--rw-rw-rw-   0        0        0   190612 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/LCAContr.png
--rw-rw-rw-   0        0        0   146574 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/LCARes.png
--rw-rw-rw-   0        0        0   370894 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/LCA_LCI.png
--rw-rw-rw-   0        0        0   245142 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/LCIAView.png
--rw-rw-rw-   0        0        0   283477 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/LoadProj.png
--rw-rw-rw-   0        0        0   244005 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/MC.png
--rw-rw-rw-   0        0        0   139690 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/MCData.png
--rw-rw-rw-   0        0        0   156870 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/MCPlot.png
--rw-rw-rw-   0        0        0   209580 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/Opt.png
--rw-rw-rw-   0        0        0    79408 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/OptSet.png
--rw-rw-rw-   0        0        0   133628 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/SWM_network.png
--rw-rw-rw-   0        0        0   172835 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/SetupLCA.png
--rw-rw-rw-   0        0        0   188034 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Images/Start.png
--rw-rw-rw-   0        0        0      628 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/Makefile
--rw-rw-rw-   0        0        0       29 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/authors.rst
--rw-rw-rw-   0        0        0     5917 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/contributing.rst
--rw-rw-rw-   0        0        0      343 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/doc_inputdata.rst
--rw-rw-rw-   0        0        0      275 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/doc_processmodels.rst
--rw-rw-rw-   0        0        0      989 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/doc_swolfpy.rst
--rw-rw-rw-   0        0        0       29 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/history.rst
--rw-rw-rw-   0        0        0      383 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/index.rst
--rw-rw-rw-   0        0        0       96 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/make.bat
--rw-rw-rw-   0        0        0       84 2021-08-24 20:23:23.000000 swolfpy-0.2.5/docs/readme.rst
--rw-rw-rw-   0        0        0       42 2022-04-07 13:42:46.000000 swolfpy-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2235 2022-04-07 13:30:16.000000 swolfpy-0.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:45.000000 swolfpy-0.2.5/swolfpy/
--rw-rw-rw-   0        0        0    11543 2022-04-06 04:44:22.000000 swolfpy-0.2.5/swolfpy/LCA_matrix.py
--rw-rw-rw-   0        0        0     7416 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/Monte_Carlo.py
--rw-rw-rw-   0        0        0    25247 2022-04-06 04:42:02.000000 swolfpy-0.2.5/swolfpy/Optimization.py
--rw-rw-rw-   0        0        0    11473 2022-02-02 23:37:51.000000 swolfpy-0.2.5/swolfpy/Parameters.py
--rw-rw-rw-   0        0        0    18940 2021-10-02 16:33:30.000000 swolfpy-0.2.5/swolfpy/ProcessDB.py
--rw-rw-rw-   0        0        0    19365 2022-01-19 02:12:20.000000 swolfpy-0.2.5/swolfpy/Project.py
--rw-rw-rw-   0        0        0   111148 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/Required_keys.py
--rw-rw-rw-   0        0        0     8207 2021-11-25 12:17:59.000000 swolfpy-0.2.5/swolfpy/Technosphere.py
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:46.000000 swolfpy-0.2.5/swolfpy/UI/
--rw-rw-rw-   0        0        0    11730 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/UI/MC_ui.py
--rw-rw-rw-   0        0        0   123968 2022-02-03 21:39:06.000000 swolfpy-0.2.5/swolfpy/UI/PySWOLF_run.py
--rw-rw-rw-   0        0        0   140761 2021-10-21 15:18:02.000000 swolfpy-0.2.5/swolfpy/UI/PySWOLF_ui.py
--rw-rw-rw-   0        0        0  1301136 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/UI/PyWOLF_Resource_rc.py
--rw-rw-rw-   0        0        0     3233 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/UI/Reference_ui.py
--rw-rw-rw-   0        0        0    11358 2021-10-21 15:18:02.000000 swolfpy-0.2.5/swolfpy/UI/Table_from_pandas.py
--rw-rw-rw-   0        0        0     4171 2021-10-21 15:18:02.000000 swolfpy-0.2.5/swolfpy/UI/Workers.py
--rw-rw-rw-   0        0        0        0 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/UI/__init__.py
--rw-rw-rw-   0        0        0     4341 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/UI/adv_opt_ui.py
--rw-rw-rw-   0        0        0     1184 2022-04-07 13:30:23.000000 swolfpy-0.2.5/swolfpy/__init__.py
--rw-rw-rw-   0        0        0     1024 2021-08-24 20:23:23.000000 swolfpy-0.2.5/swolfpy/swolfpy_method.py
--rw-rw-rw-   0        0        0     3275 2021-11-25 12:17:59.000000 swolfpy-0.2.5/swolfpy/utils.py
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:45.000000 swolfpy-0.2.5/swolfpy.egg-info/
--rw-rw-rw-   0        0        0     9538 2022-04-07 13:42:43.000000 swolfpy-0.2.5/swolfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1529 2022-04-07 13:42:43.000000 swolfpy-0.2.5/swolfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-07 13:42:43.000000 swolfpy-0.2.5/swolfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-04-07 13:42:43.000000 swolfpy-0.2.5/swolfpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      250 2022-04-07 13:42:43.000000 swolfpy-0.2.5/swolfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-04-07 13:42:43.000000 swolfpy-0.2.5/swolfpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-07 13:42:46.000000 swolfpy-0.2.5/tests/
--rw-rw-rw-   0        0        0    61440 2021-08-31 00:11:23.000000 swolfpy-0.2.5/tests/.coverage
--rw-rw-rw-   0        0        0       38 2021-08-24 20:23:23.000000 swolfpy-0.2.5/tests/__init__.py
--rw-rw-rw-   0        0        0     4828 2021-08-24 20:23:23.000000 swolfpy-0.2.5/tests/test_swolfpy.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:03:00.050901 swolfpy-1.0.0/
+-rw-rw-rw-   0        0        0      802 2023-06-04 17:35:50.000000 swolfpy-1.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1586 2022-11-25 03:16:38.000000 swolfpy-1.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1122 2023-06-04 17:35:50.000000 swolfpy-1.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    18431 2022-11-25 05:25:00.000000 swolfpy-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0      273 2022-11-25 05:47:32.000000 swolfpy-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8173 2023-06-04 18:03:00.047889 swolfpy-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5711 2023-06-04 17:35:50.000000 swolfpy-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-04 18:02:59.678889 swolfpy-1.0.0/docs/
+-rw-rw-rw-   0        0        0     9516 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/Getting_started.rst
+drwxrwxrwx   0        0        0        0 2023-06-04 18:02:59.767887 swolfpy-1.0.0/docs/Images/
+-rw-rw-rw-   0        0        0   119274 2022-11-25 05:48:12.000000 swolfpy-1.0.0/docs/Images/AddCol.png
+-rw-rw-rw-   0        0        0   131147 2022-11-25 07:14:39.000000 swolfpy-1.0.0/docs/Images/AddTreat.png
+-rw-rw-rw-   0        0        0   154839 2022-11-25 05:52:28.000000 swolfpy-1.0.0/docs/Images/CreateScen.png
+-rw-rw-rw-   0        0        0   192895 2022-11-25 05:51:44.000000 swolfpy-1.0.0/docs/Images/DefSys.png
+-rw-rw-rw-   0        0        0    33184 2022-11-25 06:11:16.000000 swolfpy-1.0.0/docs/Images/IPM_CommonData.png
+-rw-rw-rw-   0        0        0    63578 2022-11-25 05:49:00.000000 swolfpy-1.0.0/docs/Images/IPM_Tech.png
+-rw-rw-rw-   0        0        0   154988 2022-11-25 06:16:15.000000 swolfpy-1.0.0/docs/Images/ImportPM.png
+-rw-rw-rw-   0        0        0   190612 2022-11-25 05:55:25.000000 swolfpy-1.0.0/docs/Images/LCAContr.png
+-rw-rw-rw-   0        0        0   146574 2022-11-25 06:36:54.000000 swolfpy-1.0.0/docs/Images/LCARes.png
+-rw-rw-rw-   0        0        0   370894 2022-11-25 05:58:53.000000 swolfpy-1.0.0/docs/Images/LCA_LCI.png
+-rw-rw-rw-   0        0        0   245142 2022-11-25 05:52:10.000000 swolfpy-1.0.0/docs/Images/LCIAView.png
+-rw-rw-rw-   0        0        0   283477 2022-11-25 05:54:33.000000 swolfpy-1.0.0/docs/Images/LoadProj.png
+-rw-rw-rw-   0        0        0   244005 2022-11-25 05:59:15.000000 swolfpy-1.0.0/docs/Images/MC.png
+-rw-rw-rw-   0        0        0   139690 2022-11-25 05:54:59.000000 swolfpy-1.0.0/docs/Images/MCData.png
+-rw-rw-rw-   0        0        0   156870 2022-11-25 05:59:37.000000 swolfpy-1.0.0/docs/Images/MCPlot.png
+-rw-rw-rw-   0        0        0   209580 2022-11-25 05:56:18.000000 swolfpy-1.0.0/docs/Images/Opt.png
+-rw-rw-rw-   0        0        0    79408 2022-11-25 05:48:28.000000 swolfpy-1.0.0/docs/Images/OptSet.png
+-rw-rw-rw-   0        0        0   133628 2022-11-25 06:00:56.000000 swolfpy-1.0.0/docs/Images/SWM_network.png
+-rw-rw-rw-   0        0        0   172835 2022-11-25 05:50:46.000000 swolfpy-1.0.0/docs/Images/SetupLCA.png
+-rw-rw-rw-   0        0        0   188034 2022-11-25 05:58:04.000000 swolfpy-1.0.0/docs/Images/Start.png
+-rw-rw-rw-   0        0        0      628 2022-11-25 05:54:42.000000 swolfpy-1.0.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2022-11-25 06:11:54.000000 swolfpy-1.0.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5979 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-11-25 06:10:07.000000 swolfpy-1.0.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0      335 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/doc_inputdata.rst
+-rw-rw-rw-   0        0        0      271 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/doc_processmodels.rst
+-rw-rw-rw-   0        0        0      982 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/doc_swolfpy.rst
+-rw-rw-rw-   0        0        0       29 2022-11-25 05:54:53.000000 swolfpy-1.0.0/docs/history.rst
+-rw-rw-rw-   0        0        0      380 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/index.rst
+-rw-rw-rw-   0        0        0       92 2023-06-04 17:35:50.000000 swolfpy-1.0.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2022-11-25 06:03:36.000000 swolfpy-1.0.0/docs/make.bat
+-rw-rw-rw-   0        0        0       84 2022-11-25 06:00:08.000000 swolfpy-1.0.0/docs/readme.rst
+-rw-rw-rw-   0        0        0    10974 2023-06-04 17:35:50.000000 swolfpy-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      335 2023-06-04 17:36:27.000000 swolfpy-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:03:00.051890 swolfpy-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 18:02:59.957887 swolfpy-1.0.0/swolfpy/
+-rw-rw-rw-   0        0        0    15980 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/LCA_matrix.py
+-rw-rw-rw-   0        0        0     8197 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/Monte_Carlo.py
+-rw-rw-rw-   0        0        0    25661 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/Optimization.py
+-rw-rw-rw-   0        0        0    12407 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/Parameters.py
+-rw-rw-rw-   0        0        0    22614 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/ProcessDB.py
+-rw-rw-rw-   0        0        0    19503 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/Project.py
+-rw-rw-rw-   0        0        0   119828 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/Required_keys.py
+-rw-rw-rw-   0        0        0     9059 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/Technosphere.py
+-rw-rw-rw-   0        0        0     1151 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/swolfpy_method.py
+-rw-rw-rw-   0        0        0     3070 2023-06-04 17:35:50.000000 swolfpy-1.0.0/swolfpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:03:00.003887 swolfpy-1.0.0/swolfpy.egg-info/
+-rw-rw-rw-   0        0        0     8173 2023-06-04 18:02:59.000000 swolfpy-1.0.0/swolfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2023-06-04 18:02:59.000000 swolfpy-1.0.0/swolfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:02:59.000000 swolfpy-1.0.0/swolfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      313 2023-06-04 18:02:59.000000 swolfpy-1.0.0/swolfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-04 18:02:59.000000 swolfpy-1.0.0/swolfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 18:03:00.042890 swolfpy-1.0.0/tests/
+-rw-rw-rw-   0        0        0    61440 2022-11-25 05:43:10.000000 swolfpy-1.0.0/tests/.coverage
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:35:50.000000 swolfpy-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4774 2023-06-04 17:35:50.000000 swolfpy-1.0.0/tests/test_swolfpy.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swolfpy-0.2.5/AUTHORS.rst` & `swolfpy-1.0.0/AUTHORS.rst`

 * *Files 27% similar despite different names*

```diff
@@ -15,12 +15,12 @@
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

### Comparing `swolfpy-0.2.5/CONTRIBUTING.rst` & `swolfpy-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/HISTORY.rst` & `swolfpy-1.0.0/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,18 @@
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
 0.2.5 (2022-04-07)
 ------------------
 
 * Minor changes in optimization and GUI
 
 
 0.2.3 (2021-11-16)
```

### Comparing `swolfpy-0.2.5/LICENSE.md` & `swolfpy-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/PKG-INFO` & `swolfpy-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,239 +1,247 @@
 Metadata-Version: 2.1
 Name: swolfpy
-Version: 0.2.5
-Summary: Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
-Home-page: https://github.com/SwolfPy-Project/swolfpy
-Author: Mojtaba Sardarmehni
-Author-email: msardar2@ncsu.edu
+Version: 1.0.0
+Summary: Solid Waste Optimization Life-cycle Framework in Python(SwolfPy).
+Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
+Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
-Description: .. General
-        
-        ================================================================
-        Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
-        ================================================================
-        
-        .. image:: https://img.shields.io/pypi/v/swolfpy.svg
-                :target: https://pypi.python.org/pypi/swolfpy
-        
-        .. image:: https://img.shields.io/pypi/pyversions/swolfpy.svg
-            :target: https://pypi.org/project/swolfpy/
-            :alt: Supported Python Versions
-        
-        .. image:: https://img.shields.io/pypi/l/swolfpy.svg
-            :target: https://pypi.org/project/swolfpy/
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/dm/swolfpy.svg?label=Pypi%20downloads
-            :target: https://pypi.org/project/swolfpy/
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/format/swolfpy.svg
-            :target: https://pypi.org/project/swolfpy/
-            :alt: Format
-        
-        .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
-                :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml/badge.svg?branch=master
-                :target: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml
-                :alt: Test
-        
-        .. image:: https://zenodo.org/badge/395802952.svg
-                :target: https://zenodo.org/badge/latestdoi/395802952
-                :alt: DOi
-        
-        .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
-           :target: https://doi.org/10.1111/jiec.13236
-           :alt: JIE DOI
-        
-        * Free software: GNU GENERAL PUBLIC LICENSE V2
-        * Website: https://swolfpy-project.github.io
-        * Documentation: https://swolfpy.readthedocs.io
-        * Repository: https://github.com/SwolfPy-Project/swolfpy
-        
-        
-        Features
-        --------
-        
-        * **Life-cycle assessment of Municipal Solid Waste (MSW) systems**
-        
-          * Comparative LCA
-          * Contribution analysis
-          * LCI report
-        
-        * **Monte Carlo simulation**
-        
-          * Uncertainty analysis
-          * Data visualization (distributions & correlations)
-        
-        * **Optimization**
-        
-          * Minimize environmental burdens or cost subject to a number of technical or policy-related constraints
-        
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
-                conda create --name swolfpy python=3.7 graphviz
-        
-        4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
-        
-        5- Activate the environment::
-        
-                conda activate swolfpy
-        
-        6- Install swolfpy in the environment::
-        
-                pip install swolfpy
-        
-        7- Open python to run swolfpy::
-        
-                python
-        
-        8- Run swolfpy in python::
-        
-                import swolfpy as sp
-                sp.swolfpy()
-        
-        .. endInstallation
-        
-        
-        =======
-        History
-        =======
-        
-        0.2.5 (2022-04-07)
-        ------------------
-        
-        * Minor changes in optimization and GUI
-        
-        
-        0.2.3 (2021-11-16)
-        ------------------
-        
-        * Improve data validation in GUI
-        * Improve warning/Pop-ups
-        
-        
-        0.2.2 (2021-10-02)
-        ------------------
-        
-        * Add Home Composting (HC)
-        * Add Gasification & Syngas combustion (GC)
-        * Add Refuse-derived fuel (RDF)
-        
-        
-        0.2.0 (2021-05-10)
-        ------------------
-        
-        * Add tab for correlation analysis.
-        * Add cost calculations.
-        * Add help to interface.
-        * Parallel optimization.
-        
-        
-        
-        0.1.8 (2020-05-20)
-        ------------------
-        
-        * Add tab for Monte Carlo results analysis.
-        * Show Sankey for mass flows after optimization.
-        * Show SWM Network graph.
-        
-        
-        
-        0.1.6 (2020-04-11)
-        ------------------
-        
-        * Add Reprocessing.
-        * Revise Functional units.
-        * Revise parameters class.
-        
-        
-        0.1.0 (2020-02-27)
-        ------------------
-        
-        * First release on PyPI.
-        * Main functionality: LCA, Monte-Carlo, and Optimization.
-        * Process Models include LF, WTE, Composting, AD, SS_MRF, and Collection.
-        
-Keywords: swolfpy
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://swolfpy-project.github.io/
+Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy
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
+================================================================
+Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
+================================================================
+
+.. image:: https://img.shields.io/pypi/v/swolfpy.svg
+        :target: https://pypi.python.org/pypi/swolfpy
+
+.. image:: https://img.shields.io/pypi/pyversions/swolfpy.svg
+    :target: https://pypi.org/project/swolfpy/
+    :alt: Supported Python Versions
+
+.. image:: https://img.shields.io/pypi/l/swolfpy.svg
+    :target: https://pypi.org/project/swolfpy/
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/swolfpy.svg?label=Pypi%20downloads
+    :target: https://pypi.org/project/swolfpy/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/format/swolfpy.svg
+    :target: https://pypi.org/project/swolfpy/
+    :alt: Format
+
+.. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
+        :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml/badge.svg?branch=master
+        :target: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml
+        :alt: Test
+
+.. image:: https://zenodo.org/badge/395802952.svg
+        :target: https://zenodo.org/badge/latestdoi/395802952
+        :alt: DOi
+
+.. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
+   :target: https://doi.org/10.1111/jiec.13236
+   :alt: JIE DOI
+
+* Free software: GNU GENERAL PUBLIC LICENSE V2
+* Website: https://swolfpy-project.github.io
+* Documentation: https://swolfpy.readthedocs.io
+* Repository: https://github.com/SwolfPy-Project/swolfpy
+
+
+Features
+--------
+
+* **Life-cycle assessment of Municipal Solid Waste (MSW) systems**
+
+  * Comparative LCA
+  * Contribution analysis
+  * LCI report
+
+* **Monte Carlo simulation**
+
+  * Uncertainty analysis
+  * Data visualization (distributions & correlations)
+
+* **Optimization**
+
+  * Minimize environmental burdens or cost subject to a number of technical or policy-related constraints
+
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
+        conda create --name swolfpy python=3.10 graphviz
+
+4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
+
+5- Activate the environment::
+
+        conda activate swolfpy
+
+6- Install swolfpy in the environment::
+
+        pip install swolfpy
+
+7- Open python to run swolfpy::
+
+        python
+
+8- Run swolfpy in python::
+
+        import swolfpy as sp
+        sp.swolfpy()
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
+0.2.5 (2022-04-07)
+------------------
+
+* Minor changes in optimization and GUI
+
+
+0.2.3 (2021-11-16)
+------------------
+
+* Improve data validation in GUI
+* Improve warning/Pop-ups
+
+
+0.2.2 (2021-10-02)
+------------------
+
+* Add Home Composting (HC)
+* Add Gasification & Syngas combustion (GC)
+* Add Refuse-derived fuel (RDF)
+
+
+0.2.0 (2021-05-10)
+------------------
+
+* Add tab for correlation analysis.
+* Add cost calculations.
+* Add help to interface.
+* Parallel optimization.
+
+
+
+0.1.8 (2020-05-20)
+------------------
+
+* Add tab for Monte Carlo results analysis.
+* Show Sankey for mass flows after optimization.
+* Show SWM Network graph.
+
+
+
+0.1.6 (2020-04-11)
+------------------
+
+* Add Reprocessing.
+* Revise Functional units.
+* Revise parameters class.
+
+
+0.1.0 (2020-02-27)
+------------------
+
+* First release on PyPI.
+* Main functionality: LCA, Monte-Carlo, and Optimization.
+* Process Models include LF, WTE, Composting, AD, SS_MRF, and Collection.
```

### Comparing `swolfpy-0.2.5/README.rst` & `swolfpy-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
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
 
 
 .. Installation
@@ -125,15 +125,15 @@
 
 2- Update conda in a terminal window or anaconda prompt::
 
         conda update conda
 
 3- Create a new environment for swolfpy::
 
-        conda create --name swolfpy python=3.7 graphviz
+        conda create --name swolfpy python=3.10 graphviz
 
 4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
 
 5- Activate the environment::
 
         conda activate swolfpy
```

### Comparing `swolfpy-0.2.5/docs/Getting_started.rst` & `swolfpy-1.0.0/docs/Getting_started.rst`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 If you want to create a new project, click the `Start New Project` button [10]. You can also load a project[11].
 
 .. figure:: /Images/Start.png
 	:align: left
 	:name: Start_fig
-	
+
 	Start tab
 
 
 Import Process Models
 ######################
 
 If you activate the radio button for `User Defined Process Models`, then you will see this (:numref:`ImportPM_fig`) tab which includes three subtabs:
@@ -56,15 +56,15 @@
 1. **Process Models**: You can select the default or user defined python models for the process models.
 2. **Common Data**: You can change the common data file.
 3. **Technosphere**: You can select the user defined LCI data or create a `User_Technosphere` database with `EcoSpold2` files and connect to it.
 
 
 If you have modified the default process models, then you should set them in this tab. You should select the process model from the drop-down list[4] and
 click the `User Defined` radio button[5]. Now you should click the `Browse` button[5] and find your python file. You can also revise the types of waste that
-each process models can accept throught the `Input Flow Type` screen [6]. Don't forget to click the `Update` button befor changing the next process model
+each process models can accept through the `Input Flow Type` screen [6]. Don't forget to click the `Update` button before changing the next process model
 otherwise your changes will be lost. When you are done, you should click the `Import Process Models` to import them and go to the next step.
 
 
 .. note:: All the python files for the process models should be in `swolfpy_processmodels` directory. If you don't know where is your installation, then do the
 			following::
 
 				import swolfpy_processmodels
@@ -86,238 +86,237 @@
 	:name: IPM_CommonData_fig
 
 	Import Process Models tab: Common Data subtab.
 
 
 In the `Technosphere` subtab (:numref:`IPM_Tech_fig`), you can select the user defined model[1] or LCI data [2].
 You can also create a `User_Technosphere` database with `EcoSpold2` files.
-Inorder to do that, you should select the directory that contains the `EcoSpold2` files[4].
+In order to do that, you should select the directory that contains the `EcoSpold2` files[4].
 You should also add the `Reference_activity_id` to the `Technosphere_References.csv` file in the `swolfpy_inputdata\Data` directory. Then you should
 browse the `Technosphere_References.csv` [3].
 
 
 .. figure:: /Images/IPM_Tech.png
 	:align: center
 	:name: IPM_Tech_fig
-	
+
 	Import Process Models tab: Technosphere subtab.
 
 
 
 
 Define SWM System
 ###################
 
 
 
 Define Collection Processes
 ***************************
 
 
-.. note:: If you are importing data, the data should be in the `csv` format and have the same column names as the default data files. 
+.. note:: If you are importing data, the data should be in the `csv` format and have the same column names as the default data files.
 		  We suggest to copy our data files and edit them to keep the structure.
 
 .. figure:: /Images/AddCol.png
 	:align: left
 	:name: AddCol_fig
-	
+
 	Define Collection Processes for SWM system.
 
 
 
 
 
 Define Treatment Processes
 ***************************
 
-.. note:: If you are importing data, the data should be in the `csv` format and have the same column names as the default data files. 
+.. note:: If you are importing data, the data should be in the `csv` format and have the same column names as the default data files.
 		  We suggest to copy our data files and edit them to keep the structure.
 
 
 .. figure:: /Images/AddTreat.png
 	:align: left
 	:name: AddTreat_fig
-	
+
 	Define Treatment Processes for SWM system.
 
 
 
 
 Define SWM System
 ******************
 
 
 .. figure:: /Images/DefSys.png
 	:align: left
 	:name: DefSys_fig
-	
+
 	Define SWM system (Distances and processes allocations).
 
 
 
 Create Scenario
 #################
 
 
 .. figure:: /Images/CreateScen.png
 	:align: left
 	:name: CreateScen_fig
-	
+
 	Create scenario tab.
 
 
 
 
 LCA
 #####
 
 Setup LCA
 **********
 
 .. figure:: /Images/SetupLCA.png
 	:align: left
 	:name: SetupLCA_fig
-	
+
 	Setup LCA tab (Selecting the functional units and impact assessment methods).
 
 
 LCA Results
 *************
 
 .. figure:: /Images/LCARes.png
 	:align: left
 	:name: LCARes_fig
-	
+
 	LCA results tab.
 
 
 Contribution Analysis
 **********************
 
 .. figure:: /Images/LCAContr.png
 	:align: left
 	:name: LCAContr_fig
-	
+
 	Contribution analysis tab (Shows the top emissions or top activities that contribute to the selected impact).
 
 
 
 Life Cycle Inventory
 *********************
 
 .. figure:: /Images/LCA_LCI.png
 	:align: left
 	:name: LCA_LCI_fig
-	
+
 	LCI tab.
 
 
 
 Monte Carlo Simulation
 #######################
 
 .. figure:: /Images/MC.png
 	:align: left
 	:name: MC_fig
-	
+
 	Monte Carlo Simulation tab.
 
 
 Monte Carlo Results
 ####################
 
 
 Data
 *****
 
 
 .. figure:: /Images/MCData.png
 	:align: left
 	:name: MCData_fig
-	
+
 	Monte Carlo Simulation results window.
 
 
 
 Plot
 *****
 
 .. figure:: /Images/MCPlot.png
 	:align: left
 	:name: MCPlot_fig
-	
+
 	Plot Monte Carlo Simulation results window.
 
 
 
 Optimization
 #############
 
 .. figure:: /Images/Opt.png
 	:align: left
 	:name: Opt_fig
-	
+
 	Optimization tab.
 
 
 
 .. figure:: /Images/OptSet.png
 	:align: left
 	:name: OptSet_fig
-	
+
 	Optimization setting window.
 
 
 
 
 
 Load Project
 ##############
 
 
 .. figure:: /Images/LoadProj.png
 	:align: left
 	:name: LoadProj_fig
-	
+
 	Load Project tab.
 
 
 
 
- 
+
 Uncertainty Distribution
 ##########################
 
 Tha `stats_arrays <https://stats-arrays.readthedocs.io/en/latest/index.html#>`_ package is used to define uncertain input parameters for the
 process models and waste materials. The table below shows the main uncertainty distributions that are currently used
 
 
 ======================= ===================== =========================== ============================= ================= ============= ===============
 Name                    ``uncertainty_type``  ``loc``                     ``scale``                     ``shape``         ``minimum``   ``maximum``
 ======================= ===================== =========================== ============================= ================= ============= ===============
-Undefined               0                     **static value**                                                                                           
-No uncertainty          1                     **static value**                                                                                           
-Lognoraml               2                     :math:`\boldsymbol{\mu}`    :math:`\boldsymbol{\sigma}`                     *Lower bound* *Upper bound*  
-Normal                  3                     :math:`\boldsymbol{\mu}`    :math:`\boldsymbol{\sigma}`                     *Lower bound* *Upper bound*  
-Uniform                 4                                                                                                 *Minimum*     *Maximum*      
-Triangular              5                     **mode**                                                                    *Minimum*     *Maximum*      
-Discrete Uniform        7                     **mode**                                                                    *Minimum*     *upper bound*    
+Undefined               0                     **static value**
+No uncertainty          1                     **static value**
+Lognormal               2                     :math:`\boldsymbol{\mu}`    :math:`\boldsymbol{\sigma}`                     *Lower bound* *Upper bound*
+Normal                  3                     :math:`\boldsymbol{\mu}`    :math:`\boldsymbol{\sigma}`                     *Lower bound* *Upper bound*
+Uniform                 4                                                                                                 *Minimum*     *Maximum*
+Triangular              5                     **mode**                                                                    *Minimum*     *Maximum*
+Discrete Uniform        7                     **mode**                                                                    *Minimum*     *upper bound*
 ======================= ===================== =========================== ============================= ================= ============= ===============
 
 Guideline to define uncertainty
 *******************************
 
 1. **Normal distributions (ID = 3)**: When there is sufficient published data.
-2. **Triangular distribution (ID = 5)**: When values are based on expert opinions with a reasonable value for the mode.
-3. **Uniform Distribution (ID=4)**: When only the range is known without preference for mode.
-4. **Lognormal distributions (ID=2)**:  When only one value is available or there is significant data and the value must be non-negative.
-5. **Discrete Uniform (ID=7)**: For True/False (0,1) parameters.(min=0,max=2).
+2. **Triangular distribution (ID = 5)**: When values are based on expert opinions with a reasonable value for the mode.
+3. **Uniform Distribution (ID=4)**: When only the range is known without preference for mode.
+4. **Lognormal distributions (ID=2)**: When only one value is available or there is significant data and the value must be non-negative.
+5. **Discrete Uniform (ID=7)**: For True/False (0,1) parameters.(min=0,max=2).
 
 
-.. note:: In **Normal distribution**, if the mean is too close to lower or upper bound (mostly for parameters that are fractions), 
+.. note:: In **Normal distribution**, if the mean is too close to lower or upper bound (mostly for parameters that are fractions),
 		  use the triangular distribution.
 
-.. note:: In **Lognormal distribution**, if the parameter is related to the emission factors, sigma should be in the range of
-		  0.04 to 0.09 based on the quality of the data.  
+.. note:: In **Lognormal distribution**, if the parameter is related to the emission factors, sigma should be in the range of
+		  0.04 to 0.09 based on the quality of the data.
 
 .. seealso:: For more information about distributions check `stats_arrays <https://stats-arrays.readthedocs.io/en/latest/index.html#>`_ website.
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swolfpy-0.2.5/docs/Images/AddCol.png` & `swolfpy-1.0.0/docs/Images/AddCol.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/AddTreat.png` & `swolfpy-1.0.0/docs/Images/AddTreat.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/CreateScen.png` & `swolfpy-1.0.0/docs/Images/CreateScen.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/DefSys.png` & `swolfpy-1.0.0/docs/Images/DefSys.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/IPM_CommonData.png` & `swolfpy-1.0.0/docs/Images/IPM_CommonData.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/IPM_Tech.png` & `swolfpy-1.0.0/docs/Images/IPM_Tech.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/ImportPM.png` & `swolfpy-1.0.0/docs/Images/ImportPM.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/LCAContr.png` & `swolfpy-1.0.0/docs/Images/LCAContr.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/LCARes.png` & `swolfpy-1.0.0/docs/Images/LCARes.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/LCA_LCI.png` & `swolfpy-1.0.0/docs/Images/LCA_LCI.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/LCIAView.png` & `swolfpy-1.0.0/docs/Images/LCIAView.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/LoadProj.png` & `swolfpy-1.0.0/docs/Images/LoadProj.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/MC.png` & `swolfpy-1.0.0/docs/Images/MC.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/MCData.png` & `swolfpy-1.0.0/docs/Images/MCData.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/MCPlot.png` & `swolfpy-1.0.0/docs/Images/MCPlot.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/Opt.png` & `swolfpy-1.0.0/docs/Images/Opt.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/OptSet.png` & `swolfpy-1.0.0/docs/Images/OptSet.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/SWM_network.png` & `swolfpy-1.0.0/docs/Images/SWM_network.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/SetupLCA.png` & `swolfpy-1.0.0/docs/Images/SetupLCA.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Images/Start.png` & `swolfpy-1.0.0/docs/Images/Start.png`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/Makefile` & `swolfpy-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/docs/conf.py` & `swolfpy-1.0.0/docs/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,182 +15,184 @@
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 
 
-
+import importlib
 import os
 import sys
-import importlib
-
-numfig = True
-
-sys.path.insert(0, os.path.abspath('..'))
-
 
 import plotly.io as pio
-pio.renderers.default = 'sphinx_gallery'
+
+numfig = True
+sys.path.insert(0, os.path.abspath(".."))
+pio.renderers.default = "sphinx_gallery"
 
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode', 'nbsphinx','sphinx.ext.mathjax']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode", "nbsphinx", "sphinx.ext.mathjax"]
 
 autodoc_mock_imports = []
-for mod in ['swolfpy',\
-            'swolfpy_inputdata','swolfpy_processmodels',\
-            'matplotlib','scipy','pandas','numpy',\
-            'bw2analyzer','stats_arrays','brightway2','bw2data',\
-            'PySide2','PySide2.QtGui', 'PySide2.QtCore', 'PySide2.QtWidgets']:
+for mod in [
+    "swolfpy",
+    "swolfpy_inputdata",
+    "swolfpy_processmodels",
+    "matplotlib",
+    "scipy",
+    "pandas",
+    "numpy",
+    "bw2analyzer",
+    "stats_arrays",
+    "brightway2",
+    "bw2data",
+    "PySide2",
+    "PySide2.QtGui",
+    "PySide2.QtCore",
+    "PySide2.QtWidgets",
+]:
     try:
         importlib.import_module(mod)
     except ImportError:
         autodoc_mock_imports.append(mod)
-        
-print('autodoc_mock_imports: {}'.format(autodoc_mock_imports))
+
+print("autodoc_mock_imports: {}".format(autodoc_mock_imports))
 
 autodoc_default_options = {
-    'member-order': 'bysource',  
-    'undoc-members': True,
-    'private-members':True
+    "member-order": "bysource",
+    "undoc-members": True,
+    "private-members": True,
 }
 
-autodoc_member_order = 'bysource'  # the other options are : 'alphabetical', 'groupwise'
+autodoc_member_order = "bysource"  # the other options are : 'alphabetical', 'groupwise'
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'swolfpy'
-copyright = "2020, Mojtaba Sardarmehni"
+project = "swolfpy"
+copyright = "2020, Mojtaba Sardarmehni"  # pylint: disable=redefined-builtin
 author = "Mojtaba Sardarmehni"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-#version = swolfpy.__version__
+# version = swolfpy.__version__
 # The full version, including alpha/beta/rc tags.
-#release = swolfpy.__version__
+# release = swolfpy.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
-html_theme_options = {'page_width': '1200px',}
+html_theme_options = {
+    "page_width": "1200px",
+}
 #
 html_logo = "../swolfpy/UI/PySWOLF_ICONS/PySWOLF.ico"
 
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'swolfpydoc'
+htmlhelp_basename = "swolfpydoc"
 
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'swolfpy.tex',
-     'swolfpy Documentation',
-     'Mojtaba Sardarmehni', 'manual'),
+    (master_doc, "swolfpy.tex", "swolfpy Documentation", "Mojtaba Sardarmehni", "manual"),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'swolfpy',
-     'swolfpy Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "swolfpy", "swolfpy Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'swolfpy',
-     'swolfpy Documentation',
-     author,
-     'swolfpy',
-     'Solid Waste Optimization Life-cycle Framework in Python',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "swolfpy",
+        "swolfpy Documentation",
+        author,
+        "swolfpy",
+        "Solid Waste Optimization Life-cycle Framework in Python",
+        "Miscellaneous",
+    ),
 ]
-
-
-
```

### Comparing `swolfpy-0.2.5/docs/doc_swolfpy.rst` & `swolfpy-1.0.0/docs/doc_swolfpy.rst`

 * *Files 9% similar despite different names*

```diff
@@ -40,40 +40,40 @@
 
 .. _swolfpy_method:
 
 swolfpy_method
 ===============
 
 .. autofunction:: swolfpy.swolfpy_method.import_methods
-   
+
 
 
 .. _LCA_matrix:
 
 LCA Matrix
 ===========
 
 .. autoclass:: swolfpy.LCA_matrix.LCA_matrix
    :members:
    :show-inheritance:
-   
-   
+
+
 
 .. _montecarlo:
 
 Monte Carlo
 ===========
 
 .. autoclass:: swolfpy.Monte_Carlo.Monte_Carlo
    :members:
    :show-inheritance:
 
 
 
-.. _optimizaiton:
+.. _optimization:
 
 Optimization
 ============
 
 .. autoclass:: swolfpy.Optimization.Optimization
    :members:
-   :show-inheritance:
+   :show-inheritance:
```

### Comparing `swolfpy-0.2.5/docs/make.bat` & `swolfpy-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swolfpy-0.2.5/swolfpy/LCA_matrix.py` & `swolfpy-1.0.0/swolfpy/LCA_matrix.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,216 +1,314 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Apr 22 19:09:14 2020
-
-@author: msmsa
-"""
-from brightway2 import LCA, get_activity
 import numpy as np
 import pandas as pd
+from brightway2 import LCA, get_activity
 
 
 class LCA_matrix(LCA):
     """
-    This class translate the ``row`` and ``col`` of the ``tech_param`` and ``bio_param`` to
-    the acticity `key` in the Brightway2 database. \n
-    Both the ``tech_param`` and ``bio_param`` has the ``dtype=[('input', '<u4'), ('output', '<u4'),
-    ('row', '<u4'), ('col', '<u4'), ('type', 'u1'), ('uncertainty_type', 'u1'), ('amount', '<f4'),
-    ('loc', '<f4'), ('scale', '<f4'), ('shape', '<f4'), ('minimum', '<f4'), ('maximum', '<f4'),
-    ('negative', '?')])`` data type. \n
+    This class translate the ``row`` and ``col`` of the ``tech_param`` and ``bio_param``
+    to the activity `key` in the Brightway2 database. \n Both the ``tech_param`` and
+    ``bio_param`` has the ``dtype=[('input', '<u4'), ('output', '<u4'), ('row', '<u4'),
+    ('col', '<u4'), ('type', 'u1'), ('uncertainty_type', 'u1'), ('amount', '<f4'), ('loc',
+    '<f4'), ('scale', '<f4'), ('shape', '<f4'), ('minimum', '<f4'), ('maximum', '<f4'),
+    ('negative', '?')])`` data type. \n.
 
-    ``self.tech_matrix`` is a dictionary that includes all the technosphere and waste exhanges as tuple ``(product,Feed)`` key and amount as value:
+    ``self.tech_matrix`` is a dictionary that includes all the technosphere and waste exchanges as tuple ``(product,Feed)`` key and amount as value:
     ``{(('LF', 'Aerobic_Residual'), ('SF1_product', 'Aerobic_Residual_MRDO')):0.828}``
 
-    ``self.bio_matrix`` is a dictionary taht includes all the biosphere exhanges as tuple ``(product,Feed)`` `key` and amount as `value`
+    ``self.bio_matrix`` is a dictionary that includes all the biosphere exchanges as tuple ``(product,Feed)`` `key` and amount as `value`
     ``{(('biosphere3', '0015ec22-72cb-4af1-8c7b-0ba0d041553c'), ('Technosphere', 'Boiler_Diesel')):6.12e-15}``
 
-    So we can update the ``tech_params`` and ``bio_params`` by tuple keys that are consistant with the keys
-    in the ``ProcessMolde.report()``. Check :ref:`Process models class <ProcessModel>` for more info.
+    So we can update the ``tech_params`` and ``bio_params`` by tuple keys that are consistent with the keys
+    in the ``ProcessModel.report()``. Check :ref:`Process models class <ProcessModel>` for more info.
     """
+
     def __init__(self, functional_unit, method):
         super().__init__(functional_unit, method[0])
         self.lci()
         self.lcia()
 
         self.functional_unit = functional_unit
         self.method = method
         self._base_method = method[0]
 
         self.activities_dict, _, self.biosphere_dict = self.reverse_dict()
 
-        self.tech_matrix = dict()
+        self.tech_matrix = {}
         for i in self.tech_params:
             self.tech_matrix[(self.activities_dict[i[2]], self.activities_dict[i[3]])] = i[6]
 
-        self.bio_matrix = dict()
+        self.bio_matrix = {}
         for i in self.bio_params:
-            if (self.biosphere_dict[i[2]], self.activities_dict[i[3]]) not in self.bio_matrix.keys():
+            if (
+                self.biosphere_dict[i[2]],
+                self.activities_dict[i[3]],
+            ) not in self.bio_matrix.keys():
                 self.bio_matrix[(self.biosphere_dict[i[2]], self.activities_dict[i[3]])] = i[6]
             else:
-                self.bio_matrix[(str(self.biosphere_dict[i[2]]) + " - 1", self.activities_dict[i[3]])] = i[6]
+                self.bio_matrix[
+                    (str(self.biosphere_dict[i[2]]) + " - 1", self.activities_dict[i[3]])
+                ] = i[6]
                 # print((str(biosphere_dict[i[2]]) + " - 1", activities_dict[i[3]]))
 
     @staticmethod
     def update_techmatrix(process_name, report_dict, tech_matrix):
         """
-        Updates the `tech_matrix` according to the  `report_dict`. `tech_matrix` is an instance of ``LCA_matrix.tech_matrix``.
-        Useful for Monte Carlo simulation, and optimization.
+        Updates the `tech_matrix` according to the  `report_dict`. `tech_matrix` is an
+        instance of ``LCA_matrix.tech_matrix``. Useful for Monte Carlo simulation, and
+        optimization.
 
         :param process_name: Name of the life-cycle process model.
         :type process_name: str
 
         :param report_dict: LCI report of the life-cycle process model (``swolfpy_processmodels.ProcessModel.report()``).
         :type report_dict: dict
 
         :param tech_matrix:
         :type tech_matrix: ``LCA_matrix.tech_matrix``
-
         """
         for material, value in report_dict["Technosphere"].items():
             for key2, value2 in value.items():
                 if not np.isnan(value2):
                     if ((key2), (process_name, material)) in tech_matrix.keys():
                         if tech_matrix[((key2), (process_name, material))] != value2:
                             tech_matrix[((key2), (process_name, material))] = value2
                     else:
-                        raise KeyError('Exchange {} is calculated but not exist in LCA technosphere'.format(((key2), (process_name, material))))
+                        raise KeyError(
+                            "Exchange {} is calculated but not exist in LCA technosphere".format(
+                                ((key2), (process_name, material))
+                            )
+                        )
                 else:
-                    raise ValueError('Amount for Exchange {} is Nan. The amount should be number, check the calculations in the process model'
-                                     .format(((key2), (process_name, material))))
+                    raise ValueError(
+                        "Amount for Exchange {} is Nan. The amount should be number, check the calculations in the process model".format(
+                            ((key2), (process_name, material))
+                        )
+                    )
 
         for material, value in report_dict["Waste"].items():
             for key2, value2 in value.items():
                 # Remove prefix from material name in the case of Transfer Station
-                if report_dict['process name'][1] == 'Transfer_Station':
-                    if 'DryRes' == material[0:6] or 'WetRes' == material[0:6]:
+                if report_dict["process name"][1] == "Transfer_Station":
+                    if "DryRes" == material[0:6] or "WetRes" == material[0:6]:
                         material_ = material[7:]
-                    elif 'ORG' == material[0:3] or 'REC' == material[0:3]:
+                    elif "ORG" == material[0:3] or "REC" == material[0:3]:
                         material_ = material[4:]
                 else:
                     material_ = material
-                key2 = (process_name + "_product", material_ + '_' + key2)
+                key2 = (process_name + "_product", material_ + "_" + key2)
                 if not np.isnan(value2):
                     if ((key2), (process_name, material)) in tech_matrix.keys():
                         if tech_matrix[((key2), (process_name, material))] != value2:
                             tech_matrix[((key2), (process_name, material))] = value2
                     else:
-                        raise KeyError('Exchange {} is calculated but not exist in LCA technosphere'.format(((key2), (process_name, material))))
+                        raise KeyError(
+                            "Exchange {} is calculated but not exist in LCA technosphere".format(
+                                ((key2), (process_name, material))
+                            )
+                        )
 
                 else:
-                    raise ValueError('Amount for Exchange {} is Nan. The amount should be number, check the calculations in the process model'
-                                     .format(((key2), (process_name, material))))
+                    raise ValueError(
+                        "Amount for Exchange {} is Nan. The amount should be number, check the calculations in the process model".format(
+                            ((key2), (process_name, material))
+                        )
+                    )
 
             ### Adding activity for transport between the collection and treatment processes
-            if 'LCI' in report_dict.keys():
+            if "LCI" in report_dict.keys():
                 for y in report_dict["LCI"].keys():
                     for m in report_dict["LCI"][y].keys():
                         for n in report_dict["LCI"][y][m].keys():
-                            if 'biosphere3' not in n:
+                            if "biosphere3" not in n:
                                 if not np.isnan(report_dict["LCI"][y][m][n]):
-                                    if (n, (process_name + '_product', y + '_' + 'to' + '_' + m)) in tech_matrix.keys():
-                                        if tech_matrix[(n, (process_name + '_product', y + '_' + 'to' + '_' + m))] != report_dict["LCI"][y][m][n]:
-                                            tech_matrix[(n, (process_name + '_product', y + '_' + 'to' + '_' + m))] = report_dict["LCI"][y][m][n]
+                                    if (
+                                        n,
+                                        (process_name + "_product", y + "_" + "to" + "_" + m),
+                                    ) in tech_matrix.keys():
+                                        if (
+                                            tech_matrix[
+                                                (
+                                                    n,
+                                                    (
+                                                        process_name + "_product",
+                                                        y + "_" + "to" + "_" + m,
+                                                    ),
+                                                )
+                                            ]
+                                            != report_dict["LCI"][y][m][n]
+                                        ):
+                                            tech_matrix[
+                                                (
+                                                    n,
+                                                    (
+                                                        process_name + "_product",
+                                                        y + "_" + "to" + "_" + m,
+                                                    ),
+                                                )
+                                            ] = report_dict["LCI"][y][m][n]
                                     else:
-                                        raise KeyError('Exchange {} is calculated but not exist in LCA technosphere'
-                                                       .format((n, (process_name + '_product', y + '_' + 'to' + '_' + m))))
+                                        raise KeyError(
+                                            "Exchange {} is calculated but not exist in LCA technosphere".format(
+                                                (
+                                                    n,
+                                                    (
+                                                        process_name + "_product",
+                                                        y + "_" + "to" + "_" + m,
+                                                    ),
+                                                )
+                                            )
+                                        )
                                 else:
-                                    raise ValueError("""Amount for Exchange {} is Nan. The amount should be number,
-                                                     check the calculations in the process model"""
-                                                     .format((n, (process_name + '_product', y + '_' + 'to' + '_' + m))))
+                                    raise ValueError(
+                                        """Amount for Exchange {} is Nan. The amount should be number,
+                                                     check the calculations in the process model""".format(
+                                            (
+                                                n,
+                                                (
+                                                    process_name + "_product",
+                                                    y + "_" + "to" + "_" + m,
+                                                ),
+                                            )
+                                        )
+                                    )
 
     @staticmethod
     def update_biomatrix(process_name, report_dict, bio_matrix):
         """
-        Updates the `bio_matrix` according to the  report_dict. `bio_matrix` is an instance of ``LCA_matrix.bio_matrix``.
-        Useful for Monte Carlo simulation, and optimization.
+        Updates the `bio_matrix` according to the  report_dict. `bio_matrix` is an
+        instance of ``LCA_matrix.bio_matrix``. Useful for Monte Carlo simulation, and
+        optimization.
 
         :param process_name: Name of the life-cycle process model.
         :type process_name: str
 
         :param report_dict: LCI report of the life-cycle process model (``swolfpy_processmodels.ProcessModel.report()``).
         :type report_dict: dict
 
         :param bio_matrix:
         :type bio_matrix: ``LCA_matrix.bio_matrix``
-
         """
         for material, value in report_dict["Biosphere"].items():
             for key2, value2 in value.items():
                 if not np.isnan(value2):
                     if bio_matrix[((key2), (process_name, material))] != value2:
                         bio_matrix[((key2), (process_name, material))] = value2
                 else:
-                    raise ValueError('Amount for Exchange {} is Nan. The amount should be number, check the calculations in the process model'
-                                     .format(((key2), (process_name, material))))
+                    raise ValueError(
+                        "Amount for Exchange {} is Nan. The amount should be number, check the calculations in the process model".format(
+                            ((key2), (process_name, material))
+                        )
+                    )
             ### Adding activity for collection cost
-            if 'LCI' in report_dict.keys():
+            if "LCI" in report_dict.keys():
                 for y in report_dict["LCI"].keys():
                     for m in report_dict["LCI"][y].keys():
                         for n in report_dict["LCI"][y][m].keys():
-                            if 'biosphere3' in n:
+                            if "biosphere3" in n:
                                 if not np.isnan(report_dict["LCI"][y][m][n]):
-                                    if (n, (process_name + '_product', y + '_' + 'to' + '_' + m)) in bio_matrix.keys():
-                                        if bio_matrix[(n, (process_name + '_product', y + '_' + 'to' + '_' + m))] != report_dict["LCI"][y][m][n]:
-                                            bio_matrix[(n, (process_name + '_product', y + '_' + 'to' + '_' + m))] = report_dict["LCI"][y][m][n]
+                                    if (
+                                        n,
+                                        (process_name + "_product", y + "_" + "to" + "_" + m),
+                                    ) in bio_matrix.keys():
+                                        if (
+                                            bio_matrix[
+                                                (
+                                                    n,
+                                                    (
+                                                        process_name + "_product",
+                                                        y + "_" + "to" + "_" + m,
+                                                    ),
+                                                )
+                                            ]
+                                            != report_dict["LCI"][y][m][n]
+                                        ):
+                                            bio_matrix[
+                                                (
+                                                    n,
+                                                    (
+                                                        process_name + "_product",
+                                                        y + "_" + "to" + "_" + m,
+                                                    ),
+                                                )
+                                            ] = report_dict["LCI"][y][m][n]
                                     else:
-                                        raise KeyError('Exchange {} is calculated but not exist in LCA biosphere'
-                                                       .format((n, (process_name + '_product', y + '_' + 'to' + '_' + m))))
+                                        raise KeyError(
+                                            "Exchange {} is calculated but not exist in LCA biosphere".format(
+                                                (
+                                                    n,
+                                                    (
+                                                        process_name + "_product",
+                                                        y + "_" + "to" + "_" + m,
+                                                    ),
+                                                )
+                                            )
+                                        )
                                 else:
-                                    raise ValueError("""Amount for Exchange {} is Nan. The amount should be number,
-                                                     check the calculations in the process model"""
-                                                     .format((n, (process_name + '_product', y + '_' + 'to' + '_' + m))))
+                                    raise ValueError(
+                                        """Amount for Exchange {} is Nan. The amount should be number,
+                                                     check the calculations in the process model""".format(
+                                            (
+                                                n,
+                                                (
+                                                    process_name + "_product",
+                                                    y + "_" + "to" + "_" + m,
+                                                ),
+                                            )
+                                        )
+                                    )
 
     @staticmethod
     def get_mass_flow(LCA, process):
         """
-        Calculates the total mass of flows to process based on the `supply_array` in ``bw2calc.lca.LCA``.
+        Calculates the total mass of flows to process based on the `supply_array` in
+        ``bw2calc.lca.LCA``.
 
         :param LCA: LCA object.
         :type LCA: ``bw2calc.lca.LCA`` or ``swolfpy.LCA_matrix.LCA_matrix``
 
         :param process: Name of the process databases.
         :type process: str
 
         :return: Total mass of flows to `process`
         :rtype: float
-
         """
         mass = 0
         for i in LCA.activity_dict:
             if process == i[0]:
-                unit = get_activity(i).as_dict()['unit'].split(' ')
+                unit = get_activity(i).as_dict()["unit"].split(" ")
                 if len(unit) > 1:
                     mass += LCA.supply_array[LCA.activity_dict[i]] * float(unit[0])
                 else:
                     mass += LCA.supply_array[LCA.activity_dict[i]]
-        return(mass)
+        return mass
 
     @staticmethod
     def get_mass_flow_comp(LCA, process, index):
         """
-        Calculates the mass of flows to process based on the `index` and `supply_array` in ``bw2calc.lca.LCA``.
+        Calculates the mass of flows to process based on the `index` and `supply_array` in
+        ``bw2calc.lca.LCA``.
 
         :param LCA: LCA object.
         :type LCA: ``bw2calc.lca.LCA`` or ``swolfpy.LCA_matrix.LCA_matrix``
 
         :param process: Name of the process databases.
         :type process: str
 
         :param index: Name of the process databases.
         :type index: str
 
         :return: Pandas series with mass flows as values and index as rows.
         :rtype: pandas.core.series.Series
-
         """
         mass = pd.Series(np.zeros(len(index)), index=index)
         for i in LCA.activity_dict:
             if process == i[0]:
                 for j in index:
                     if j == i[1]:
-                        unit = get_activity(i).as_dict()['unit'].split(' ')
+                        unit = get_activity(i).as_dict()["unit"].split(" ")
                         if len(unit) > 1:
                             mass[j] += LCA.supply_array[LCA.activity_dict[i]] * float(unit[0])
                         else:
                             mass[j] += LCA.supply_array[LCA.activity_dict[i]]
-        return(mass)
+        return mass
```

### Comparing `swolfpy-0.2.5/swolfpy/Monte_Carlo.py` & `swolfpy-1.0.0/swolfpy/Monte_Carlo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Apr 22 19:45:04 2020
+import multiprocessing as mp
+import os
 
-@author: msmsa
-"""
 import numpy as np
 import pandas as pd
-import os
-from .LCA_matrix import LCA_matrix
-import multiprocessing as mp
 from brightway2 import LCA, projects
 
+from .LCA_matrix import LCA_matrix
+
 
 class Monte_Carlo(LCA_matrix):
-    """Setups the Monte Carlo simulation. This class is inherited from ``swolfpy.LCA_matrix``. \n
-    The Monte Carlo simulation will be only done for  the process models, common data
-    or parameters than the class gets by arguments.
+    """
+    Setups the Monte Carlo simulation. This class is inherited from
+    ``swolfpy.LCA_matrix``. \n The Monte Carlo simulation will be only done for  the
+    process models, common data or parameters than the class gets by arguments.
 
     :param functional_unit: ``{flow:amount}``
     :type functional_unit: dict
 
     :param method: List of methods for MC.
     :type method: list
 
@@ -36,87 +34,147 @@
     :type common_data: ``swolfpy_inputdata.CommonData.CommonData`` , optional
 
     :param parameters: ``Parameters`` object
     :type parameters: ``swolfpy_inputdata.Parameters.Parameters``,optional
 
     :param seed: seed for ``stats_arrays.RandomNumberGenerator``
     :type seed: int, optional
-
     """
-    def __init__(self, functional_unit, method, project, process_models=None, process_model_names=None,
-                 common_data=None, parameters=None, seed=None):
+
+    def __init__(
+        self,
+        functional_unit,
+        method,
+        project,
+        process_models=None,
+        process_model_names=None,
+        common_data=None,
+        parameters=None,
+        seed=None,
+    ):
         super().__init__(functional_unit, method)
 
         self.process_models = process_models
         self.process_model_names = process_model_names
         self.parameters = parameters
         self.common_data = common_data
         self.project = project
         if seed:
             self.seed = seed
         else:
             self.seed = 0
 
     def run(self, nproc, n):
-        """ Runs the Monte Carlo ``n`` times with ``nproc`` processors. Calls and map the ``Monte_Carlo.worker()`` to the processors.
+        """
+        Runs the Monte Carlo ``n`` times with ``nproc`` processors. Calls and map the
+        ``Monte_Carlo.worker()`` to the processors.
 
         :param nproc: Number of processors allocated to MC
         :type nproc: int
         :param n: Number of iterations in MC
         :type n: int
-
         """
 
         def pool_adapter(x):
-            return(x)
+            return x
 
         with pool_adapter(mp.Pool(processes=nproc)) as pool:
-            res = pool.map(Monte_Carlo.worker,
-                           [(self.project, self.functional_unit, self.method, self.parameters, self.process_models,
-                             self.process_model_names, self.common_data, self.tech_matrix, self.bio_matrix, self.seed + i * 100, n // nproc)
-                            for i in range(nproc)])
+            res = pool.map(
+                Monte_Carlo.worker,
+                [
+                    (
+                        self.project,
+                        self.functional_unit,
+                        self.method,
+                        self.parameters,
+                        self.process_models,
+                        self.process_model_names,
+                        self.common_data,
+                        self.tech_matrix,
+                        self.bio_matrix,
+                        self.seed + i * 100,
+                        n // nproc,
+                    )
+                    for i in range(nproc)
+                ],
+            )
         self.results = [x for lst in res for x in lst]
-# =============================================================================
-#         res = Monte_Carlo.worker((self.project, self.functional_unit, self.method, self.parameters, self.process_models, self.process_model_names,
-#                                   self.common_data, self.tech_matrix, self.bio_matrix, self.seed, n//nproc))
-#         self.results = [x for lst in res for x in lst]
-# =============================================================================
+
+    # =============================================================================
+    #         res = Monte_Carlo.worker((self.project, self.functional_unit, self.method, self.parameters, self.process_models, self.process_model_names,
+    #                                   self.common_data, self.tech_matrix, self.bio_matrix, self.seed, n//nproc))
+    #         self.results = [x for lst in res for x in lst]
+    # =============================================================================
 
     @staticmethod
     def worker(args):
         """
-        Setups the Monte Carlo for process models and input data and then creates the ``LCA`` object
-        and Calls the ``Monte_Carlo.parallel_mc()`` for `n` times.
+        Setups the Monte Carlo for process models and input data and then creates the
+        ``LCA`` object and Calls the ``Monte_Carlo.parallel_mc()`` for `n` times.
         """
-        project, functional_unit, method, parameters, process_models, process_model_names, common_data, tech_matrix, bio_matrix, seed, n = args
+        (
+            project,
+            functional_unit,
+            method,
+            parameters,
+            process_models,
+            process_model_names,
+            common_data,
+            tech_matrix,
+            bio_matrix,
+            seed,
+            n,
+        ) = args
         projects.set_current(project, writable=False)
         if common_data:
             common_data.setup_MC(seed + 100000)
         if process_models:
             for seed_, x in enumerate(process_models):
                 x.setup_MC(seed + seed_)
         if parameters:
             parameters.setup_MC(seed + 200000)
 
         lca = LCA(functional_unit, method[0])
         lca.lci()
         lca.lcia()
-        return [Monte_Carlo.parallel_mc(lca, project, functional_unit, method, tech_matrix, bio_matrix, process_models=process_models,
-                process_model_names=process_model_names, parameters=parameters, common_data=common_data, index=x)
-                for x in range(n)]
+        return [
+            Monte_Carlo.parallel_mc(
+                lca,
+                method,
+                tech_matrix,
+                bio_matrix,
+                process_models=process_models,
+                process_model_names=process_model_names,
+                parameters=parameters,
+                common_data=common_data,
+                index=x,
+            )
+            for x in range(n)
+        ]
 
     @staticmethod
-    def parallel_mc(lca, project, functional_unit, method, tech_matrix, bio_matrix, process_models=None, process_model_names=None,
-                    parameters=None, common_data=None, index=None):
-        """
-        Calls the ``InputData.gen_MC()`` , ``ProcessModel.MC_calc()``  and ``parameters.MC_calc()`` and then gets the new LCI and updates
-        the ``tech_matrix`` and ``bio_matrix``. Creates new ``bio_param`` and ``tech_param`` and then recalculate the LCA.
+    def parallel_mc(
+        lca,
+        method,
+        tech_matrix,
+        bio_matrix,
+        process_models=None,
+        process_model_names=None,
+        parameters=None,
+        common_data=None,
+        index=None,
+    ):
+        """
+        Calls the ``InputData.gen_MC()`` , ``ProcessModel.MC_calc()``  and
+        ``parameters.MC_calc()`` and then gets the new LCI and updates the ``tech_matrix``
+        and ``bio_matrix``.
 
+        Creates new ``bio_param`` and ``tech_param`` and then recalculate the LCA.
         """
-        uncertain_inputs = list()
+        uncertain_inputs = []
         if process_models:
             if common_data:
                 uncertain_inputs += common_data.gen_MC()
                 for process in process_models:
                     process.CommonData = common_data
                     uncertain_inputs += process.MC_calc()
             else:
@@ -142,39 +200,43 @@
 
         lca.rebuild_technosphere_matrix(tech)
         lca.rebuild_biosphere_matrix(bio)
         lca.lci_calculation()
         if lca.lcia:
             lca.lcia_calculation()
 
-        lca_results = dict()
+        lca_results = {}
         lca_results[method[0]] = lca.score
 
         if len(method) > 1:
             for i in range(1, len(method)):
                 lca.switch_method(method[i])
                 lca.lcia_calculation()
                 lca_results[method[i]] = lca.score
             lca.switch_method(method[0])
         print(os.getpid(), index)
-        return(os.getpid(), lca_results, uncertain_inputs)
+        return (os.getpid(), lca_results, uncertain_inputs)
 
     ### Export results
     def result_to_DF(self):
-        """ Returns the results from the Monte Carlo in a ``pandas.DataFrame`` format.
+        """
+        Returns the results from the Monte Carlo in a ``pandas.DataFrame`` format.
 
         :return: Monte Carlo results
         :rtype: ``pandas.DataFrame``
         """
         output = pd.DataFrame()
         # Reporting the LCIA results; Create a column for each method
         for j in self.results[0][1].keys():
             output[j] = [self.results[i][1][j] for i in range(len(self.results))]
         # Reporting the input data
         for j in range(len(self.results[0][2])):
-            output[self.results[0][2][j][0]] = [self.results[i][2][j][1] for i in range(len(self.results))]
-        return(output)
+            output[self.results[0][2][j][0]] = [
+                self.results[i][2][j][1] for i in range(len(self.results))
+            ]
+        return output
 
     def save_results(self, name):
-        """ Save the results from the Monte Carlo to pickle file.
+        """
+        Save the results from the Monte Carlo to pickle file.
         """
         self.result_to_DF().to_pickle(name)
```

### Comparing `swolfpy-0.2.5/swolfpy/Optimization.py` & `swolfpy-1.0.0/swolfpy/Optimization.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,83 +1,94 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Apr 22 19:35:26 2020
+import json
+import multiprocessing as mp
+import os
+from copy import deepcopy
+from functools import partial
+from multiprocessing import Pool, cpu_count
+from multiprocessing.dummy import Pool as ThreadPool
+from time import time
 
-@author: msmsa
-"""
-from .LCA_matrix import LCA_matrix
 import numpy as np
 import pandas as pd
-from scipy.optimize import minimize
 import plotly.graph_objects as go
-from plotly.offline import plot
-from copy import deepcopy
-import json
-from multiprocessing import Pool, cpu_count, TimeoutError
-from multiprocessing.dummy import Pool as ThreadPool
-from functools import partial
-import os
 import pyDOE
-from time import time
 from brightway2 import projects
+from plotly.offline import plot
+from scipy.optimize import minimize
+
+from .LCA_matrix import LCA_matrix
 
 
 class Optimization(LCA_matrix):
     """
 
     :param functional_unit:
     :type functional_unit: dict
     :param method:
-    :type method: lsit
+    :type method: list
     :param project:
     :type project: ``swolfpy.Project.Project``
 
     """
+
     def __init__(self, functional_unit, method, project):
         super().__init__(functional_unit, method)
         self.project = project
         self.Treatment_processes = deepcopy(self.project.Treatment_processes)
         self.Collection_processes = deepcopy(self.project.Collection_processes)
         self.N_param = len(self.project.parameters_list)
 
         self.n_scheme_vars = 0
 
     @staticmethod
-    def config(project):
+    def get_config(project):
         columns = []
         schemes = {}
         for col in project.Collection_processes:
             columns.append(col)
-            columns.append(col + ' mode')
-            schemes[col] = project.Collection_processes[col]['model'].col_schm
+            columns.append(col + " mode")
+            schemes[col] = project.Collection_processes[col]["model"].col_schm
 
-        index = [('RWC', 'N/A', 'N/A'),
-                 ('RWC', 'N/A', 'SSR'),
-                 ('RWC', 'SSYW', 'N/A'),
-                 ('RWC', 'SSYW', 'SSR'),
-                 ('RWC', 'SSO', 'N/A'),
-                 ('RWC', 'SSO', 'SSR'),
-                 ('RWC', 'SSO_AnF', 'N/A'),
-                 ('RWC', 'SSO_AnF', 'SSR'),
-                 ('REC_WetRes', 'N/A', 'REC_WetRes'),
-                 ('REC_WetRes', 'SSYW', 'REC_WetRes'),
-                 ('REC_WetRes', 'SSO', 'REC_WetRes'),
-                 ('REC_WetRes', 'SSO_AnF', 'REC_WetRes'),
-                 ('ORG_DryRes', 'ORG_DryRes', 'N/A'),
-                 ('ORG_DryRes', 'ORG_DryRes', 'SSR')]
+        index = [
+            ("RWC", "N/A", "N/A"),
+            ("RWC", "N/A", "SSR"),
+            ("RWC", "SSYW", "N/A"),
+            ("RWC", "SSYW", "SSR"),
+            ("RWC", "SSO", "N/A"),
+            ("RWC", "SSO", "SSR"),
+            ("RWC", "SSO_AnF", "N/A"),
+            ("RWC", "SSO_AnF", "SSR"),
+            ("REC_WetRes", "N/A", "REC_WetRes"),
+            ("REC_WetRes", "SSYW", "REC_WetRes"),
+            ("REC_WetRes", "SSO", "REC_WetRes"),
+            ("REC_WetRes", "SSO_AnF", "REC_WetRes"),
+            ("ORG_DryRes", "ORG_DryRes", "N/A"),
+            ("ORG_DryRes", "ORG_DryRes", "SSR"),
+        ]
 
         config_pd = pd.DataFrame(index=index, columns=columns)
         if len(config_pd.columns) > 0:
             for c in columns[1::2]:
-                config_pd[c] = ['Optimize', 'Optimize',
-                                'Optimize', 'Optimize',
-                                'Optimize', 'Optimize',
-                                'Fix', 'Fix',
-                                'Fix', 'Fix', 'Fix',
-                                'Fix', 'Fix', 'Fix']
+                config_pd[c] = [
+                    "Optimize",
+                    "Optimize",
+                    "Optimize",
+                    "Optimize",
+                    "Optimize",
+                    "Optimize",
+                    "Fix",
+                    "Fix",
+                    "Fix",
+                    "Fix",
+                    "Fix",
+                    "Fix",
+                    "Fix",
+                    "Fix",
+                ]
 
             for col, sch in schemes.items():
                 for k, v in sch.items():
                     if k in index:
                         config_pd[col][k] = v
         return config_pd.fillna(0.0)
 
@@ -85,89 +96,95 @@
         self.config = config
         self.scheme_vars_index = self.N_param
         self.scheme_vars_dict = {}
         self.x0_col = []
 
         for c in self.config.columns[1::2]:
             for i in self.config.index:
-                if self.config[c][i] == 'Optimize':
-                    self.scheme_vars_dict[self.scheme_vars_index] = (c.split(' mode')[0], i)
-                    self.x0_col.append(self.config[c.split(' mode')[0]][i])
+                if self.config[c][i] == "Optimize":
+                    self.scheme_vars_dict[self.scheme_vars_index] = (c.split(" mode")[0], i)
+                    self.x0_col.append(self.config[c.split(" mode")[0]][i])
                     self.scheme_vars_index += 1
                     self.n_scheme_vars += 1
 
         for process in self.config.columns[0::2]:
             for schm in self.config.index:
-                if schm in self.Treatment_processes[process]['model'].col_schm:
-                    self.Treatment_processes[process]['model'].col_schm[schm] = self.config.loc[[schm], process].values[0]
+                if schm in self.Treatment_processes[process]["model"].col_schm:
+                    self.Treatment_processes[process]["model"].col_schm[schm] = self.config.loc[
+                        [schm], process
+                    ].values[0]
 
     def update_col_scheme(self, x):
         process_set = set()
         if self.n_scheme_vars:
             for k, v in self.scheme_vars_dict.items():
                 process = v[0]
                 process_set.add(process)
-                self.Treatment_processes[process]['model'].col_schm[v[1]] = x[k]
+                self.Treatment_processes[process]["model"].col_schm[v[1]] = x[k]
             for process in process_set:
-                self.Treatment_processes[process]['model']._normalize_scheme(DropOff=False, warn=False)
+                self.Treatment_processes[process]["model"]._normalize_scheme(
+                    DropOff=False, warn=False
+                )
 
     ### Objective function
     def _objective_function(self, x):
         """
-        Use the new parameters (Waste fractions) to update the ``tech_matrix`` (``tech_param``)
-        and reculate the LCA score.
+        Use the new parameters (Waste fractions) to update the ``tech_matrix``
+        (``tech_param``) and recalculate the LCA score.
         """
         if self.oldx != list(x):  # Calculations are done only when the function get new x.
-            if self.oldx[0:self.N_param] != list(x)[0:self.N_param]:
-                param_exchanges = self.project.parameters.Param_exchanges(x[0:self.N_param])
+            if self.oldx[0 : self.N_param] != list(x)[0 : self.N_param]:
+                param_exchanges = self.project.parameters.Param_exchanges(x[0 : self.N_param])
                 for key, value in param_exchanges.items():
                     if key in self.tech_matrix:
                         self.tech_matrix[key] = value
 
-            if self.collection and self.oldx[self.N_param:] != list(x)[self.N_param:]:
+            if self.collection and self.oldx[self.N_param :] != list(x)[self.N_param :]:
                 self.update_col_scheme(x)
                 for col in self.Collection_processes:
-                    model = self.Treatment_processes[col]['model']
+                    model = self.Treatment_processes[col]["model"]
                     model.calc()
                     report_dict = model.report()
                     process_name = model.process_name
                     LCA_matrix.update_techmatrix(process_name, report_dict, self.tech_matrix)
                     LCA_matrix.update_biomatrix(process_name, report_dict, self.bio_matrix)
 
             tech = np.array(list(self.tech_matrix.values()), dtype=float)
             bio = np.array(list(self.bio_matrix.values()), dtype=float)
 
             self.rebuild_technosphere_matrix(tech)
             self.rebuild_biosphere_matrix(bio)
             self.lci_calculation()
-            if self.lcia:
+            if self.lcia:  # pylint: disable=using-constant-test
                 self.lcia_calculation()
 
             self.oldx = list(x)
-        return(self.score / 10**self.magnitude)
+        return self.score / 10**self.magnitude
 
     ### Mass to process
-    def get_mass_flow(self, key, KeyType, x):
+    def get_mass_flow_from_supply_array(self, key, KeyType, x):
         """
         calculate the mass to the process from the `supply_array` matrix.
         """
         self._objective_function(x)
 
         mass_flow = 0
-        if KeyType == 'WasteToProcess':
+        if KeyType == "WasteToProcess":
             for i in range(len(self.supply_array)):
                 if key == self.activities_dict[i]:
                     mass_flow += self.supply_array[i]
 
-        elif KeyType == 'Process':
+        elif KeyType == "Process":
             for i in range(len(self.supply_array)):
                 if key == self.activities_dict[i][0]:
                     mass_flow += self.supply_array[i]
         else:
-            raise ValueError(""" KeyType for the get_mass_flow function is not defined correct.""")
+            raise ValueError(
+                """ KeyType for the get_mass_flow_from_supply_array function is not defined correct."""
+            )
         return mass_flow
 
     ### Emission flow in LCI
     def get_emission_amount(self, emission, x):
         """
         calculate the mass of the `emission` to biosphere from the `inventory`.
         """
@@ -193,294 +210,332 @@
         return score
 
     def _create_equality(self, N_param_Ingroup):
         """
         Check that the sum of parameters in each group should be one.
         """
         local_index = self.Param_index
-        f = (lambda x: sum([x[i] for i in range(local_index, local_index + N_param_Ingroup)]) - 1)
+        f = lambda x: sum([x[i] for i in range(local_index, local_index + N_param_Ingroup)]) - 1
         self.Param_index += N_param_Ingroup
         return f
 
     def _create_inequality(self, key, limit, KeyType, ConstType):
         """
 
-        :param key: process name, key for activtity in process or key for activity in biosphere
+        :param key: process name, key for activity in process or key for activity in biosphere
         :type key: str or tuple
         :param limit:
         :type limit: float
         :param KeyType: ``"Process"``, ``"WasteToProcess"``, ``"Emission"``
         :type KeyType: str
         :param ConstType: ``"<="`` , ``">="``
         :type ConstType: str
 
         """
-        if ConstType not in ['<=', '>=']:
+        if ConstType not in ["<=", ">="]:
             raise ValueError(" Constraint Type is not defined correct ")
 
-        if KeyType == 'Process':
-            if ConstType == '<=':
-                f = (lambda x: limit - self.get_mass_flow(key, KeyType, x))
+        if KeyType == "Process":
+            if ConstType == "<=":
+                f = lambda x: limit - self.get_mass_flow_from_supply_array(key, KeyType, x)
             else:
-                f = (lambda x: self.get_mass_flow(key, KeyType, x) - limit)
+                f = lambda x: self.get_mass_flow_from_supply_array(key, KeyType, x) - limit
             return f
 
-        elif KeyType == 'WasteToProcess':
-            if ConstType == '<=':
-                f = (lambda x: limit - self.get_mass_flow(key, KeyType, x))
+        elif KeyType == "WasteToProcess":
+            if ConstType == "<=":
+                f = lambda x: limit - self.get_mass_flow_from_supply_array(key, KeyType, x)
             else:
-                f = (lambda x: self.get_mass_flow(key, KeyType, x) - limit)
+                f = lambda x: self.get_mass_flow_from_supply_array(key, KeyType, x) - limit
             return f
 
-        elif KeyType == 'Emission':
-            if ConstType == '<=':
-                f = (lambda x: limit - self.get_emission_amount(key, x))
+        elif KeyType == "Emission":
+            if ConstType == "<=":
+                f = lambda x: limit - self.get_emission_amount(key, x)
             else:
-                f = (lambda x: self.get_emission_amount(key, x) - limit)
+                f = lambda x: self.get_emission_amount(key, x) - limit
             return f
 
-        elif KeyType == 'Impact':
-            if ConstType == '<=':
-                f = (lambda x: limit - self.get_impact_amount(key, x))
+        elif KeyType == "Impact":
+            if ConstType == "<=":
+                f = lambda x: limit - self.get_impact_amount(key, x)
             else:
-                f = (lambda x: self.get_impact_amount(key, x) - limit)
+                f = lambda x: self.get_impact_amount(key, x) - limit
             return f
 
+        return None
+
     def _create_collection_constraints(self, cons):
         const_dict = {}
         if self.n_scheme_vars:
             for k in self.scheme_vars_dict:
                 process = self.scheme_vars_dict[k][0]
                 if process not in const_dict:
                     const_dict[process] = []
                 const_dict[process].append(k)
-        print("\n\n collection constraints dict: \n", const_dict, '\n\n')
+        print("\n\n collection constraints dict: \n", const_dict, "\n\n")
 
         for k in const_dict:
             self._col_const_helper(const_dict, k, cons)
 
     def _col_const_helper(self, const_dict, k, cons):
         def helper_sum(x, index):
-            return(sum([x[i] for i in index]))
+            return sum([x[i] for i in index])
 
         fix = 0
         for i in self.config.index:
-            if self.config[k + ' mode'][i] == 'Fix':
+            if self.config[k + " mode"][i] == "Fix":
                 fix += self.config[k][i]
-        cons.append({'type': 'eq',
-                     'fun': (lambda x: helper_sum(x, const_dict[k]) + fix - 1),
-                     'Name': '{} main const'.format(k)})
+        cons.append(
+            {
+                "type": "eq",
+                "fun": (lambda x: helper_sum(x, const_dict[k]) + fix - 1),
+                "Name": "{} main const".format(k),
+            }
+        )
 
     def _create_constraints(self):
         cons = list()
         group = dict()
 
         # Index for the parameters
         self.Param_index = 0
 
-        # Number of parameters in each group (from one source to different denstinations)
+        # Number of parameters in each group (from one source to different destinations)
         for key in self.project.parameters.param_uncertainty_dict.keys():
             group[key] = len(self.project.parameters.param_uncertainty_dict[key])
 
         # Equal constraint (sum of the parameters in each group should be one)
         for vals in group.values():
-            cons.append({'type': 'eq',
-                         'fun': self._create_equality(N_param_Ingroup=vals)})
+            cons.append({"type": "eq", "fun": self._create_equality(N_param_Ingroup=vals)})
 
         if self.collection and self.n_scheme_vars:
             self._create_collection_constraints(cons)
 
         if self.constraints:
             for key in self.constraints.keys():
-                cons.append({'type': 'ineq',
-                             'fun': self._create_inequality(key, self.constraints[key]['limit'], self.constraints[key]['KeyType'],
-                                                            self.constraints[key]['ConstType'])})
+                cons.append(
+                    {
+                        "type": "ineq",
+                        "fun": self._create_inequality(
+                            key,
+                            self.constraints[key]["limit"],
+                            self.constraints[key]["KeyType"],
+                            self.constraints[key]["ConstType"],
+                        ),
+                    }
+                )
         return cons
 
     @staticmethod
-    def multi_start_optimization(optObject, constraints=None, collection=False, n_iter=30,
-                                 nproc=None, timeout=None, initialize_guess='random'):
+    def multi_start_optimization(
+        optObject,
+        constraints=None,
+        collection=False,
+        n_iter=30,
+        nproc=None,
+        timeout=None,
+        initialize_guess="random",
+    ):
         """
         Call the ``scipy.optimize.minimize()`` to minimize the LCA score. \n
-        ``constraints`` is python dictionary. \n
-        Constraint type can be ``'<='`` or ``'>='``. \n
-        Three kind of constraints are defined as below: \n
-        * **Process:** Constraint on the total mass to the processs. The ``'KeyType'`` should be ``'Process'``
-          (e.g., The capacity of the WTE). Examaple:
+        ``constraints`` is python dictionary. \n Constraint type can be ``'<='`` or
+        ``'>='``. \n Three kind of constraints are defined as below: \n.
+
+        * **Process:** Constraint on the total mass to the process. The ``'KeyType'`` should be ``'Process'``
+          (e.g., The capacity of the WTE). Example:
 
         >>> constraints = {}
         >>> # Use name the the process as key in dict
         >>> constraints['WTE'] = {'limit':100, 'KeyType':'Process','ConstType':"<="}
 
-        * **WasteToProcess:** Constraint on the total mass of waste fraction to the processs. The ``'KeyType'`` should
-          be ``'WasteToProcess'`` (e.g., Ban food waste from landfill). Examaple:
+        * **WasteToProcess:** Constraint on the total mass of waste fraction to the process. The ``'KeyType'`` should
+          be ``'WasteToProcess'`` (e.g., Ban food waste from landfill). Example:
 
         >>> constraints = {}
         >>> # Use database key as key in dict
         >>> constraints[('LF','Food_Waste_Vegetable')] = {'limit':0, 'KeyType':'WasteToProcess','ConstType':"<="}
 
-        * **Emission:** Constraint on the emissions. The ``'KeyType'`` should be ``'Emission'`` (e.g., CO2 emissions Cap). Examaple:
+        * **Emission:** Constraint on the emissions. The ``'KeyType'`` should be ``'Emission'`` (e.g., CO2 emissions Cap). Example:
 
         >>> constraints = {}
         >>> # Use database key as key in dict
         >>> constraints[('biosphere3', 'eba59fd6-f37e-41dc-9ca3-c7ea22d602c7')] = {'limit':100,'KeyType':'Emission','ConstType':"<="}
-
         """
         optObject.constraints = constraints
         optObject.collection = collection
 
         optObject.magnitude = len(str(int(abs(optObject.score))))
 
-        global_min = 1E100
+        global_min = 1e100
 
         if optObject.collection:
             n_dec_vars = len(optObject.project.parameters_list) + optObject.n_scheme_vars
         else:
             n_dec_vars = len(optObject.project.parameters_list)
 
         bnds = tuple([(0, 1) for _ in range(n_dec_vars)])
 
         args = []
-        if initialize_guess == 'LHS':
+        if initialize_guess == "LHS":
             all_x0 = pyDOE.lhs(n_dec_vars, samples=n_iter)
-        elif initialize_guess == 'random':
+        elif initialize_guess == "random":
             all_x0 = np.random.rand(n_iter, n_dec_vars)
-        elif initialize_guess == 'binary':
-            all_x0 = np.random.randint(low=0,
-                                       high=2,
-                                       size=(n_iter, n_dec_vars))
+        elif initialize_guess == "binary":
+            all_x0 = np.random.randint(low=0, high=2, size=(n_iter, n_dec_vars))
         else:
-            raise ValueError(f'The {initialize_guess} method for generating the initial guess is not correct!')
+            raise ValueError(
+                f"The {initialize_guess} method for generating the initial guess is not correct!"
+            )
 
         for j in range(n_iter):
             args.append((optObject, bnds, all_x0[j], j))
 
         if not nproc:
             nproc = cpu_count()
 
         all_results = []
-        pool = Pool(processes=nproc, maxtasksperchild=1)
-        for arg in args:
-            abortable_func = partial(Optimization.abortable_worker, Optimization.worker, timeout=timeout)
-            all_results.append(pool.apply_async(abortable_func, args=arg))
-        results = [res.get() for res in all_results]
-        pool.close()
-        pool.join()
+        with Pool(processes=nproc, maxtasksperchild=1) as pool:
+            for arg in args:
+                abortable_func = partial(
+                    Optimization.abortable_worker, Optimization.worker, timeout=timeout
+                )
+                all_results.append(pool.apply_async(abortable_func, args=arg))
+
+            results = [res.get() for res in all_results]
+
         optObject.all_results = results
 
         optObject.res_global = False
         for i, res in enumerate(optObject.all_results):
             if res:
                 if res.success:
                     if res.fun < global_min:
                         optObject.res_global = res
                         global_min = res.fun
-                print("""\n
+                print(
+                    """\n
                       Iteration: {}
                       Status: {}, Message: {}
                       Objective function: {}
                       Global min: {} \n
-                      """.format(i,
-                                 res.success, res.message,
-                                 res.fun * 10**optObject.magnitude,
-                                 global_min * 10**optObject.magnitude))
+                      """.format(
+                        i,
+                        res.success,
+                        res.message,
+                        res.fun * 10**optObject.magnitude,
+                        global_min * 10**optObject.magnitude,
+                    )
+                )
             else:
-                print("""\n
+                print(
+                    """\n
                       Iteration: {}
                       Status: {}, Message: {}
                       Objective function: {}
                       Global min: {} \n
-                      """.format(i,
-                                 False, 'Aborting due to timeout!',
-                                 'NAN',
-                                 global_min * 10**optObject.magnitude))
+                      """.format(
+                        i,
+                        False,
+                        "Aborting due to timeout!",
+                        "NAN",
+                        global_min * 10**optObject.magnitude,
+                    )
+                )
 
         if not optObject.res_global:
             optObject.success = False
-            print('None of the iterations were successful!')
+            print("None of the iterations were successful!")
             return None
 
         if optObject.res_global.success:
             optObject.oldx = [0 for i in range(n_dec_vars)]
             optObject.success = True
             optObject.optimized_x = list()
             optObject.res_global.x = optObject.res_global.x.round(decimals=4)
             optObject._objective_function(optObject.res_global.x)
 
             for i in range(len(optObject.project.parameters_list)):
-                optObject.optimized_x.append({'name': optObject.project.parameters_list[i]['name'],
-                                              'amount': optObject.res_global.x[i]})
+                optObject.optimized_x.append(
+                    {
+                        "name": optObject.project.parameters_list[i]["name"],
+                        "amount": optObject.res_global.x[i],
+                    }
+                )
 
             if optObject.collection:
                 for k, v in optObject.scheme_vars_dict.items():
-                    optObject.optimized_x.append({'name': v,
-                                                  'amount': optObject.res_global.x[k]})
+                    optObject.optimized_x.append({"name": v, "amount": optObject.res_global.x[k]})
 
             return optObject.res_global
         else:
             optObject.success = False
             print(optObject.res_global.message)
             return optObject.res_global
 
     @staticmethod
     def abortable_worker(func, *args, **kwargs):
         iteration = args[3]
-        timeout = kwargs.get('timeout', None)
+        timeout = kwargs.get("timeout", None)
         p = ThreadPool(1)
         res = p.apply_async(func, args)
         try:
-            return(res.get(timeout))  # Wait timeout seconds for func to complete.
-        except TimeoutError:
+            return res.get(timeout)  # Wait timeout seconds for func to complete.
+        except mp.TimeoutError:
             print("(Iteration:{}, PID:{}): Aborting due to timeout!".format(iteration, os.getpid()))
             return None
 
     @staticmethod
     def worker(optObject, bnds, x0, iteration):
         start = time()
         projects.set_current(optObject.project.project_name, writable=False)
         print("Iteration: {} PID: {}\n".format(iteration, os.getpid()))
         optObject.oldx = [0 for i in range(len(x0))]
         optObject.cons = optObject._create_constraints()
-        res = minimize(optObject._objective_function, x0, method='SLSQP', bounds=bnds, constraints=optObject.cons)
+        res = minimize(
+            optObject._objective_function,
+            x0,
+            method="SLSQP",
+            bounds=bnds,
+            constraints=optObject.cons,
+        )
 
         time_ = round(time() - start)
-        print("Iteration: {} PID: {} time:{} sec, Success:{} \n".format(iteration,
-                                                                        os.getpid(),
-                                                                        time_,
-                                                                        res.success))
-        res['time'] = time_
-        res['PID'] = os.getpid()
-        return(res)
+        print(
+            "Iteration: {} PID: {} time:{} sec, Success:{} \n".format(
+                iteration, os.getpid(), time_, res.success
+            )
+        )
+        res["time"] = time_
+        res["PID"] = os.getpid()
+        return res
 
     def set_optimized_parameters_to_project(self):
         assert hasattr(self, "project"), "Must run optimize_parameters first"
-        assert self.success, "Optimization has to be sucessful first"
+        assert self.success, "Optimization has to be successful first"
 
         self.project.update_parameters(self.optimized_x)
 
     def plot_sankey(self, optimized_flow=True, show=True, fileName=None, params=None):
-        """Plots a sankey diagram for the waste mass flows. \n
-        Calls the ``plotly.graph_objs.Sankey`` to plot sankey. \n
-        Calculates the mass flows by calling ``self.get_mass_flow()``. \n
+        """
+        Plots a sankey diagram for the waste mass flows. \n Calls the
+        ``plotly.graph_objs.Sankey`` to plot sankey. \n Calculates the mass flows by
+        calling ``self.get_mass_flow_from_supply_array()``. \n.
 
         :param optimized_flow: If ``True``, it plots the sankey based on the optimized waste fractions.
-                                If ``False``, it plost the sankey based on the current waste fractions by calling ``self.project.parameters_list``.
+                                If ``False``, it plots the sankey based on the current waste fractions by calling ``self.project.parameters_list``.
         :type optimized_flow: bool
 
         :param show: If ``True``, it will show the figure
         :type show: bool
-
         """
         if optimized_flow:
-            params = [i['amount'] for i in self.optimized_x]
+            params = [i["amount"] for i in self.optimized_x]
         else:
-            if params:
-                params = params
-            else:
-                params = [i['amount'] for i in self.project.parameters_list]
+            params = params or [i["amount"] for i in self.project.parameters_list]
 
             self.oldx = [0 for i in range(len(params))]
             self.magnitude = len(str(int(abs(self.score))))
             self.N_param = len(self.project.parameters_list)
             self.col_model = []
 
         product = []
@@ -498,101 +553,108 @@
         target = []
         value = []
         label_link = []
         color = []
 
         # Color & shape for plotting the SWM Network
         # https://www.rapidtables.com/web/color/RGB_Color.html
-        edge_color = {'RWC': (160, 82, 45),  # sienna	#A0522D
-                      'SSR': (0, 0, 255),  # blue	#0000FF
-                      'DSR': (0, 0, 205),  # medium blue	#0000CD
-                      'MSR': (65, 105, 225),  # royal blue	#4169E1
-                      'LV': (0, 255, 0),  # lime	#00FF00
-                      'SSYW': (0, 100, 0),  # dark green	#006400
-                      'SSO': (0, 255, 127),  # spring green	#00FF7F
-                      'SSO_HC': (128, 128, 0),  # olive #808000
-                      'SSO_AnF': (127, 255, 0),  # chartreuse #7FFF00
-                      'ORG': (46, 139, 87),  # sea green	#2E8B57
-                      'DryRes': (222, 184, 135),  # burly wood	#DEB887
-                      'REC': (0, 191, 255),  # deep sky blue	#00BFFF
-                      'WetRes': (210, 105, 30),  # chocolate	#D2691E
-                      'MRDO': (205, 133, 63),  # peru	#CD853F
-                      'SSYWDO': (107, 142, 35),  # olive drab	#6B8E23
-                      'MSRDO': (106, 90, 205),  # slate blue	#6A5ACD
-                      'Bottom_Ash': (128, 128, 128),  # Gray	#808080
-                      'Fly_Ash': (0, 0, 0),  # black	#000000
-                      'Unreacted_Ash': (128, 128, 128),  # Gray	#808080
-                      'Separated_Organics': (50, 205, 50),  # lime green	#32CD32
-                      'Separated_Recyclables': (0, 128, 128),  # teal	#008080
-                      'Other_Residual': (139, 69, 19),  # saddle brown	#8B4513
-                      'RDF': (255, 0, 0)}  # Red	#FF0000
+        edge_color = {
+            "RWC": (160, 82, 45),  # sienna	#A0522D
+            "SSR": (0, 0, 255),  # blue	#0000FF
+            "DSR": (0, 0, 205),  # medium blue	#0000CD
+            "MSR": (65, 105, 225),  # royal blue	#4169E1
+            "LV": (0, 255, 0),  # lime	#00FF00
+            "SSYW": (0, 100, 0),  # dark green	#006400
+            "SSO": (0, 255, 127),  # spring green	#00FF7F
+            "SSO_HC": (128, 128, 0),  # olive #808000
+            "SSO_AnF": (127, 255, 0),  # chartreuse #7FFF00
+            "ORG": (46, 139, 87),  # sea green	#2E8B57
+            "DryRes": (222, 184, 135),  # burly wood	#DEB887
+            "REC": (0, 191, 255),  # deep sky blue	#00BFFF
+            "WetRes": (210, 105, 30),  # chocolate	#D2691E
+            "MRDO": (205, 133, 63),  # peru	#CD853F
+            "SSYWDO": (107, 142, 35),  # olive drab	#6B8E23
+            "MSRDO": (106, 90, 205),  # slate blue	#6A5ACD
+            "Bottom_Ash": (128, 128, 128),  # Gray	#808080
+            "Fly_Ash": (0, 0, 0),  # black	#000000
+            "Unreacted_Ash": (128, 128, 128),  # Gray	#808080
+            "Separated_Organics": (50, 205, 50),  # lime green	#32CD32
+            "Separated_Recyclables": (0, 128, 128),  # teal	#008080
+            "Other_Residual": (139, 69, 19),  # saddle brown	#8B4513
+            "RDF": (255, 0, 0),
+        }  # Red	#FF0000
         for i in self.project.CommonData.Reprocessing_Index:
             edge_color[i] = (0, 0, 139)  # dark blue	#00008B
 
         for x in product:
             key, frac = x
             source.append(label.index(key[0]))
             target.append(label.index(key[1]))
             label_link.append(key[2])
             # color.append('rgba({},{},{}, 0.8)'.format(*np.random.randint(256, size=3)))
-            color.append('rgba({}, {}, {}, 0.8)'.format(*edge_color[key[2]]))
+            color.append("rgba({}, {}, {}, 0.8)".format(*edge_color[key[2]]))
             mass = 0.0
-            for m in self.project.CommonData.Index + ['RDF']:
-                mass += self.get_mass_flow((key[0] + '_product', m + '_' + key[2]), 'WasteToProcess', params)
-                mass += self.get_mass_flow((key[0] + '_product', key[2]), 'WasteToProcess', params)
+            for m in self.project.CommonData.Index + ["RDF"]:
+                mass += self.get_mass_flow_from_supply_array(
+                    (key[0] + "_product", m + "_" + key[2]), "WasteToProcess", params
+                )
+                mass += self.get_mass_flow_from_supply_array(
+                    (key[0] + "_product", key[2]), "WasteToProcess", params
+                )
 
             value.append(np.round(mass * frac, 3))
 
-        print("""
+        print(
+            """
               # Sankey Mass flows
               label = {}
               source = {}
               target = {}
               label_link = {}
-              value = {}""".format(label, source, target, label_link, value))
+              value = {}""".format(
+                label, source, target, label_link, value
+            )
+        )
+
+        node = dict(
+            pad=20,
+            thickness=20,
+            line=dict(color="black", width=0.5),
+            label=label,
+            color="rgba({}, {}, {}, 0.8)".format(*(176, 196, 222)),
+        )  # light steel blue	#B0C4DE
 
-        node = dict(pad=20,
-                    thickness=20,
-                    line=dict(color="black", width=0.5),
-                    label=label,
-                    color='rgba({}, {}, {}, 0.8)'.format(*(176, 196, 222)))  # light steel blue	#B0C4DE
-
-        link = dict(source=source,
-                    target=target,
-                    value=value,
-                    label=label_link,
-                    color=color)
+        link = dict(source=source, target=target, value=value, label=label_link, color=color)
 
-        # The other good option for the valueformat is ".3f". Yes
+        # The other good option for the value format is ".3f". Yes
         score = self._objective_function(params) * 10**self.magnitude
         if score >= 1000 or score <= -1000:
             score = "{:,.0f}".format(score)
-        elif score <= 0.1 and score >= -0.1:
+        elif -0.1 <= score <= 0.1:
             score = "{:,.4f}".format(score)
-        elif score <= 1 and score >= -1:
+        elif score - 1 <= score <= 1:
             score = "{:,.3f}".format(score)
         else:
             score = "{:,.2f}".format(score)
 
-        layout = go.Layout(title_text="LCIA: " + str(self.method[0]) + f"= {score}",
-                           font_size=16,
-                           hoverlabel=dict(font_size=14))
-        data = go.Sankey(valueformat=".3s",
-                         valuesuffix="Mg",
-                         node=node,
-                         link=link)
+        layout = go.Layout(
+            title_text="LCIA: " + str(self.method[0]) + f"= {score}",
+            font_size=16,
+            hoverlabel=dict(font_size=14),
+        )
+        data = go.Sankey(valueformat=".3s", valuesuffix="Mg", node=node, link=link)
         fig = go.Figure(data=[data], layout=layout)
-        plot(fig, filename=fileName if fileName else 'plot.html', auto_open=show)
+        plot(fig, filename=fileName if fileName else "plot.html", auto_open=show)
 
         # Store data for ploting the sankey
         store_data = {}
-        store_data['title_text'] = "Impact " + str(self.method[0]) + f": {score}"
-        store_data['font_size'] = 16
-        store_data['hoverlabel'] = dict(font_size=14)
-        store_data['valueformat'] = ".3s"
-        store_data['valuesuffix'] = "Mg"
-        store_data['node'] = node
-        store_data['link'] = link
+        store_data["title_text"] = "Impact " + str(self.method[0]) + f": {score}"
+        store_data["font_size"] = 16
+        store_data["hoverlabel"] = dict(font_size=14)
+        store_data["valueformat"] = ".3s"
+        store_data["valuesuffix"] = "Mg"
+        store_data["node"] = node
+        store_data["link"] = link
 
-        filename = fileName.split('.')[0] + '.JSON' if fileName else 'Sankey_Data.JSON'
-        with open(filename, 'w') as outfile:
+        filename = fileName.split(".")[0] + ".JSON" if fileName else "Sankey_Data.JSON"
+        with open(filename, mode="w", encoding="utf-8") as outfile:
             json.dump(store_data, outfile, indent=4)
```

### Comparing `swolfpy-0.2.5/swolfpy/Parameters.py` & `swolfpy-1.0.0/swolfpy/Parameters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,187 +1,244 @@
-from stats_arrays import UncertaintyBase, MCRandomNumberGenerator
 import copy
+
 import graphviz
+from stats_arrays import MCRandomNumberGenerator, UncertaintyBase
 
 
 def approx_eq(x, y):
-    tol = 1.0E-6
+    tol = 1.0e-6
     return abs(x - y) <= max(abs(x), abs(y)) * tol
 
 
-class Parameters():
+class Parameters:
     def __init__(self, processes, CommonData):
-        self.param_uncertainty_dict = dict()
-        self.static_param_dict = dict()
-        self.params_dict = dict()
-
-        self.MC_param_name = list()  # name of parameters that include uncertainty
-        self.MC_param_base = list()  # uncertainty base for parameters that have uncertainty
-        self.MC_param_uncertainty_dict = dict()
+        self.param_uncertainty_dict = {}
+        self.static_param_dict = {}
+        self.params_dict = {}
+
+        self.MC_param_name = []  # name of parameters that include uncertainty
+        self.MC_param_base = []  # uncertainty base for parameters that have uncertainty
+        self.MC_param_uncertainty_dict = {}
 
         self.processes = processes
         self.nodes = list(self.processes.keys())
 
         # Color & shape for plotting the SWM Network
-        self.edge_color = {'RWC': 'black', 'SSR': 'blue', 'DSR': 'blue',
-                           'MSR': 'blue',
-                           'LV': 'green4', 'SSYW': 'green4', 'SSO': 'green4',
-                           'SSO_AnF': 'green4', 'SSO_HC': 'green4',
-                           'ORG': 'green4', 'DryRes': 'black',
-                           'REC': 'blue', 'WetRes': 'black',
-                           'MRDO': 'black', 'SSYWDO': 'green4', 'MSRDO': 'blue',
-                           'Bottom_Ash': 'gray', 'Fly_Ash': 'gray',
-                           'Unreacted_Ash': 'gray',
-                           'Separated_Organics': 'green4',
-                           'Separated_Recyclables': 'blue',
-                           'Other_Residual': 'black', 'RDF': 'red'}
+        self.edge_color = {
+            "RWC": "black",
+            "SSR": "blue",
+            "DSR": "blue",
+            "MSR": "blue",
+            "LV": "green4",
+            "SSYW": "green4",
+            "SSO": "green4",
+            "SSO_AnF": "green4",
+            "SSO_HC": "green4",
+            "ORG": "green4",
+            "DryRes": "black",
+            "REC": "blue",
+            "WetRes": "black",
+            "MRDO": "black",
+            "SSYWDO": "green4",
+            "MSRDO": "blue",
+            "Bottom_Ash": "gray",
+            "Fly_Ash": "gray",
+            "Unreacted_Ash": "gray",
+            "Separated_Organics": "green4",
+            "Separated_Recyclables": "blue",
+            "Other_Residual": "black",
+            "RDF": "red",
+        }
         for i in CommonData.Reprocessing_Index:
-            self.edge_color[i] = 'blue'
+            self.edge_color[i] = "blue"
         self.node_shape = {}
         self.node_color = {}
         for p in self.processes:
-            if self.processes[p]['model'].Process_Type != 'Collection':
-                self.node_shape[p] = 'rectangle'
-                self.node_color[p] = 'cyan3'
+            if self.processes[p]["model"].Process_Type != "Collection":
+                self.node_shape[p] = "rectangle"
+                self.node_color[p] = "cyan3"
             else:
-                self.node_shape[p] = 'oval'
-                self.node_color[p] = 'azure'
+                self.node_shape[p] = "oval"
+                self.node_color[p] = "azure"
 
-    def add_parameter(self, product, process_model_from, process_model_to, value, dynamic_param=True):
+    def add_parameter(
+        self, product, process_model_from, process_model_to, value, dynamic_param=True
+    ):
         """
-        Define new parameter
+        Define new parameter.
 
         :param product: Name of stream
         :type product: str
         :param process_model_from: Name of the process which is source of stream
         :type process_model_from: str
         :param process_model_to: Name of the process which is destination of stream
         :type process_model_to: str
         :param value: Value for the parameter
         :type value: float
-
         """
-        param_name = 'frac_of_' + product + '_from_' + process_model_from + '_to_' + process_model_to
+        param_name = (
+            "frac_of_" + product + "_from_" + process_model_from + "_to_" + process_model_to
+        )
         key = product + process_model_from
         if dynamic_param:
             if key not in self.param_uncertainty_dict.keys():
-                self.param_uncertainty_dict[key] = list()
-                self.param_uncertainty_dict[key].append([process_model_to, value, param_name, (process_model_from, process_model_to, product)])
+                self.param_uncertainty_dict[key] = []
+                self.param_uncertainty_dict[key].append(
+                    [
+                        process_model_to,
+                        value,
+                        param_name,
+                        (process_model_from, process_model_to, product),
+                    ]
+                )
             else:
-                self.param_uncertainty_dict[key].append([process_model_to, value, param_name, (process_model_from, process_model_to, product)])
+                self.param_uncertainty_dict[key].append(
+                    [
+                        process_model_to,
+                        value,
+                        param_name,
+                        (process_model_from, process_model_to, product),
+                    ]
+                )
         else:
             if key not in self.static_param_dict.keys():
-                self.static_param_dict[key] = list()
-                self.static_param_dict[key].append([process_model_to, value, param_name, (process_model_from, process_model_to, product)])
+                self.static_param_dict[key] = []
+                self.static_param_dict[key].append(
+                    [
+                        process_model_to,
+                        value,
+                        param_name,
+                        (process_model_from, process_model_to, product),
+                    ]
+                )
             else:
-                self.static_param_dict[key].append([process_model_to, value, param_name, (process_model_from, process_model_to, product)])
+                self.static_param_dict[key].append(
+                    [
+                        process_model_to,
+                        value,
+                        param_name,
+                        (process_model_from, process_model_to, product),
+                    ]
+                )
 
-    def SWM_network(self, view=True, show_vals=True, all_flow=True,
-                    filename='SWM_network'):
+    def SWM_network(self, view=True, show_vals=True, all_flow=True, filename="SWM_network"):
         """
-        To render the generated DOT source code, you also need to install `Graphviz <https://www.graphviz.org/download>`_.
+        To render the generated DOT source code, you also need to install `Graphviz.
 
-        ..note:: Make sure that the directory containing the dot executable is on your systems path.
+        <https://www.graphviz.org/download>`_.
 
+        ..note:: Make sure that the directory containing the dot executable is on your systems path.
         """
         # Initialize SWM network
-        self.network = graphviz.Digraph(name=filename, filename=filename + '.gv', format='png', engine='dot')
-        self.network.graph_attr['rankdir'] = 'LR'
+        self.network = graphviz.Digraph(
+            name=filename, filename=filename + ".gv", format="png", engine="dot"
+        )
+        self.network.graph_attr["rankdir"] = "LR"
         for x in self.nodes:
-            self.network.node(x, shape=self.node_shape[x], fillcolor=self.node_color[x], style='filled', width='1.2')
+            self.network.node(
+                x,
+                shape=self.node_shape[x],
+                fillcolor=self.node_color[x],
+                style="filled",
+                width="1.2",
+            )
 
         for param_dict in [self.param_uncertainty_dict.values(), self.static_param_dict.values()]:
             for y in param_dict:
                 for x in y:
                     if show_vals:
                         if all_flow:
                             self.add_edge(x[3][0], x[3][1], x[3][2], x[1])
                         elif not all_flow and x[1] > 0:
                             self.add_edge(x[3][0], x[3][1], x[3][2], x[1])
                         else:
                             pass
                     else:
                         self.add_edge(x[3][0], x[3][1], x[3][2])
         try:
-            self.network.render(filename + '.gv', view=view)
+            self.network.render(filename + ".gv", view=view)
         except Exception:
-            print("""
+            print(
+                """
             To render the generated DOT source code, you also need to install Graphviz (`Graphviz <https://www.graphviz.org/download>`_).\n
             Make sure that the directory containing the dot executable is on your systems’ path.
-            """)
+            """
+            )
 
     def add_edge(self, head, tail, name, value=None):
         if isinstance(value, (int, float)):
-            self.network.edge(head, tail, label=name + ' ({})'.format(value), color=self.edge_color[name])
+            self.network.edge(
+                head, tail, label=name + " ({})".format(value), color=self.edge_color[name]
+            )
         else:
             self.network.edge(head, tail, label=name, color=self.edge_color[name])
 
     def default_parameters_list(self):
         default_parameters_list = []
         for items in self.param_uncertainty_dict.values():
             for list_item in items:
-                default_parameters_list.append({'name': list_item[2], 'amount': 1 / len(items)})
-        return(default_parameters_list)
+                default_parameters_list.append({"name": list_item[2], "amount": 1 / len(items)})
+        return default_parameters_list
 
     def parameters_list(self):
         parameters_list = []
         for items in self.param_uncertainty_dict.values():
             for list_item in items:
-                parameters_list.append({'name': list_item[2], 'amount': list_item[1]})
-        return(parameters_list)
+                parameters_list.append({"name": list_item[2], "amount": list_item[1]})
+        return parameters_list
 
     def update_values(self, param_name, val, simulation=False):
         if simulation:
             param_uncertainty_dict = self.MC_param_uncertainty_dict
         else:
             param_uncertainty_dict = self.param_uncertainty_dict
 
         for items in param_uncertainty_dict.values():
             for list_item in items:
                 if list_item[2] == param_name:
                     list_item[1] = val
 
     def check_sum(self):
         """
-        Check that sum of the waste fractions (parameters) for each stream from one source to all available destinations is 1.
+        Check that sum of the waste fractions (parameters) for each stream from one source
+        to all available destinations is 1.
         """
         sum_ = 0
         flag = 1
         for item in self.param_uncertainty_dict.values():
             for list_item in item:
                 sum_ += list_item[1]
                 if list_item[1] < 0 or list_item[1] > 1:
-                    raise ValueError("Parameters should be in range(0,1), check: {}".format(list_item[2]))
+                    raise ValueError(
+                        "Parameters should be in range(0,1), check: {}".format(list_item[2])
+                    )
             if not approx_eq(sum_, 1):
                 msg = "Sum of the parameters in group is not 1: \n"
                 for i in item:
                     print("{}: {}".format(i[2], i[1]))
                     msg += "{}: {}\n".format(i[2], i[1])
                 raise ValueError(msg)
-                sum_ = 0
-                flag = 0
-                break
             sum_ = 0
         return flag
 
     def add_uncertainty(self, param_name, **kwargs):
         """
         add uncertainty to parameter.
 
         :param param_name: Name of the parameter (wastefraction) that has uncertainty
         :type param_name: str
         """
-        base_dict = dict()
-        base_dict['loc'] = kwargs.get('loc', None)
-        base_dict['scale'] = kwargs.get('scale', None)
-        base_dict['shape'] = kwargs.get('shape', None)
-        base_dict['minimum'] = kwargs.get('minimum', None)
-        base_dict['maximum'] = kwargs.get('maximum', None)
-        base_dict['negative'] = kwargs.get('negative', None)
-        base_dict['uncertainty_type'] = kwargs.get('uncertainty_type', None)
+        base_dict = {}
+        base_dict["loc"] = kwargs.get("loc", None)
+        base_dict["scale"] = kwargs.get("scale", None)
+        base_dict["shape"] = kwargs.get("shape", None)
+        base_dict["minimum"] = kwargs.get("minimum", None)
+        base_dict["maximum"] = kwargs.get("maximum", None)
+        base_dict["negative"] = kwargs.get("negative", None)
+        base_dict["uncertainty_type"] = kwargs.get("uncertainty_type", None)
 
         if param_name not in self.MC_param_name:
             self.MC_param_name.append(param_name)
             self.MC_param_base.append(base_dict)
         else:
             self.MC_param_base[self.MC_param_name.index(param_name)] = base_dict
 
@@ -191,73 +248,78 @@
         """
         self.vars = UncertaintyBase.from_dicts(*self.MC_param_base)
         self.rand = MCRandomNumberGenerator(self.vars, seed=seed)
         self.MC_param_uncertainty_dict = copy.deepcopy(self.param_uncertainty_dict)
 
     def MC_calc(self):
         """
-        Generates new values for uncertain parameters
+        Generates new values for uncertain parameters.
         """
         new_vals = self.rand.next()
         for i in range(len(new_vals)):
             self.update_values(self.MC_param_name[i], new_vals[i], simulation=True)
 
         # Normalizing the generated random numbers
         self.normalize()
 
-        param_exchanges_dict = dict()
-        param_keys = list()
-        param_vals = list()
+        param_exchanges_dict = {}
+        param_keys = []
+        param_vals = []
         for key in self.params_dict.keys():
             param_keys.append(key)
             param_vals.append(self.MC_get_param_val(key))
             for item in self.params_dict[key]:
                 param_exchanges_dict[item] = self.MC_get_param_val(key)
-        return(param_exchanges_dict, tuple(zip(param_keys, param_vals)))
+        return (param_exchanges_dict, tuple(zip(param_keys, param_vals)))
 
     def normalize(self):
         """
         Normalize the parameters after updating the valuse by monte carlo.
         """
         for item in self.MC_param_uncertainty_dict.values():
             sum_ = 0
             for list_item in item:
                 if list_item[1] < 0:
-                    raise ValueError("Parameters should be positive, check the uncertainty base for param: {}".format(list_item[2]))
+                    raise ValueError(
+                        "Parameters should be positive, check the uncertainty base for param: {}".format(
+                            list_item[2]
+                        )
+                    )
                 sum_ += list_item[1]
 
             for list_item in item:
                 if sum_ != 0:
                     list_item[1] = list_item[1] / sum_
                 else:
                     list_item[1] = 1 / len(item)
 
     def MC_get_param_val(self, param_name):
         """
-        Report the uncertain value created for parameter
+        Report the uncertain value created for parameter.
 
         :param param_name: Name of the parameter (wastefraction) that has uncertainty
         :type param_name: str
-        :return: Value fo the parameter
+        :return: Value of the parameter
         :rtype: float
         """
         for item in self.MC_param_uncertainty_dict.values():
             for list_item in item:
                 if list_item[2] == param_name:
                     return list_item[1]
+        return None
 
     def Param_exchanges(self, new_vals):
         """
-        Returns the parameters exchanges with the new values
+        Returns the parameters exchanges with the new values.
         """
-        param_exchanges_dict = dict()
+        param_exchanges_dict = {}
         self.MC_param_uncertainty_dict = copy.deepcopy(self.param_uncertainty_dict)
         param_list = list(self.params_dict.keys())
 
         # update parameter
         for i in range(len(new_vals)):
             self.update_values(param_list[i], new_vals[i], simulation=True)
         # update parameters exchanges dict
         for key in param_list:
             for item in self.params_dict[key]:
                 param_exchanges_dict[item] = self.MC_get_param_val(key)
-        return(param_exchanges_dict)
+        return param_exchanges_dict
```

### Comparing `swolfpy-0.2.5/swolfpy/ProcessDB.py` & `swolfpy-1.0.0/swolfpy/ProcessDB.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Mar 13 21:42:51 2019
-
-@author: msmsa
-"""
 import numpy as np
 from brightway2 import Database
 
 
-class ProcessDB():
+class ProcessDB:
     def __init__(self, process_name, waste_treatment, CommonData, process_types, Distance=None):
         self.Report = {}
         self.P_Name = process_name
-        self.P_Pr_Name = self.P_Name + '_product'
+        self.P_Pr_Name = self.P_Name + "_product"
         self.Distance = Distance
         self.CommonData = CommonData
         self._process_types = process_types
 
         self.waste_treatment = waste_treatment
 
         # Databases
@@ -31,23 +26,28 @@
 
     @staticmethod
     def init_DB(DB_name, waste_flows):
         db_data = {}
         for x in waste_flows:
             # add activity to database
             db_data[(DB_name, x)] = {
-                'name': DB_name + "_" + x,
-                'reference product': DB_name + "_" + x,
-                'unit': 'Mg/year',
-                'exchanges': []}
+                "name": DB_name + "_" + x,
+                "reference product": DB_name + "_" + x,
+                "unit": "Mg/year",
+                "exchanges": [],
+            }
 
-        print("""
+        print(
+            """
               ####
               ++++++ Initializing the {}
-              """.format(DB_name))
+              """.format(
+                DB_name
+            )
+        )
 
         db = Database(DB_name)
         db.write(db_data)
 
     def Write_DB(self, waste_flows, parameters, Process_Type):
         """
         .. _Write_DB:
@@ -56,282 +56,437 @@
         create_static_parameters = True
         self.db_data = {}
         self.db_Pr_data = {}
         self.parameters = []  # List of dictionaries ({'name':Formula ,'amount':0})
         self.list_of_params = []  # List of parameters name
         self.list_of_static_params = []
         self.act_in_group = set()
-        self.params_dict = dict()  # Dictionary that has set() include the key (input,act) for all the exchanges with parameters.
+        self.params_dict = (
+            dict()
+        )  # Dictionary that has set() include the key (input,act) for all the exchanges with parameters.
         self.uncertain_parameters = parameters
 
-        for x in waste_flows:    # x is waste fraction
+        for x in waste_flows:  # x is waste fraction
             # add activity to database
             self.db_data[(self.P_Name, x)] = {
-                'name': self.P_Name + "_" + x,
-                'reference product': self.P_Name + "_" + x,
-                'unit': 'Mg/year',
-                'exchanges': []}
-            if Process_Type == 'Collection':
-                self.db_data[(self.P_Name, x)]['unit'] = '{} Mg/year'.format(np.round(sum(self.Report["Waste"][x].values()), decimals=2))
+                "name": self.P_Name + "_" + x,
+                "reference product": self.P_Name + "_" + x,
+                "unit": "Mg/year",
+                "exchanges": [],
+            }
+            if Process_Type == "Collection":
+                self.db_data[(self.P_Name, x)]["unit"] = "{} Mg/year".format(
+                    np.round(sum(self.Report["Waste"][x].values()), decimals=2)
+                )
             # Reference flow
-            ex = self.exchange(Input=(self.P_Name, x),
-                               Type='production',
-                               Unit=self.db_data[(self.P_Name, x)]['unit'],
-                               Amount=1)
-            self.db_data[(self.P_Name, x)]['exchanges'].append(ex)
+            ex = self.exchange(
+                Input=(self.P_Name, x),
+                Type="production",
+                Unit=self.db_data[(self.P_Name, x)]["unit"],
+                Amount=1,
+            )
+            self.db_data[(self.P_Name, x)]["exchanges"].append(ex)
 
-            if Process_Type == 'Transfer_Station':
+            if Process_Type == "Transfer_Station":
                 xx = ProcessDB._helper_wasteflow_name(x)
             else:
                 xx = x
 
             for key in self.Report["Waste"][x]:
-                ex = self.exchange((self.P_Pr_Name, xx + '_' + key), 'technosphere', 'Mg/year', self.Report["Waste"][x][key])
-                self.db_data[(self.P_Name, x)]['exchanges'].append(ex)
+                ex = self.exchange(
+                    (self.P_Pr_Name, xx + "_" + key),
+                    "technosphere",
+                    "Mg/year",
+                    self.Report["Waste"][x][key],
+                )
+                self.db_data[(self.P_Name, x)]["exchanges"].append(ex)
 
                 # add activity to Waste_database
-                self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)] = {
-                    'name': self.P_Pr_Name + "_" + xx + '_' + key,
-                    'reference product': self.P_Pr_Name + "_" + xx + '_' + key,
-                    'unit': 'Mg/year',
-                    'exchanges': []}
+                self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)] = {
+                    "name": self.P_Pr_Name + "_" + xx + "_" + key,
+                    "reference product": self.P_Pr_Name + "_" + xx + "_" + key,
+                    "unit": "Mg/year",
+                    "exchanges": [],
+                }
                 # Reference flow
-                ex = self.exchange(Input=(self.P_Pr_Name, xx + '_' + key),
-                                   Type='production',
-                                   Unit=self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['unit'],
-                                   Amount=1)
-                self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex)
-                self.act_in_group.add((self.P_Pr_Name, xx + '_' + key))
+                ex = self.exchange(
+                    Input=(self.P_Pr_Name, xx + "_" + key),
+                    Type="production",
+                    Unit=self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["unit"],
+                    Amount=1,
+                )
+                self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(ex)
+                self.act_in_group.add((self.P_Pr_Name, xx + "_" + key))
 
                 # Streams that are not the same with their source.
-                if key in ['Bottom_Ash', 'Fly_Ash', 'RDF'] + self.CommonData.Reprocessing_Index:
+                if key in ["Bottom_Ash", "Fly_Ash", "RDF"] + self.CommonData.Reprocessing_Index:
                     # finding the destination
                     for p in self.waste_treatment[key]:
                         # adding exchange to waste processing
                         if len(self.waste_treatment[key]) > 1 or not create_static_parameters:
-                            Formula = "frac_of_" + key + '_from_' + self.P_Name + '_to_' + p
+                            Formula = "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
                         else:
                             Formula = None
-                            if "frac_of_" + key + '_from_' + self.P_Name + '_to_' + p not in self.list_of_static_params:
-                                self.list_of_static_params.append("frac_of_" + key + '_from_' + self.P_Name + '_to_' + p)
-                                self.uncertain_parameters.add_parameter(key, self.P_Name, p, 1, dynamic_param=False)
-
-                        ex = self.exchange((p, key), 'technosphere', 'Mg/year', 0 if Formula else 1, Formula=Formula,
-                                           Act=(self.P_Pr_Name, xx + '_' + key), product=key)
-                        self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex)
-
-                        # addin exchange for transportation between the process models
-                        ex_trnp = self.exchange((self.P_Pr_Name, self.P_Name + '_' + 'to' + '_' + p), 'technosphere', 'Mg/year',
-                                                0 if Formula else 1, Formula=Formula,
-                                                Act=(self.P_Pr_Name, xx + '_' + key), product=key)
-                        self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex_trnp)
+                            if (
+                                "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
+                                not in self.list_of_static_params
+                            ):
+                                self.list_of_static_params.append(
+                                    "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
+                                )
+                                self.uncertain_parameters.add_parameter(
+                                    key, self.P_Name, p, 1, dynamic_param=False
+                                )
+
+                        ex = self.exchange(
+                            (p, key),
+                            "technosphere",
+                            "Mg/year",
+                            0 if Formula else 1,
+                            Formula=Formula,
+                            Act=(self.P_Pr_Name, xx + "_" + key),
+                            product=key,
+                        )
+                        self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(ex)
+
+                        # adding exchange for transportation between the process models
+                        ex_trnp = self.exchange(
+                            (self.P_Pr_Name, self.P_Name + "_" + "to" + "_" + p),
+                            "technosphere",
+                            "Mg/year",
+                            0 if Formula else 1,
+                            Formula=Formula,
+                            Act=(self.P_Pr_Name, xx + "_" + key),
+                            product=key,
+                        )
+                        self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(
+                            ex_trnp
+                        )
 
                 # Streams that are same with the source.
-                elif key in ['Separated_Organics', 'Other_Residual', 'Separated_Recyclables', 'Unreacted_Ash']:
+                elif key in [
+                    "Separated_Organics",
+                    "Other_Residual",
+                    "Separated_Recyclables",
+                    "Unreacted_Ash",
+                ]:
                     # finding the destination
                     for p in self.waste_treatment[key]:
                         # adding exchange to waste processing
                         if len(self.waste_treatment[key]) > 1 or not create_static_parameters:
-                            Formula = "frac_of_" + key + '_from_' + self.P_Name + '_to_' + p
+                            Formula = "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
                         else:
                             Formula = None
-                            if "frac_of_" + key + '_from_' + self.P_Name + '_to_' + p not in self.list_of_static_params:
-                                self.list_of_static_params.append("frac_of_" + key + '_from_' + self.P_Name + '_to_' + p)
-                                self.uncertain_parameters.add_parameter(key, self.P_Name, p, 1, dynamic_param=False)
+                            if (
+                                "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
+                                not in self.list_of_static_params
+                            ):
+                                self.list_of_static_params.append(
+                                    "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
+                                )
+                                self.uncertain_parameters.add_parameter(
+                                    key, self.P_Name, p, 1, dynamic_param=False
+                                )
 
                         # adding exchange to waste processing
-                        ex = self.exchange((p, xx), 'technosphere', 'Mg/year', 0 if Formula else 1, Formula=Formula,
-                                           Act=(self.P_Pr_Name, xx + '_' + key), product=key)
-                        self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex)
-
-                        # addin exchange for transportation between the process models
-                        ex_trnp = self.exchange((self.P_Pr_Name, self.P_Name + '_' + 'to' + '_' + p), 'technosphere', 'Mg/year',
-                                                0 if Formula else 1, Formula=Formula,
-                                                Act=(self.P_Pr_Name, xx + '_' + key), product=key)
-                        self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex_trnp)
+                        ex = self.exchange(
+                            (p, xx),
+                            "technosphere",
+                            "Mg/year",
+                            0 if Formula else 1,
+                            Formula=Formula,
+                            Act=(self.P_Pr_Name, xx + "_" + key),
+                            product=key,
+                        )
+                        self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(ex)
+
+                        # adding exchange for transportation between the process models
+                        ex_trnp = self.exchange(
+                            (self.P_Pr_Name, self.P_Name + "_" + "to" + "_" + p),
+                            "technosphere",
+                            "Mg/year",
+                            0 if Formula else 1,
+                            Formula=Formula,
+                            Act=(self.P_Pr_Name, xx + "_" + key),
+                            product=key,
+                        )
+                        self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(
+                            ex_trnp
+                        )
 
                 ### Collection streams.
                 # Transportation between the collection and treatment processes are calculate inside collection model.
                 elif key in self.CommonData.Collection_Index:
                     # finding the destination
                     for p in self.waste_treatment[key]:
                         # adding exchange to waste processing
                         if len(self.waste_treatment[key]) > 1 or not create_static_parameters:
-                            Formula = "frac_of_" + key + '_from_' + self.P_Name + '_to_' + p
+                            Formula = "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
                         else:
                             Formula = None
-                            if "frac_of_" + key + '_from_' + self.P_Name + '_to_' + p not in self.list_of_static_params:
-                                self.list_of_static_params.append("frac_of_" + key + '_from_' + self.P_Name + '_to_' + p)
-                                self.uncertain_parameters.add_parameter(key, self.P_Name, p, 1, dynamic_param=False)
-                        if self._process_types[p] == 'Transfer_Station':
-                            ex = self.exchange(Input=(p, key + '_' + x),
-                                               Type='technosphere',
-                                               Unit='Mg/year',
-                                               Amount=0 if Formula else 1,
-                                               Formula=Formula,
-                                               Act=(self.P_Pr_Name, xx + '_' + key),
-                                               product=key)
+                            if (
+                                "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
+                                not in self.list_of_static_params
+                            ):
+                                self.list_of_static_params.append(
+                                    "frac_of_" + key + "_from_" + self.P_Name + "_to_" + p
+                                )
+                                self.uncertain_parameters.add_parameter(
+                                    key, self.P_Name, p, 1, dynamic_param=False
+                                )
+                        if self._process_types[p] == "Transfer_Station":
+                            ex = self.exchange(
+                                Input=(p, key + "_" + x),
+                                Type="technosphere",
+                                Unit="Mg/year",
+                                Amount=0 if Formula else 1,
+                                Formula=Formula,
+                                Act=(self.P_Pr_Name, xx + "_" + key),
+                                product=key,
+                            )
                         else:
-                            ex = self.exchange(Input=(p, x),
-                                               Type='technosphere',
-                                               Unit='Mg/year',
-                                               Amount=0 if Formula else 1,
-                                               Formula=Formula,
-                                               Act=(self.P_Pr_Name, xx + '_' + key),
-                                               product=key)
-
-                        self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex)
-
-                        # addin exchange for transportation between the collection sector and treatment processs
-                        if p in self.Report['LCI'][key].keys():
-                            ex_trnp = self.exchange((self.P_Pr_Name, key + '_' + 'to' + '_' + p), 'technosphere', 'Mg/year',
-                                                    0 if Formula else 1, Formula=Formula,
-                                                    Act=(self.P_Pr_Name, x + '_' + key), product=key)
-                            self.db_Pr_data[(self.P_Pr_Name, xx + '_' + key)]['exchanges'].append(ex_trnp)
+                            ex = self.exchange(
+                                Input=(p, x),
+                                Type="technosphere",
+                                Unit="Mg/year",
+                                Amount=0 if Formula else 1,
+                                Formula=Formula,
+                                Act=(self.P_Pr_Name, xx + "_" + key),
+                                product=key,
+                            )
+
+                        self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(ex)
+
+                        # adding exchange for transportation between the collection sector and treatment process
+                        if p in self.Report["LCI"][key].keys():
+                            ex_trnp = self.exchange(
+                                (self.P_Pr_Name, key + "_" + "to" + "_" + p),
+                                "technosphere",
+                                "Mg/year",
+                                0 if Formula else 1,
+                                Formula=Formula,
+                                Act=(self.P_Pr_Name, x + "_" + key),
+                                product=key,
+                            )
+                            self.db_Pr_data[(self.P_Pr_Name, xx + "_" + key)]["exchanges"].append(
+                                ex_trnp
+                            )
                         else:
-                            raise ValueError('Inconsistent treatment processes in model and collection')
+                            raise ValueError(
+                                "Inconsistent treatment processes in model and collection"
+                            )
                 else:
-                    raise Exception(f'Unknown waste proudct! {key} is not defined in PrcessDB class')
+                    raise Exception(
+                        f"Unknown waste product! {key} is not defined in PrcessDB class"
+                    )
 
-            ### Adding the technosphere exchnages to activities
+            ### Adding the technosphere exchanges to activities
             for key in self.Report["Technosphere"][x]:
-                # if self.Report["Technosphere"][x][key] != 0:
-                if True:
-                    ex = self.exchange(key, 'technosphere', 'Mg/year', self.Report["Technosphere"][x][key])
-                    self.db_data[(self.P_Name, x)]['exchanges'].append(ex)
+                ex = self.exchange(
+                    key, "technosphere", "Mg/year", self.Report["Technosphere"][x][key]
+                )
+                self.db_data[(self.P_Name, x)]["exchanges"].append(ex)
 
-            ### Adding the biosphere exchnages
+            ### Adding the biosphere exchanges
             for key in self.Report["Biosphere"][x]:
-                # if self.Report["Biosphere"][x][key] != 0:
-                if True:
-                    ex = self.exchange(key, 'biosphere', 'kg', self.Report["Biosphere"][x][key])
-                    self.db_data[(self.P_Name, x)]['exchanges'].append(ex)
+                ex = self.exchange(key, "biosphere", "kg", self.Report["Biosphere"][x][key])
+                self.db_data[(self.P_Name, x)]["exchanges"].append(ex)
 
-            if Process_Type == 'Collection':
+            if Process_Type == "Collection":
                 ### Adding activity for transport between the collection and treatment processes
                 self._add_transport_from_collection()
             else:
                 ### Adding activity for transport between the treatment processes
                 self._add_transport_between_processes()
 
         ### writing the databases
-        self._writre_DB_from_dict()
+        self._write_DB_from_dict()
 
-        return(self.parameters, self.act_in_group)
+        return (self.parameters, self.act_in_group)
 
     def _add_transport_from_collection(self):
         """
-        Adding activity for transport between the collection and treatment processes
+        Adding activity for transport between the collection and treatment processes.
         """
         for y in self.Report["LCI"].keys():
             for m in self.Report["LCI"][y].keys():
-                self.db_Pr_data[(self.P_Pr_Name, y + '_' + 'to' + '_' + m)] = {
-                    'name': 'LCI' + '_' + y + '_to' + '_' + m,
-                    'reference product': 'LCI' + '_' + y + '_to' + '_' + m,
-                    'unit': 'Mg/year',
-                    'exchanges': []}
+                self.db_Pr_data[(self.P_Pr_Name, y + "_" + "to" + "_" + m)] = {
+                    "name": "LCI" + "_" + y + "_to" + "_" + m,
+                    "reference product": "LCI" + "_" + y + "_to" + "_" + m,
+                    "unit": "Mg/year",
+                    "exchanges": [],
+                }
                 # Reference flow
-                ex = self.exchange(Input=(self.P_Pr_Name, y + '_' + 'to' + '_' + m),
-                                   Type='production',
-                                   Unit=self.db_Pr_data[(self.P_Pr_Name, y + '_' + 'to' + '_' + m)]['unit'],
-                                   Amount=1)
-                self.db_Pr_data[(self.P_Pr_Name, y + '_' + 'to' + '_' + m)]['exchanges'].append(ex)
+                ex = self.exchange(
+                    Input=(self.P_Pr_Name, y + "_" + "to" + "_" + m),
+                    Type="production",
+                    Unit=self.db_Pr_data[(self.P_Pr_Name, y + "_" + "to" + "_" + m)]["unit"],
+                    Amount=1,
+                )
+                self.db_Pr_data[(self.P_Pr_Name, y + "_" + "to" + "_" + m)]["exchanges"].append(ex)
                 ### Adding exchage to transport activity between the collection and treatment processes
                 for n in self.Report["LCI"][y][m].keys():
-                    ex = self.exchange(n, 'technosphere' if 'biosphere3' not in n else 'biosphere', '_', self.Report["LCI"][y][m][n])
-                    self.db_Pr_data[(self.P_Pr_Name, y + '_' + 'to' + '_' + m)]['exchanges'].append(ex)
+                    ex = self.exchange(
+                        n,
+                        "technosphere" if "biosphere3" not in n else "biosphere",
+                        "_",
+                        self.Report["LCI"][y][m][n],
+                    )
+                    self.db_Pr_data[(self.P_Pr_Name, y + "_" + "to" + "_" + m)]["exchanges"].append(
+                        ex
+                    )
 
     def _add_transport_between_processes(self):
         """
-        Adding activity for transport between the treatment processes
+        Adding activity for transport between the treatment processes.
         """
-        # check whether transportation is needed or not (if no waste is proudced, then no transportation is needed)
+        # check whether transportation is needed or not (if no waste is produced, then no transportation is needed)
         if len(self.db_Pr_data) > 0:
             for p, q in self.Distance.Distance.keys():
                 if p == self.P_Name and p != q:
-                    self.db_Pr_data[(self.P_Pr_Name, p + '_' + 'to' + '_' + q)] = {
-                        'name': 'LCI' + '_' + p + '_' + 'to' + '_' + q,
-                        'reference product': 'LCI' + '_' + p + '_' + 'to' + '_' + q,
-                        'unit': 'Mg/year',
-                        'exchanges': []}
+                    self.db_Pr_data[(self.P_Pr_Name, p + "_" + "to" + "_" + q)] = {
+                        "name": "LCI" + "_" + p + "_" + "to" + "_" + q,
+                        "reference product": "LCI" + "_" + p + "_" + "to" + "_" + q,
+                        "unit": "Mg/year",
+                        "exchanges": [],
+                    }
                     # Reference flow
-                    ex = self.exchange(Input=(self.P_Pr_Name, p + '_' + 'to' + '_' + q),
-                                       Type='production',
-                                       Unit=self.db_Pr_data[(self.P_Pr_Name, p + '_' + 'to' + '_' + q)]['unit'],
-                                       Amount=1)
-                    self.db_Pr_data[(self.P_Pr_Name, p + '_' + 'to' + '_' + q)]['exchanges'].append(ex)
+                    ex = self.exchange(
+                        Input=(self.P_Pr_Name, p + "_" + "to" + "_" + q),
+                        Type="production",
+                        Unit=self.db_Pr_data[(self.P_Pr_Name, p + "_" + "to" + "_" + q)]["unit"],
+                        Amount=1,
+                    )
+                    self.db_Pr_data[(self.P_Pr_Name, p + "_" + "to" + "_" + q)]["exchanges"].append(
+                        ex
+                    )
                     ### Adding exchage to transport activity between the treatment processes
                     for mode in self.Distance.Distance[(p, q)].keys():
-                        if mode == 'Heavy Duty Truck':
-                            ex = self.exchange(('Technosphere', 'Internal_Process_Transportation_Heavy_Duty_Diesel_Truck'),
-                                               'technosphere', 'Mg/year', 1000 * self.Distance.Distance[(p, q)][mode], Formula=None,
-                                               Act=None, product=None)  # unit converion Mg to kg
-                        elif mode == 'Medium Duty Truck':
-                            ex = self.exchange(('Technosphere', 'Internal_Process_Transportation_Medium_Duty_Diesel_Truck'),
-                                               'technosphere', 'Mg/year', 1000 * self.Distance.Distance[(p, q)][mode], Formula=None,
-                                               Act=None, product=None)  # unit converion Mg to kg
-                        elif mode == 'Rail':
-                            ex = self.exchange(('Technosphere', 'Internal_Process_Transportation_Rail'),
-                                               'technosphere', 'Mg/year', 1000 * self.Distance.Distance[(p, q)][mode], Formula=None,
-                                               Act=None, product=None)  # unit converion Mg to kg
-                        elif mode == 'Barge':
-                            ex = self.exchange(('Technosphere', 'Internal_Process_Transportation_Barge'),
-                                               'technosphere', 'Mg/year', 1000 * self.Distance.Distance[(p, q)][mode], Formula=None,
-                                               Act=None, product=None)  # unit converion Mg to kg
-                        elif mode == 'Cargo Ship':
-                            ex = self.exchange(('Technosphere', 'Internal_Process_Transportation_Cargo_Ship'),
-                                               'technosphere', 'Mg/year', 1000 * self.Distance.Distance[(p, q)][mode], Formula=None,
-                                               Act=None, product=None)  # unit converion Mg to kg
+                        if mode == "Heavy Duty Truck":
+                            ex = self.exchange(
+                                (
+                                    "Technosphere",
+                                    "Internal_Process_Transportation_Heavy_Duty_Diesel_Truck",
+                                ),
+                                "technosphere",
+                                "Mg/year",
+                                1000 * self.Distance.Distance[(p, q)][mode],
+                                Formula=None,
+                                Act=None,
+                                product=None,
+                            )  # unit conversion Mg to kg
+                        elif mode == "Medium Duty Truck":
+                            ex = self.exchange(
+                                (
+                                    "Technosphere",
+                                    "Internal_Process_Transportation_Medium_Duty_Diesel_Truck",
+                                ),
+                                "technosphere",
+                                "Mg/year",
+                                1000 * self.Distance.Distance[(p, q)][mode],
+                                Formula=None,
+                                Act=None,
+                                product=None,
+                            )  # unit conversion Mg to kg
+                        elif mode == "Rail":
+                            ex = self.exchange(
+                                ("Technosphere", "Internal_Process_Transportation_Rail"),
+                                "technosphere",
+                                "Mg/year",
+                                1000 * self.Distance.Distance[(p, q)][mode],
+                                Formula=None,
+                                Act=None,
+                                product=None,
+                            )  # unit conversion Mg to kg
+                        elif mode == "Barge":
+                            ex = self.exchange(
+                                ("Technosphere", "Internal_Process_Transportation_Barge"),
+                                "technosphere",
+                                "Mg/year",
+                                1000 * self.Distance.Distance[(p, q)][mode],
+                                Formula=None,
+                                Act=None,
+                                product=None,
+                            )  # unit conversion Mg to kg
+                        elif mode == "Cargo Ship":
+                            ex = self.exchange(
+                                ("Technosphere", "Internal_Process_Transportation_Cargo_Ship"),
+                                "technosphere",
+                                "Mg/year",
+                                1000 * self.Distance.Distance[(p, q)][mode],
+                                Formula=None,
+                                Act=None,
+                                product=None,
+                            )  # unit conversion Mg to kg
                         else:
-                            raise ValueError(f'Transport mode {mode} is incorrect!')
-                        self.db_Pr_data[(self.P_Pr_Name, p + '_' + 'to' + '_' + q)]['exchanges'].append(ex)
+                            raise ValueError(f"Transport mode {mode} is incorrect!")
+                        self.db_Pr_data[(self.P_Pr_Name, p + "_" + "to" + "_" + q)][
+                            "exchanges"
+                        ].append(ex)
 
-    def _writre_DB_from_dict(self):
+    def _write_DB_from_dict(self):
         if len(self.db_Pr_data) > 0:
-            print("""
+            print(
+                """
                   ####
                   ++++++ Writing the {}
-                  """.format(self.P_Pr_Name))
+                  """.format(
+                    self.P_Pr_Name
+                )
+            )
 
             self.database_Product.write(self.db_Pr_data)
 
-        print("""
+        print(
+            """
               ####
               ++++++ Writing the {}
-              """.format(self.P_Name))
+              """.format(
+                self.P_Name
+            )
+        )
         db = Database(self.P_Name)
         db.write(self.db_data)
         self.uncertain_parameters.params_dict.update(self.params_dict)
 
     def exchange(self, Input, Type, Unit, Amount, Formula=None, Act=None, product=None):
         """
-        return exchange in a dictionary format
+        Return exchange in a dictionary format.
         """
         exchange = {}
-        exchange['amount'] = Amount
-        exchange['input'] = Input
-        exchange['type'] = Type
-        exchange['unit'] = Unit
+        exchange["amount"] = Amount
+        exchange["input"] = Input
+        exchange["type"] = Type
+        exchange["unit"] = Unit
 
         if Formula:
-            exchange['formula'] = Formula
+            exchange["formula"] = Formula
             if Act is None or product is None:
-                raise TypeError('swolfpy error: Act and product are not defined for formula(parameter): {}'.format(Formula))
+                raise TypeError(
+                    "swolfpy error: Act and product are not defined for formula(parameter): {}".format(
+                        Formula
+                    )
+                )
             if Formula not in self.list_of_params:
-                self.parameters.append({'name': Formula, 'amount': 0})
+                self.parameters.append({"name": Formula, "amount": 0})
                 self.list_of_params.append(Formula)
                 self.params_dict[Formula] = set()
                 self.params_dict[Formula].add((Input, Act))
                 self.uncertain_parameters.add_parameter(product, self.P_Name, Input[0], 0)
             else:
                 self.params_dict[Formula].add((Input, Act))
 
-        return(exchange)
+        return exchange
 
     @staticmethod
-    def _helper_wasteflow_name(name):
-        if 'DryRes' == name[0:6] or 'WetRes' == name[0:6]:
-            return(name[7:])
-        elif 'ORG' == name[0:3] or 'REC' == name[0:3]:
-            return(name[4:])
+    def _helper_wasteflow_name(name: str) -> str:
+        """
+        Removes the collection index and returns the waste fraction index.
+        """
+        if name[0:6] in ["DryRes", "WetRes"]:
+            return name[7:]
+        elif name[0:4] in ["SSYW"]:
+            return name[5:]
+        elif name[0:3] in ["ORG", "REC", "SSO", "SSR", "RWC"]:
+            return name[4:]
         else:
-            return(None)
+            return None
```

### Comparing `swolfpy-0.2.5/swolfpy/Project.py` & `swolfpy-1.0.0/swolfpy/Project.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed May 29 12:13:23 2019
+import pickle
 
-@author: msmsa
-"""
-from brightway2 import projects, Database, parameters, LCA, get_activity, calculation_setups, MultiLCA, Method
-from bw2data.parameters import ActivityParameter
-from .ProcessDB import ProcessDB
-from bw2analyzer import ContributionAnalysis
-from .Parameters import Parameters
-from .Technosphere import Technosphere
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from brightway2 import (
+    LCA,
+    Database,
+    Method,
+    MultiLCA,
+    calculation_setups,
+    get_activity,
+    parameters,
+    projects,
+)
+from bw2analyzer import ContributionAnalysis
+from bw2data.parameters import ActivityParameter
+
+from .Parameters import Parameters
+from .ProcessDB import ProcessDB
+from .Technosphere import Technosphere
 
 
-class Project():
+class Project:
     """
-    Project class creates a new project in Birghtway2.
+    Project class creates a new project in Brightway2.
 
     :param project_name: Name for the project
     :type project_name: str
 
     :param CommonData: CommonData object
-    :type CommonData: class: `swolfpy.ProcessMoldes.CommonData`
+    :type CommonData: class: `swolfpy_inputdata.CommonData`
 
     :param Treatment_processes: Dictionary for treatment processes include their input type and model.
     :type Treatment_processes: dict
 
     :param Distance: Distance object.
     :type Distance: class: `swolfpy.Distance.Distance`
 
@@ -79,37 +86,47 @@
     >>> demo.parameters.default_parameters_list()
         [{'name': 'frac_of_Bottom_Ash_from_WTE_to_LF', 'amount': 1.0},
          {'name': 'frac_of_Fly_Ash_from_WTE_to_LF', 'amount': 1.0},
          {'name': 'frac_of_RWC_from_SF_COl_to_LF', 'amount': 0.5},
          {'name': 'frac_of_RWC_from_SF_COl_to_WTE', 'amount': 0.5}]
     >>> demo.update_parameters(demo.parameters.default_parameters_list())
     """
-    def __init__(self, project_name, CommonData, Treatment_processes, Distance,
-                 Collection_processes=None, Technosphere_obj=None, signal=None):
+
+    def __init__(
+        self,
+        project_name,
+        CommonData,
+        Treatment_processes,
+        Distance,
+        Collection_processes=None,
+        Technosphere_obj=None,
+    ):
         if Technosphere_obj:
             self.Technosphere = Technosphere_obj
             self.project_name = self.Technosphere.project_name
             if self.project_name != project_name:
-                raise Warning('The project name should be same with the name selected for creating the technosphere')
+                raise Warning(
+                    "The project name should be same with the name selected for creating the technosphere"
+                )
         else:
             self.project_name = project_name
             self.Technosphere = Technosphere(self.project_name)
 
         self.CommonData = CommonData
         self.Treatment_processes = Treatment_processes
         self.Collection_processes = Collection_processes
         self.Distance = Distance
         if self.Collection_processes:
             for j in self.Collection_processes.keys():
                 self.Treatment_processes[j] = self.Collection_processes[j]
 
-        self.processes = [x for x in self.Treatment_processes.keys()]
+        self.processes = list(self.Treatment_processes.keys())
         self.processTypes = {}
         for p in self.processes:
-            self.processTypes[p] = self.Treatment_processes[p]['model'].Process_Type
+            self.processTypes[p] = self.Treatment_processes[p]["model"].Process_Type
 
         projects.set_current(self.project_name)
 
         self.waste_treatment = {}
         for i in self.CommonData.All_Waste_Pr_Index:
             self.waste_treatment[i] = self._find_destination(i)
 
@@ -118,64 +135,68 @@
         # Creating swolfpy parameter class
         self.parameters = Parameters(self.Treatment_processes, self.CommonData)
 
         self._progress = 0
 
     def _find_destination(self, product):
         """
-        Find the processes that can treat the `product`. This function check the ``input_type`` in the ``Treatment_processes`` dictionary.
+        Find the processes that can treat the `product`. This function check the
+        ``input_type`` in the ``Treatment_processes`` dictionary.
 
         :param product: Waste product e.g., RWC, Fly_Ash, Separated_Organics, Other_Residual
         :type product: str
 
         :return: A list of the discovered processes in the ``Treatment_processes`` dictionary that can treat the `product`
         :rtype: list
-
         """
         destination = []
         for P in self.Treatment_processes:
-            if product in self.Treatment_processes[P]['input_type']:
+            if product in self.Treatment_processes[P]["input_type"]:
                 destination.append(P)
-        return(destination)
+        return destination
 
     def init_project(self, signal=None):
         """
-        Calls the Create_Technosphere_ method to initilize a project.\n
-        This function create an empty database for each process as a placeholder, so swolfpy
-        can browse these databases in the next step (writing project) and
-        create exchanges between them.
+        Calls the Create_Technosphere_ method to initialize a project.\n This function
+        create an empty database for each process as a placeholder, so swolfpy can browse
+        these databases in the next step (writing project) and create exchanges between
+        them.
         """
         if signal:
             self._progress += 5
             signal.emit(self._progress)
 
         self.Technosphere.Create_Technosphere()
 
         if signal:
             self._progress += 10
             signal.emit(self._progress)
 
         # Initializing the databases
         for DB_name in self.Treatment_processes:
-            if self.Treatment_processes[DB_name]['model'].Process_Type in ['Treatment', 'Collection']:
+            if self.Treatment_processes[DB_name]["model"].Process_Type in [
+                "Treatment",
+                "Collection",
+            ]:
                 ProcessDB.init_DB(DB_name, self.CommonData.Index)
-            elif self.Treatment_processes[DB_name]['model'].Process_Type == 'Reprocessing':
+            elif self.Treatment_processes[DB_name]["model"].Process_Type == "Reprocessing":
                 ProcessDB.init_DB(DB_name, self.CommonData.Reprocessing_Index)
-            elif self.Treatment_processes[DB_name]['model'].Process_Type == 'RDF':
-                ProcessDB.init_DB(DB_name, ['RDF'])
+            elif self.Treatment_processes[DB_name]["model"].Process_Type == "RDF":
+                ProcessDB.init_DB(DB_name, ["RDF"])
 
         Database("waste").register()
         self.waste_BD = Database("waste")
 
         if signal:
             self._progress += 5
             signal.emit(self._progress)
 
     def write_project(self, signal=None):
-        """ Call the import_database_ for all the process models.
+        """
+        Call the import_database_ for all the process models.
         """
         self.parameters_dict = {}
         self.parameters_list = []
         self.act_include_param = {}
         for j in self.Treatment_processes:
             (P, G) = self._import_database(j)
             self.parameters_dict[j] = P
@@ -192,246 +213,281 @@
 
         Instantiate the ProcessDB_ class for the process model and gets the LCI report from it; then translates
         the report for Brightway2 and populates the databases by Write_DB_ method.
 
         :return: Returns a tuple (parameters,act_in_group)
         :rtype: tuple
         """
-        self.process_model[name] = ProcessDB(name, self.waste_treatment, self.CommonData, self.processTypes, self.Distance)
-        self.Treatment_processes[name]['model'].calc()
-        self.process_model[name].Report = self.Treatment_processes[name]['model'].report()
-
-        if self.Treatment_processes[name]['model'].Process_Type in ['Treatment', 'Collection']:
-            (P, G) = self.process_model[name].Write_DB(waste_flows=self.CommonData.Index,
-                                                       parameters=self.parameters,
-                                                       Process_Type=self.Treatment_processes[name]['model'].Process_Type)
-
-        elif self.Treatment_processes[name]['model'].Process_Type == 'Reprocessing':
-            (P, G) = self.process_model[name].Write_DB(waste_flows=self.CommonData.Reprocessing_Index,
-                                                       parameters=self.parameters,
-                                                       Process_Type=self.Treatment_processes[name]['model'].Process_Type)
-
-        elif self.Treatment_processes[name]['model'].Process_Type == 'Transfer_Station':
-            (P, G) = self.process_model[name].Write_DB(waste_flows=self.Treatment_processes[name]['model']._Extened_Index,
-                                                       parameters=self.parameters,
-                                                       Process_Type=self.Treatment_processes[name]['model'].Process_Type)
-        elif self.Treatment_processes[name]['model'].Process_Type == 'RDF':
-            (P, G) = self.process_model[name].Write_DB(waste_flows=['RDF'],
-                                                       parameters=self.parameters,
-                                                       Process_Type=self.Treatment_processes[name]['model'].Process_Type)
-        return((P, G))
+        self.process_model[name] = ProcessDB(
+            name, self.waste_treatment, self.CommonData, self.processTypes, self.Distance
+        )
+        self.Treatment_processes[name]["model"].calc()
+        self.process_model[name].Report = self.Treatment_processes[name]["model"].report()
+
+        if self.Treatment_processes[name]["model"].Process_Type in ["Treatment", "Collection"]:
+            (P, G) = self.process_model[name].Write_DB(
+                waste_flows=self.CommonData.Index,
+                parameters=self.parameters,
+                Process_Type=self.Treatment_processes[name]["model"].Process_Type,
+            )
+
+        elif self.Treatment_processes[name]["model"].Process_Type == "Reprocessing":
+            (P, G) = self.process_model[name].Write_DB(
+                waste_flows=self.CommonData.Reprocessing_Index,
+                parameters=self.parameters,
+                Process_Type=self.Treatment_processes[name]["model"].Process_Type,
+            )
+
+        elif self.Treatment_processes[name]["model"].Process_Type == "Transfer_Station":
+            (P, G) = self.process_model[name].Write_DB(
+                waste_flows=self.Treatment_processes[name]["model"]._Extened_Index,
+                parameters=self.parameters,
+                Process_Type=self.Treatment_processes[name]["model"].Process_Type,
+            )
+        elif self.Treatment_processes[name]["model"].Process_Type == "RDF":
+            (P, G) = self.process_model[name].Write_DB(
+                waste_flows=["RDF"],
+                parameters=self.parameters,
+                Process_Type=self.Treatment_processes[name]["model"].Process_Type,
+            )
+        return (P, G)
 
     def report_parameters(self):
         """
         Reports the `parameters` in dictionary format.
 
         :return: dictionary include the processes as key and parameters in each process as values.
         :rtype: dict
-
         """
-        return(self.parameters_dict)
+        return self.parameters_dict
 
     def report_parameters_list(self):
         """
         Reports the `parameters` in list format.
 
         :return: List of `parameters` (waste fractions) in the project
         :rtype: list
-
         """
-        return(self.parameters_list)
+        return self.parameters_list
 
     def group_exchanges(self, signal=None):
         """
-        Create a group for the `parameters` in each database and add the exchanges that include these `parameters`
-        to this group. As a results, model know to update the values in those exchanges when the `parameter` is updated
+        Create a group for the `parameters` in each database and add the exchanges that
+        include these `parameters` to this group.
+
+        As a results, model know to update the values in those exchanges when the
+        `parameter` is updated
         """
         for j in self.processes:
-            print("""
+            print(
+                """
                   Grouping the exchanges with parameters in Database {}
-                  """.format(j))
+                  """.format(
+                    j
+                )
+            )
             if len(self.act_include_param[j]) > 0:
                 for r in self.act_include_param[j]:
                     parameters.add_exchanges_to_group(j, r)
 
             if signal:
                 self._progress += 70 / len(self.processes)
                 signal.emit(self._progress)
 
         if signal:
             signal.emit(100)
 
     def update_parameters(self, new_param_data, signal=None):
         """
-        Updates the `parameters` and their related exchanges based on the `new_param_data`.
+        Updates the `parameters` and their related exchanges based on the
+        `new_param_data`.
 
         :param new_param_data: List of `parameters` (waste fractions) in the project with new values
         :type new_param_data: list
 
         .. note:: `parameters` are waste fractions which show what fraction of waste from one source
                     go to different destinations, so sum of parameters from each source should be 1. (0<= `parameters` <=1)
-
         """
 
         progress = 0
         if signal:
             signal.emit(progress)
 
         for j in new_param_data:
             for k in self.parameters_list:
-                if k['name'] == j['name']:
-                    self.parameters.update_values(j['name'], j['amount'])
+                if k["name"] == j["name"]:
+                    self.parameters.update_values(j["name"], j["amount"])
 
         if self.parameters.check_sum():
             for j in new_param_data:
                 for k in self.parameters_list:
-                    if k['name'] == j['name']:
-                        k['amount'] = j['amount']
+                    if k["name"] == j["name"]:
+                        k["amount"] = j["amount"]
             parameters.new_project_parameters(new_param_data)
             for j in self.processes:
                 if len(self.act_include_param[j]) > 0:
                     ActivityParameter.recalculate_exchanges(j)
 
                 progress += 100 / len(self.processes)
                 if signal:
                     signal.emit(progress)
 
         else:
             for j in new_param_data:
                 for k in self.parameters_list:
-                    if k['name'] == j['name']:
-                        self.parameters.update_values(k['name'], k['amount'])
+                    if k["name"] == j["name"]:
+                        self.parameters.update_values(k["name"], k["amount"])
 
     def create_scenario(self, input_dict, scenario_name):
-        """Creates a new scenario (activity).
         """
-        input_dict = input_dict
+        Creates a new scenario (activity).
+        """
         # Calculate Unit
         mass = 0
         for P in input_dict:
             for y in input_dict[P]:
                 if input_dict[P][y] != 0:
-                    unit_i = get_activity((P, y)).as_dict()['unit'].split(sep=' ')
+                    unit_i = get_activity((P, y)).as_dict()["unit"].split(sep=" ")
                     if len(unit_i) > 1:
                         mass += float(unit_i[0]) * input_dict[P][y]
-                    if unit_i[0] == 'Mg/year':
+                    if unit_i[0] == "Mg/year":
                         mass += 1 * input_dict[P][y]
-        new_act = self.waste_BD.new_activity(code=scenario_name, name=scenario_name, type="process",
-                                             unit='{} Mg/year'.format(np.round(mass, decimals=2)),
-                                             **{'reference product': scenario_name})
+        new_act = self.waste_BD.new_activity(
+            code=scenario_name,
+            name=scenario_name,
+            type="process",
+            unit="{} Mg/year".format(np.round(mass, decimals=2)),
+            **{"reference product": scenario_name},
+        )
         new_act.save()
         new_act.new_exchange(input=new_act, amount=1, type="production").save()
         for P in input_dict:
             for y in input_dict[P]:
                 if input_dict[P][y] != 0:
-                    new_act.new_exchange(input=(P, y), amount=input_dict[P][y], type="technosphere").save()
+                    new_act.new_exchange(
+                        input=(P, y), amount=input_dict[P][y], type="technosphere"
+                    ).save()
 
     @staticmethod
     def setup_LCA(name, functional_units, impact_methods):
         """
         Perform LCA by instantiating the ``bw2calc.multi_lca`` class from Brightway2.
+
         ``bw2calc.multi_lca`` is a wrapper class for performing LCA calculations with many
         functional units and LCIA methods.
         """
         if len(functional_units) > 0 and len(impact_methods) > 0:
-            calculation_setups[name] = {'inv': functional_units, 'ia': impact_methods}
+            calculation_setups[name] = {"inv": functional_units, "ia": impact_methods}
             MultiLca = MultiLCA(name)
             index = [str(x) for x in list(MultiLca.all.keys())]
             columns = [str(x) for x in impact_methods]
-            results = pd.DataFrame(MultiLca.results,
-                                   columns=columns,
-                                   index=index)
-            return(results)
+            results = pd.DataFrame(MultiLca.results, columns=columns, index=index)
+            return results
         else:
-            raise ValueError('Check the in inputs')
+            raise ValueError("Check the in inputs")
 
     @staticmethod
-    def contribution_analysis(functional_unit, impact_method, limit, limit_type='number', target='emissions',
-                              figsize=(6, 4), font_scale=1):
+    def contribution_analysis(
+        functional_unit,
+        impact_method,
+        limit,
+        limit_type="number",
+        target="emissions",
+        figsize=(6, 4),
+        font_scale=1,
+    ):
         """
-        Perform LCA by instantiating the ``bw2calc.lca.LCA`` class from ``Brightway2`` and then
-        perform contribution analysis by ``bw2analyzer.ContributionAnalysis`` class.
+        Perform LCA by instantiating the ``bw2calc.lca.LCA`` class from ``Brightway2`` and
+        then perform contribution analysis by ``bw2analyzer.ContributionAnalysis`` class.
         Check the following functions in ``bw2analyzer`` for more info:
 
         * ``bw2analyzer.ContributionAnalysis.annotated_top_processes``
         * ``bw2analyzer.ContributionAnalysis.annotated_top_emissions``
-
         """
         lca = LCA(functional_unit, impact_method)
         lca.lci()
         lca.lcia()
         impacts = []
         amounts = []
         activities = []
         flow_unit = []
         compartments = []
         f = font_scale * 14
 
-        if target == 'activities':
-            data = ContributionAnalysis().annotated_top_processes(lca, limit=50, limit_type='number')
+        if target == "activities":
+            data = ContributionAnalysis().annotated_top_processes(
+                lca, limit=50, limit_type="number"
+            )
         else:
-            data = ContributionAnalysis().annotated_top_emissions(lca, limit=50, limit_type='number')
+            data = ContributionAnalysis().annotated_top_emissions(
+                lca, limit=50, limit_type="number"
+            )
         for impact, amount, act in data:
             impacts.append(impact)
             amounts.append(amount)
-            flow_unit.append(act.as_dict()['unit'])
-            if target == 'activities':
-                activities.append(act.as_dict()['name'].replace('_', ' '))
+            flow_unit.append(act.as_dict()["unit"])
+            if target == "activities":
+                activities.append(act.as_dict()["name"].replace("_", " "))
             else:
-                activities.append(act.as_dict()['name'])
-                compartments.append(act.as_dict()['categories'])
+                activities.append(act.as_dict()["name"])
+                compartments.append(act.as_dict()["categories"])
 
-        if target == 'activities':
-            top_df = pd.DataFrame(columns=['Activity', 'Flow', 'Flow Unit', 'Contribution', 'Unit'])
-            top_df['Activity'] = activities
+        if target == "activities":
+            top_df = pd.DataFrame(columns=["Activity", "Flow", "Flow Unit", "Contribution", "Unit"])
+            top_df["Activity"] = activities
         else:
-            top_df = pd.DataFrame(columns=['Emission', 'Compartment', 'Flow', 'Flow Unit', 'Contribution', 'Unit'])
-            top_df['Emission'] = activities
-            top_df['Compartment'] = compartments
-
-        top_df['Flow'] = amounts
-        top_df['Flow Unit'] = flow_unit
-        top_df['Contribution'] = impacts
-        top_df['Unit'] = Method(lca.method).metadata['unit']
+            top_df = pd.DataFrame(
+                columns=["Emission", "Compartment", "Flow", "Flow Unit", "Contribution", "Unit"]
+            )
+            top_df["Emission"] = activities
+            top_df["Compartment"] = compartments
+
+        top_df["Flow"] = amounts
+        top_df["Flow Unit"] = flow_unit
+        top_df["Contribution"] = impacts
+        top_df["Unit"] = Method(lca.method).metadata["unit"]
 
-        if limit_type == 'number':
+        if limit_type == "number":
             DF = top_df.loc[0:limit, :]
         else:
-            for i, j in enumerate(top_df['Contribution']):
+            for i, j in enumerate(top_df["Contribution"]):
                 if abs(j) <= abs((limit * lca.score)):
                     break
                 DF = top_df.loc[0:i, :]
 
-        plot_DF = pd.DataFrame(data=[[x for x in DF['Contribution']]],
-                               columns=DF.iloc[:, 0].values,
-                               index=list(functional_unit.keys()))
-
-        legend = ['Net']
-        if target == 'emissions':
-            for x, y in DF[['Emission', 'Compartment']].values:
-                y = str(y).replace("'", '')
-                legend.append('{}\n{}'.format(x, y))
+        plot_DF = pd.DataFrame(
+            data=[list(DF["Contribution"])],
+            columns=DF.iloc[:, 0].values,
+            index=list(functional_unit.keys()),
+        )
+
+        legend = ["Net"]
+        if target == "emissions":
+            for x, y in DF[["Emission", "Compartment"]].values:
+                y = str(y).replace("'", "")
+                legend.append("{}\n{}".format(x, y))
         else:
-            for x in DF['Activity'].values:
+            for x in DF["Activity"].values:
                 if len(x) > 20:
-                    x = x[0:15] + x[15:].replace(' ', '\n', 1)
+                    x = x[0:15] + x[15:].replace(" ", "\n", 1)
                 legend.append(x)
 
         fig, ax = plt.subplots(figsize=figsize)
-        plot_DF.plot(kind='bar', stacked=True, ax=ax, alpha=0.9)
-        ax.set_title('Contribution to {}'.format(str(lca.method).replace("'", '')), fontsize=f)
-        ax.scatter(0, lca.score, s=50, marker='D', edgecolor='w', facecolor='k')
-        ax.legend(legend, fontsize=f, bbox_to_anchor=(1, 0, .2, 1), loc=2)
-        ax.tick_params(axis='both', which='major', labelsize=f, rotation='auto')
-        ax.tick_params(axis='both', which='minor', labelsize=f, rotation='auto')
-        ax.set_ylabel(Method(lca.method).metadata['unit'], fontsize=f)
-        return(DF, (fig, ax))
+        plot_DF.plot(kind="bar", stacked=True, ax=ax, alpha=0.9)
+        ax.set_title("Contribution to {}".format(str(lca.method).replace("'", "")), fontsize=f)
+        ax.scatter(0, lca.score, s=50, marker="D", edgecolor="w", facecolor="k")
+        ax.legend(legend, fontsize=f, bbox_to_anchor=(1, 0, 0.2, 1), loc=2)
+        ax.tick_params(axis="both", which="major", labelsize=f, rotation="auto")
+        ax.tick_params(axis="both", which="minor", labelsize=f, rotation="auto")
+        ax.set_ylabel(Method(lca.method).metadata["unit"], fontsize=f)
+        return (DF, (fig, ax))
 
     def save(self, filename):
         """
-        Dumps the ``Project`` class to pickle file. User can load the pickle and use it later.
+        Dumps the ``Project`` class to pickle file. User can load the pickle and use it
+        later.
 
         :param filename:
         :type filename: str
         """
-        import pickle
-        pickle.dump(self, open(filename, "wb"))
+        with open(filename, "wb") as f:
+            pickle.dump(self, f)
```

### Comparing `swolfpy-0.2.5/swolfpy/Technosphere.py` & `swolfpy-1.0.0/swolfpy/Technosphere.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,172 +1,231 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Wed Apr  8 11:18:40 2020
+import warnings
 
-@author: msmsa
-"""
-from brightway2 import Database, projects, bw2setup, databases
 import bw2io
 import pandas as pd
+from brightway2 import Database, bw2setup, databases, projects
+from swolfpy_inputdata import Technosphere_Input
+
 from .Required_keys import biosphere_keys
 from .swolfpy_method import import_methods
-from swolfpy_inputdata import Technosphere_Input
-import warnings
 
 
 class Technosphere:
     """
     :param project_name: Name for the project
     :type project_name: str
-    :param LCI_path: Patht to the technosphere LIC csv file
+    :param LCI_path: Path to the technosphere LIC csv file
     :type LCI_path: str
-    :param LCI_Reference_path: Path to the csv file for the technosphere refrences
+    :param LCI_Reference_path: Path to the csv file for the technosphere references
     :type LCI_Reference_path: str
     :param Ecospold2_Path: Path to the user defined technosphere LCI with ecospold2 format.
     :type Ecospold2_Path: str
     """
+
     def __init__(self, project_name, LCI_path=None, LCI_Reference_path=None, Ecospold2_Path=None):
         self.project_name = project_name
-        self.technosphere_db_name = 'Technosphere'
-        self.user_tech_name = 'User_Technosphere'
+        self.technosphere_db_name = "Technosphere"
+        self.user_tech_name = "User_Technosphere"
 
         self.InputData = Technosphere_Input(LCI_path, LCI_Reference_path, Ecospold2_Path)
         self.LCI_swolfpy_data = self.InputData.LCI_swolfpy_data
         self.LCI_reference = self.InputData.LCI_reference
         self.Ecospold2_Path = self.InputData.Ecospold2_Path
 
     def Create_Technosphere(self):
         """
         .. _Create_Technosphere:
 
         Initialize a `project` in Brightway2 by calling the ``bw2setup()`` function which creates the `biosphere3`
-        database and imports the impact assesment methods. \n
-        It also addes 7 new biosphere flows for cost calculations swoflpy. \n
+        database and imports the impact assessment methods. \n
+        It also adds 7 new biosphere flows for cost calculations swolfpy. \n
         New impact methods are imported by calling the  ``import_methods()`` from swolfpy_method_ module. \n
 
         Note: If the `project` already exists, it will delete all the databases except 'biosphere3'. `Technosphere` database is written from the
         `SWOLF_AccountMode_LCI DATA.csv` in the `Data` folder unless user select new file with it's `path`.
         """
         projects.set_current(self.project_name)
         bw2setup()
-        db = Database('biosphere3')
-        if len(db.search('capital cost')) == 0:
-            db.new_activity(code='Capital_Cost', name="Capital Cost", unit='USD', categories=('economic', ),
-                            type='economic', location='US').save()
-            db.new_activity(code='Operational_Cost', name="Operational Cost", unit='USD', categories=('economic', ),
-                            type='economic', location='US').save()
-            db.new_activity(code='Utility_Cost', name="Utility Cost", unit='USD', categories=('economic', ),
-                            type='economic', location='US').save()
-            db.new_activity(code='Fuel_Cost', name="Fuel Cost", unit='USD', categories=('economic', ),
-                            type='economic', location='US').save()
-            db.new_activity(code='Electricity_Cost', name="Electricity Cost", unit='USD', categories=('economic', ),
-                            type='economic', location='US').save()
-            db.new_activity(code='Transportation_Cost', name="Transportation Cost", unit='USD', categories=('economic', ),
-                            type='economic', location='US').save()
-            db.new_activity(code='Material_Cost', name="Material Cost", unit='USD', categories=('economic',),
-                            type='economic', location='US').save()
+        db = Database("biosphere3")
+        if len(db.search("capital cost")) == 0:
+            db.new_activity(
+                code="Capital_Cost",
+                name="Capital Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
+            db.new_activity(
+                code="Operational_Cost",
+                name="Operational Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
+            db.new_activity(
+                code="Utility_Cost",
+                name="Utility Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
+            db.new_activity(
+                code="Fuel_Cost",
+                name="Fuel Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
+            db.new_activity(
+                code="Electricity_Cost",
+                name="Electricity Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
+            db.new_activity(
+                code="Transportation_Cost",
+                name="Transportation Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
+            db.new_activity(
+                code="Material_Cost",
+                name="Material Cost",
+                unit="USD",
+                categories=("economic",),
+                type="economic",
+                location="US",
+            ).save()
 
         # adding swolf methods
         import_methods()
 
         # Deleting the old (expired) databases (if exist)
-        xx = [x for x in databases]
+        xx = list(databases)
         for x in xx:
-            if x not in ['biosphere3']:
+            if x not in ["biosphere3"]:
                 del databases[x]
-        if self.LCI_reference['Reference_activity_id'].count() > 0:
-            self._Write_user_technospher()
+        if self.LCI_reference["Reference_activity_id"].count() > 0:
+            self._Write_user_technosphere()
             db = Database(self.user_tech_name)
             self.user_tech_keys = {}
             for x in db:
-                self.user_tech_keys[x.as_dict()['activity']] = x.key
+                self.user_tech_keys[x.as_dict()["activity"]] = x.key
         self._write_technosphere()
 
-    def _Write_user_technospher(self):
+    def _Write_user_technosphere(self):
         """
-        Creates the user technosphere database from Ecospold2 files. \n
-        Interface with Brightway2: Calls the ``bw2io.importers.SingleOutputEcospold2Importer`` function.
+        Creates the user technosphere database from Ecospold2 files.
+
+        \n Interface with Brightway2: Calls the
+        ``bw2io.importers.SingleOutputEcospold2Importer`` function.
         """
-        self.user_tech = bw2io.importers.SingleOutputEcospold2Importer(dirpath=self.Ecospold2_Path, db_name=self.user_tech_name)
+        self.user_tech = bw2io.importers.SingleOutputEcospold2Importer(
+            dirpath=self.Ecospold2_Path, db_name=self.user_tech_name
+        )
         self.user_tech.apply_strategies()
         stats = self.user_tech.statistics()
         if stats[2] > 0:
-            warnings.warn('There is {} unlink flows in the user defined technosphere (ecospold files). Make sure you are using the LCI ecosplod'
-                          .format(stats[2]))
-            print('\nUnique unlinked exchanges:\n')
+            warnings.warn(
+                "There is {} unlink flows in the user defined technosphere (ecospold files). Make sure you are using the LCI ecospold".format(
+                    stats[2]
+                )
+            )
+            print("\nUnique unlinked exchanges:\n")
             for x in self.user_tech.unlinked:
-                print(x['type'], x['name'], x['amount'])
+                print(x["type"], x["name"], x["amount"])
 
-            print('\nAdd unlinked flows to biosphere database:\n')
+            print("\nAdd unlinked flows to biosphere database:\n")
             self.user_tech.add_unlinked_flows_to_biosphere_database()
 
-        print("""
+        print(
+            """
                 ####
                 ++++++  Writing the {}
-                """.format(self.user_tech_name))
+                """.format(
+                self.user_tech_name
+            )
+        )
         self.user_tech.write_database()
 
     def _write_technosphere(self):
         """
-        Creates the swolfpy technosphere database.\n
+        Creates the swolfpy technosphere database.\n.
         """
         self.technosphere_data = {}
         # activities
-        names = [x for x in self.LCI_swolfpy_data.columns][3:]
+        names = list(self.LCI_swolfpy_data.columns)[3:]
         for x in names:
             # add activity to database
             self.technosphere_data[(self.technosphere_db_name, x)] = {
-                'name': x,
-                'reference product': x,
-                'unit': (lambda y: 'NA' if pd.isnull(y) else y)(self.LCI_swolfpy_data[x][0]),
-                'exchanges': []}
+                "name": x,
+                "reference product": x,
+                "unit": "NA"
+                if pd.isnull(self.LCI_swolfpy_data[x][0])
+                else self.LCI_swolfpy_data[x][0],
+                "exchanges": [],
+            }
             # Reference flow
             ex = {}
-            ex['amount'] = 1
-            ex['input'] = (self.technosphere_db_name, x)
-            ex['type'] = 'production'
-            ex['unit'] = self.technosphere_data[(self.technosphere_db_name, x)]['unit']
-            self.technosphere_data[(self.technosphere_db_name, x)]['exchanges'].append(ex)
+            ex["amount"] = 1
+            ex["input"] = (self.technosphere_db_name, x)
+            ex["type"] = "production"
+            ex["unit"] = self.technosphere_data[(self.technosphere_db_name, x)]["unit"]
+            self.technosphere_data[(self.technosphere_db_name, x)]["exchanges"].append(ex)
 
-            if pd.isnull(self.LCI_reference['Reference_activity_id'][x]):
+            if pd.isnull(self.LCI_reference["Reference_activity_id"][x]):
                 i = 0
                 for val in self.LCI_swolfpy_data[x][2:]:
                     if float(self._check_nan(val)) != 0:
                         ex = {}  # add exchange to activities
-                        ex['amount'] = float(self._check_nan(val))
-                        ex['input'] = biosphere_keys[i][0]
-                        ex['type'] = 'biosphere'
-                        ex['unit'] = 'kg'
-                        self.technosphere_data[(self.technosphere_db_name, x)]['exchanges'].append(ex)
+                        ex["amount"] = float(self._check_nan(val))
+                        ex["input"] = biosphere_keys[i][0]
+                        ex["type"] = "biosphere"
+                        ex["unit"] = "kg"
+                        self.technosphere_data[(self.technosphere_db_name, x)]["exchanges"].append(
+                            ex
+                        )
                     i += 1
             else:
                 ex = {}  # add exchange to activities
-                ex['amount'] = 1
-                ex['input'] = self.user_tech_keys[self.LCI_reference['Reference_activity_id'][x]]
-                ex['type'] = 'technosphere'
-                ex['unit'] = self.LCI_reference['Unit'][x]
-                self.technosphere_data[(self.technosphere_db_name, x)]['exchanges'].append(ex)
+                ex["amount"] = 1
+                ex["input"] = self.user_tech_keys[self.LCI_reference["Reference_activity_id"][x]]
+                ex["type"] = "technosphere"
+                ex["unit"] = self.LCI_reference["Unit"][x]
+                self.technosphere_data[(self.technosphere_db_name, x)]["exchanges"].append(ex)
 
-            if not pd.isnull(self.LCI_reference['Cost_key'][x]):  # adding the cost to technosphere
+            if not pd.isnull(self.LCI_reference["Cost_key"][x]):  # adding the cost to technosphere
                 ex = {}  # add exchange to activities
-                ex['amount'] = self._check_nan(self.LCI_reference['Cost'][x])
-                ex['input'] = ('biosphere3', self.LCI_reference['Cost_key'][x])
-                ex['type'] = 'biosphere'
-                ex['unit'] = self.LCI_reference['Cost_Unit'][x]
-                self.technosphere_data[(self.technosphere_db_name, x)]['exchanges'].append(ex)
+                ex["amount"] = self._check_nan(self.LCI_reference["Cost"][x])
+                ex["input"] = ("biosphere3", self.LCI_reference["Cost_key"][x])
+                ex["type"] = "biosphere"
+                ex["unit"] = self.LCI_reference["Cost_Unit"][x]
+                self.technosphere_data[(self.technosphere_db_name, x)]["exchanges"].append(ex)
 
-        print("""
+        print(
+            """
                 ####
                 ++++++  Writing the {}
-                """.format(self.technosphere_db_name))
+                """.format(
+                self.technosphere_db_name
+            )
+        )
         self.technosphere_db = Database(self.technosphere_db_name)
         self.technosphere_db.write(self.technosphere_data)
         # replace zeros when there is no data ("nan")
 
     def _check_nan(self, x):
         """
         Check the `x` and return 0 if `x` is `nan`.
-
         """
         if str(x) == "nan":
             return 0
         return x
```

### Comparing `swolfpy-0.2.5/swolfpy/__init__.py` & `swolfpy-1.0.0/swolfpy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # -*- coding: utf-8 -*-
 """
 @author: msardar2
 
 Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
 """
-from .Technosphere import Technosphere
-from .Project import Project
-from .swolfpy_method import import_methods
-from .Optimization import Optimization
-from .Monte_Carlo import Monte_Carlo
-from .UI.PySWOLF_run import MyQtApp
-from PySide2 import QtWidgets
 import sys
 import warnings
 
+from PySide2 import QtWidgets
+
+from .Monte_Carlo import Monte_Carlo
+from .Optimization import Optimization
+from .Project import Project
+from .swolfpy_method import import_methods
+from .Technosphere import Technosphere
+from .UI.PySWOLF_run import MyQtApp
 
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
 
-__all__ = ['Technosphere',
-           'Project',
-           'import_methods',
-           'Optimization',
-           'Monte_Carlo',
-           'MyQtApp',
-           'swolfpy']
+__all__ = [
+    "Technosphere",
+    "Project",
+    "import_methods",
+    "Optimization",
+    "Monte_Carlo",
+    "MyQtApp",
+    "swolfpy",
+]
 
-__version__ = '0.2.5'
+__version__ = "1.0.0"
 
 
-class swolfpy():
+class swolfpy:
     def __init__(self):
         if not QtWidgets.QApplication.instance():
             self.app = QtWidgets.QApplication(sys.argv)
         else:
             self.app = QtWidgets.QApplication.instance()
 
         self.qt_app = MyQtApp()
```

### Comparing `swolfpy-0.2.5/swolfpy/swolfpy_method.py` & `swolfpy-1.0.0/swolfpy/swolfpy_method.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Thu Apr  4 14:41:00 2019
+import os
 
-@author: msardar2
-"""
 import pandas as pd
-from brightway2 import methods, Method
-import os
-import swolfpy_inputdata.Data.LCIA_Methods as m
+import swolfpy_inputdata.data.lcia_methods as m
+from brightway2 import Method, methods
 
 
 def import_methods(path_to_methods=None):
     """
     Imports the user defined LCIA methods from the csv files in the path.
     """
     if not path_to_methods:
         path_to_methods = m.__path__[0]
     files = os.listdir(path_to_methods)
     for f in files:
-        if '.csv' in f:
-            df = pd.read_csv(path_to_methods + '/' + f)
+        if ".csv" in f:
+            df = pd.read_csv(path_to_methods + "/" + f)
             CF = []
             for i in df.index:
-                CF.append((eval(df['key'][i]), df['value'][i]))
+                CF.append((eval(df["key"][i]), df["value"][i]))
             name = eval(f[:-4])
-            Method(name).register(**{'unit': df['unit'][0],
-                                     'num_cfs': len(df),
-                                     'filename': f,
-                                     'path_source_file': path_to_methods})
+            Method(name).register(
+                **{
+                    "unit": df["unit"][0],
+                    "num_cfs": len(df),
+                    "filename": f,
+                    "path_source_file": path_to_methods,
+                }
+            )
             Method(name).write(CF)
     methods.flush()
```

### Comparing `swolfpy-0.2.5/swolfpy/utils.py` & `swolfpy-1.0.0/swolfpy/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # -*- coding: utf-8 -*-
-"""
-Created on Mon Jun 29 16:07:33 2020
-
-@author: msmsa
-"""
 import json
-import plotly.graph_objects as go
-from plotly.offline import plot
+
 import brightway2 as bw2
 import pandas as pd
+import plotly.graph_objects as go
+from plotly.offline import plot
 
 
 def plot_sankey(data_json, fileName=None):
     """
     Plot sankey diagram from the JSON file created by SwolfPy.
     """
-    with open(data_json) as json_file:
+    with open(data_json, mode="r", encoding="utf-8") as json_file:
         data = json.load(json_file)
 
-    layout = go.Layout(title_text=data['title_text'],
-                       font_size=data['font_size'],
-                       title_font={'color': 'black', 'family': "Times New Roman"},
-                       hoverlabel=data['hoverlabel'])
-    data_ = go.Sankey(valueformat=data['valueformat'],
-                      valuesuffix=data['valuesuffix'],
-                      node=data['node'],
-                      link=data['link'])
+    layout = go.Layout(
+        title_text=data["title_text"],
+        font_size=data["font_size"],
+        title_font={"color": "black", "family": "Times New Roman"},
+        hoverlabel=data["hoverlabel"],
+    )
+    data_ = go.Sankey(
+        valueformat=data["valueformat"],
+        valuesuffix=data["valuesuffix"],
+        node=data["node"],
+        link=data["link"],
+    )
     fig = go.Figure(data=[data_], layout=layout)
-    plot(fig, filename=fileName if fileName else 'plot.html', auto_open=True)
+    plot(fig, filename=fileName if fileName else "plot.html", auto_open=True)
 
 
 def dump_method(methodName, path=None):
     """
     Dump the LCIA method to a `csv` file in `path` directory.
     """
     method = bw2.Method(methodName)
@@ -40,54 +40,52 @@
     value = []
     unit = []
     name = []
     categories = []
     for i in data:
         key.append(i[0])
         value.append(i[1])
-        if 'unit' not in method.metadata:
-            method.metadata['unit'] = None
-        unit.append(method.metadata['unit'])
+        if "unit" not in method.metadata:
+            method.metadata["unit"] = None
+        unit.append(method.metadata["unit"])
         act = bw2.get_activity(i[0])
-        name.append(act.as_dict()['name'])
-        categories.append(act.as_dict()['categories'])
-    DF = pd.DataFrame({'key': key,
-                       'name': name,
-                       'categories': categories,
-                       'value': value,
-                       'unit': unit})
+        name.append(act.as_dict()["name"])
+        categories.append(act.as_dict()["categories"])
+    DF = pd.DataFrame(
+        {"key": key, "name": name, "categories": categories, "value": value, "unit": unit}
+    )
     if path:
         DF.to_csv(path + "/" + str(methodName) + ".csv", index=False)
     else:
-        DF.to_csv(str(methodName) + '.csv', index=False)
-    return(DF)
+        DF.to_csv(str(methodName) + ".csv", index=False)
+    return DF
 
 
 def find_biosphere_flows(flow_name, compartment=None, subcompartment=None, exact_match=True):
     """
-    Finds flows in the biosphere and reports the keys from biosph.
+    Finds flows in the biosphere and reports the keys.
     """
     key = []
     name = []
     categories = []
-    db = bw2.Database('biosphere3')
+    db = bw2.Database("biosphere3")
     for act in db:
         act_dict = act.as_dict()
-        if (exact_match and act_dict['name'] == flow_name) or (not exact_match and flow_name.lower() in act_dict['name'].lower()):
+        if (exact_match and act_dict["name"] == flow_name) or (
+            not exact_match and flow_name.lower() in act_dict["name"].lower()
+        ):
             if compartment and subcompartment:
-                if act_dict['categories'] == (compartment, subcompartment):
+                if act_dict["categories"] == (compartment, subcompartment):
                     key.append(act.key)
-                    name.append(act_dict['name'])
-                    categories.append(act_dict['categories'])
+                    name.append(act_dict["name"])
+                    categories.append(act_dict["categories"])
             elif compartment:
-                if act_dict['categories'][0] == compartment:
+                if act_dict["categories"][0] == compartment:
                     key.append(act.key)
-                    name.append(act_dict['name'])
-                    categories.append(act_dict['categories'])
+                    name.append(act_dict["name"])
+                    categories.append(act_dict["categories"])
             else:
                 key.append(act.key)
-                name.append(act_dict['name'])
-                categories.append(act_dict['categories'])
-    DF = pd.DataFrame({'key': key,
-                       'name': name,
-                       'categories': categories})
+                name.append(act_dict["name"])
+                categories.append(act_dict["categories"])
+    DF = pd.DataFrame({"key": key, "name": name, "categories": categories})
     return DF
```

### Comparing `swolfpy-0.2.5/swolfpy.egg-info/PKG-INFO` & `swolfpy-1.0.0/swolfpy.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,239 +1,247 @@
 Metadata-Version: 2.1
 Name: swolfpy
-Version: 0.2.5
-Summary: Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
-Home-page: https://github.com/SwolfPy-Project/swolfpy
-Author: Mojtaba Sardarmehni
-Author-email: msardar2@ncsu.edu
+Version: 1.0.0
+Summary: Solid Waste Optimization Life-cycle Framework in Python(SwolfPy).
+Author-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
+Maintainer-email: Mojtaba Sardarmehni <msardar2@alumni.ncsu.edu>
 License: GNU GENERAL PUBLIC LICENSE V2
-Description: .. General
-        
-        ================================================================
-        Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
-        ================================================================
-        
-        .. image:: https://img.shields.io/pypi/v/swolfpy.svg
-                :target: https://pypi.python.org/pypi/swolfpy
-        
-        .. image:: https://img.shields.io/pypi/pyversions/swolfpy.svg
-            :target: https://pypi.org/project/swolfpy/
-            :alt: Supported Python Versions
-        
-        .. image:: https://img.shields.io/pypi/l/swolfpy.svg
-            :target: https://pypi.org/project/swolfpy/
-            :alt: License
-        
-        .. image:: https://img.shields.io/pypi/dm/swolfpy.svg?label=Pypi%20downloads
-            :target: https://pypi.org/project/swolfpy/
-            :alt: Downloads
-        
-        .. image:: https://img.shields.io/pypi/format/swolfpy.svg
-            :target: https://pypi.org/project/swolfpy/
-            :alt: Format
-        
-        .. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
-                :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        .. image:: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml/badge.svg?branch=master
-                :target: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml
-                :alt: Test
-        
-        .. image:: https://zenodo.org/badge/395802952.svg
-                :target: https://zenodo.org/badge/latestdoi/395802952
-                :alt: DOi
-        
-        .. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
-           :target: https://doi.org/10.1111/jiec.13236
-           :alt: JIE DOI
-        
-        * Free software: GNU GENERAL PUBLIC LICENSE V2
-        * Website: https://swolfpy-project.github.io
-        * Documentation: https://swolfpy.readthedocs.io
-        * Repository: https://github.com/SwolfPy-Project/swolfpy
-        
-        
-        Features
-        --------
-        
-        * **Life-cycle assessment of Municipal Solid Waste (MSW) systems**
-        
-          * Comparative LCA
-          * Contribution analysis
-          * LCI report
-        
-        * **Monte Carlo simulation**
-        
-          * Uncertainty analysis
-          * Data visualization (distributions & correlations)
-        
-        * **Optimization**
-        
-          * Minimize environmental burdens or cost subject to a number of technical or policy-related constraints
-        
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
-                conda create --name swolfpy python=3.7 graphviz
-        
-        4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
-        
-        5- Activate the environment::
-        
-                conda activate swolfpy
-        
-        6- Install swolfpy in the environment::
-        
-                pip install swolfpy
-        
-        7- Open python to run swolfpy::
-        
-                python
-        
-        8- Run swolfpy in python::
-        
-                import swolfpy as sp
-                sp.swolfpy()
-        
-        .. endInstallation
-        
-        
-        =======
-        History
-        =======
-        
-        0.2.5 (2022-04-07)
-        ------------------
-        
-        * Minor changes in optimization and GUI
-        
-        
-        0.2.3 (2021-11-16)
-        ------------------
-        
-        * Improve data validation in GUI
-        * Improve warning/Pop-ups
-        
-        
-        0.2.2 (2021-10-02)
-        ------------------
-        
-        * Add Home Composting (HC)
-        * Add Gasification & Syngas combustion (GC)
-        * Add Refuse-derived fuel (RDF)
-        
-        
-        0.2.0 (2021-05-10)
-        ------------------
-        
-        * Add tab for correlation analysis.
-        * Add cost calculations.
-        * Add help to interface.
-        * Parallel optimization.
-        
-        
-        
-        0.1.8 (2020-05-20)
-        ------------------
-        
-        * Add tab for Monte Carlo results analysis.
-        * Show Sankey for mass flows after optimization.
-        * Show SWM Network graph.
-        
-        
-        
-        0.1.6 (2020-04-11)
-        ------------------
-        
-        * Add Reprocessing.
-        * Revise Functional units.
-        * Revise parameters class.
-        
-        
-        0.1.0 (2020-02-27)
-        ------------------
-        
-        * First release on PyPI.
-        * Main functionality: LCA, Monte-Carlo, and Optimization.
-        * Process Models include LF, WTE, Composting, AD, SS_MRF, and Collection.
-        
-Keywords: swolfpy
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://swolfpy-project.github.io/
+Project-URL: Documentation, https://swolfpy.readthedocs.io/en/latest/
+Project-URL: Source Code, https://github.com/SwolfPy-Project/swolfpy
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
+================================================================
+Solid Waste Optimization Life-cycle Framework in Python(SwolfPy)
+================================================================
+
+.. image:: https://img.shields.io/pypi/v/swolfpy.svg
+        :target: https://pypi.python.org/pypi/swolfpy
+
+.. image:: https://img.shields.io/pypi/pyversions/swolfpy.svg
+    :target: https://pypi.org/project/swolfpy/
+    :alt: Supported Python Versions
+
+.. image:: https://img.shields.io/pypi/l/swolfpy.svg
+    :target: https://pypi.org/project/swolfpy/
+    :alt: License
+
+.. image:: https://img.shields.io/pypi/dm/swolfpy.svg?label=Pypi%20downloads
+    :target: https://pypi.org/project/swolfpy/
+    :alt: Downloads
+
+.. image:: https://img.shields.io/pypi/format/swolfpy.svg
+    :target: https://pypi.org/project/swolfpy/
+    :alt: Format
+
+.. image:: https://readthedocs.org/projects/swolfpy/badge/?version=latest
+        :target: https://swolfpy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml/badge.svg?branch=master
+        :target: https://github.com/SwolfPy-Project/swolfpy/actions/workflows/python-app.yml
+        :alt: Test
+
+.. image:: https://zenodo.org/badge/395802952.svg
+        :target: https://zenodo.org/badge/latestdoi/395802952
+        :alt: DOi
+
+.. image:: https://img.shields.io/badge/JIE%20DOI-10.1111%2Fjiec.13236-blue
+   :target: https://doi.org/10.1111/jiec.13236
+   :alt: JIE DOI
+
+* Free software: GNU GENERAL PUBLIC LICENSE V2
+* Website: https://swolfpy-project.github.io
+* Documentation: https://swolfpy.readthedocs.io
+* Repository: https://github.com/SwolfPy-Project/swolfpy
+
+
+Features
+--------
+
+* **Life-cycle assessment of Municipal Solid Waste (MSW) systems**
+
+  * Comparative LCA
+  * Contribution analysis
+  * LCI report
+
+* **Monte Carlo simulation**
+
+  * Uncertainty analysis
+  * Data visualization (distributions & correlations)
+
+* **Optimization**
+
+  * Minimize environmental burdens or cost subject to a number of technical or policy-related constraints
+
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
+        conda create --name swolfpy python=3.10 graphviz
+
+4- Add Graphviz executables to your system PATH (This step is optional; Enables plotting SWM network). You can find Graphviz executables in ``\\miniconda3\\envs\\swolfpy\\Library\\bin\\graphviz`` folder or search for ``dot.exe`` file in your system. Add the directory to the ``Path`` variable in your environment variables.
+
+5- Activate the environment::
+
+        conda activate swolfpy
+
+6- Install swolfpy in the environment::
+
+        pip install swolfpy
+
+7- Open python to run swolfpy::
+
+        python
+
+8- Run swolfpy in python::
+
+        import swolfpy as sp
+        sp.swolfpy()
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
+0.2.5 (2022-04-07)
+------------------
+
+* Minor changes in optimization and GUI
+
+
+0.2.3 (2021-11-16)
+------------------
+
+* Improve data validation in GUI
+* Improve warning/Pop-ups
+
+
+0.2.2 (2021-10-02)
+------------------
+
+* Add Home Composting (HC)
+* Add Gasification & Syngas combustion (GC)
+* Add Refuse-derived fuel (RDF)
+
+
+0.2.0 (2021-05-10)
+------------------
+
+* Add tab for correlation analysis.
+* Add cost calculations.
+* Add help to interface.
+* Parallel optimization.
+
+
+
+0.1.8 (2020-05-20)
+------------------
+
+* Add tab for Monte Carlo results analysis.
+* Show Sankey for mass flows after optimization.
+* Show SWM Network graph.
+
+
+
+0.1.6 (2020-04-11)
+------------------
+
+* Add Reprocessing.
+* Revise Functional units.
+* Revise parameters class.
+
+
+0.1.0 (2020-02-27)
+------------------
+
+* First release on PyPI.
+* Main functionality: LCA, Monte-Carlo, and Optimization.
+* Process Models include LF, WTE, Composting, AD, SS_MRF, and Collection.
```

### Comparing `swolfpy-0.2.5/swolfpy.egg-info/SOURCES.txt` & `swolfpy-1.0.0/swolfpy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

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
 docs/Getting_started.rst
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/doc_inputdata.rst
 docs/doc_processmodels.rst
@@ -48,22 +49,12 @@
 swolfpy/Technosphere.py
 swolfpy/__init__.py
 swolfpy/swolfpy_method.py
 swolfpy/utils.py
 swolfpy.egg-info/PKG-INFO
 swolfpy.egg-info/SOURCES.txt
 swolfpy.egg-info/dependency_links.txt
-swolfpy.egg-info/not-zip-safe
 swolfpy.egg-info/requires.txt
 swolfpy.egg-info/top_level.txt
-swolfpy/UI/MC_ui.py
-swolfpy/UI/PySWOLF_run.py
-swolfpy/UI/PySWOLF_ui.py
-swolfpy/UI/PyWOLF_Resource_rc.py
-swolfpy/UI/Reference_ui.py
-swolfpy/UI/Table_from_pandas.py
-swolfpy/UI/Workers.py
-swolfpy/UI/__init__.py
-swolfpy/UI/adv_opt_ui.py
 tests/.coverage
 tests/__init__.py
 tests/test_swolfpy.py
```

### Comparing `swolfpy-0.2.5/tests/.coverage` & `swolfpy-1.0.0/tests/.coverage`

 * *Files identical despite different names*

