# Comparing `tmp/PyXAB-0.2.2.tar.gz` & `tmp/PyXAB-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyXAB-0.2.2.tar", last modified: Thu May 25 00:38:32 2023, max compression
+gzip compressed data, was "dist/PyXAB-0.2.3.tar", last modified: Sun Jun  4 18:12:07 2023, max compression
```

## Comparing `PyXAB-0.2.2.tar` & `PyXAB-0.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.396742 PyXAB-0.2.2/
--rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.2/LICENSE
--rw-r--r--   0 william    (501) staff       (20)    16395 2023-05-25 00:38:32.397036 PyXAB-0.2.2/PKG-INFO
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.370209 PyXAB-0.2.2/PyXAB/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.2/PyXAB/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.380143 PyXAB-0.2.2/PyXAB/algos/
--rw-r--r--   0 william    (501) staff       (20)     1415 2023-05-24 05:55:11.000000 PyXAB-0.2.2/PyXAB/algos/Algo.py
--rw-r--r--   0 william    (501) staff       (20)     6201 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/DOO.py
--rw-r--r--   0 william    (501) staff       (20)     5406 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/GPO.py
--rw-r--r--   0 william    (501) staff       (20)    10197 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/HCT.py
--rw-r--r--   0 william    (501) staff       (20)     8980 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/HOO.py
--rw-r--r--   0 william    (501) staff       (20)     2428 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/PCT.py
--rw-r--r--   0 william    (501) staff       (20)     5740 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/POO.py
--rw-r--r--   0 william    (501) staff       (20)     5461 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/SOO.py
--rw-r--r--   0 william    (501) staff       (20)     7241 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/SequOOL.py
--rw-r--r--   0 william    (501) staff       (20)     7408 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/StoSOO.py
--rw-r--r--   0 william    (501) staff       (20)    11065 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/StroquOOL.py
--rw-r--r--   0 william    (501) staff       (20)    12008 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/VHCT.py
--rw-r--r--   0 william    (501) staff       (20)     2430 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/VPCT.py
--rw-r--r--   0 william    (501) staff       (20)     5288 2023-05-24 05:55:19.000000 PyXAB-0.2.2/PyXAB/algos/Zooming.py
--rw-r--r--   0 william    (501) staff       (20)      331 2023-05-24 05:55:11.000000 PyXAB-0.2.2/PyXAB/algos/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.385873 PyXAB-0.2.2/PyXAB/partition/
--rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/BinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/DimensionBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/KaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.2/PyXAB/partition/Node.py
--rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/Partition.py
--rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/RandomBinaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/RandomKaryPartition.py
--rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/partition/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.393239 PyXAB-0.2.2/PyXAB/synthetic_obj/
--rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Ackley.py
--rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Cexample.py
--rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/DifficultFunc.py
--rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/DoubleSine.py
--rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Garland.py
--rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Himmelblau.py
--rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Objective.py
--rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/Rastrigin.py
--rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.2/PyXAB/synthetic_obj/__init__.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.395729 PyXAB-0.2.2/PyXAB/utils/
--rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.2/PyXAB/utils/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.2/PyXAB/utils/plot.py
--rw-r--r--   0 william    (501) staff       (20)     2477 2023-05-24 05:55:11.000000 PyXAB-0.2.2/PyXAB/utils/run_synthetic.py
--rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.2/PyXAB/utils/visualize_gif.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2023-05-25 00:38:32.371773 PyXAB-0.2.2/PyXAB.egg-info/
--rw-r--r--   0 william    (501) staff       (20)    16395 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     1179 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       25 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)        6 2023-05-25 00:38:32.000000 PyXAB-0.2.2/PyXAB.egg-info/top_level.txt
--rw-r--r--   0 william    (501) staff       (20)    14056 2023-05-25 00:37:31.000000 PyXAB-0.2.2/README.md
--rw-r--r--   0 william    (501) staff       (20)      103 2023-05-25 00:38:32.397677 PyXAB-0.2.2/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)     3881 2023-05-24 05:55:19.000000 PyXAB-0.2.2/setup.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.236171 PyXAB-0.2.3/
+-rw-r--r--   0 william    (501) staff       (20)     1066 2022-03-24 15:30:00.000000 PyXAB-0.2.3/LICENSE
+-rw-r--r--   0 william    (501) staff       (20)    16549 2023-06-04 18:12:07.236432 PyXAB-0.2.3/PKG-INFO
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.215739 PyXAB-0.2.3/PyXAB/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.3/PyXAB/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.223299 PyXAB-0.2.3/PyXAB/algos/
+-rw-r--r--   0 william    (501) staff       (20)     1415 2023-05-24 05:55:11.000000 PyXAB-0.2.3/PyXAB/algos/Algo.py
+-rw-r--r--   0 william    (501) staff       (20)     6201 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/DOO.py
+-rw-r--r--   0 william    (501) staff       (20)     5406 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/GPO.py
+-rw-r--r--   0 william    (501) staff       (20)    10197 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/HCT.py
+-rw-r--r--   0 william    (501) staff       (20)     8980 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/HOO.py
+-rw-r--r--   0 william    (501) staff       (20)     2428 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/PCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5740 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/POO.py
+-rw-r--r--   0 william    (501) staff       (20)     5461 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/SOO.py
+-rw-r--r--   0 william    (501) staff       (20)     7241 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/SequOOL.py
+-rw-r--r--   0 william    (501) staff       (20)     7408 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/StoSOO.py
+-rw-r--r--   0 william    (501) staff       (20)    11065 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/StroquOOL.py
+-rw-r--r--   0 william    (501) staff       (20)    12008 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/VHCT.py
+-rw-r--r--   0 william    (501) staff       (20)     2430 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/VPCT.py
+-rw-r--r--   0 william    (501) staff       (20)     5288 2023-05-24 05:55:19.000000 PyXAB-0.2.3/PyXAB/algos/Zooming.py
+-rw-r--r--   0 william    (501) staff       (20)      331 2023-05-24 05:55:11.000000 PyXAB-0.2.3/PyXAB/algos/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.227411 PyXAB-0.2.3/PyXAB/partition/
+-rw-r--r--   0 william    (501) staff       (20)     2806 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/BinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3131 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/DimensionBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2807 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/KaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     2298 2023-02-16 03:14:10.000000 PyXAB-0.2.3/PyXAB/partition/Node.py
+-rw-r--r--   0 william    (501) staff       (20)     3019 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/Partition.py
+-rw-r--r--   0 william    (501) staff       (20)     2861 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/RandomBinaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)     3068 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/RandomKaryPartition.py
+-rw-r--r--   0 william    (501) staff       (20)       83 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/partition/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.232699 PyXAB-0.2.3/PyXAB/synthetic_obj/
+-rw-r--r--   0 william    (501) staff       (20)     2534 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/Ackley.py
+-rw-r--r--   0 william    (501) staff       (20)     1027 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/Cexample.py
+-rw-r--r--   0 william    (501) staff       (20)     1224 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/DifficultFunc.py
+-rw-r--r--   0 william    (501) staff       (20)     4145 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/DoubleSine.py
+-rw-r--r--   0 william    (501) staff       (20)     2118 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/Garland.py
+-rw-r--r--   0 william    (501) staff       (20)     2095 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/Himmelblau.py
+-rw-r--r--   0 william    (501) staff       (20)      484 2023-02-16 02:41:47.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/Objective.py
+-rw-r--r--   0 william    (501) staff       (20)     2116 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/Rastrigin.py
+-rw-r--r--   0 william    (501) staff       (20)      380 2023-02-16 02:41:47.000000 PyXAB-0.2.3/PyXAB/synthetic_obj/__init__.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.235439 PyXAB-0.2.3/PyXAB/utils/
+-rw-r--r--   0 william    (501) staff       (20)        0 2022-03-22 23:40:33.000000 PyXAB-0.2.3/PyXAB/utils/__init__.py
+-rw-r--r--   0 william    (501) staff       (20)     1467 2023-02-16 03:14:10.000000 PyXAB-0.2.3/PyXAB/utils/plot.py
+-rw-r--r--   0 william    (501) staff       (20)     2477 2023-05-24 05:55:11.000000 PyXAB-0.2.3/PyXAB/utils/run_synthetic.py
+-rw-r--r--   0 william    (501) staff       (20)     4350 2023-03-13 03:58:11.000000 PyXAB-0.2.3/PyXAB/utils/visualize_gif.py
+drwxr-xr-x   0 william    (501) staff       (20)        0 2023-06-04 18:12:07.217248 PyXAB-0.2.3/PyXAB.egg-info/
+-rw-r--r--   0 william    (501) staff       (20)    16549 2023-06-04 18:12:07.000000 PyXAB-0.2.3/PyXAB.egg-info/PKG-INFO
+-rw-r--r--   0 william    (501) staff       (20)     1179 2023-06-04 18:12:07.000000 PyXAB-0.2.3/PyXAB.egg-info/SOURCES.txt
+-rw-r--r--   0 william    (501) staff       (20)        1 2023-06-04 18:12:07.000000 PyXAB-0.2.3/PyXAB.egg-info/dependency_links.txt
+-rw-r--r--   0 william    (501) staff       (20)       25 2023-06-04 18:12:07.000000 PyXAB-0.2.3/PyXAB.egg-info/requires.txt
+-rw-r--r--   0 william    (501) staff       (20)        6 2023-06-04 18:12:07.000000 PyXAB-0.2.3/PyXAB.egg-info/top_level.txt
+-rw-r--r--   0 william    (501) staff       (20)    14138 2023-06-04 18:11:00.000000 PyXAB-0.2.3/README.md
+-rw-r--r--   0 william    (501) staff       (20)      103 2023-06-04 18:12:07.237073 PyXAB-0.2.3/setup.cfg
+-rw-r--r--   0 william    (501) staff       (20)     3881 2023-06-04 18:11:43.000000 PyXAB-0.2.3/setup.py
```

### Comparing `PyXAB-0.2.2/LICENSE` & `PyXAB-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PKG-INFO` & `PyXAB-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.2
+Version: 0.2.3
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -41,29 +41,36 @@
         </a>
         <a href="https://github.com/psf/black" target="blank">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
         </a>
         </p>
         
         
