# Comparing `tmp/veta-0.7.6.tar.gz` & `tmp/veta-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veta-0.7.6.tar", last modified: Fri Apr 28 14:56:22 2023, max compression
+gzip compressed data, was "veta-0.7.7.tar", last modified: Sun Jun  4 20:58:26 2023, max compression
```

## Comparing `veta-0.7.6.tar` & `veta-0.7.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.961646 veta-0.7.6/
--rw-r--r--   0 pbarbosa   (503) staff       (20)      155 2022-06-29 16:21:39.000000 veta-0.7.6/.gitignore
--rw-r--r--   0 pbarbosa   (503) staff       (20)      600 2023-01-13 02:44:49.000000 veta-0.7.6/Dockerfile
--rw-r--r--   0 pbarbosa   (503) staff       (20)    35149 2022-06-18 20:35:59.000000 veta-0.7.6/LICENSE
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34987 2023-04-28 14:56:22.960880 veta-0.7.6/PKG-INFO
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34853 2022-12-29 20:23:55.000000 veta-0.7.6/README.md
--rw-r--r--   0 pbarbosa   (503) staff       (20)      484 2022-12-30 18:52:40.000000 veta-0.7.6/conda_environment.yml
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1026 2023-04-28 14:55:43.000000 veta-0.7.6/pyproject.toml
--rw-r--r--   0 pbarbosa   (503) staff       (20)       38 2023-04-28 14:56:22.962058 veta-0.7.6/setup.cfg
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.886912 veta-0.7.6/src/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.6/src/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    24435 2023-04-28 14:55:43.000000 veta-0.7.6/src/base.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    22309 2023-01-13 02:18:40.000000 veta-0.7.6/src/benchmark.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.888311 veta-0.7.6/src/config/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:06:31.000000 veta-0.7.6/src/config/__init__.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.931448 veta-0.7.6/src/config/example_imgs/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/.gitkeep
--rw-r--r--   0 pbarbosa   (503) staff       (20)    41469 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/benchmark_af.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   176304 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/benchmark_dist.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   530128 2022-06-29 16:21:39.000000 veta-0.7.6/src/config/example_imgs/benchmark_performance.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   105415 2022-06-29 16:21:39.000000 veta-0.7.6/src/config/example_imgs/benchmark_thresholds.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   187077 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/heatmap.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   236867 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/inspect_ratios.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   149613 2022-06-29 16:21:39.000000 veta-0.7.6/src/config/example_imgs/inspect_ratios2.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)    51272 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/logo.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   175417 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/ml_fi.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   253954 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/ml_performance.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   183865 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/pearson_corr.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   391054 2022-12-29 18:11:14.000000 veta-0.7.6/src/config/example_imgs/per_bin_score.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   510397 2022-12-29 18:11:14.000000 veta-0.7.6/src/config/example_imgs/per_bin_score_split_ss.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)  1012850 2022-06-18 21:05:58.000000 veta-0.7.6/src/config/example_imgs/roc_analysis.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)   642538 2022-06-29 16:21:39.000000 veta-0.7.6/src/config/example_imgs/roc_curves.png
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1352 2023-04-26 18:03:35.000000 veta-0.7.6/src/config/tools_config.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)    14407 2023-04-28 14:55:43.000000 veta-0.7.6/src/interrogate.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.942639 veta-0.7.6/src/plots/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.6/src/plots/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    23298 2023-02-08 17:08:39.000000 veta-0.7.6/src/plots/plots_benchmark_mode.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     8896 2023-04-28 14:55:43.000000 veta-0.7.6/src/plots/plots_interrogate_mode.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15452 2023-02-08 17:08:39.000000 veta-0.7.6/src/plots/plots_intronic_analysis.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     6557 2022-12-29 18:11:14.000000 veta-0.7.6/src/plots/plots_machine_learning.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     5079 2022-06-18 21:06:31.000000 veta-0.7.6/src/plots/plots_threshold_analysis.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)      822 2022-06-18 21:05:58.000000 veta-0.7.6/src/plots/plots_utils.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.949557 veta-0.7.6/src/predictions/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.6/src/predictions/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1001 2022-07-06 23:37:56.000000 veta-0.7.6/src/predictions/apply.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     9437 2022-12-29 18:11:14.000000 veta-0.7.6/src/predictions/filters.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    16825 2022-12-30 18:52:40.000000 veta-0.7.6/src/predictions/introns.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    21103 2022-12-29 18:11:14.000000 veta-0.7.6/src/predictions/metapredictions.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     7359 2022-08-25 13:25:47.000000 veta-0.7.6/src/predictions/metrics.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15342 2022-12-29 18:11:14.000000 veta-0.7.6/src/predictions/thresholds.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    11304 2022-12-29 18:11:14.000000 veta-0.7.6/src/predictions/utils_classifiers.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.955731 veta-0.7.6/src/preprocessing/
--rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.6/src/preprocessing/__init__.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     4279 2022-07-06 23:37:56.000000 veta-0.7.6/src/preprocessing/clinvar.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     6443 2022-10-07 22:13:57.000000 veta-0.7.6/src/preprocessing/location.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     3400 2022-06-18 21:06:31.000000 veta-0.7.6/src/preprocessing/osutils.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)     5996 2022-08-17 17:31:38.000000 veta-0.7.6/src/preprocessing/tables.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    22594 2023-04-28 14:55:43.000000 veta-0.7.6/src/preprocessing/utils_tools.py
--rw-r--r--   0 pbarbosa   (503) staff       (20)    15511 2022-12-29 18:11:14.000000 veta-0.7.6/src/preprocessing/vcf.py
-drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-04-28 14:56:22.960157 veta-0.7.6/src/veta.egg-info/
--rw-r--r--   0 pbarbosa   (503) staff       (20)    34987 2023-04-28 14:56:22.000000 veta-0.7.6/src/veta.egg-info/PKG-INFO
--rw-r--r--   0 pbarbosa   (503) staff       (20)     1728 2023-04-28 14:56:22.000000 veta-0.7.6/src/veta.egg-info/SOURCES.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)        1 2023-04-28 14:56:22.000000 veta-0.7.6/src/veta.egg-info/dependency_links.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)       35 2023-04-28 14:56:22.000000 veta-0.7.6/src/veta.egg-info/entry_points.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)      229 2023-04-28 14:56:22.000000 veta-0.7.6/src/veta.egg-info/requires.txt
--rw-r--r--   0 pbarbosa   (503) staff       (20)       80 2023-04-28 14:56:22.000000 veta-0.7.6/src/veta.egg-info/top_level.txt
--rwxr-xr-x   0 pbarbosa   (503) staff       (20)    12813 2022-12-29 18:11:14.000000 veta-0.7.6/src/veta.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.973071 veta-0.7.7/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      155 2022-06-29 16:21:39.000000 veta-0.7.7/.gitignore
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      600 2023-01-13 02:44:49.000000 veta-0.7.7/Dockerfile
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35149 2022-06-18 20:35:59.000000 veta-0.7.7/LICENSE
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35110 2023-06-04 20:58:26.971825 veta-0.7.7/PKG-INFO
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    34977 2023-06-04 20:46:42.000000 veta-0.7.7/README.md
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      484 2022-12-30 18:52:40.000000 veta-0.7.7/conda_environment.yml
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1026 2023-06-04 20:46:42.000000 veta-0.7.7/pyproject.toml
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       38 2023-06-04 20:58:26.973418 veta-0.7.7/setup.cfg
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.836107 veta-0.7.7/src/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    24480 2023-06-04 20:46:42.000000 veta-0.7.7/src/base.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    22309 2023-01-13 02:18:40.000000 veta-0.7.7/src/benchmark.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.838228 veta-0.7.7/src/config/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:06:31.000000 veta-0.7.7/src/config/__init__.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.913746 veta-0.7.7/src/config/example_imgs/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/.gitkeep
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    41469 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/benchmark_af.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   176304 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/benchmark_dist.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   530128 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/benchmark_performance.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   105415 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/benchmark_thresholds.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   187077 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/heatmap.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   236867 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/inspect_ratios.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   149613 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/inspect_ratios2.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    51272 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/logo.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   175417 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/ml_fi.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   253954 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/ml_performance.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   183865 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/pearson_corr.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   391054 2022-12-29 18:11:14.000000 veta-0.7.7/src/config/example_imgs/per_bin_score.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   510397 2022-12-29 18:11:14.000000 veta-0.7.7/src/config/example_imgs/per_bin_score_split_ss.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)  1012850 2022-06-18 21:05:58.000000 veta-0.7.7/src/config/example_imgs/roc_analysis.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)   642538 2022-06-29 16:21:39.000000 veta-0.7.7/src/config/example_imgs/roc_curves.png
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1381 2023-06-04 20:46:42.000000 veta-0.7.7/src/config/tools_config.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    14407 2023-04-28 14:55:43.000000 veta-0.7.7/src/interrogate.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.933590 veta-0.7.7/src/plots/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/plots/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    23298 2023-05-17 14:26:55.000000 veta-0.7.7/src/plots/plots_benchmark_mode.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     8896 2023-04-28 14:55:43.000000 veta-0.7.7/src/plots/plots_interrogate_mode.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15452 2023-02-08 17:08:39.000000 veta-0.7.7/src/plots/plots_intronic_analysis.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     6557 2022-12-29 18:11:14.000000 veta-0.7.7/src/plots/plots_machine_learning.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     5079 2022-06-18 21:06:31.000000 veta-0.7.7/src/plots/plots_threshold_analysis.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      822 2022-06-18 21:05:58.000000 veta-0.7.7/src/plots/plots_utils.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.950294 veta-0.7.7/src/predictions/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/predictions/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1001 2023-05-24 00:01:45.000000 veta-0.7.7/src/predictions/apply.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     9481 2023-06-04 20:46:42.000000 veta-0.7.7/src/predictions/filters.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    16825 2022-12-30 18:52:40.000000 veta-0.7.7/src/predictions/introns.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    21143 2023-06-04 20:46:42.000000 veta-0.7.7/src/predictions/metapredictions.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     7359 2022-08-25 13:25:47.000000 veta-0.7.7/src/predictions/metrics.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15342 2022-12-29 18:11:14.000000 veta-0.7.7/src/predictions/thresholds.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    11304 2022-12-29 18:11:14.000000 veta-0.7.7/src/predictions/utils_classifiers.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.963503 veta-0.7.7/src/preprocessing/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        0 2022-06-18 21:05:58.000000 veta-0.7.7/src/preprocessing/__init__.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     4279 2022-07-06 23:37:56.000000 veta-0.7.7/src/preprocessing/clinvar.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     6443 2023-06-04 20:46:42.000000 veta-0.7.7/src/preprocessing/location.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     3400 2022-06-18 21:06:31.000000 veta-0.7.7/src/preprocessing/osutils.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     5996 2022-08-17 17:31:38.000000 veta-0.7.7/src/preprocessing/tables.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    22802 2023-06-04 20:46:42.000000 veta-0.7.7/src/preprocessing/utils_tools.py
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    15511 2022-12-29 18:11:14.000000 veta-0.7.7/src/preprocessing/vcf.py
+drwxr-xr-x   0 pbarbosa   (503) staff       (20)        0 2023-06-04 20:58:26.969899 veta-0.7.7/src/veta.egg-info/
+-rw-r--r--   0 pbarbosa   (503) staff       (20)    35110 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/PKG-INFO
+-rw-r--r--   0 pbarbosa   (503) staff       (20)     1728 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/SOURCES.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)        1 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/dependency_links.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       35 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/entry_points.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)      229 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/requires.txt
+-rw-r--r--   0 pbarbosa   (503) staff       (20)       80 2023-06-04 20:58:26.000000 veta-0.7.7/src/veta.egg-info/top_level.txt
+-rwxr-xr-x   0 pbarbosa   (503) staff       (20)    12813 2022-12-29 18:11:14.000000 veta-0.7.7/src/veta.py
```

### Comparing `veta-0.7.6/Dockerfile` & `veta-0.7.7/Dockerfile`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/LICENSE` & `veta-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/PKG-INFO` & `veta-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veta
-Version: 0.7.6
+Version: 0.7.7
 Summary: Simple variant prediction evaluation
 Author-email: Pedro Barbosa <psbpedrobarbosa@gmail.com>
 License: https://opensource.org/licenses/GPL-3.0
 Project-URL: homepage, https://github.com/PedroBarbosa/VETA
 Project-URL: repository, https://github.com/PedroBarbosa/VETA
 Project-URL: documentation, https://github.com/PedroBarbosa/VETA
 Requires-Python: ~=3.8
@@ -273,15 +273,15 @@
 |				                          | FunSeq2	          | > 1.5		             | Yes		                   | vcfanno       |
 |				                          | CAPICE	          | > 0.02               | Yes		                   | vcfanno       |
 | Fitness measurement             | CADD_v1.5         | > 15                 | Yes                       | vcfanno       |
 |                                 | CADD-Splice       | > 15                 | Yes                       | vcfanno       |
 |                                 | DANN              | > 0.9                | Yes                       | vcfanno       |
 |                                 | fitCons           | > 0.4                | No                        | vcfanno       |
 |                                 | LINSIGHT          | > 0.056              | Yes                       | vcfanno       |
-| Splicing                        | MaxEntScan        | \|MaxEntScan_diff\|> 1 | No                      | kipoi         |
+| Splicing                        | MaxEntScan        | \|MaxEntScan_diff\|> 3 | No                      | VEP           |
 |                                 | dbscSNV           | > 0.6                | Yes                       | VEP           |
 |                                 | SPIDEX            | \|dpsi_zscore\| > 2  | No                        | vcfanno       |
 |                                 | TraP              | > 0.221 for coding, 0.174 for intronic | Yes     | vcfanno       |
 |                                 | SpliceAI          | > 0.2                | No                        | vcfanno       |
 | 		                            | HAL               | \|deltaPSI\| > 5	   | No			                   | kipoi         |
 |                                 | S-CAP             | Different thresholds | Yes                       | vcfanno       |
 |                                 | MMSplice          | \|deltaLogitPSI\| > 2| No                        | kipoi         |
@@ -291,14 +291,15 @@
 |                                 | IntSplice2        | > 0.5                | Yes                       | vcfanno       |
 |                                 | MLCsplice         | > 0.5                | Yes                       | vcfanno       |
 |                                 | SQUIRLS           | > 0.074              |Yes                        | model_inference |
 |                                 | CI-SpliceAI       | > 0.190              | No                        | model_inference |
 |                                 | Pangolin          | \|splicing_diff\| > 0.2 | No                     | model_inference |
 |                                 | SPiP              | > 0.452              | Yes                       | model_inference |
 |                                 | AbSplice-DNA      | > 0.01               | Yes                       | vcfanno       |
+|                                 | PDIVAS            | > 0.151              | Yes                       | vcfanno       |
 |                                 | LaBranchoR        | > 0.1                | Yes                       | kipoi         |
 <a name="manual_config"></a>
 #### Manual config file
 
 This config file maps the tool name to the corresponding annotation field in the VCF. It allows adding custom methods, as long as the field exists in the VCF.
 The config file must be tab-delimited just like [this one](https://github.com/PedroBarbosa/VETA/blob/master/src/config/tools_config.txt).
 Lines starting with '#' are skipped. For tools with native support within VETA (listed in the table above, where the tool name must be matched), only the 2 columns are required. For custom methods, additional columns must be set. Column specifications are as follows:
```

