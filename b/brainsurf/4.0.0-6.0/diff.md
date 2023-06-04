# Comparing `tmp/brainsurf-4.0.0.tar.gz` & `tmp/brainsurf-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsurf-4.0.0.tar", last modified: Sun Jun  4 06:21:55 2023, max compression
+gzip compressed data, was "brainsurf-6.0.tar", last modified: Tue May 30 17:14:54 2023, max compression
```

## Comparing `brainsurf-4.0.0.tar` & `brainsurf-6.0.tar`

### file list

```diff
@@ -1,62 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:55.061015 brainsurf-4.0.0/
--rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-4.0.0/LICENSE
--rw-rw-rw-   0        0        0     2154 2023-06-04 06:21:55.058998 brainsurf-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:54.906031 brainsurf-4.0.0/brainsurf/
--rw-rw-rw-   0        0        0       70 2023-06-04 06:21:41.000000 brainsurf-4.0.0/brainsurf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:54.962906 brainsurf-4.0.0/brainsurf/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-4.0.0/brainsurf/analysis/__init__.py
--rw-rw-rw-   0        0        0     1062 2023-05-31 17:53:32.000000 brainsurf-4.0.0/brainsurf/analysis/corelation_analysis.py
--rw-rw-rw-   0        0        0     1756 2023-05-31 17:53:43.000000 brainsurf-4.0.0/brainsurf/analysis/erp_analysis.py
--rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-4.0.0/brainsurf/analysis/multi_fractal.py
--rw-rw-rw-   0        0        0     1321 2023-05-31 17:55:16.000000 brainsurf-4.0.0/brainsurf/analysis/power_spectrum.py
--rw-rw-rw-   0        0        0     3087 2023-05-21 15:49:59.000000 brainsurf-4.0.0/brainsurf/analysis/stats_analysis.py
--rw-rw-rw-   0        0        0      959 2023-05-31 18:01:11.000000 brainsurf-4.0.0/brainsurf/analysis/time_frequency.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:54.969905 brainsurf-4.0.0/brainsurf/cognitive_analysis_module/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-4.0.0/brainsurf/cognitive_analysis_module/__init__.py
--rw-rw-rw-   0        0        0     9253 2023-05-31 18:05:01.000000 brainsurf-4.0.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py
--rw-rw-rw-   0        0        0     1044 2023-05-31 18:02:02.000000 brainsurf-4.0.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:54.995159 brainsurf-4.0.0/brainsurf/data/
--rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-4.0.0/brainsurf/data/__init__.py
--rw-rw-rw-   0        0        0    14893 2023-05-31 18:40:24.000000 brainsurf-4.0.0/brainsurf/data/comparative_visualize.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-4.0.0/brainsurf/data/csv.py
--rw-rw-rw-   0        0        0      169 2023-06-03 12:38:55.000000 brainsurf-4.0.0/brainsurf/data/df.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-4.0.0/brainsurf/data/edf.py
--rw-rw-rw-   0        0        0    11535 2023-06-04 03:07:04.000000 brainsurf-4.0.0/brainsurf/data/eeg_data.py
--rw-rw-rw-   0        0        0     3483 2023-05-30 19:11:59.000000 brainsurf-4.0.0/brainsurf/data/eeg_data_visualization.py
--rw-rw-rw-   0        0        0      213 2023-06-03 12:32:49.000000 brainsurf-4.0.0/brainsurf/data/mff.py
--rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-4.0.0/brainsurf/data/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:55.005694 brainsurf-4.0.0/brainsurf/machine_learning/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-4.0.0/brainsurf/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-4.0.0/brainsurf/machine_learning/eeg_binary_classification.py
--rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-4.0.0/brainsurf/machine_learning/rnn_module.py
--rw-rw-rw-   0        0        0     2813 2023-05-31 18:17:21.000000 brainsurf-4.0.0/brainsurf/machine_learning/time_series.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:55.019818 brainsurf-4.0.0/brainsurf/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-4.0.0/brainsurf/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2506 2023-05-31 18:22:57.000000 brainsurf-4.0.0/brainsurf/preprocessing/artifact_removal.py
--rw-rw-rw-   0        0        0     2108 2023-05-10 15:28:37.000000 brainsurf-4.0.0/brainsurf/preprocessing/baseline.py
--rw-rw-rw-   0        0        0     1137 2023-05-10 15:30:11.000000 brainsurf-4.0.0/brainsurf/preprocessing/epoching.py
--rw-rw-rw-   0        0        0     4216 2023-05-17 19:24:17.000000 brainsurf-4.0.0/brainsurf/preprocessing/filtering.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:55.027380 brainsurf-4.0.0/brainsurf/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-4.0.0/brainsurf/utils/__init__.py
--rw-rw-rw-   0        0        0      236 2023-05-31 18:25:45.000000 brainsurf-4.0.0/brainsurf/utils/data.py
--rw-rw-rw-   0        0        0      879 2023-04-29 03:52:10.000000 brainsurf-4.0.0/brainsurf/utils/performance_eval.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:55.056991 brainsurf-4.0.0/brainsurf/visualization/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-4.0.0/brainsurf/visualization/__init__.py
--rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-4.0.0/brainsurf/visualization/plot_cluster.py
--rw-rw-rw-   0        0        0      510 2023-04-29 03:44:56.000000 brainsurf-4.0.0/brainsurf/visualization/plot_coherence.py
--rw-rw-rw-   0        0        0      420 2023-04-29 03:45:05.000000 brainsurf-4.0.0/brainsurf/visualization/plot_cross-correlation.py
--rw-rw-rw-   0        0        0      243 2023-05-21 15:27:09.000000 brainsurf-4.0.0/brainsurf/visualization/plot_eeg_signal.py
--rw-rw-rw-   0        0        0      262 2023-04-29 03:45:13.000000 brainsurf-4.0.0/brainsurf/visualization/plot_heatmap.py
--rw-rw-rw-   0        0        0     1013 2023-04-29 03:45:23.000000 brainsurf-4.0.0/brainsurf/visualization/plot_power_spectrum.py
--rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-4.0.0/brainsurf/visualization/plot_spectogram.py
--rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-4.0.0/brainsurf/visualization/plot_time_series.py
--rw-rw-rw-   0        0        0      623 2023-04-29 03:46:07.000000 brainsurf-4.0.0/brainsurf/visualization/plot_topomap.py
-drwxrwxrwx   0        0        0        0 2023-06-04 06:21:54.943826 brainsurf-4.0.0/brainsurf.egg-info/
--rw-rw-rw-   0        0        0     2154 2023-06-04 06:21:54.000000 brainsurf-4.0.0/brainsurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1758 2023-06-04 06:21:54.000000 brainsurf-4.0.0/brainsurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 06:21:54.000000 brainsurf-4.0.0/brainsurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-04 06:21:54.000000 brainsurf-4.0.0/brainsurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 06:21:54.000000 brainsurf-4.0.0/brainsurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 06:21:55.061015 brainsurf-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1178 2023-06-04 06:21:29.000000 brainsurf-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.864503 brainsurf-6.0/
+-rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-6.0/LICENSE
+-rw-rw-rw-   0        0        0     2152 2023-05-30 17:14:54.863547 brainsurf-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.673360 brainsurf-6.0/brainsurf/
+-rw-rw-rw-   0        0        0       68 2023-05-30 17:14:46.000000 brainsurf-6.0/brainsurf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.729464 brainsurf-6.0/brainsurf/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-6.0/brainsurf/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-05-23 17:17:31.000000 brainsurf-6.0/brainsurf/analysis/corelation_analysis.py
+-rw-rw-rw-   0        0        0     3601 2023-04-29 05:21:32.000000 brainsurf-6.0/brainsurf/analysis/erp_analysis.py
+-rw-rw-rw-   0        0        0     1455 2023-05-21 15:27:09.000000 brainsurf-6.0/brainsurf/analysis/find_range.py
+-rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-6.0/brainsurf/analysis/multi_fractal.py
+-rw-rw-rw-   0        0        0     1367 2023-04-29 04:19:06.000000 brainsurf-6.0/brainsurf/analysis/power_spectrum.py
+-rw-rw-rw-   0        0        0     3087 2023-05-21 15:49:59.000000 brainsurf-6.0/brainsurf/analysis/stats_analysis.py
+-rw-rw-rw-   0        0        0      493 2023-04-28 15:40:11.000000 brainsurf-6.0/brainsurf/analysis/time_frequency.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:11:03.000000 brainsurf-6.0/brainsurf/analysis/wavelet_transform.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.741023 brainsurf-6.0/brainsurf/cognitive_analysis_module/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-6.0/brainsurf/cognitive_analysis_module/__init__.py
+-rw-rw-rw-   0        0        0    10182 2023-05-24 17:42:19.000000 brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py
+-rw-rw-rw-   0        0        0     1028 2023-05-23 18:15:54.000000 brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.750570 brainsurf-6.0/brainsurf/comparitive_analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:51.000000 brainsurf-6.0/brainsurf/comparitive_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-05-14 16:53:07.000000 brainsurf-6.0/brainsurf/comparitive_analysis/meditation_comparision.py
+-rw-rw-rw-   0        0        0     1376 2023-05-23 17:05:32.000000 brainsurf-6.0/brainsurf/comparitive_analysis/t_test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.776957 brainsurf-6.0/brainsurf/data/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-6.0/brainsurf/data/__init__.py
+-rw-rw-rw-   0        0        0    21380 2023-05-29 16:47:53.000000 brainsurf-6.0/brainsurf/data/comparative_visualize.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-6.0/brainsurf/data/csv.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-6.0/brainsurf/data/edf.py
+-rw-rw-rw-   0        0        0    11884 2023-05-23 18:39:23.000000 brainsurf-6.0/brainsurf/data/eeg_data.py
+-rw-rw-rw-   0        0        0     2915 2023-05-21 15:27:09.000000 brainsurf-6.0/brainsurf/data/eeg_data_visualization.py
+-rw-rw-rw-   0        0        0     1237 2023-05-17 18:40:22.000000 brainsurf-6.0/brainsurf/data/mff.py
+-rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-6.0/brainsurf/data/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.801613 brainsurf-6.0/brainsurf/machine_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-6.0/brainsurf/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-6.0/brainsurf/machine_learning/eeg_binary_classification.py
+-rw-rw-rw-   0        0        0      764 2023-05-08 17:36:08.000000 brainsurf-6.0/brainsurf/machine_learning/meditative_non_meditative.py
+-rw-rw-rw-   0        0        0     2470 2023-05-10 16:29:13.000000 brainsurf-6.0/brainsurf/machine_learning/rnn.py
+-rw-rw-rw-   0        0        0     2428 2023-05-10 16:31:42.000000 brainsurf-6.0/brainsurf/machine_learning/rnn2.py
+-rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-6.0/brainsurf/machine_learning/rnn_module.py
+-rw-rw-rw-   0        0        0     2220 2023-05-08 16:44:59.000000 brainsurf-6.0/brainsurf/machine_learning/t2.py
+-rw-rw-rw-   0        0        0     3385 2023-05-08 17:24:37.000000 brainsurf-6.0/brainsurf/machine_learning/time_series.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.815154 brainsurf-6.0/brainsurf/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-6.0/brainsurf/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:45:53.000000 brainsurf-6.0/brainsurf/preprocessing/artifact_removal.py
+-rw-rw-rw-   0        0        0     2108 2023-05-10 15:28:37.000000 brainsurf-6.0/brainsurf/preprocessing/baseline.py
+-rw-rw-rw-   0        0        0     1137 2023-05-10 15:30:11.000000 brainsurf-6.0/brainsurf/preprocessing/epoching.py
+-rw-rw-rw-   0        0        0     4216 2023-05-17 19:24:17.000000 brainsurf-6.0/brainsurf/preprocessing/filtering.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.828732 brainsurf-6.0/brainsurf/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-6.0/brainsurf/utils/__init__.py
+-rw-rw-rw-   0        0        0      943 2023-05-17 20:26:04.000000 brainsurf-6.0/brainsurf/utils/data.py
+-rw-rw-rw-   0        0        0      879 2023-04-29 03:52:10.000000 brainsurf-6.0/brainsurf/utils/performance_eval.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.860944 brainsurf-6.0/brainsurf/visualization/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-6.0/brainsurf/visualization/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-6.0/brainsurf/visualization/plot_cluster.py
+-rw-rw-rw-   0        0        0      510 2023-04-29 03:44:56.000000 brainsurf-6.0/brainsurf/visualization/plot_coherence.py
+-rw-rw-rw-   0        0        0      420 2023-04-29 03:45:05.000000 brainsurf-6.0/brainsurf/visualization/plot_cross-correlation.py
+-rw-rw-rw-   0        0        0      243 2023-05-21 15:27:09.000000 brainsurf-6.0/brainsurf/visualization/plot_eeg_signal.py
+-rw-rw-rw-   0        0        0      262 2023-04-29 03:45:13.000000 brainsurf-6.0/brainsurf/visualization/plot_heatmap.py
+-rw-rw-rw-   0        0        0     1013 2023-04-29 03:45:23.000000 brainsurf-6.0/brainsurf/visualization/plot_power_spectrum.py
+-rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-6.0/brainsurf/visualization/plot_spectogram.py
+-rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-6.0/brainsurf/visualization/plot_time_series.py
+-rw-rw-rw-   0        0        0      623 2023-04-29 03:46:07.000000 brainsurf-6.0/brainsurf/visualization/plot_topomap.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:54.698239 brainsurf-6.0/brainsurf.egg-info/
+-rw-rw-rw-   0        0        0     2152 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2109 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 17:14:54.000000 brainsurf-6.0/brainsurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 17:14:54.865521 brainsurf-6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-05-30 17:14:44.000000 brainsurf-6.0/setup.py
```

### Comparing `brainsurf-4.0.0/LICENSE` & `brainsurf-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/PKG-INFO` & `brainsurf-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 4.0.0
+Version: 6.0
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-4.0.0/README.md` & `brainsurf-6.0/README.md`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/analysis/multi_fractal.py` & `brainsurf-6.0/brainsurf/analysis/multi_fractal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/analysis/power_spectrum.py` & `brainsurf-6.0/brainsurf/analysis/power_spectrum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from scipy.signal import welch, coherence, correlate
 import astropy as ast 
-from scipy.signal import periodogram , multitaper
+# from scipy.signal import periodogram , multitaper
 
 def psd_fft(data, sfreq, freq_range=(0, 100)):
+    n_freqs = int(sfreq/2) + 1
     fft_data = np.fft.rfft(data)
     power_spectrum = np.abs(fft_data)**2 / len(data)
     freqs = np.fft.rfftfreq(len(data), 1.0/sfreq)
     mask = (freqs >= freq_range[0]) & (freqs <= freq_range[1])
     freqs = freqs[mask]
     power_spectrum = power_spectrum[mask]
     return freqs, power_spectrum
@@ -19,21 +20,21 @@
     return freqs, psd
 
 def psd_lombscargle(signal, fs):
     time = np.arange(len(signal))/fs
     frequency, power = ast.timeseries.LombScargle(time, signal).autopower(normalization='psd')
     return frequency, power
 
-def psd_multitaper(signal, fs, nperseg=256, NW=3):
-    f, Pxx = multitaper(signal, fs, nperseg=nperseg, NW=NW, adaptive=True)
-    return f, Pxx.mean(axis=1)
-
-def psd_periodogram(signal, fs, nfft=None):
-    f, Pxx = periodogram(signal, fs, nfft=nfft)
-    return f, Pxx
+# def psd_multitaper(signal, fs, nperseg=256, NW=3):
+#     f, Pxx = multitaper(signal, fs, nperseg=nperseg, NW=NW, adaptive=True)
+#     return f, Pxx.mean(axis=1)
+
+# def psd_periodogram(signal, fs, nfft=None):
+#     f, Pxx = periodogram(signal, fs, nfft=nfft)
+#     return f, Pxx
 
 def calculate_nperseg(data):
     n = len(data)
     if n < 256:
         nperseg = n
     elif n < 2048:
         nperseg = 256
```