-        PyXAB is a Python open-source library for *X*-armed bandit algorithms, a prestigious set of optimizers for online black-box optimization, i.e., optimize an objective without gradients, also known as the continuous-arm bandit (CAB), Lipschitz bandit, 
-        global optimization (GO) and bandit-based black-box optimization problems.
+        PyXAB is a Python open-source library for *X*-armed bandit algorithms, a prestigious set of optimizers for online black-box optimization and 
+        hyperparameter optimization.
         
         
         <p align='center'>
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_trajectory.gif" alt="trajectory" width="48%"/>  
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_heatmap.gif" alt="heatmap" width="48%"/>  
         </p>
         
-        PyXAB contains the implementations of **more than 10 optimization algorithms**, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
-         [StoSOO (Valko et al., 2013)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most
-        recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL  (Bartlett et al.,2019)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
+        PyXAB contains the implementations of **10+** optimization algorithms, including the classic ones such as [Zooming](https://arxiv.org/pdf/0809.4882.pdf), 
+         [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT](https://proceedings.mlr.press/v32/azar14.html), and the most
+        recent works such as [GPO](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT](https://arxiv.org/abs/2106.09215).
         PyXAB also provides the most commonly-used synthetic objectives to evaluate the performance of different algorithms and the implementations for different hierarchical partitions
         
-        **The algorithms are maximization algorithms!**
+        **PyXAB is featured for:**
+        
+        - **User-friendly APIs, clear documentation, and detailed examples**
+        - **Comprehensive library** of optimization algorithms, partitions and synthetic objectives
+        - **High standard code quality and testing coverage**
+        
+        
+        **Reminder**: The algorithms are maximization algorithms!
         
         ## Quick Links
         
         - [Quick Example](#Quick-Example)
         - [Documentations](#Documentations)
         - [Installation](#Installation)
         - [Features](#Features)
@@ -76,15 +83,14 @@
         ## Quick Example
         PyXAB follows a natural and straightforward API design completely aligned with the online blackbox
         optimization paradigm. The following is a simple 6-line usage example.
         
         First, we define the parameter domain and the algorithm to run. 
         At every round  `t`, call `algo.pull(t)` to get a point and call 
         `algo.receive_reward(t, reward)` to give the algorithm the objective evaluation (reward)
-        ```
         
         ```python3
         domain = [[0, 1]]               # Parameter is 1-D and between 0 and 1
         algo = T_HOO(rounds=1000, domain=domain) 
         for t in range(1000):
             point = algo.pull(t)
             reward = 1                  #TODO: User-defined objective returns the reward
@@ -187,22 +193,25 @@
           author = {Li, Wenjie and Li, Haoze and Honorio, Jean and Song, Qifan},
           title = {PyXAB -- A Python Library for $\mathcal{X}$-Armed Bandit and Online Blackbox Optimization Algorithms},
           publisher = {arXiv},
           year = {2023},
         }
         ```
         
-        We would appreciate it if you could cite our related works.
+        We would also appreciate it if you could cite our related works.
         
         ```text
-        @article{li2021optimum,
-          title={Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization},
-          author={Li, Wenjie and Wang, Chi-Hua, Qifan Song and Cheng, Guang},
-          journal={arXiv preprint arXiv:2106.09215},
-          year={2021}
+        @article{li2023optimumstatistical,
+            title={Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization},
+            author={Wenjie Li and Chi-Hua Wang and Guang Cheng and Qifan Song},
+            journal={Transactions on Machine Learning Research},
+            issn={2835-8856},
+            year={2023},
+            url={https://openreview.net/forum?id=ClIcmwdlxn},
+            note={}
         }
         ```
         
         ```text
         @misc{li2022Federated,
           doi = {10.48550/ARXIV.2205.15268},
           url = {https://arxiv.org/abs/2205.15268},
```

#### html2text {}

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.2 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.2.3 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li Author-
 email: lil3549@purdue.edu License: MIT Description: # PyXAB - Python *X*-Armed
 Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
 license] [Code_style:_black]
 PyXAB is a Python open-source library for *X*-armed bandit algorithms, a
-prestigious set of optimizers for online black-box optimization, i.e., optimize
-an objective without gradients, also known as the continuous-arm bandit (CAB),
-Lipschitz bandit, global optimization (GO) and bandit-based black-box
-optimization problems.
+prestigious set of optimizers for online black-box optimization and
+hyperparameter optimization.
                             [trajectory] [heatmap]
-PyXAB contains the implementations of **more than 10 optimization algorithms**,
-including the classic ones such as [HOO (Bubeck et al., 2011)](https://
-jmlr.org/papers/v12/bubeck11a.html), [StoSOO (Valko et al., 2013)](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et
-al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most recent
-works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/
-xuedong19a.html), [StroquOOL (Bartlett et al.,2019)](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al,
-2021)](https://arxiv.org/abs/2106.09215). PyXAB also provides the most
-commonly-used synthetic objectives to evaluate the performance of different
-algorithms and the implementations for different hierarchical partitions **The
-algorithms are maximization algorithms!** ## Quick Links - [Quick Example]
-(#Quick-Example) - [Documentations](#Documentations) - [Installation]
-(#Installation) - [Features](#Features) * [*X*-armed bandit algorithms]
-(#Stochastic-X-armed-bandit-algorithms) * [Hierarchical partition ]
-(#Hierarchical-partition) * [Synthetic objectives](#Synthetic-objectives) -
-[Contributing](#Contributing) - [Citations](#Citations) ## Quick Example PyXAB
-follows a natural and straightforward API design completely aligned with the
-online blackbox optimization paradigm. The following is a simple 6-line usage
-example. First, we define the parameter domain and the algorithm to run. At
-every round `t`, call `algo.pull(t)` to get a point and call
-`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation
-(reward) ``` ```python3 domain = [[0, 1]] # Parameter is 1-D and between 0 and
-1 algo = T_HOO(rounds=1000, domain=domain) for t in range(1000): point =
-algo.pull(t) reward = 1 #TODO: User-defined objective returns the reward
-algo.receive_reward(t, reward) ``` More detailed examples can be found [here]
-(https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/
-index.html) ## Documentations * The most up-to-date [documentations](https://
-pyxab.readthedocs.io/) * The [roadmap](https://github.com/users/WilliamLwj/
-projects/1) for our project * Our [manuscript](https://arxiv.org/abs/
-2303.04030) for the library ## Installation To install via pip, run the
-following lines of code ```bash pip install PyXAB # normal install pip install
---upgrade PyXAB # or update if needed ``` To install via git, run the following
-lines of code ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd
-PyXAB pip install . ``` ## Features: ### *X*-armed bandit algorithms *
-Algorithm starred are meta-algorithms (wrappers) | Algorithm | Research Paper |
-Year | |-----------------------------------------------------------------------
---------------|----------------------------------------------------------------
+PyXAB contains the implementations of **10+** optimization algorithms,
+including the classic ones such as [Zooming](https://arxiv.org/pdf/
+0809.4882.pdf), [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+algos/StoSOO.py), and [HCT](https://proceedings.mlr.press/v32/azar14.html), and
+the most recent works such as [GPO](https://proceedings.mlr.press/v98/
+xuedong19a.html), [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/StroquOOL.py) and [VHCT](https://arxiv.org/abs/2106.09215). PyXAB
+also provides the most commonly-used synthetic objectives to evaluate the
+performance of different algorithms and the implementations for different
+hierarchical partitions **PyXAB is featured for:** - **User-friendly APIs,
+clear documentation, and detailed examples** - **Comprehensive library** of
+optimization algorithms, partitions and synthetic objectives - **High standard
+code quality and testing coverage** **Reminder**: The algorithms are
+maximization algorithms! ## Quick Links - [Quick Example](#Quick-Example) -
+[Documentations](#Documentations) - [Installation](#Installation) - [Features]
+(#Features) * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-
+algorithms) * [Hierarchical partition ](#Hierarchical-partition) * [Synthetic
+objectives](#Synthetic-objectives) - [Contributing](#Contributing) -
+[Citations](#Citations) ## Quick Example PyXAB follows a natural and
+straightforward API design completely aligned with the online blackbox
+optimization paradigm. The following is a simple 6-line usage example. First,
+we define the parameter domain and the algorithm to run. At every round `t`,
+call `algo.pull(t)` to get a point and call `algo.receive_reward(t, reward)` to
+give the algorithm the objective evaluation (reward) ```python3 domain = [[0,
+1]] # Parameter is 1-D and between 0 and 1 algo = T_HOO(rounds=1000,
+domain=domain) for t in range(1000): point = algo.pull(t) reward = 1 #TODO:
+User-defined objective returns the reward algo.receive_reward(t, reward) ```
+More detailed examples can be found [here](https://pyxab.readthedocs.io/en/
+latest/getting_started/auto_examples/index.html) ## Documentations * The most
+up-to-date [documentations](https://pyxab.readthedocs.io/) * The [roadmap]
+(https://github.com/users/WilliamLwj/projects/1) for our project * Our
+[manuscript](https://arxiv.org/abs/2303.04030) for the library ## Installation
+To install via pip, run the following lines of code ```bash pip install PyXAB #
+normal install pip install --upgrade PyXAB # or update if needed ``` To install
+via git, run the following lines of code ```bash git clone https://github.com/
+WilliamLwj/PyXAB.git cd PyXAB pip install . ``` ## Features: ### *X*-armed
+bandit algorithms * Algorithm starred are meta-algorithms (wrappers) |
+Algorithm | Research Paper | Year | |------------------------------------------
+-------------------------------------------|-----------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------|------| | [Zooming](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed
-Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-
-HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-
-Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) |
-[Optimistic Optimization of a Deterministic Function without the Knowledge of
-its Smoothness](https://proceedings.neurips.cc/paper/2011/file/
-7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
+------------------------------------------------------------------------|------
+| | [Zooming](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
+Zooming.py) | [Multi-Armed Bandits in Metric Spaces](https://arxiv.org/pdf/
+0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://jmlr.org/papers/v12/
+bubeck11a.html) | 2011 | | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/DOO.py) | [Optimistic Optimization of a Deterministic Function
+without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
+2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
 Optimization of a Deterministic Function without the Knowledge of its
 Smoothness](https://proceedings.neurips.cc/paper/2011/file/
 7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
 Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
 valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
@@ -127,21 +126,22 @@
 instructions](https://pyxab.readthedocs.io/en/latest/info/contributing.html)
 before submitting a pull request. ## Citations If you use our package in your
 research or projects, we kindly ask you to cite our work ```text @misc
 {Li2023PyXAB, doi = {10.48550/ARXIV.2303.04030}, url = {https://arxiv.org/abs/
 2303.04030}, author = {Li, Wenjie and Li, Haoze and Honorio, Jean and Song,
 Qifan}, title = {PyXAB -- A Python Library for $\mathcal{X}$-Armed Bandit and
 Online Blackbox Optimization Algorithms}, publisher = {arXiv}, year = {2023}, }
-``` We would appreciate it if you could cite our related works. ```text
-@article{li2021optimum, title={Optimum-statistical Collaboration Towards
-General and Efficient Black-box Optimization}, author={Li, Wenjie and Wang,
-Chi-Hua, Qifan Song and Cheng, Guang}, journal={arXiv preprint arXiv:
-2106.09215}, year={2021} } ``` ```text @misc{li2022Federated, doi = {10.48550/
-ARXIV.2205.15268}, url = {https://arxiv.org/abs/2205.15268}, author = {Li,
-Wenjie and Song, Qifan and Honorio, Jean and Lin, Guang}, title = {Federated X-
-Armed Bandit}, publisher = {arXiv}, year = {2022}, } ``` Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type:
-text/markdown
+``` We would also appreciate it if you could cite our related works. ```text
+@article{li2023optimumstatistical, title={Optimum-statistical Collaboration
+Towards General and Efficient Black-box Optimization}, author={Wenjie Li and
+Chi-Hua Wang and Guang Cheng and Qifan Song}, journal={Transactions on Machine
+Learning Research}, issn={2835-8856}, year={2023}, url={https://openreview.net/
+forum?id=ClIcmwdlxn}, note={} } ``` ```text @misc{li2022Federated, doi =
+{10.48550/ARXIV.2205.15268}, url = {https://arxiv.org/abs/2205.15268}, author =
+{Li, Wenjie and Song, Qifan and Honorio, Jean and Lin, Guang}, title =
+{Federated X-Armed Bandit}, publisher = {arXiv}, year = {2022}, } ``` Platform:
+UNKNOWN Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
```

### Comparing `PyXAB-0.2.2/PyXAB/algos/Algo.py` & `PyXAB-0.2.3/PyXAB/algos/Algo.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/DOO.py` & `PyXAB-0.2.3/PyXAB/algos/DOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/GPO.py` & `PyXAB-0.2.3/PyXAB/algos/GPO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/HCT.py` & `PyXAB-0.2.3/PyXAB/algos/HCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/HOO.py` & `PyXAB-0.2.3/PyXAB/algos/HOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/PCT.py` & `PyXAB-0.2.3/PyXAB/algos/PCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/POO.py` & `PyXAB-0.2.3/PyXAB/algos/POO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/SOO.py` & `PyXAB-0.2.3/PyXAB/algos/SOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/SequOOL.py` & `PyXAB-0.2.3/PyXAB/algos/SequOOL.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/StoSOO.py` & `PyXAB-0.2.3/PyXAB/algos/StoSOO.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/StroquOOL.py` & `PyXAB-0.2.3/PyXAB/algos/StroquOOL.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/VHCT.py` & `PyXAB-0.2.3/PyXAB/algos/VHCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/VPCT.py` & `PyXAB-0.2.3/PyXAB/algos/VPCT.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/algos/Zooming.py` & `PyXAB-0.2.3/PyXAB/algos/Zooming.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/BinaryPartition.py` & `PyXAB-0.2.3/PyXAB/partition/BinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/DimensionBinaryPartition.py` & `PyXAB-0.2.3/PyXAB/partition/DimensionBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/KaryPartition.py` & `PyXAB-0.2.3/PyXAB/partition/KaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/Node.py` & `PyXAB-0.2.3/PyXAB/partition/Node.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/Partition.py` & `PyXAB-0.2.3/PyXAB/partition/Partition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/RandomBinaryPartition.py` & `PyXAB-0.2.3/PyXAB/partition/RandomBinaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/partition/RandomKaryPartition.py` & `PyXAB-0.2.3/PyXAB/partition/RandomKaryPartition.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/Ackley.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/Ackley.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/Cexample.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/Cexample.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/DifficultFunc.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/DifficultFunc.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/DoubleSine.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/DoubleSine.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/Garland.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/Garland.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/Himmelblau.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/Himmelblau.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/synthetic_obj/Rastrigin.py` & `PyXAB-0.2.3/PyXAB/synthetic_obj/Rastrigin.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/utils/plot.py` & `PyXAB-0.2.3/PyXAB/utils/plot.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/utils/run_synthetic.py` & `PyXAB-0.2.3/PyXAB/utils/run_synthetic.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB/utils/visualize_gif.py` & `PyXAB-0.2.3/PyXAB/utils/visualize_gif.py`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/PyXAB.egg-info/PKG-INFO` & `PyXAB-0.2.3/PyXAB.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyXAB
-Version: 0.2.2
+Version: 0.2.3
 Summary: PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.
 Home-page: https://github.com/WilliamLwj/PyXAB
 Author: Wenjie Li, Haoze Li
 Author-email: lil3549@purdue.edu
 License: MIT
 Description: 
         
@@ -41,29 +41,36 @@
         </a>
         <a href="https://github.com/psf/black" target="blank">
         <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
         </a>
         </p>
         
         
-        PyXAB is a Python open-source library for *X*-armed bandit algorithms, a prestigious set of optimizers for online black-box optimization, i.e., optimize an objective without gradients, also known as the continuous-arm bandit (CAB), Lipschitz bandit, 
-        global optimization (GO) and bandit-based black-box optimization problems.
+        PyXAB is a Python open-source library for *X*-armed bandit algorithms, a prestigious set of optimizers for online black-box optimization and 
+        hyperparameter optimization.
         
         
         <p align='center'>
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_trajectory.gif" alt="trajectory" width="48%"/>  
           <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_heatmap.gif" alt="heatmap" width="48%"/>  
         </p>
         
-        PyXAB contains the implementations of **more than 10 optimization algorithms**, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
-         [StoSOO (Valko et al., 2013)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most
-        recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL  (Bartlett et al.,2019)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
+        PyXAB contains the implementations of **10+** optimization algorithms, including the classic ones such as [Zooming](https://arxiv.org/pdf/0809.4882.pdf), 
+         [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT](https://proceedings.mlr.press/v32/azar14.html), and the most
+        recent works such as [GPO](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT](https://arxiv.org/abs/2106.09215).
         PyXAB also provides the most commonly-used synthetic objectives to evaluate the performance of different algorithms and the implementations for different hierarchical partitions
         
-        **The algorithms are maximization algorithms!**
+        **PyXAB is featured for:**
+        
+        - **User-friendly APIs, clear documentation, and detailed examples**
+        - **Comprehensive library** of optimization algorithms, partitions and synthetic objectives
+        - **High standard code quality and testing coverage**
+        
+        
+        **Reminder**: The algorithms are maximization algorithms!
         
         ## Quick Links
         
         - [Quick Example](#Quick-Example)
         - [Documentations](#Documentations)
         - [Installation](#Installation)
         - [Features](#Features)
@@ -76,15 +83,14 @@
         ## Quick Example
         PyXAB follows a natural and straightforward API design completely aligned with the online blackbox
         optimization paradigm. The following is a simple 6-line usage example.
         
         First, we define the parameter domain and the algorithm to run. 
         At every round  `t`, call `algo.pull(t)` to get a point and call 
         `algo.receive_reward(t, reward)` to give the algorithm the objective evaluation (reward)
-        ```
         
         ```python3
         domain = [[0, 1]]               # Parameter is 1-D and between 0 and 1
         algo = T_HOO(rounds=1000, domain=domain) 
         for t in range(1000):
             point = algo.pull(t)
             reward = 1                  #TODO: User-defined objective returns the reward
@@ -187,22 +193,25 @@
           author = {Li, Wenjie and Li, Haoze and Honorio, Jean and Song, Qifan},
           title = {PyXAB -- A Python Library for $\mathcal{X}$-Armed Bandit and Online Blackbox Optimization Algorithms},
           publisher = {arXiv},
           year = {2023},
         }
         ```
         
-        We would appreciate it if you could cite our related works.
+        We would also appreciate it if you could cite our related works.
         
         ```text
-        @article{li2021optimum,
-          title={Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization},
-          author={Li, Wenjie and Wang, Chi-Hua, Qifan Song and Cheng, Guang},
-          journal={arXiv preprint arXiv:2106.09215},
-          year={2021}
+        @article{li2023optimumstatistical,
+            title={Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization},
+            author={Wenjie Li and Chi-Hua Wang and Guang Cheng and Qifan Song},
+            journal={Transactions on Machine Learning Research},
+            issn={2835-8856},
+            year={2023},
+            url={https://openreview.net/forum?id=ClIcmwdlxn},
+            note={}
         }
         ```
         
         ```text
         @misc{li2022Federated,
           doi = {10.48550/ARXIV.2205.15268},
           url = {https://arxiv.org/abs/2205.15268},
```

#### html2text {}

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1 Name: PyXAB Version: 0.2.2 Summary: PyXAB - A Python
+Metadata-Version: 2.1 Name: PyXAB Version: 0.2.3 Summary: PyXAB - A Python
 Library for X-Armed Bandit and Online Blackbox Optimization Algorithms. Home-
 page: https://github.com/WilliamLwj/PyXAB Author: Wenjie Li, Haoze Li Author-
 email: lil3549@purdue.edu License: MIT Description: # PyXAB - Python *X*-Armed
 Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
 license] [Code_style:_black]
 PyXAB is a Python open-source library for *X*-armed bandit algorithms, a
-prestigious set of optimizers for online black-box optimization, i.e., optimize
-an objective without gradients, also known as the continuous-arm bandit (CAB),
-Lipschitz bandit, global optimization (GO) and bandit-based black-box
-optimization problems.
+prestigious set of optimizers for online black-box optimization and
+hyperparameter optimization.
                             [trajectory] [heatmap]
-PyXAB contains the implementations of **more than 10 optimization algorithms**,
-including the classic ones such as [HOO (Bubeck et al., 2011)](https://
-jmlr.org/papers/v12/bubeck11a.html), [StoSOO (Valko et al., 2013)](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et
-al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most recent
-works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/
-xuedong19a.html), [StroquOOL (Bartlett et al.,2019)](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al,
-2021)](https://arxiv.org/abs/2106.09215). PyXAB also provides the most
-commonly-used synthetic objectives to evaluate the performance of different
-algorithms and the implementations for different hierarchical partitions **The
-algorithms are maximization algorithms!** ## Quick Links - [Quick Example]
-(#Quick-Example) - [Documentations](#Documentations) - [Installation]
-(#Installation) - [Features](#Features) * [*X*-armed bandit algorithms]
-(#Stochastic-X-armed-bandit-algorithms) * [Hierarchical partition ]
-(#Hierarchical-partition) * [Synthetic objectives](#Synthetic-objectives) -
-[Contributing](#Contributing) - [Citations](#Citations) ## Quick Example PyXAB
-follows a natural and straightforward API design completely aligned with the
-online blackbox optimization paradigm. The following is a simple 6-line usage
-example. First, we define the parameter domain and the algorithm to run. At
-every round `t`, call `algo.pull(t)` to get a point and call
-`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation
-(reward) ``` ```python3 domain = [[0, 1]] # Parameter is 1-D and between 0 and
-1 algo = T_HOO(rounds=1000, domain=domain) for t in range(1000): point =
-algo.pull(t) reward = 1 #TODO: User-defined objective returns the reward
-algo.receive_reward(t, reward) ``` More detailed examples can be found [here]
-(https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/
-index.html) ## Documentations * The most up-to-date [documentations](https://
-pyxab.readthedocs.io/) * The [roadmap](https://github.com/users/WilliamLwj/
-projects/1) for our project * Our [manuscript](https://arxiv.org/abs/
-2303.04030) for the library ## Installation To install via pip, run the
-following lines of code ```bash pip install PyXAB # normal install pip install
---upgrade PyXAB # or update if needed ``` To install via git, run the following
-lines of code ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd
-PyXAB pip install . ``` ## Features: ### *X*-armed bandit algorithms *
-Algorithm starred are meta-algorithms (wrappers) | Algorithm | Research Paper |
-Year | |-----------------------------------------------------------------------
---------------|----------------------------------------------------------------
+PyXAB contains the implementations of **10+** optimization algorithms,
+including the classic ones such as [Zooming](https://arxiv.org/pdf/
+0809.4882.pdf), [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+algos/StoSOO.py), and [HCT](https://proceedings.mlr.press/v32/azar14.html), and
+the most recent works such as [GPO](https://proceedings.mlr.press/v98/
+xuedong19a.html), [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/StroquOOL.py) and [VHCT](https://arxiv.org/abs/2106.09215). PyXAB
+also provides the most commonly-used synthetic objectives to evaluate the
+performance of different algorithms and the implementations for different
+hierarchical partitions **PyXAB is featured for:** - **User-friendly APIs,
+clear documentation, and detailed examples** - **Comprehensive library** of
+optimization algorithms, partitions and synthetic objectives - **High standard
+code quality and testing coverage** **Reminder**: The algorithms are
+maximization algorithms! ## Quick Links - [Quick Example](#Quick-Example) -
+[Documentations](#Documentations) - [Installation](#Installation) - [Features]
+(#Features) * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-
+algorithms) * [Hierarchical partition ](#Hierarchical-partition) * [Synthetic
+objectives](#Synthetic-objectives) - [Contributing](#Contributing) -
+[Citations](#Citations) ## Quick Example PyXAB follows a natural and
+straightforward API design completely aligned with the online blackbox
+optimization paradigm. The following is a simple 6-line usage example. First,
+we define the parameter domain and the algorithm to run. At every round `t`,
+call `algo.pull(t)` to get a point and call `algo.receive_reward(t, reward)` to
+give the algorithm the objective evaluation (reward) ```python3 domain = [[0,
+1]] # Parameter is 1-D and between 0 and 1 algo = T_HOO(rounds=1000,
+domain=domain) for t in range(1000): point = algo.pull(t) reward = 1 #TODO:
+User-defined objective returns the reward algo.receive_reward(t, reward) ```
+More detailed examples can be found [here](https://pyxab.readthedocs.io/en/
+latest/getting_started/auto_examples/index.html) ## Documentations * The most
+up-to-date [documentations](https://pyxab.readthedocs.io/) * The [roadmap]
+(https://github.com/users/WilliamLwj/projects/1) for our project * Our
+[manuscript](https://arxiv.org/abs/2303.04030) for the library ## Installation
+To install via pip, run the following lines of code ```bash pip install PyXAB #
+normal install pip install --upgrade PyXAB # or update if needed ``` To install
+via git, run the following lines of code ```bash git clone https://github.com/
+WilliamLwj/PyXAB.git cd PyXAB pip install . ``` ## Features: ### *X*-armed
+bandit algorithms * Algorithm starred are meta-algorithms (wrappers) |
+Algorithm | Research Paper | Year | |------------------------------------------
+-------------------------------------------|-----------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------|------| | [Zooming](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed
-Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-
-HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-
-Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) |
-[Optimistic Optimization of a Deterministic Function without the Knowledge of
-its Smoothness](https://proceedings.neurips.cc/paper/2011/file/
-7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
+------------------------------------------------------------------------|------
+| | [Zooming](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
+Zooming.py) | [Multi-Armed Bandits in Metric Spaces](https://arxiv.org/pdf/
+0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://jmlr.org/papers/v12/
+bubeck11a.html) | 2011 | | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/DOO.py) | [Optimistic Optimization of a Deterministic Function
+without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
+2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
 Optimization of a Deterministic Function without the Knowledge of its
 Smoothness](https://proceedings.neurips.cc/paper/2011/file/
 7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
 Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
 valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
@@ -127,21 +126,22 @@
 instructions](https://pyxab.readthedocs.io/en/latest/info/contributing.html)
 before submitting a pull request. ## Citations If you use our package in your
 research or projects, we kindly ask you to cite our work ```text @misc
 {Li2023PyXAB, doi = {10.48550/ARXIV.2303.04030}, url = {https://arxiv.org/abs/
 2303.04030}, author = {Li, Wenjie and Li, Haoze and Honorio, Jean and Song,
 Qifan}, title = {PyXAB -- A Python Library for $\mathcal{X}$-Armed Bandit and
 Online Blackbox Optimization Algorithms}, publisher = {arXiv}, year = {2023}, }
-``` We would appreciate it if you could cite our related works. ```text
-@article{li2021optimum, title={Optimum-statistical Collaboration Towards
-General and Efficient Black-box Optimization}, author={Li, Wenjie and Wang,
-Chi-Hua, Qifan Song and Cheng, Guang}, journal={arXiv preprint arXiv:
-2106.09215}, year={2021} } ``` ```text @misc{li2022Federated, doi = {10.48550/
-ARXIV.2205.15268}, url = {https://arxiv.org/abs/2205.15268}, author = {Li,
-Wenjie and Song, Qifan and Honorio, Jean and Lin, Guang}, title = {Federated X-
-Armed Bandit}, publisher = {arXiv}, year = {2022}, } ``` Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: Implementation :: CPython Classifier: Programming Language :: Python
-:: Implementation :: PyPy Requires-Python: >=3.6.0 Description-Content-Type:
-text/markdown
+``` We would also appreciate it if you could cite our related works. ```text
+@article{li2023optimumstatistical, title={Optimum-statistical Collaboration
+Towards General and Efficient Black-box Optimization}, author={Wenjie Li and
+Chi-Hua Wang and Guang Cheng and Qifan Song}, journal={Transactions on Machine
+Learning Research}, issn={2835-8856}, year={2023}, url={https://openreview.net/
+forum?id=ClIcmwdlxn}, note={} } ``` ```text @misc{li2022Federated, doi =
+{10.48550/ARXIV.2205.15268}, url = {https://arxiv.org/abs/2205.15268}, author =
+{Li, Wenjie and Song, Qifan and Honorio, Jean and Lin, Guang}, title =
+{Federated X-Armed Bandit}, publisher = {arXiv}, year = {2022}, } ``` Platform:
+UNKNOWN Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Programming
+Language :: Python :: Implementation :: PyPy Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
```

### Comparing `PyXAB-0.2.2/PyXAB.egg-info/SOURCES.txt` & `PyXAB-0.2.3/PyXAB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyXAB-0.2.2/README.md` & `PyXAB-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,29 +32,36 @@
 </a>
 <a href="https://github.com/psf/black" target="blank">
 <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black" />
 </a>
 </p>
 
 
-PyXAB is a Python open-source library for *X*-armed bandit algorithms, a prestigious set of optimizers for online black-box optimization, i.e., optimize an objective without gradients, also known as the continuous-arm bandit (CAB), Lipschitz bandit, 
-global optimization (GO) and bandit-based black-box optimization problems.
+PyXAB is a Python open-source library for *X*-armed bandit algorithms, a prestigious set of optimizers for online black-box optimization and 
+hyperparameter optimization.
 
 
 <p align='center'>
   <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_trajectory.gif" alt="trajectory" width="48%"/>  
   <img src="https://raw.githubusercontent.com/WilliamLwj/PyXAB/main/figs/HCT_heatmap.gif" alt="heatmap" width="48%"/>  
 </p>
 
-PyXAB contains the implementations of **more than 10 optimization algorithms**, including the classic ones such as [HOO (Bubeck et al., 2011)](https://jmlr.org/papers/v12/bubeck11a.html), 
- [StoSOO (Valko et al., 2013)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most
-recent works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL  (Bartlett et al.,2019)](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al, 2021)](https://arxiv.org/abs/2106.09215).
+PyXAB contains the implementations of **10+** optimization algorithms, including the classic ones such as [Zooming](https://arxiv.org/pdf/0809.4882.pdf), 
+ [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT](https://proceedings.mlr.press/v32/azar14.html), and the most
+recent works such as [GPO](https://proceedings.mlr.press/v98/xuedong19a.html), [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT](https://arxiv.org/abs/2106.09215).
 PyXAB also provides the most commonly-used synthetic objectives to evaluate the performance of different algorithms and the implementations for different hierarchical partitions
 
-**The algorithms are maximization algorithms!**
+**PyXAB is featured for:**
+
+- **User-friendly APIs, clear documentation, and detailed examples**
+- **Comprehensive library** of optimization algorithms, partitions and synthetic objectives
+- **High standard code quality and testing coverage**
+
+
+**Reminder**: The algorithms are maximization algorithms!
 
 ## Quick Links
 
 - [Quick Example](#Quick-Example)
 - [Documentations](#Documentations)
 - [Installation](#Installation)
 - [Features](#Features)
@@ -67,15 +74,14 @@
 ## Quick Example
 PyXAB follows a natural and straightforward API design completely aligned with the online blackbox
 optimization paradigm. The following is a simple 6-line usage example.
 
 First, we define the parameter domain and the algorithm to run. 
 At every round  `t`, call `algo.pull(t)` to get a point and call 
 `algo.receive_reward(t, reward)` to give the algorithm the objective evaluation (reward)
-```
 
 ```python3
 domain = [[0, 1]]               # Parameter is 1-D and between 0 and 1
 algo = T_HOO(rounds=1000, domain=domain) 
 for t in range(1000):
     point = algo.pull(t)
     reward = 1                  #TODO: User-defined objective returns the reward
@@ -178,22 +184,25 @@
   author = {Li, Wenjie and Li, Haoze and Honorio, Jean and Song, Qifan},
   title = {PyXAB -- A Python Library for $\mathcal{X}$-Armed Bandit and Online Blackbox Optimization Algorithms},
   publisher = {arXiv},
   year = {2023},
 }
 ```
 
-We would appreciate it if you could cite our related works.
+We would also appreciate it if you could cite our related works.
 
 ```text
-@article{li2021optimum,
-  title={Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization},
-  author={Li, Wenjie and Wang, Chi-Hua, Qifan Song and Cheng, Guang},
-  journal={arXiv preprint arXiv:2106.09215},
-  year={2021}
+@article{li2023optimumstatistical,
+    title={Optimum-statistical Collaboration Towards General and Efficient Black-box Optimization},
+    author={Wenjie Li and Chi-Hua Wang and Guang Cheng and Qifan Song},
+    journal={Transactions on Machine Learning Research},
+    issn={2835-8856},
+    year={2023},
+    url={https://openreview.net/forum?id=ClIcmwdlxn},
+    note={}
 }
 ```
 
 ```text
 @misc{li2022Federated,
   doi = {10.48550/ARXIV.2205.15268},
   url = {https://arxiv.org/abs/2205.15268},
```

#### html2text {}

```diff
@@ -1,66 +1,65 @@
  # PyXAB - Python *X*-Armed Bandit
 [PyPI_version] [https://codecov.io/gh/WilliamLwj/PyXAB/branch/main/graph/
 badge.svg?token=VACRX9AQBM] [Documentation_Status] [Code_style:_black]
 [testing] [github-PyXAB_forks] [github-PyXAB_stars] [downloads] [github-PyXAB
 license] [Code_style:_black]
 PyXAB is a Python open-source library for *X*-armed bandit algorithms, a
-prestigious set of optimizers for online black-box optimization, i.e., optimize
-an objective without gradients, also known as the continuous-arm bandit (CAB),
-Lipschitz bandit, global optimization (GO) and bandit-based black-box
-optimization problems.
+prestigious set of optimizers for online black-box optimization and
+hyperparameter optimization.
                             [trajectory] [heatmap]
-PyXAB contains the implementations of **more than 10 optimization algorithms**,
-including the classic ones such as [HOO (Bubeck et al., 2011)](https://
-jmlr.org/papers/v12/bubeck11a.html), [StoSOO (Valko et al., 2013)](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py), and [HCT (Azar et
-al., 2014)](https://proceedings.mlr.press/v32/azar14.html), and the most recent
-works such as [GPO (Shang et al., 2019)](https://proceedings.mlr.press/v98/
-xuedong19a.html), [StroquOOL (Bartlett et al.,2019)](https://github.com/
-WilliamLwj/PyXAB/blob/main/PyXAB/algos/StroquOOL.py) and [VHCT (Li et al,
-2021)](https://arxiv.org/abs/2106.09215). PyXAB also provides the most
-commonly-used synthetic objectives to evaluate the performance of different
-algorithms and the implementations for different hierarchical partitions **The
-algorithms are maximization algorithms!** ## Quick Links - [Quick Example]
-(#Quick-Example) - [Documentations](#Documentations) - [Installation]
-(#Installation) - [Features](#Features) * [*X*-armed bandit algorithms]
-(#Stochastic-X-armed-bandit-algorithms) * [Hierarchical partition ]
-(#Hierarchical-partition) * [Synthetic objectives](#Synthetic-objectives) -
-[Contributing](#Contributing) - [Citations](#Citations) ## Quick Example PyXAB
-follows a natural and straightforward API design completely aligned with the
-online blackbox optimization paradigm. The following is a simple 6-line usage
-example. First, we define the parameter domain and the algorithm to run. At
-every round `t`, call `algo.pull(t)` to get a point and call
-`algo.receive_reward(t, reward)` to give the algorithm the objective evaluation
-(reward) ``` ```python3 domain = [[0, 1]] # Parameter is 1-D and between 0 and
-1 algo = T_HOO(rounds=1000, domain=domain) for t in range(1000): point =
-algo.pull(t) reward = 1 #TODO: User-defined objective returns the reward
-algo.receive_reward(t, reward) ``` More detailed examples can be found [here]
-(https://pyxab.readthedocs.io/en/latest/getting_started/auto_examples/
-index.html) ## Documentations * The most up-to-date [documentations](https://
-pyxab.readthedocs.io/) * The [roadmap](https://github.com/users/WilliamLwj/
-projects/1) for our project * Our [manuscript](https://arxiv.org/abs/
-2303.04030) for the library ## Installation To install via pip, run the
-following lines of code ```bash pip install PyXAB # normal install pip install
---upgrade PyXAB # or update if needed ``` To install via git, run the following
-lines of code ```bash git clone https://github.com/WilliamLwj/PyXAB.git cd
-PyXAB pip install . ``` ## Features: ### *X*-armed bandit algorithms *
-Algorithm starred are meta-algorithms (wrappers) | Algorithm | Research Paper |
-Year | |-----------------------------------------------------------------------
---------------|----------------------------------------------------------------
+PyXAB contains the implementations of **10+** optimization algorithms,
+including the classic ones such as [Zooming](https://arxiv.org/pdf/
+0809.4882.pdf), [StoSOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/
+algos/StoSOO.py), and [HCT](https://proceedings.mlr.press/v32/azar14.html), and
+the most recent works such as [GPO](https://proceedings.mlr.press/v98/
+xuedong19a.html), [StroquOOL](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/StroquOOL.py) and [VHCT](https://arxiv.org/abs/2106.09215). PyXAB
+also provides the most commonly-used synthetic objectives to evaluate the
+performance of different algorithms and the implementations for different
+hierarchical partitions **PyXAB is featured for:** - **User-friendly APIs,
+clear documentation, and detailed examples** - **Comprehensive library** of
+optimization algorithms, partitions and synthetic objectives - **High standard
+code quality and testing coverage** **Reminder**: The algorithms are
+maximization algorithms! ## Quick Links - [Quick Example](#Quick-Example) -
+[Documentations](#Documentations) - [Installation](#Installation) - [Features]
+(#Features) * [*X*-armed bandit algorithms](#Stochastic-X-armed-bandit-
+algorithms) * [Hierarchical partition ](#Hierarchical-partition) * [Synthetic
+objectives](#Synthetic-objectives) - [Contributing](#Contributing) -
+[Citations](#Citations) ## Quick Example PyXAB follows a natural and
+straightforward API design completely aligned with the online blackbox
+optimization paradigm. The following is a simple 6-line usage example. First,
+we define the parameter domain and the algorithm to run. At every round `t`,
+call `algo.pull(t)` to get a point and call `algo.receive_reward(t, reward)` to
+give the algorithm the objective evaluation (reward) ```python3 domain = [[0,
+1]] # Parameter is 1-D and between 0 and 1 algo = T_HOO(rounds=1000,
+domain=domain) for t in range(1000): point = algo.pull(t) reward = 1 #TODO:
+User-defined objective returns the reward algo.receive_reward(t, reward) ```
+More detailed examples can be found [here](https://pyxab.readthedocs.io/en/
+latest/getting_started/auto_examples/index.html) ## Documentations * The most
+up-to-date [documentations](https://pyxab.readthedocs.io/) * The [roadmap]
+(https://github.com/users/WilliamLwj/projects/1) for our project * Our
+[manuscript](https://arxiv.org/abs/2303.04030) for the library ## Installation
+To install via pip, run the following lines of code ```bash pip install PyXAB #
+normal install pip install --upgrade PyXAB # or update if needed ``` To install
+via git, run the following lines of code ```bash git clone https://github.com/
+WilliamLwj/PyXAB.git cd PyXAB pip install . ``` ## Features: ### *X*-armed
+bandit algorithms * Algorithm starred are meta-algorithms (wrappers) |
+Algorithm | Research Paper | Year | |------------------------------------------
+-------------------------------------------|-----------------------------------
 -------------------------------------------------------------------------------
--------------------------------------------|------| | [Zooming](https://
-github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/Zooming.py) | [Multi-Armed
-Bandits in Metric Spaces](https://arxiv.org/pdf/0809.4882.pdf) | 2008 | | [T-
-HOO](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/HOO.py) | [*X*-
-Armed Bandit](https://jmlr.org/papers/v12/bubeck11a.html) | 2011 | | [DOO]
-(https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/DOO.py) |
-[Optimistic Optimization of a Deterministic Function without the Knowledge of
-its Smoothness](https://proceedings.neurips.cc/paper/2011/file/
-7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
+------------------------------------------------------------------------|------
+| | [Zooming](https://github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/
+Zooming.py) | [Multi-Armed Bandits in Metric Spaces](https://arxiv.org/pdf/
+0809.4882.pdf) | 2008 | | [T-HOO](https://github.com/WilliamLwj/PyXAB/blob/
+main/PyXAB/algos/HOO.py) | [*X*-Armed Bandit](https://jmlr.org/papers/v12/
+bubeck11a.html) | 2011 | | [DOO](https://github.com/WilliamLwj/PyXAB/blob/main/
+PyXAB/algos/DOO.py) | [Optimistic Optimization of a Deterministic Function
+without the Knowledge of its Smoothness](https://proceedings.neurips.cc/paper/
+2011/file/7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [SOO](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/SOO.py) | [Optimistic
 Optimization of a Deterministic Function without the Knowledge of its
 Smoothness](https://proceedings.neurips.cc/paper/2011/file/
 7e889fb76e0e07c11733550f2a6c7a5a-Paper.pdf) | 2011 | | [StoSOO](https://
 github.com/WilliamLwj/PyXAB/blob/main/PyXAB/algos/StoSOO.py) | [Stochastic
 Simultaneous Optimistic Optimization](http://proceedings.mlr.press/v28/
 valko13.pdf) | 2013 | | [HCT](https://github.com/WilliamLwj/PyXAB/blob/main/
@@ -123,15 +122,16 @@
 instructions](https://pyxab.readthedocs.io/en/latest/info/contributing.html)
 before submitting a pull request. ## Citations If you use our package in your
 research or projects, we kindly ask you to cite our work ```text @misc
 {Li2023PyXAB, doi = {10.48550/ARXIV.2303.04030}, url = {https://arxiv.org/abs/
 2303.04030}, author = {Li, Wenjie and Li, Haoze and Honorio, Jean and Song,
 Qifan}, title = {PyXAB -- A Python Library for $\mathcal{X}$-Armed Bandit and
 Online Blackbox Optimization Algorithms}, publisher = {arXiv}, year = {2023}, }
-``` We would appreciate it if you could cite our related works. ```text
-@article{li2021optimum, title={Optimum-statistical Collaboration Towards
-General and Efficient Black-box Optimization}, author={Li, Wenjie and Wang,
-Chi-Hua, Qifan Song and Cheng, Guang}, journal={arXiv preprint arXiv:
-2106.09215}, year={2021} } ``` ```text @misc{li2022Federated, doi = {10.48550/
-ARXIV.2205.15268}, url = {https://arxiv.org/abs/2205.15268}, author = {Li,
-Wenjie and Song, Qifan and Honorio, Jean and Lin, Guang}, title = {Federated X-
-Armed Bandit}, publisher = {arXiv}, year = {2022}, } ```
+``` We would also appreciate it if you could cite our related works. ```text
+@article{li2023optimumstatistical, title={Optimum-statistical Collaboration
+Towards General and Efficient Black-box Optimization}, author={Wenjie Li and
+Chi-Hua Wang and Guang Cheng and Qifan Song}, journal={Transactions on Machine
+Learning Research}, issn={2835-8856}, year={2023}, url={https://openreview.net/
+forum?id=ClIcmwdlxn}, note={} } ``` ```text @misc{li2022Federated, doi =
+{10.48550/ARXIV.2205.15268}, url = {https://arxiv.org/abs/2205.15268}, author =
+{Li, Wenjie and Song, Qifan and Honorio, Jean and Lin, Guang}, title =
+{Federated X-Armed Bandit}, publisher = {arXiv}, year = {2022}, } ```
```

### Comparing `PyXAB-0.2.2/setup.py` & `PyXAB-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyXAB'
 DESCRIPTION = 'PyXAB - A Python Library for X-Armed Bandit and Online Blackbox Optimization Algorithms.'
 URL = 'https://github.com/WilliamLwj/PyXAB'
 EMAIL = 'lil3549@purdue.edu'
 AUTHOR = 'Wenjie Li, Haoze Li'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy>=1.20.3',
     'matplotlib',
     # 'requests', 'maya', 'records',
 ]
```