### Comparing `veta-0.7.6/README.md` & `veta-0.7.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 |				                          | FunSeq2	          | > 1.5		             | Yes		                   | vcfanno       |
 |				                          | CAPICE	          | > 0.02               | Yes		                   | vcfanno       |
 | Fitness measurement             | CADD_v1.5         | > 15                 | Yes                       | vcfanno       |
 |                                 | CADD-Splice       | > 15                 | Yes                       | vcfanno       |
 |                                 | DANN              | > 0.9                | Yes                       | vcfanno       |
 |                                 | fitCons           | > 0.4                | No                        | vcfanno       |
 |                                 | LINSIGHT          | > 0.056              | Yes                       | vcfanno       |
-| Splicing                        | MaxEntScan        | \|MaxEntScan_diff\|> 1 | No                      | kipoi         |
+| Splicing                        | MaxEntScan        | \|MaxEntScan_diff\|> 3 | No                      | VEP           |
 |                                 | dbscSNV           | > 0.6                | Yes                       | VEP           |
 |                                 | SPIDEX            | \|dpsi_zscore\| > 2  | No                        | vcfanno       |
 |                                 | TraP              | > 0.221 for coding, 0.174 for intronic | Yes     | vcfanno       |
 |                                 | SpliceAI          | > 0.2                | No                        | vcfanno       |
 | 		                            | HAL               | \|deltaPSI\| > 5	   | No			                   | kipoi         |
 |                                 | S-CAP             | Different thresholds | Yes                       | vcfanno       |
 |                                 | MMSplice          | \|deltaLogitPSI\| > 2| No                        | kipoi         |