### Comparing `brainsurf-4.0.0/brainsurf/analysis/stats_analysis.py` & `brainsurf-6.0/brainsurf/analysis/stats_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py` & `brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import numpy as np
 from scipy.stats import ttest_rel, wilcoxon
-import pandas as pd
-from scipy import stats
-from brainsurf.cognitive_analysis_module.cognitive_indexes import calculate_arousal_index, calculate_band_power, calculate_engagement, calculate_neural_activity, calculate_pe
+# from .cognitive_indexes import calculate_pe,calculate_band_power,calculate_arousal_index, calculate_neural_activity,calculate_engagement
 
 def calculate_cognitive_indexes(data_before, data_after):
     """
     Calculate cognitive indexes from EEG data to assess attention, mental workload, or cognitive performance.
     Examples of cognitive indexes include response time, error rates, or other relevant measures.
 
     Args:
@@ -14,14 +12,38 @@
     - data_after (pandas.DataFrame): EEG data after meditation.
 
     Returns:
     - cognitive_indexes_before (numpy.ndarray): Cognitive indexes calculated from data_before.
     - cognitive_indexes_after (numpy.ndarray): Cognitive indexes calculated from data_after.
     """
 
+    def calculate_band_power(freqs, power, bands):
+        band_power = {}
+        for band, f_range in bands.items():
+            idx = np.logical_and(freqs >= f_range[0], freqs <= f_range[1])
+            band_power[band] = np.trapz(power[idx], freqs[idx])
+
+        return band_power
+
+    def calculate_pe(alpha_power, beta_power):
+        pe = beta_power / alpha_power
+        return pe
+
+    def calculate_arousal_index(alpha_power, theta_power):
+        ai = alpha_power / theta_power
+        return ai
+
+    def calculate_neural_activity(delta_power, theta_power, alpha_power, beta_power):
+        na = (delta_power + theta_power) / (alpha_power + beta_power)
+        return na
+
+    def calculate_engagement(alpha_power, theta_power, delta_power):
+        eng = (alpha_power + theta_power) / delta_power
+        return eng
+
     # Extract the necessary data columns from data_before
     freqs_before = data_before['sec']
     alpha_power_before = data_before['alpha']
     beta_power_before = data_before['beta']
     delta_power_before = data_before['delta']
     theta_power_before = data_before['theta']
 