@@ -278,14 +278,15 @@
 |                                 | IntSplice2        | > 0.5                | Yes                       | vcfanno       |
 |                                 | MLCsplice         | > 0.5                | Yes                       | vcfanno       |
 |                                 | SQUIRLS           | > 0.074              |Yes                        | model_inference |
 |                                 | CI-SpliceAI       | > 0.190              | No                        | model_inference |
 |                                 | Pangolin          | \|splicing_diff\| > 0.2 | No                     | model_inference |
 |                                 | SPiP              | > 0.452              | Yes                       | model_inference |
 |                                 | AbSplice-DNA      | > 0.01               | Yes                       | vcfanno       |
+|                                 | PDIVAS            | > 0.151              | Yes                       | vcfanno       |
 |                                 | LaBranchoR        | > 0.1                | Yes                       | kipoi         |
 <a name="manual_config"></a>
 #### Manual config file
 
 This config file maps the tool name to the corresponding annotation field in the VCF. It allows adding custom methods, as long as the field exists in the VCF.
 The config file must be tab-delimited just like [this one](https://github.com/PedroBarbosa/VETA/blob/master/src/config/tools_config.txt).
 Lines starting with '#' are skipped. For tools with native support within VETA (listed in the table above, where the tool name must be matched), only the 2 columns are required. For custom methods, additional columns must be set. Column specifications are as follows:
```

### Comparing `veta-0.7.6/pyproject.toml` & `veta-0.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "veta"
 description = "Simple variant prediction evaluation"
 authors = [
     {name = "Pedro Barbosa", email = "psbpedrobarbosa@gmail.com"},
 ]
 
-version = "0.7.6"
+version = "0.7.7"
 readme = "README.md"
 requires-python = "~=3.8"
 dependencies = [
     "matplotlib==3.5.1",
     "numpy==1.23.5",
     "pandas==1.4.2",
     "seaborn==0.11.2",
```

### Comparing `veta-0.7.6/src/base.py` & `veta-0.7.7/src/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 from collections import defaultdict
-from posixpath import split
 from typing import Union, List, Tuple
 
 import hgvs
 import pandas as pd
 from importlib import resources
 import config
 
@@ -344,14 +343,15 @@
             "ConSpliceML": available_functions['conspliceml'],
             "IntSplice2": available_functions['to_numeric'],
             "CI-SpliceAI": available_functions['spliceai'],
             "Pangolin": available_functions['pangolin'],
             "SPiP": available_functions['spip'],
             "MLCsplice": available_functions['top_max'],
             "AbSplice-DNA": available_functions['absplice_dna'],
+            "PDIVAS": available_functions['conspliceml_like'],
             "LaBranchoR": available_functions['labranchor']
         }
 
         _functions_that_require_loc = ["process_trap"]
         _functions_that_require_symbol = ["process_spliceai", "process_conspliceml"]
         _absent_tools = {_tool: info for _tool, info in self.tools_config.items()
                          if _tool not in clean_functions.keys()}
@@ -429,15 +429,15 @@
                                  "ClinPred", "MISTIC",
                                  "EVE", "EVE_class20", "EVE_class50","EVE_class90",                             
                                  "CardioBoost", "CardioVAI",
                                  "fitCons", "LINSIGHT", "ReMM", "GWAVA", "FATHMM-MKL",
                                  "Eigen", "FunSeq2", "CADD_v1.5", "CADD-Splice", "DANN", "CAPICE",
                                  "HAL", "SPIDEX", "dbscSNV", "MaxEntScan", "SpliceAI", "S-CAP", "ConSpliceML",
                                  "TraP", "MMSplice", "SQUIRLS", "IntSplice2", "kipoiSplice4", "kipoiSplice4_cons",
-                                 "CI-SpliceAI", "Pangolin", "SPiP", "LaBranchoR", "MLCsplice", "AbSplice-DNA"]
+                                 "CI-SpliceAI", "Pangolin", "SPiP", "LaBranchoR", "MLCsplice", "PDIVAS", "AbSplice-DNA"]
 
         AVAILABLE_SCOPES = ["Protein", "Conservation", "Whole_genome", "Splicing"]
         AVAILABLE_FUNCTIONS = ['to_numeric', 'top_max', 'top_min', 'top_min_abs',
                                'categorical_to_numeric', 'kipoi_like', 'carol_like', 
                                'trap', 'scap', 'conspliceml', 'conspliceml_like',
                                'spliceai', 'ci_spliceai',
                                'pangolin', 'spip', 'labranchor']
```

### Comparing `veta-0.7.6/src/benchmark.py` & `veta-0.7.7/src/benchmark.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/benchmark_af.png` & `veta-0.7.7/src/config/example_imgs/benchmark_af.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/benchmark_dist.png` & `veta-0.7.7/src/config/example_imgs/benchmark_dist.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/benchmark_performance.png` & `veta-0.7.7/src/config/example_imgs/benchmark_performance.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/benchmark_thresholds.png` & `veta-0.7.7/src/config/example_imgs/benchmark_thresholds.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/heatmap.png` & `veta-0.7.7/src/config/example_imgs/heatmap.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/inspect_ratios.png` & `veta-0.7.7/src/config/example_imgs/inspect_ratios.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/inspect_ratios2.png` & `veta-0.7.7/src/config/example_imgs/inspect_ratios2.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/logo.png` & `veta-0.7.7/src/config/example_imgs/logo.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/ml_fi.png` & `veta-0.7.7/src/config/example_imgs/ml_fi.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/ml_performance.png` & `veta-0.7.7/src/config/example_imgs/ml_performance.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/pearson_corr.png` & `veta-0.7.7/src/config/example_imgs/pearson_corr.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/per_bin_score.png` & `veta-0.7.7/src/config/example_imgs/per_bin_score.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/per_bin_score_split_ss.png` & `veta-0.7.7/src/config/example_imgs/per_bin_score_split_ss.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/roc_analysis.png` & `veta-0.7.7/src/config/example_imgs/roc_analysis.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/example_imgs/roc_curves.png` & `veta-0.7.7/src/config/example_imgs/roc_curves.png`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/config/tools_config.txt` & `veta-0.7.7/src/config/tools_config.txt`

 * *Files 11% similar despite different names*