@@ -88,17 +110,18 @@
         # Perform Wilcoxon signed-rank test
         test_statistic, p_value = wilcoxon(cognitive_indexes_before, cognitive_indexes_after)
     else:
         raise ValueError("Invalid test_type. Options: 'paired_ttest', 'wilcoxon'")
 
     return test_statistic, p_value
 
+import pandas as pd
+from scipy import stats
 
-
-def compare_eeg_data_stats(pre_merged, post_merged):
+def analyze_eeg_data(pre_merged, post_merged):
     # Extract the relevant feature columns
     pre_eeg_raw = pre_merged['raw']
     pre_alpha = pre_merged['alpha']
     pre_beta = pre_merged['beta']
     pre_theta = pre_merged['theta']
     pre_delta = pre_merged['delta']
 
@@ -134,17 +157,21 @@
         'Feature': ['EEG', 'Alpha', 'Beta', 'Theta', 'Delta'],
         'T-Stat': [t_statistic_raw, t_statistic_alpha, t_statistic_beta, t_statistic_theta, t_statistic_delta],
         'P-Value (T-Test)': [p_value_raw, p_value_alpha, p_value_beta, p_value_theta, p_value_delta],
         'F-Stat': [f_statistic_raw, f_statistic_alpha, f_statistic_beta, f_statistic_theta, f_statistic_delta],
         'P-Value (ANOVA)': [p_value_anova_raw, p_value_anova_alpha, p_value_anova_beta, p_value_anova_theta, p_value_anova_delta],
         'Effect Size': [effect_size_raw, effect_size_alpha, effect_size_beta, effect_size_theta, effect_size_delta]
     })
+
     return results
 
 
+import pandas as pd
+import numpy as np
+
 def analyze_stroop_data(data):
     # Convert the data to a pandas DataFrame for easier analysis
     df = pd.DataFrame(data, columns=["Color 1", "Color 2", "Congruent", "Response Time", "Accuracy", "Block", "Trial"])
 
     # Calculate average response time for congruent and incongruent trials
     congruent_rt = df[df["Congruent"] == 1]["Response Time"]
     incongruent_rt = df[df["Congruent"] == 0]["Response Time"]
@@ -161,28 +188,23 @@
 
     avg_congruent_acc = np.mean(congruent_acc)
     avg_incongruent_acc = np.mean(incongruent_acc)
 
     # Perform t-test for accuracy (without using scipy)
     t_value_acc, p_value_acc = independent_ttest(congruent_acc, incongruent_acc)
 
-    # Store the results in a dictionary
-    results = {
-        "Average Response Time - Congruent": avg_congruent_rt,
-        "Average Response Time - Incongruent": avg_incongruent_rt,
-        "T-Test - Response Time - t-value": t_value,
-        "T-Test - Response Time - p-value": p_value,
-        "Average Accuracy - Congruent": avg_congruent_acc,
-        "Average Accuracy - Incongruent": avg_incongruent_acc,
-        "T-Test - Accuracy - t-value": t_value_acc,
-        "T-Test - Accuracy - p-value": p_value_acc
-    }
-
-    return results
-
+    # Print the results
+    print("Response Time Analysis:")
+    print("Average Response Time - Congruent: {:.2f}".format(avg_congruent_rt))
+    print("Average Response Time - Incongruent: {:.2f}".format(avg_incongruent_rt))
+    print("T-Test - Response Time: t-value = {:.2f}, p-value = {:.4f}".format(t_value, p_value))
+    print("\nAccuracy Analysis:")
+    print("Average Accuracy - Congruent: {:.2f}%".format(avg_congruent_acc * 100))
+    print("Average Accuracy - Incongruent: {:.2f}%".format(avg_incongruent_acc * 100))
+    print("T-Test - Accuracy: t-value = {:.2f}, p-value = {:.4f}".format(t_value_acc, p_value_acc))
 
 def independent_ttest(x, y):
     # Calculate the t-value and p-value for two independent samples
     mean_diff = np.mean(x) - np.mean(y)
     var_x = np.var(x, ddof=1)
     var_y = np.var(y, ddof=1)
     n_x = len(x)