```diff
@@ -52,20 +52,21 @@
 
 # Splicing
 SQUIRLS	SQUIRLS_SCORE
 IntSplice2	IntSplice2
 HAL	HAL_DIFF
 SPIDEX	dpsi_zscore
 dbscSNV	ada_score,rf_score
-MaxEntScan	maxentscan_5,maxentscan_3
+MaxEntScan	MES-SWA_acceptor_diff,MES-SWA_donor_diff
 SpliceAI	SpliceAI,SpliceAI_ind
 S-CAP	SCAP
 TraP	TraP
 ConSpliceML	ConSpliceML
 MMSplice	mmsplice_deltaPSI
 kipoiSplice4	kipoisplice_4
 CI-SpliceAI	CI-SpliceAI
 Pangolin	Pangolin
 SPiP	SPiP
 MLCsplice	MLCsplice
 AbSplice-DNA	AbSplice_DNA
+PDIVAS	PDIVAS
 LaBranchoR	labranchoR
```

### Comparing `veta-0.7.6/src/interrogate.py` & `veta-0.7.7/src/interrogate.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/plots/plots_benchmark_mode.py` & `veta-0.7.7/src/plots/plots_benchmark_mode.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/plots/plots_interrogate_mode.py` & `veta-0.7.7/src/plots/plots_interrogate_mode.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/plots/plots_intronic_analysis.py` & `veta-0.7.7/src/plots/plots_intronic_analysis.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/plots/plots_machine_learning.py` & `veta-0.7.7/src/plots/plots_machine_learning.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/plots/plots_threshold_analysis.py` & `veta-0.7.7/src/plots/plots_threshold_analysis.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/plots/plots_utils.py` & `veta-0.7.7/src/plots/plots_utils.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/predictions/apply.py` & `veta-0.7.7/src/predictions/apply.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/predictions/filters.py` & `veta-0.7.7/src/predictions/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         ('SQUIRLS', '>', 0.074, 'Splicing'), #CI-SpliceAI paper
         ('IntSplice2', '>', 0.5, 'Splicing'),
         ('CI-SpliceAI', '>', 0.190, 'Splicing'),
         ('Pangolin', '>', 0.2, 'Splicing'),
         ('SPiP', '>', 0.452, 'Splicing'),
         ('MLCsplice', '>', 0.5, 'Splicing'),
         ('AbSplice-DNA', '>', 0.01, 'Splicing'),