```

### Comparing `brainsurf-4.0.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py` & `brainsurf-6.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import numpy as np
 
 def calculate_band_power(freqs, power, bands):
-        band_power = {}
-        for band, f_range in bands.items():
-            idx = np.logical_and(freqs >= f_range[0], freqs <= f_range[1])
-            band_power[band] = np.trapz(power[idx], freqs[idx])
+    band_power = {}
+    for band, f_range in bands.items():
+        idx = np.logical_and(freqs >= f_range[0], freqs <= f_range[1])
+        band_power[band] = np.trapz(power[idx], freqs[idx])
 
-        return band_power
+    return band_power
 
 def calculate_pe(alpha_power, beta_power):
     pe = beta_power / alpha_power
     return pe
 
+
 def calculate_arousal_index(alpha_power, theta_power):
     ai = alpha_power / theta_power
     return ai
 
+
 def calculate_neural_activity(delta_power, theta_power, alpha_power, beta_power):
     na = (delta_power + theta_power) / (alpha_power + beta_power)
     return na
 
 def calculate_engagement(alpha_power, theta_power, delta_power):
     eng = (alpha_power + theta_power) / delta_power
     return eng
```

### Comparing `brainsurf-4.0.0/brainsurf/data/eeg_data.py` & `brainsurf-6.0/brainsurf/data/eeg_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,21 @@
 import pandas as pd
 import pyedflib