+        ('PDIVAS', '>', 0.151, 'Splicing'),
         ('LaBranchoR', '>', 0.1, 'Splicing')
     ]
 
     DEFAULT_TOOLS = [t[0] for t in _default_list]
     _updated_list = []
     for _tool, info in config_dict.items():
```

### Comparing `veta-0.7.6/src/predictions/introns.py` & `veta-0.7.7/src/predictions/introns.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/predictions/metapredictions.py` & `veta-0.7.7/src/predictions/metapredictions.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         :param bool undersample: Undersample data based on majority class
         (useful for unbalanced data)
         :param bool only_numeric: Include only numerical features (tool scores).
             Default: `False`. If `True`, categorical and boolean features
             will not be included.
         """
         # Remove useless columns
-        useless_cols = ['index', 'chr', 'pos', 'ref', 'alt', 'id', 'HGVSc']
-
+        useless_cols = [c for c in ['index', 'chr', 'pos', 'ref', 'alt', 'id', 'HGVSc'] if c in df.columns]
+        
         df = df.drop(useless_cols, axis=1)
 
         self.label_fields = ['label']  # 'outcome' would also work
         self.categorical_fields = ['type', 'subtype', 'Gene', 'Consequence']
 
         self.out_dir = out_dir
         self.location = location
```

### Comparing `veta-0.7.6/src/predictions/metrics.py` & `veta-0.7.7/src/predictions/metrics.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/predictions/thresholds.py` & `veta-0.7.7/src/predictions/thresholds.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/predictions/utils_classifiers.py` & `veta-0.7.7/src/predictions/utils_classifiers.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/preprocessing/clinvar.py` & `veta-0.7.7/src/preprocessing/clinvar.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/preprocessing/location.py` & `veta-0.7.7/src/preprocessing/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,23 +107,23 @@
 
     try:
         return CONSEQUENCES[conseq][idx]
     
     except KeyError:
         raise ValueError("Consequence not registered. {}".format(conseq))
 
-ranges_split_at_ss = [(0, 2, '1-2'),
+ranges_split_at_ss = [(1, 2, '1-2'),
           (3, 10, '3-10'),
           (11, 40, '11-40'),
           (41, 200, '41-200'),
           (201, 500, '201-500'),
           (501, 1000, '501-1000'),
           (1001, 5000000, '1000+')]
 
-ranges = [(0, 10, '1-10'),
+ranges = [(1, 10, '1-10'),
           (11, 40, '11-40'),
           (41, 200, '41-200'),
           (201, 500, '201-500'),
           (501, 1000, '501-1000'),
           (1001, 5000000, '1000+')]
```

### Comparing `veta-0.7.6/src/preprocessing/osutils.py` & `veta-0.7.7/src/preprocessing/osutils.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/preprocessing/tables.py` & `veta-0.7.7/src/preprocessing/tables.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/preprocessing/utils_tools.py` & `veta-0.7.7/src/preprocessing/utils_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,27 +59,29 @@
                          'config file in a tool that expects a '
                          'single field with a single numeric value. '
                          'Error: {}'.format(preds))
 
     _p = preds[0]
     if isinstance(_p, float):
         score = round(_p, 4)
-
+    elif isinstance(_p, int):
+        return abs(_p) if absolute else _p
     else:
         try:
             if any([k in _p for k in [',', '|', '&']]):
                 raise ValueError('Multiple predictions were found '
                                  'for a tool that expects a single '
                                  'numeric value: {}'.format(_p))
 
             score = round(float(_p), 4)
 
         except (TypeError, ValueError):
             return np.nan
 
+  
     return abs(score) if absolute else score
 
 
 def categorical_to_numerical(pred: list):
     """
     Parse single prediction that comes as 
     a category and transform it in a numeric