-import mne
+import h5py 
 import numpy as np
 from scipy.signal import welch
+
+
 class EEGData:
     def __init__(self, **kwargs):
         self.data = pd.DataFrame(kwargs)
 
     def __len__(self):
         return len(self.data)
-    def drop_columns(self, columns):
-        """
-        Drop specified columns from the EEGData object.
-
-        Parameters:
-            columns (str or list): The column(s) to drop.
-
-        Returns:
-            None
-        """
-        if isinstance(columns, str):
-            columns = [columns]  # Convert single column name to a list
 
-        existing_columns = list(self.data.columns)
-        columns_to_drop = [col for col in columns if col in existing_columns]
-
-        if columns_to_drop:
-            self.data.drop(columns=columns_to_drop, inplace=True)
-        else:
-            print("Specified column(s) not found in the EEGData object.")
     def get_data(self):
         return self.data
 
     def data_length(self):
         length = 0
         for value in self.data.values():
             if isinstance(value, list):
@@ -208,21 +191,17 @@
             raise ValueError("Required keys 'raw' and 'sec' are missing in the EEGData object.")
 
 
 
 
 class EEGDataFactory:
     def create_eeg_data(self, input_file):
-        if isinstance(input_file, pd.DataFrame):
-            eeg_data = EEGData()
-            for column in input_file.columns:
-                eeg_data.add_data(column, input_file[column])
-            return eeg_data
+
         #CSV
-        elif input_file.endswith('.csv'):
+        if input_file.endswith('.csv'):
             data = self.parse_csv(input_file)
             if 'sec' in data.columns and 'EEG' in data.columns and 'alpha' in data.columns and 'beta' in data.columns and 'delta' in data.columns and 'theta ' in data.columns:
                 # CSV data with sec, alpha, beta,  delta and theta columns            
                 return EEGData(sec=data['sec'], raw=data['EEG'], alpha=data['alpha'], beta=data['beta'], theta=data['theta '], delta =data['delta'])
             elif 'sec' in data.columns:
                 # CSV data with raw and sec columns
                 return EEGData(sec=data['sec'], raw=data['EEG'])
@@ -234,20 +213,27 @@
             # Parse EDF data
             data = self.parse_edf(input_file)
             channel_names = data['channel_names']
             raw_data = data['raw_data']
             return EEGData(channel_names=channel_names, raw_data=raw_data)
     
         elif input_file.endswith('.mff'):
-            raw = mne.io.read_raw_egi(input_file)
-            eeg_data = raw.get_data()
-            time_points = raw.times
-            baseline = pd.DataFrame(data=eeg_data.T, columns=raw.ch_names)
-            baseline['sec'] = time_points
-            return baseline
+            data = self.parse_mff(input_file)
+           
+            if 'sec' in data.columns and 'EEG' in data.columns and 'alpha' in data.columns and 'beta' in data.columns and 'delta' in data.columns and 'theta ' in data.columns:
+                    # CSV data with sec, alpha, beta, and gamma columns            
+                    return EEGData(sec=data['sec'], raw=data['EEG'], alpha=data['alpha'], beta=data['beta'], theta=data['theta '], delta =data['delta'])
+            elif 'sec' in data.columns:
+                    # CSV data with raw and time columns
+                    return EEGData(time=data['sec'], raw=data['EEG'])
+            elif 'EEG' in data.col:
+                    # CSV data with only raw data
+                    return EEGData(raw=data['EEG'])
+            else:
+                return EEGData(sec=data['time'], raw=data['EEG'], channel_names=channel_names)
             # Create EEGData object with the extracted data           
         
         elif input_file.endswith('.xlsx'):
             data = self.parse_xlsx(input_file)
             # Extract relevant information from the XLSX data
             if 'sec' in data.columns and 'EEG' in data.columns and 'alpha' in data.columns and 'beta' in data.columns and 'delta' in data.columns and 'theta ' in data.columns:
                     # CSV data with sec, alpha, beta, and gamma columns            
@@ -256,16 +242,25 @@
                     # CSV data with raw and time columns
                     return EEGData(sec=data['sec'], raw=data['EEG'])
             else:
                     # CSV data with only raw data
                     return EEGData(raw=data['EEG'])
         else:
             raise ValueError("Invalid file format. Only CSV, EDF, MFF, and XLSX files are supported.")
-    
-    
+ 
+  
+    def parse_mff(self, input_file):
+        # Implement your MFF file parsing logic here
+        with h5py.File(input_file, 'r') as f:
+            sec = f['/path/to/timestamps'][()]  # Replace '/path/to/timestamps' with the actual dataset path
+            eeg_signals = f['/path/to/eeg_signals'][()]  # Replace '/path/to/eeg_signals' with the actual dataset path
+            channel_names = f['/path/to/channel_names'][()]  # Replace '/path/to/channel_names' with the actual dataset path
+        
+        data = {'sec': sec, 'eeg_signals': eeg_signals, 'channel_names': channel_names}
+        return data
 
     def parse_csv(self, input_file):
         data = pd.read_csv(input_file)
         return data
 
     def parse_edf(self, input_file):
         f = pyedflib.EdfReader(input_file)
```

### Comparing `brainsurf-4.0.0/brainsurf/data/eeg_data_visualization.py` & `brainsurf-6.0/brainsurf/data/eeg_data_visualization.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,54 +6,48 @@
 from scipy.signal import coherence
 from scipy.signal import correlate2d
 
 class EEGVisualizationFactory:
     def __init__(self, data):
         self.data = data
 
-    def plot_eeg_signal(self, x_label='Time [sec]', y_label='EEG', title='EEG Signal'):
+    def plot_eeg_signal(self):
         sec = self.data['sec']
-        eeg = self.data['raw']
-        plt.plot(sec, eeg)
-        plt.xlabel(x_label)
-        plt.ylabel(y_label)
-        plt.title(title)
+        EEG = self.data['raw']
+        plt.plot(sec, EEG)
+        plt.xlabel('Time [sec]')
+        plt.ylabel('EEG')
+        plt.title('EEG Signal')
         plt.show()
 
-    def plot_spectrogram(self, channel, fs=None, window='hann', nperseg=256, noverlap=None,
-                         cmap='RdBu_r', scaling='density', x_label='Time [sec]', y_label='Frequency [Hz]',
-                         title=None):
+    def plot_spectrogram(self, channel):
         sec = self.data['sec']
-        channel_data = self.data[channel]
-        if fs is None:
-            fs = 1.0 / (sec[1] - sec[0])
-        f, t, Sxx = spectrogram(channel_data, fs=fs, window=window, nperseg=nperseg, noverlap=noverlap, scaling=scaling)
+        data = self.data[channel]
+        fs = 1.0 / (sec[1] - sec[0])
+        window = 'hann'
+        nperseg = 256
+        noverlap = None
+        cmap = 'RdBu_r'
+        scaling = 'density'
+        f, t, Sxx = spectrogram(data, fs=fs, window=window, nperseg=nperseg, noverlap=noverlap, scaling=scaling)
         plt.pcolormesh(t, f, Sxx, cmap=cmap)
-        plt.ylabel(y_label)
-        plt.xlabel(x_label)
-        if title is not None:
-            plt.title(title)
-        else:
-            plt.title(f'Spectrogram ({channel})')
+        plt.ylabel('Frequency [Hz]')
+        plt.xlabel('Time [sec]')
+        plt.title(f'Spectrogram ({channel})')
         plt.colorbar()
         plt.show()
 
-    def plot_power_spectrum(self, channel, fs=None, x_label='Frequency [Hz]', y_label='Power Spectral Density',
-                            title=None):
+    def plot_power_spectrum(self, channel):
         sec = self.data['sec']
-        channel_data = self.data[channel]
-        if fs is None:
-            fs = 1.0 / (sec[1] - sec[0])
-        f, Pxx = plt.psd(channel_data, Fs=fs)
-        plt.xlabel(x_label)
-        plt.ylabel(y_label)
-        if title is not None:
-            plt.title(title)
-        else:
-            plt.title(f'Power Spectrum ({channel})')
+        data = self.data[channel]
+        fs = 1.0 / (sec[1] - sec[0])
+        f, Pxx = plt.psd(data, Fs=fs)
+        plt.xlabel('Frequency [Hz]')
+        plt.ylabel('Power Spectral Density')
+        plt.title(f'Power Spectrum ({channel})')
         plt.show()
 
     def plot_coherence(self, channel1, channel2, freq_range=None):
         sec = self.data['sec']
         data1 = self.data[channel1]
         data2 = self.data[channel2]
         fs = 1.0 / (sec[1] - sec[0])