@@ -392,22 +394,26 @@
     if all(v is None or v == "." for v in preds):
         return np.nan
     
     if all("|" not in v for v in preds):
         return np.nan
     
     _preds = preds[0].split(",")
+  
     _max = 0
     for _p in _preds:
-       
-        new_max = round(float(_p.split("|")[1]), 3)
-        if abs(new_max) > _max:
-            _max = abs(new_max)
-
-    return _max
+        try:
+            new_max = round(float(_p.split("|")[1]), 3)
+            if abs(new_max) > _max or np.isnan(_max):
+                _max = abs(new_max)
+           
+        except ValueError:
+            if _max == 0:
+                _max = np.nan
+    return _max 
 
 def process_conspliceml(preds: pd.Series):
     """
     Process ConSpliceML  scores to return
     a single numeric value for the gene
     where variant occurs
```

### Comparing `veta-0.7.6/src/preprocessing/vcf.py` & `veta-0.7.7/src/preprocessing/vcf.py`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/veta.egg-info/PKG-INFO` & `veta-0.7.7/src/veta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veta
-Version: 0.7.6
+Version: 0.7.7
 Summary: Simple variant prediction evaluation
 Author-email: Pedro Barbosa <psbpedrobarbosa@gmail.com>
 License: https://opensource.org/licenses/GPL-3.0
 Project-URL: homepage, https://github.com/PedroBarbosa/VETA
 Project-URL: repository, https://github.com/PedroBarbosa/VETA
 Project-URL: documentation, https://github.com/PedroBarbosa/VETA
 Requires-Python: ~=3.8
@@ -273,15 +273,15 @@
 |				                          | FunSeq2	          | > 1.5		             | Yes		                   | vcfanno       |
 |				                          | CAPICE	          | > 0.02               | Yes		                   | vcfanno       |
 | Fitness measurement             | CADD_v1.5         | > 15                 | Yes                       | vcfanno       |
 |                                 | CADD-Splice       | > 15                 | Yes                       | vcfanno       |
 |                                 | DANN              | > 0.9                | Yes                       | vcfanno       |
 |                                 | fitCons           | > 0.4                | No                        | vcfanno       |
 |                                 | LINSIGHT          | > 0.056              | Yes                       | vcfanno       |
-| Splicing                        | MaxEntScan        | \|MaxEntScan_diff\|> 1 | No                      | kipoi         |
+| Splicing                        | MaxEntScan        | \|MaxEntScan_diff\|> 3 | No                      | VEP           |
 |                                 | dbscSNV           | > 0.6                | Yes                       | VEP           |
 |                                 | SPIDEX            | \|dpsi_zscore\| > 2  | No                        | vcfanno       |
 |                                 | TraP              | > 0.221 for coding, 0.174 for intronic | Yes     | vcfanno       |
 |                                 | SpliceAI          | > 0.2                | No                        | vcfanno       |
 | 		                            | HAL               | \|deltaPSI\| > 5	   | No			                   | kipoi         |
 |                                 | S-CAP             | Different thresholds | Yes                       | vcfanno       |
 |                                 | MMSplice          | \|deltaLogitPSI\| > 2| No                        | kipoi         |
@@ -291,14 +291,15 @@
 |                                 | IntSplice2        | > 0.5                | Yes                       | vcfanno       |
 |                                 | MLCsplice         | > 0.5                | Yes                       | vcfanno       |
 |                                 | SQUIRLS           | > 0.074              |Yes                        | model_inference |
 |                                 | CI-SpliceAI       | > 0.190              | No                        | model_inference |
 |                                 | Pangolin          | \|splicing_diff\| > 0.2 | No                     | model_inference |
 |                                 | SPiP              | > 0.452              | Yes                       | model_inference |
 |                                 | AbSplice-DNA      | > 0.01               | Yes                       | vcfanno       |
+|                                 | PDIVAS            | > 0.151              | Yes                       | vcfanno       |
 |                                 | LaBranchoR        | > 0.1                | Yes                       | kipoi         |
 <a name="manual_config"></a>
 #### Manual config file
 
 This config file maps the tool name to the corresponding annotation field in the VCF. It allows adding custom methods, as long as the field exists in the VCF.
 The config file must be tab-delimited just like [this one](https://github.com/PedroBarbosa/VETA/blob/master/src/config/tools_config.txt).
 Lines starting with '#' are skipped. For tools with native support within VETA (listed in the table above, where the tool name must be matched), only the 2 columns are required. For custom methods, additional columns must be set. Column specifications are as follows:
```

### Comparing `veta-0.7.6/src/veta.egg-info/SOURCES.txt` & `veta-0.7.7/src/veta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veta-0.7.6/src/veta.py` & `veta-0.7.7/src/veta.py`

 * *Files identical despite different names*