@@ -79,22 +73,18 @@
         plt.plot(corr)
         plt.xlabel('Time')
         plt.ylabel('Cross-Correlation')
         plt.title(f'Cross-Correlation ({channel1} vs {channel2})')
         plt.show()
 
     def plot_heatmap(self):
-        eeg_df = pd.DataFrame(self.data)
-        # Calculate the correlation matrix
-        corr_matrix = eeg_df.corr()
-        # Plot the correlation heatmap
-        plt.figure(figsize=(10, 8))
-        sns.heatmap(corr_matrix, cmap='RdBu_r', annot=True, fmt=".2f", vmin=-1, vmax=1)
-        plt.title('EEG Data Heatmap')
-        plt.xticks(rotation=90)
-        plt.yticks(rotation=0)
-        plt.show()
-
+       corr_matrix = self.data.corr()
+       plt.figure(figsize=(10, 8))
+       sns.heatmap(corr_matrix, cmap='RdBu_r', annot=True, fmt=".2f", vmin=-1, vmax=1)
+       plt.title('EEG Data Heatmap')
+       plt.xticks(rotation=90)
+       plt.yticks(rotation=0)
+       plt.show()
```

### Comparing `brainsurf-4.0.0/brainsurf/machine_learning/eeg_binary_classification.py` & `brainsurf-6.0/brainsurf/machine_learning/eeg_binary_classification.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/machine_learning/rnn_module.py` & `brainsurf-6.0/brainsurf/machine_learning/rnn_module.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/machine_learning/time_series.py` & `brainsurf-6.0/brainsurf/machine_learning/time_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import numpy as np
 import pandas as pd
 from sklearn.metrics import r2_score
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler
-from sklearn.metrics import mean_squared_error
+from sklearn.metrics import accuracy_score, mean_squared_error
+from sklearn.model_selection import GridSearchCV
+from sklearn.linear_model import LinearRegression
+from sklearn.tree import DecisionTreeRegressor
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.ensemble import RandomForestRegressor
 import matplotlib.pyplot as plt
+
 def load_data(filepath):
     data = pd.read_csv(filepath)
     print(data.head())
     return data
 
 def preprocess_data(data):
     """
@@ -89,7 +93,15 @@
     axs[0, 0].legend()
     axs[0, 1].legend()
     axs[1, 0].legend()
     axs[1, 1].legend()
 
     plt.show()
 
+
+if __name__ == '__main__':
+    data = load_data('C:/Users/Preethi V Hiremath/OneDrive/Desktop/Projects/esp/brainsurf/data/eeg_data/sample_data2.csv')
+    preprocessed_data = preprocess_data(data)
+    X_train, X_test, y_train, y_test = split_data(preprocessed_data)
+    model = train_model(X_train, y_train)
+    evaluate_model(model, X_test, y_test)
+    visualize_predictions(model, X_test, y_test)
```

### Comparing `brainsurf-4.0.0/brainsurf/preprocessing/baseline.py` & `brainsurf-6.0/brainsurf/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/preprocessing/epoching.py` & `brainsurf-6.0/brainsurf/preprocessing/epoching.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/preprocessing/filtering.py` & `brainsurf-6.0/brainsurf/preprocessing/filtering.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/utils/performance_eval.py` & `brainsurf-6.0/brainsurf/utils/performance_eval.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/visualization/plot_power_spectrum.py` & `brainsurf-6.0/brainsurf/visualization/plot_power_spectrum.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/visualization/plot_time_series.py` & `brainsurf-6.0/brainsurf/visualization/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf/visualization/plot_topomap.py` & `brainsurf-6.0/brainsurf/visualization/plot_topomap.py`

 * *Files identical despite different names*

### Comparing `brainsurf-4.0.0/brainsurf.egg-info/PKG-INFO` & `brainsurf-6.0/brainsurf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 4.0.0
+Version: 6.0
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-4.0.0/setup.py` & `brainsurf-6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='brainsurf',
-    version='4.0.0',
+    version='6.0',
     description='EEG Signal Processing Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='preethivhiremath',
     author_email='preethivhiremath.vh@gmail.com',
     url='https://github.com/preethihiremath/brainsurf',
     packages=find_packages(),
```

