# Comparing `tmp/napari-gemspa-0.0.1.tar.gz` & `tmp/napari-gemspa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-gemspa-0.0.1.tar", last modified: Mon May 29 21:38:16 2023, max compression
+gzip compressed data, was "napari-gemspa-0.0.2.tar", last modified: Sat Jun  3 23:48:14 2023, max compression
```

## Comparing `napari-gemspa-0.0.1.tar` & `napari-gemspa-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 21:38:16.719494 napari-gemspa-0.0.1/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1512 2023-04-13 14:56:39.000000 napari-gemspa-0.0.1/LICENSE
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       96 2023-04-02 00:08:59.000000 napari-gemspa-0.0.1/MANIFEST.in
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1292 2023-05-29 21:38:16.719587 napari-gemspa-0.0.1/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       18 2023-04-02 00:20:37.000000 napari-gemspa-0.0.1/README.md
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      180 2023-05-29 21:11:06.000000 napari-gemspa-0.0.1/pyproject.toml
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1761 2023-05-29 21:38:16.720041 napari-gemspa-0.0.1/setup.cfg
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 21:38:16.712791 napari-gemspa-0.0.1/src/
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 21:38:16.718484 napari-gemspa-0.0.1/src/napari_gemspa/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      320 2023-05-29 19:40:41.000000 napari-gemspa-0.0.1/src/napari_gemspa/__init__.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    24485 2023-05-27 15:09:54.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_analyze_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    18018 2023-05-27 15:09:54.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_data_views.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8218 2023-05-25 14:04:49.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_file_import_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     6607 2023-05-24 21:58:16.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_filter_links_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     5344 2023-05-24 21:58:16.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_link_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8171 2023-05-24 22:06:34.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_locate_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    10202 2023-05-24 21:55:19.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_plugin.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     7655 2023-05-24 16:12:18.000000 napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     2582 2023-05-22 18:46:47.000000 napari-gemspa-0.0.1/src/napari_gemspa/_reader.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      644 2023-04-02 00:08:59.000000 napari-gemspa-0.0.1/src/napari_gemspa/_sample_data.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1764 2023-05-24 21:55:19.000000 napari-gemspa-0.0.1/src/napari_gemspa/_utils.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     2894 2023-05-25 14:41:34.000000 napari-gemspa-0.0.1/src/napari_gemspa/_writer.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1352 2023-05-29 19:40:41.000000 napari-gemspa-0.0.1/src/napari_gemspa/napari.yaml
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-05-29 21:38:16.719392 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1292 2023-05-29 21:38:16.000000 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      819 2023-05-29 21:38:16.000000 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/SOURCES.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)        1 2023-05-29 21:38:16.000000 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/dependency_links.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       60 2023-05-29 21:38:16.000000 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/entry_points.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      137 2023-05-29 21:38:16.000000 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/requires.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       14 2023-05-29 21:38:16.000000 napari-gemspa-0.0.1/src/napari_gemspa.egg-info/top_level.txt
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.881116 napari-gemspa-0.0.2/
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1512 2023-04-13 14:56:39.000000 napari-gemspa-0.0.2/LICENSE
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)       96 2023-04-02 00:08:59.000000 napari-gemspa-0.0.2/MANIFEST.in
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     9798 2023-06-03 23:48:14.881227 napari-gemspa-0.0.2/PKG-INFO
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     8524 2023-06-03 23:42:01.000000 napari-gemspa-0.0.2/README.md
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      130 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/pyproject.toml
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1761 2023-06-03 23:48:14.881777 napari-gemspa-0.0.2/setup.cfg
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.874477 napari-gemspa-0.0.2/src/
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.876077 napari-gemspa-0.0.2/src/_tests/
+-rw-------   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/_tests/__init__.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1777 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/_tests/run_napari.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     3224 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/_tests/test_gemspa_locate_worker.py
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.880060 napari-gemspa-0.0.2/src/napari_gemspa/
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      320 2023-05-29 19:40:41.000000 napari-gemspa-0.0.2/src/napari_gemspa/__init__.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    25898 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_analyze_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    19439 2023-06-03 18:51:07.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_data_views.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     8770 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_file_import_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     6596 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_filter_links_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     6021 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_link_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     8503 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_locate_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    10201 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_plugin.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     7789 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     2582 2023-05-22 18:46:47.000000 napari-gemspa-0.0.2/src/napari_gemspa/_reader.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1764 2023-05-24 21:55:19.000000 napari-gemspa-0.0.2/src/napari_gemspa/_utils.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     3553 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_writer.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1352 2023-05-29 19:40:41.000000 napari-gemspa-0.0.2/src/napari_gemspa/napari.yaml
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.881000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     9798 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/PKG-INFO
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      873 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/SOURCES.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)        1 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/dependency_links.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)       60 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/entry_points.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      137 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/requires.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)       21 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/top_level.txt
```

### Comparing `napari-gemspa-0.0.1/LICENSE` & `napari-gemspa-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.1/setup.cfg` & `napari-gemspa-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-gemspa
-version = 0.0.1
+version = 0.0.2
 description = A plugin for analysis of single particle tracking experiments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/liamholtlab/napari-gemspa
 author = Sarah Keegan
 author_email = sarah.keegan@nyulangone.org
 license = BSD-3-Clause
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_analyze_widget.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_analyze_widget.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-from ._gemspa_widget import GEMspaWidget, GEMspaWorker
-import pandas as pd
+"""Defines: GEMspaAnalyzeWidget, GEMspaAnalyzeWorker"""
+
 import numpy as np
+import pandas as pd
 from gemspa_spt import ParticleTracks
-from qtpy.QtWidgets import (QGridLayout, QLabel, QLineEdit, QCheckBox, QVBoxLayout, QComboBox)
 from qtpy.QtCore import Slot
-from ._utils import show_error, convert_to_int, convert_to_float, remove_outside_mask
+from qtpy.QtWidgets import (
+    QCheckBox,
+    QComboBox,
+    QGridLayout,
+    QLabel,
+    QLineEdit,
+    QVBoxLayout,
+)
 
-"""Defines: GEMspaAnalyzeWidget, GEMspaAnalyzeWorker"""
+from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+from ._utils import convert_to_float, convert_to_int, remove_outside_mask, show_error
 
 
 class GEMspaAnalyzeWorker(GEMspaWorker):
-    """Worker for the Analyze plugin
-
-    """
+    """Worker for the Analyze plugin"""
 
     def __init__(self):
         super().__init__()
 
     @Slot(dict)
     def run(self, state):
         """Execute the processing"""
 
-        input_params = state['inputs']
-        state_params = state['parameters']
+        input_params = state["inputs"]
+        state_params = state["parameters"]
 
-        batch = state_params['batch']
-        track_id = state_params['track_id']
-        microns_per_pixel = state_params['microns_per_pixel']
-        time_lag_sec = state_params['time_lag_sec']
-        min_len_fit = state_params['min_len_fit']
-        max_lagtime_fit = state_params['max_lagtime_fit']
-        error_term_fit = state_params['error_term_fit']
+        batch = state_params["batch"]
+        track_id = state_params["track_id"]
+        microns_per_pixel = state_params["microns_per_pixel"]
+        time_lag_sec = state_params["time_lag_sec"]
+        min_len_fit = state_params["min_len_fit"]
+        max_lagtime_fit = state_params["max_lagtime_fit"]
+        error_term_fit = state_params["error_term_fit"]
 
         # TODO
         # frame_start = state_params['frame_start']
         # frame_end = state_params['frame_end']
 
-        tracks_layer_data = input_params['tracks_layer_data']
+        tracks_layer_data = input_params["tracks_layer_data"]
 
         # Find out 2d or 3d
         if tracks_layer_data.shape[1] == 5:
             z_col = True
-            track_cols = ['track_id', 'frame', 'z', 'y', 'x']
+            track_cols = ["track_id", "frame", "z", "y", "x"]
         elif tracks_layer_data.shape[1] == 4:
             z_col = False
-            track_cols = ['track_id', 'frame', 'y', 'x']
+            track_cols = ["track_id", "frame", "y", "x"]
         else:
             raise ValueError("Tracks layer has an unexpected dimension.")
 
         # create data frame of track data
         track_data_df = pd.DataFrame(tracks_layer_data, columns=track_cols)
 
         # process the entire movie - limited by frame start/end
@@ -59,204 +65,309 @@
         #                                   (track_data_df['frame'] <= frame_end)]
         #     self.log.emit(f"After filter for frames from {frame_start} to {frame_end}, number of tracks: " +
         #                   f"{track_data_df['track_id'].nunique()}")
 
         # if labels layer was chosen, remove all tracks that contain points that are outside labeled regions
         # *note* this function is not implemented for 3D (z-dimensional) data
         # *note* if not run in batch mode (only analyze a single track), the labels layer is ignored
-        if batch and 'labels_layer_data' in input_params:
-            labeled_mask = input_params['labels_layer_data']
-            track_data_df = remove_outside_mask(track_data_df, labeled_mask, id_column='track_id')
+        if batch and "labels_layer_data" in input_params:
+            labeled_mask = input_params["labels_layer_data"]
+            track_data_df = remove_outside_mask(
+                track_data_df, labeled_mask, id_column="track_id"
+            )
             self.log.emit(
-                f"Removed particles outside of mask region, number of particles: {track_data_df['track_id'].nunique()}")
+                f"Removed particles outside of mask region, number of particles: {track_data_df['track_id'].nunique()}"
+            )
 
         # Create the gemspa-spt class object for performing analysis
         if not z_col:
             # ParticleTracks class expects a column for z-dimension
             tracks = ParticleTracks(np.insert(track_data_df.to_numpy(), 2, 0, axis=1))
         else:
             tracks = ParticleTracks(track_data_df.to_numpy())
         tracks.microns_per_pixel = microns_per_pixel
         tracks.time_lag_sec = time_lag_sec
 
+        # add the x/y/z positions in microns to the track data for output later
+        if "z" in track_data_df:
+            track_data_df["z (microns)"] = track_data_df["z"] * microns_per_pixel
+        track_data_df["y (microns)"] = track_data_df["y"] * microns_per_pixel
+        track_data_df["x (microns)"] = track_data_df["x"] * microns_per_pixel
+
         out_data = dict()
         if batch:
-
             # Ensemble average effective Diffusion (linear) and alpha (log-log)
             msds = tracks.msd_all_tracks()
             step_sizes = tracks.step_size_all_tracks()
             r_of_g = tracks.r_of_g_all_tracks()
             ens_msds, n_ens_tracks = tracks.ensemble_avg_msd()
 
             # fit ensemble MSD, get D and alpha
-            D, E, r_squared1 = tracks.fit_msd_linear(t=ens_msds[1:, 0],
-                                                     msd=ens_msds[1:, 4],
-                                                     dim=2,
-                                                     max_lagtime=max_lagtime_fit,
-                                                     err=error_term_fit)
-            K, alpha, r_squared2 = tracks.fit_msd_loglog(t=ens_msds[1:, 0],
-                                                         msd=ens_msds[1:, 4],
-                                                         dim=2,
-                                                         max_lagtime=max_lagtime_fit)
-            data = [['sum',
-                     D,
-                     E,
-                     r_squared1,
-                     K,
-                     alpha,
-                     r_squared2]]
-            ens_fit_data = pd.DataFrame(data, columns=['dim', 'D', 'E', 'r_sq (lin)', 'K', 'a', 'r_sq (log)'])
-            ens_fit_data = ens_fit_data.round({'D': 4, 'E': 4, 'r_sq (lin)': 2, 'K': 4, 'a': 4, 'r_sq (log)': 2})
-
-            summary_data = {'ens_fit_results': ens_fit_data,
-                            'ens_msd': ens_msds[1:max_lagtime_fit + 1, [0, 4]]
-                            }
+            D, E, r_squared1 = tracks.fit_msd_linear(
+                t=ens_msds[1:, 0],
+                msd=ens_msds[1:, 4],
+                dim=2,
+                max_lagtime=max_lagtime_fit,
+                err=error_term_fit,
+            )
+            K, alpha, r_squared2 = tracks.fit_msd_loglog(
+                t=ens_msds[1:, 0],
+                msd=ens_msds[1:, 4],
+                dim=2,
+                max_lagtime=max_lagtime_fit,
+            )
+            data = [["sum", D, E, r_squared1, K, alpha, r_squared2]]
+            ens_fit_data = pd.DataFrame(
+                data,
+                columns=[
+                    "dim",
+                    "D",
+                    "E",
+                    "r_sq (lin)",
+                    "K",
+                    "a",
+                    "r_sq (log)",
+                ],
+            )
+            ens_fit_data = ens_fit_data.round(
+                {
+                    "D": 4,
+                    "E": 4,
+                    "r_sq (lin)": 2,
+                    "K": 4,
+                    "a": 4,
+                    "r_sq (log)": 2,
+                }
+            )
+
+            summary_data = {
+                "ens_fit_results": ens_fit_data,
+                "ens_msd": ens_msds[1 : max_lagtime_fit + 1, [0, 4]],
+            }
 
             # fit the msd of each track - linear and loglog scale
-            tracks.fit_msd_all_tracks(linear_fit=True,
-                                      min_len=min_len_fit,
-                                      max_lagtime=max_lagtime_fit,
-                                      err=error_term_fit)
-            tracks.fit_msd_all_tracks(linear_fit=False,
-                                      min_len=min_len_fit,
-                                      max_lagtime=max_lagtime_fit,
-                                      err=error_term_fit)
+            tracks.fit_msd_all_tracks(
+                linear_fit=True,
+                min_len=min_len_fit,
+                max_lagtime=max_lagtime_fit,
+                err=error_term_fit,
+            )
+            tracks.fit_msd_all_tracks(
+                linear_fit=False,
+                min_len=min_len_fit,
+                max_lagtime=max_lagtime_fit,
+                err=error_term_fit,
+            )
 
-            self.log.emit(f"Total number of tracks: {len(tracks.track_ids)}\n" +
-                          f"After length filter, number of tracks: {len(tracks.linear_fit_results)}\n")
+            self.log.emit(
+                f"Total number of tracks: {len(tracks.track_ids)}\n"
+                + f"After length filter, number of tracks: {len(tracks.linear_fit_results)}\n"
+            )
 
             # Gather the fit data and r-of-g
-            all_fit_data = np.concatenate([tracks.linear_fit_results,
-                                           tracks.loglog_fit_results[:, 2:]
-                                           ], axis=1)
-            all_fit_data = pd.DataFrame(all_fit_data, columns=['track_id',
-                                                               'dim',
-                                                               'D',
-                                                               'E',
-                                                               'r_sq (lin)',
-                                                               'K',
-                                                               'a',
-                                                               'r_sq (log)'])
-            all_fit_data.drop('dim', axis=1, inplace=True)
-            all_fit_data = all_fit_data.round({'D': 4, 'E': 4, 'r_sq (lin)': 2,
-                                               'K': 4, 'a': 4, 'r_sq (log)': 2})
+            all_fit_data = np.concatenate(
+                [tracks.linear_fit_results, tracks.loglog_fit_results[:, 2:]],
+                axis=1,
+            )
+            all_fit_data = pd.DataFrame(
+                all_fit_data,
+                columns=[
+                    "track_id",
+                    "dim",
+                    "D",
+                    "E",
+                    "r_sq (lin)",
+                    "K",
+                    "a",
+                    "r_sq (log)",
+                ],
+            )
+            all_fit_data.drop("dim", axis=1, inplace=True)
+            all_fit_data = all_fit_data.round(
+                {
+                    "D": 4,
+                    "E": 4,
+                    "r_sq (lin)": 2,
+                    "K": 4,
+                    "a": 4,
+                    "r_sq (log)": 2,
+                }
+            )
 
             # Merge fit results with track data
-            msds = pd.DataFrame(msds[:, [1, 5]], columns=['tau', 'msd'])
+            msds = pd.DataFrame(msds[:, [1, 5]], columns=["tau", "msd"])
             msds.msd = msds.msd.where(msds.tau > 0, other=np.nan)
-            step_sizes = pd.DataFrame(step_sizes[:, [1, 5]], columns=['t', 'step_size'])
-            step_sizes.step_size = step_sizes.step_size.where(step_sizes.t > 0, other=np.nan)
-            r_of_g = pd.DataFrame(r_of_g[:, 1:], columns=['t', 'radius_gyration'])
-            r_of_g.radius_gyration = r_of_g.radius_gyration.where(r_of_g.t > 0, other=np.nan)
+            msds = msds.round({"msd": 4})
+
+            step_sizes = pd.DataFrame(step_sizes[:, [1, 5]], columns=["t", "step_size"])
+            step_sizes.step_size = step_sizes.step_size.where(
+                step_sizes.t > 0, other=np.nan
+            )
+            step_sizes = step_sizes.round({"step_size": 4})
+
+            r_of_g = pd.DataFrame(r_of_g[:, 1:], columns=["t", "radius_gyration"])
+            r_of_g.radius_gyration = r_of_g.radius_gyration.where(
+                r_of_g.t > 0, other=np.nan
+            )
+            r_of_g = r_of_g.round({"radius_gyration": 4})
+
+            track_lengths = pd.DataFrame(
+                tracks.track_lengths, columns=["track_id", "track_length"]
+            )
 
             # time is t from step size, already in table
-            r_of_g.drop('t', axis=1, inplace=True)
+            r_of_g.drop("t", axis=1, inplace=True)
 
             track_data_df = pd.concat([track_data_df, msds, step_sizes, r_of_g], axis=1)
 
-            merged_data = track_data_df.merge(all_fit_data, how='left', on='track_id')
+            track_data_df = track_data_df.merge(
+                track_lengths, how="left", on="track_id"
+            )
+
+            merged_data = track_data_df.merge(
+                all_fit_data, how="left", on="track_id", indicator="_merge"
+            )
+            merged_data["MSD_fitted"] = 0
+            merged_data["MSD_fitted"].where(
+                merged_data["_merge"] != "both", other=1, inplace=True
+            )
+            merged_data.drop("_merge", axis=1, inplace=True)
+            # TODO: confirm right_only does not exist in the column values
 
             # Add frame start and frame end to the fit results
-            frames = merged_data.groupby('track_id', as_index=False).agg(frame_start=('frame', 'min'),
-                                                                         frame_end=('frame', 'max'))
-            merged_data = frames.merge(merged_data, how='right', on='track_id')
+            frames = merged_data.groupby("track_id", as_index=False).agg(
+                frame_start=("frame", "min"), frame_end=("frame", "max")
+            )
+            merged_data = frames.merge(merged_data, how="right", on="track_id")
 
             # emit the output data
-            out_data = {'df': merged_data,
-                        'summary_data': summary_data,
-                        'batch': batch,
-                        'tracks_layer_scale': input_params['tracks_layer_scale'],
-                        'image_layer_shape': input_params['image_layer_shape'],
-                        'color_by': state['color_by'],
-                        'color_by_min_max': state['color_by_min_max']
-                        }
+            out_data = {
+                "df": merged_data,
+                "summary_data": summary_data,
+                "batch": batch,
+                "tracks_layer_scale": input_params["tracks_layer_scale"],
+                "image_layer_shape": input_params["image_layer_shape"],
+                "color_by": state["color_by"],
+                "color_by_min_max": state["color_by_min_max"],
+            }
         else:
             if track_id in tracks.track_lengths[:, 0]:
-
                 msds = tracks.msd(track_id, fft=True)
                 step_sizes = tracks.step_size(track_id)
                 r_of_g = tracks.r_of_g(track_id)
                 frames = tracks.tracks[tracks.tracks[:, 0] == track_id, 1]
 
                 # Fit for Diffusion coefficient etc
                 data = []
                 for dim in tracks.dim_columns.keys():
-                    if not z_col and dim == 'z':
+                    if not z_col and dim == "z":
                         continue
                     col = tracks.dim_columns[dim]
 
                     # there is no track id so reduce column index by 1
                     col -= 1
 
-                    if dim == 'sum':
+                    if dim == "sum":
                         d = tracks.dimension
                     else:
                         d = 1
 
-                    D, E, r_squared1 = tracks.fit_msd_linear(t=msds[1:, 0],
-                                                             msd=msds[1:, col],
-                                                             dim=d,
-                                                             max_lagtime=max_lagtime_fit,
-                                                             err=error_term_fit)
-                    K, alpha, r_squared2 = tracks.fit_msd_loglog(t=msds[1:, 0],
-                                                                 msd=msds[1:, col],
-                                                                 dim=d,
-                                                                 max_lagtime=max_lagtime_fit)
-
-                    data.append([track_id,
-                                 frames.min(),
-                                 frames.max(),
-                                 dim,
-                                 D,
-                                 E,
-                                 r_squared1,
-                                 K,
-                                 alpha,
-                                 r_squared2])
-
-                data = pd.DataFrame(data, columns=['track_id',
-                                                   'start',
-                                                   'end',
-                                                   'dim',
-                                                   'D',
-                                                   'E',
-                                                   'r_sq (lin)',
-                                                   'K',
-                                                   'a',
-                                                   'r_sq (log)'])
+                    D, E, r_squared1 = tracks.fit_msd_linear(
+                        t=msds[1:, 0],
+                        msd=msds[1:, col],
+                        dim=d,
+                        max_lagtime=max_lagtime_fit,
+                        err=error_term_fit,
+                    )
+                    K, alpha, r_squared2 = tracks.fit_msd_loglog(
+                        t=msds[1:, 0],
+                        msd=msds[1:, col],
+                        dim=d,
+                        max_lagtime=max_lagtime_fit,
+                    )
+
+                    data.append(
+                        [
+                            track_id,
+                            frames.min(),
+                            frames.max(),
+                            dim,
+                            D,
+                            E,
+                            r_squared1,
+                            K,
+                            alpha,
+                            r_squared2,
+                        ]
+                    )
+
+                data = pd.DataFrame(
+                    data,
+                    columns=[
+                        "track_id",
+                        "start",
+                        "end",
+                        "dim",
+                        "D",
+                        "E",
+                        "r_sq (lin)",
+                        "K",
+                        "a",
+                        "r_sq (log)",
+                    ],
+                )
 
                 # Radius of gyration, for entire track only
-                data['radius_gyration'] = 0
-                data['radius_gyration'].where(data['dim'] != 'sum',
-                                              other=tracks.r_of_g(track_id, full=False),
-                                              inplace=True)
-
-                data = data.round({'D': 4, 'E': 4, 'r_sq (lin)': 2,
-                                   'K': 4, 'a': 4, 'r_sq (log)': 2,
-                                   'radius_gyration': 4})
-
-                summary_data = {'fit_results': data,
-                                'msd': msds[1:max_lagtime_fit + 1, [0, 4]]
-                                }
-
-                track_data_df = pd.DataFrame(tracks_layer_data[tracks_layer_data[:, 0] == track_id, :], columns=track_cols)
-                msds = pd.DataFrame(msds[:, [0, 4]], columns=['tau', 'msd'])
-                msds = msds.round({'msd': 4})
-                step_sizes = pd.DataFrame(step_sizes[:, [0, 4]], columns=['t', 'step_size'])
-                step_sizes = step_sizes.round({'step_size': 4})
-
-                r_of_g = pd.DataFrame(r_of_g[:, 1:], columns=['radius_gyration'])
-                r_of_g = r_of_g.round({'radius_gyration': 4})
-
-                track_data_df = pd.concat([track_data_df, msds, step_sizes, r_of_g], axis=1)
-
-                out_data = {'df': track_data_df,
-                            'summary_data': summary_data,
-                            'batch': batch,
-                            }
+                data["radius_gyration"] = 0
+                data["radius_gyration"].where(
+                    data["dim"] != "sum",
+                    other=tracks.r_of_g(track_id, full=False),
+                    inplace=True,
+                )
+
+                data = data.round(
+                    {
+                        "D": 4,
+                        "E": 4,
+                        "r_sq (lin)": 2,
+                        "K": 4,
+                        "a": 4,
+                        "r_sq (log)": 2,
+                        "radius_gyration": 4,
+                    }
+                )
+
+                summary_data = {
+                    "fit_results": data,
+                    "msd": msds[1 : max_lagtime_fit + 1, [0, 4]],
+                }
+
+                track_data_df = track_data_df[track_data_df["track_id"] == track_id]
+                track_data_df.index = range(len(track_data_df))
+
+                msds = pd.DataFrame(msds[:, [0, 4]], columns=["tau", "msd"])
+                msds = msds.round({"msd": 4})
+
+                step_sizes = pd.DataFrame(
+                    step_sizes[:, [0, 4]], columns=["t", "step_size"]
+                )
+                step_sizes = step_sizes.round({"step_size": 4})
+
+                r_of_g = pd.DataFrame(r_of_g[:, 1:], columns=["radius_gyration"])
+                r_of_g = r_of_g.round({"radius_gyration": 4})
+
+                track_data_df = pd.concat(
+                    [track_data_df, msds, step_sizes, r_of_g], axis=1
+                )
+
+                out_data = {
+                    "df": track_data_df,
+                    "summary_data": summary_data,
+                    "batch": batch,
+                }
             else:
                 self.log.emit(f"Track id {track_id} not found.")
 
         self.update_data.emit(out_data)
         super().run()
 
 
@@ -264,56 +375,62 @@
     """Widget for Analysis plugin"""
 
     name = "GEMspaAnalyzeWidget"
 
     def __init__(self, napari_viewer, title="Analyze tracks with GEMspa:"):
         super().__init__(napari_viewer, title)
 
-        self._batch_check = QCheckBox('Process all tracks')
-        self._error_term_fit_check = QCheckBox('Fit with error term')
+        self._batch_check = QCheckBox("Process all tracks")
+        self._error_term_fit_check = QCheckBox("Fit with error term")
         self._color_by_combo = QComboBox()
 
         # Add check boxes for how to draw rainbow tracks
-        self._color_by_checks = [QCheckBox("Track id"),
-                                 QCheckBox("Diffusion coefficient (D)"),
-                                 QCheckBox("Anomalous exponent (alpha)"),
-                                 QCheckBox("Step size (microns)"),
-                                 QCheckBox("Goodness-of-fit for D (R-sq)"),
-                                 QCheckBox("Time (from track start)"),
-                                 QCheckBox("Time (from movie start)")
-                                 ]
-        self._columns_map = {"Track id": "track_id",
-                             "Diffusion coefficient (D)": "D",
-                             "Anomalous exponent (alpha)": "a",
-                             "Step size (microns)": "step_size",
-                             "Goodness-of-fit for D (R-sq)": "r_sq (lin)",
-                             "Time (from movie start)": "frame",
-                             "Time (from track start)": "t"
-                             }
-
-        self._color_by_min_D_input = QLineEdit('0')
-        self._color_by_max_D_input = QLineEdit('2')
-        self._color_by_min_alpha_input = QLineEdit('0')
-        self._color_by_max_alpha_input = QLineEdit('2')
-
-        self._input_values = {'Track id': QLineEdit(''),
-                              'Microns per px': QLineEdit('0.134'),
-                              'Time lag (sec)': QLineEdit('0.010'),
-                              'Min track len for fit (frames)': QLineEdit('11'),
-                              'Max time lag for fit (frames)': QLineEdit('10'),
-                              }
+        self._color_by_checks = [
+            QCheckBox("Track id"),
+            QCheckBox("Diffusion coefficient (D)"),
+            QCheckBox("Anomalous exponent (alpha)"),
+            QCheckBox("Step size (microns)"),
+            QCheckBox("Goodness-of-fit for D (R-sq)"),
+            QCheckBox("Track length (frames)"),
+            QCheckBox("Time (from track start)"),
+            QCheckBox("Time (from movie start)"),
+        ]
+        self._columns_map = {
+            "Track id": "track_id",
+            "Diffusion coefficient (D)": "D",
+            "Anomalous exponent (alpha)": "a",
+            "Step size (microns)": "step_size",
+            "Goodness-of-fit for D (R-sq)": "r_sq (lin)",
+            "Track length (frames)": "track_length",
+            "Time (from movie start)": "frame",
+            "Time (from track start)": "t",
+        }
+
+        self._color_by_min_D_input = QLineEdit("0")
+        self._color_by_max_D_input = QLineEdit("2")
+        self._color_by_min_alpha_input = QLineEdit("0")
+        self._color_by_max_alpha_input = QLineEdit("2")
+
+        self._input_values = {
+            "Track id": QLineEdit(""),
+            "Microns per px": QLineEdit("0.134"),
+            "Time lag (sec)": QLineEdit("0.010"),
+            "Min track len for fit (frames)": QLineEdit("11"),
+            "Max time lag for fit (frames)": QLineEdit("10"),
+        }
         # These must be input by the user
-        self._required_inputs = ['Microns per px',
-                                 'Time lag (sec)',
-                                 'Min track len for fit (frames)',
-                                 'Max time lag for fit (frames)']
+        self._required_inputs = [
+            "Microns per px",
+            "Time lag (sec)",
+            "Min track len for fit (frames)",
+            "Max time lag for fit (frames)",
+        ]
         self.init_ui()
 
     def init_ui(self):
-
         # Set up the input GUI items
         layout = QVBoxLayout()
 
         grid_layout = QGridLayout()
         grid_layout.setContentsMargins(0, 0, 0, 0)
         i = 0
 
@@ -330,15 +447,15 @@
             grid_layout.addWidget(self._input_values[key], i, 1)
             self._input_values[key].setFixedWidth(50)
             i += 1
 
         grid_layout.addWidget(self._error_term_fit_check, i, 0, 1, 2)
         i += 1
 
-        grid_layout.addWidget(QLabel('Show plot of tracks colored by:'), i, 0)
+        grid_layout.addWidget(QLabel("Show plot of tracks colored by:"), i, 0)
         i += 1
 
         for check_box in self._color_by_checks:
             grid_layout.addWidget(check_box, i, 0, 1, 2)
             if check_box.text() == "Diffusion coefficient (D)":
                 grid_layout.addWidget(QLabel("Min"), i, 1)
                 grid_layout.addWidget(self._color_by_min_D_input, i, 2)
@@ -373,151 +490,191 @@
 
     def check_inputs(self):
         # Special case for track id, it is required if batch is not checked
         keys = list(self._input_values.keys())
         required_keys = self._required_inputs[:]
         if self._batch_check.isChecked():
             # ignore track id completely
-            keys.remove('Track id')
+            keys.remove("Track id")
         else:
             # it is required, if batch is not checked
-            required_keys.append('Track id')
+            required_keys.append("Track id")
 
         valid = True
         for key in keys:
             text = self._input_values[key].text()
             if key in required_keys or text:
                 # if input is not blank, check it is a number
                 try:
                     _ = float(text)
                 except ValueError:
                     show_error(f"{key} input must be a number")
                     valid = False
 
-        for line_input in [self._color_by_min_D_input,
-                      self._color_by_max_D_input,
-                      self._color_by_min_alpha_input,
-                      self._color_by_max_alpha_input]:
+        for line_input in [
+            self._color_by_min_D_input,
+            self._color_by_max_D_input,
+            self._color_by_min_alpha_input,
+            self._color_by_max_alpha_input,
+        ]:
             text = line_input.text()
             if text:
                 # if input is not blank, check it is a number
                 try:
                     _ = float(text)
                 except ValueError:
-                    show_error(f"Min/Max for color by must be a number")
+                    show_error("Min/Max for color by must be a number")
                     valid = False
 
         return valid
 
     def state(self, layer_names) -> dict:
-
-        inputs_dict = {'tracks_layer_name': layer_names['tracks'],
-                       'image_layer_name': layer_names['image'],
-                       'tracks_layer_scale': self.viewer.layers[layer_names['tracks']].scale,
-                       'image_layer_shape': self.viewer.layers[layer_names['image']].data.shape,
-                       'tracks_layer_data': self.viewer.layers[layer_names['tracks']].data,
-                       'tracks_layer_props': self.viewer.layers[layer_names['tracks']].properties
-                       }
-        if 'labels' in layer_names:
-            inputs_dict['labels_layer_name'] = layer_names['labels']
-            inputs_dict['labels_layer_data'] = self.viewer.layers[layer_names['labels']].data
+        inputs_dict = {
+            "tracks_layer_name": layer_names["tracks"],
+            "image_layer_name": layer_names["image"],
+            "tracks_layer_scale": self.viewer.layers[layer_names["tracks"]].scale,
+            "image_layer_shape": self.viewer.layers[layer_names["image"]].data.shape,
+            "tracks_layer_data": self.viewer.layers[layer_names["tracks"]].data,
+            "tracks_layer_props": self.viewer.layers[layer_names["tracks"]].properties,
+        }
+        if "labels" in layer_names:
+            inputs_dict["labels_layer_name"] = layer_names["labels"]
+            inputs_dict["labels_layer_data"] = self.viewer.layers[
+                layer_names["labels"]
+            ].data
 
         if self._batch_check.isChecked():
             track_id = None
         else:
-            track_id = convert_to_int(self._input_values['Track id'].text())
+            track_id = convert_to_int(self._input_values["Track id"].text())
 
         color_by = {}
         for check_box in self._color_by_checks:
             color_by[check_box.text()] = check_box.isChecked()
 
-        return {'name': self.name,
-                'inputs': inputs_dict,
-                'parameters': {'track_id': track_id,
-                               'microns_per_pixel': convert_to_float(
-                                   self._input_values['Microns per px'].text()),
-                               'time_lag_sec': convert_to_float(
-                                   self._input_values['Time lag (sec)'].text()),
-                               'min_len_fit': convert_to_int(
-                                   self._input_values['Min track len for fit (frames)'].text()),
-                               'max_lagtime_fit': convert_to_int(
-                                   self._input_values['Max time lag for fit (frames)'].text()),
-                               'batch': self._batch_check.isChecked(),
-                               'error_term_fit': self._error_term_fit_check.isChecked(),
-                               },
-                'color_by': color_by,
-                'color_by_min_max': {'D': [convert_to_float(self._color_by_min_D_input.text()),
-                                           convert_to_float(self._color_by_max_D_input.text())],
-                                     'a': [convert_to_float(self._color_by_min_alpha_input.text()),
-                                           convert_to_float(self._color_by_max_alpha_input.text())]
-                                     }
-                }
+        return {
+            "name": self.name,
+            "inputs": inputs_dict,
+            "parameters": {
+                "track_id": track_id,
+                "microns_per_pixel": convert_to_float(
+                    self._input_values["Microns per px"].text()
+                ),
+                "time_lag_sec": convert_to_float(
+                    self._input_values["Time lag (sec)"].text()
+                ),
+                "min_len_fit": convert_to_int(
+                    self._input_values["Min track len for fit (frames)"].text()
+                ),
+                "max_lagtime_fit": convert_to_int(
+                    self._input_values["Max time lag for fit (frames)"].text()
+                ),
+                "batch": self._batch_check.isChecked(),
+                "error_term_fit": self._error_term_fit_check.isChecked(),
+            },
+            "color_by": color_by,
+            "color_by_min_max": {
+                "D": [
+                    convert_to_float(self._color_by_min_D_input.text()),
+                    convert_to_float(self._color_by_max_D_input.text()),
+                ],
+                "a": [
+                    convert_to_float(self._color_by_min_alpha_input.text()),
+                    convert_to_float(self._color_by_max_alpha_input.text()),
+                ],
+            },
+        }
 
     def update_data(self, out_dict):
         """Set the worker outputs to napari layers"""
 
         layer = None
         title = ""
-        if 'df' in out_dict:
-            df = out_dict['df']
-
-            if out_dict['batch']:
+        if "df" in out_dict:
+            df = out_dict["df"]
 
+            if out_dict["batch"]:
                 # Add layer if run in batch mode
-                kwargs = {'scale': out_dict['tracks_layer_scale'],
-                          'blending': 'translucent',
-                          'tail_length': df['frame'].max(),
-                          'name': 'Analyzed tracks'}
+                kwargs = {
+                    "scale": out_dict["tracks_layer_scale"],
+                    "blending": "translucent",
+                    "tail_length": int(df["frame"].max()),
+                    "name": "Analyzed tracks",
+                }
 
                 layer = self._add_napari_layer("tracks", df, **kwargs)
                 title = layer.name
 
                 # Show full rainbow tracks plot for each type requested
-                img_shape = out_dict['image_layer_shape'][1:]  # assume first dimension of image shape is frame
+                img_shape = out_dict["image_layer_shape"][
+                    1:
+                ]  # assume first dimension of image shape is frame
                 aspect_ratio = img_shape[0] / img_shape[1]
-                color_by = out_dict['color_by']
+                color_by = out_dict["color_by"]
                 for key in color_by.keys():
                     if color_by[key]:
                         col = self._columns_map[key]
-                        plots_viewer = self._new_plots_viewer(f"{title}: {key}", figsize=(6, 6 * aspect_ratio), close_last=False)
-                        if col in out_dict['color_by_min_max']:
-                            color_range = out_dict['color_by_min_max'][col]
-                            print(f"Min/Max for {col} = {color_range[0]}/{color_range[1]}")
+                        plots_viewer = self._new_plots_viewer(
+                            f"{title}: {key}",
+                            figsize=(6, 6 * aspect_ratio),
+                            close_last=False,
+                        )
+                        if col in out_dict["color_by_min_max"]:
+                            color_range = out_dict["color_by_min_max"][col]
+                            print(
+                                f"Min/Max for {col} = {color_range[0]}/{color_range[1]}"
+                            )
                         else:
                             color_range = None
-                        plots_viewer.plot_rainbow_tracks(df, img_shape, col, color_range)
+                        plots_viewer.plot_rainbow_tracks(
+                            df, img_shape, col, color_range
+                        )
                         plots_viewer.show()
             else:
                 title = "Analyzed track"
 
             if self.display_table_view:
                 # Show table of properties (analysis results)
-                if out_dict['batch']:
+                if out_dict["batch"]:
                     # only show one line for each track if run in batch mode
                     # take last not first when dropping duplicates to pull the r-of-g for full length track
                     # remove the tracks that were filtered for length (fit results are all nan's)
-                    df = df.drop_duplicates(subset='track_id', keep='last')
-                    df = df.drop(labels=['frame', 'y', 'x', 'tau', 'msd', 't', 'step_size'], axis=1)
-                    if 'z' in df.columns:
+                    df = df.drop_duplicates(subset="track_id", keep="last")
+                    df = df[df["MSD_fitted"] == 1]
+                    df = df.drop(
+                        labels=[
+                            "frame",
+                            "y",
+                            "x",
+                            "y (microns)",
+                            "x (microns)",
+                            "tau",
+                            "msd",
+                            "t",
+                            "step_size",
+                            "MSD_fitted",
+                        ],
+                        axis=1,
+                    )
+                    if "z" in df.columns:
                         # also drop z if it exists
-                        df = df.drop(labels=['z'], axis=1)
-                    df.dropna(inplace=True,
-                              subset=['D', 'E', 'r_sq (lin)', 'K', 'a', 'r_sq (log)'],
-                              how='all')
+                        df = df.drop(labels=["z", "z (microns)"], axis=1)
 
                 properties_viewer = self._new_properties_viewer(title, close_last=False)
                 properties_viewer.reload_from_pandas(df)
                 properties_viewer.show()
 
-            if 'summary_data' in out_dict:
-                plots_viewer = self._new_plots_viewer(title, close_last=False)
+            if "summary_data" in out_dict:
+                if out_dict["batch"]:
+                    plots_viewer = self._new_plots_viewer(title, close_last=False)
+                else:
+                    plots_viewer = self._new_plots_viewer(
+                        title, figsize=(10, 3), close_last=False
+                    )
+
                 plots_viewer.plot_analyze_results(out_dict)
                 plots_viewer.show()
 
-                if out_dict['batch']:
+                if out_dict["batch"]:
                     plots_viewer = self._new_plots_viewer(title, close_last=False)
                     plots_viewer.plot_tracks_info(out_dict)
                     plots_viewer.show()
-
-
-
-
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_data_views.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_data_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+"""Defines: GEMspaPlottingWindow, GEMspaTableWidget, GEMspaTableWindow"""
+
+import matplotlib as mpl
 import napari
-import pandas as pd
 import numpy as np
-import matplotlib as mpl
-from qtpy.QtCore import Qt, QCoreApplication, QRect
-from qtpy.QtWidgets import (QWidget, QApplication, QVBoxLayout,
-                            QTableWidget, QAbstractItemView, QTableWidgetItem,
-                            QMainWindow, QMenuBar, QMenu, QAction, QFileDialog)
-
-from matplotlib.backends.backend_qtagg import (FigureCanvas, NavigationToolbar2QT as NavigationToolbar)
+import pandas as pd
+from matplotlib.backends.backend_qtagg import FigureCanvas
+from matplotlib.backends.backend_qtagg import NavigationToolbar2QT as NavigationToolbar
 from matplotlib.figure import Figure
-
-
-"""Defines: GEMspaPlottingWindow, GEMspaTableWidget, GEMspaTableWindow"""
+from qtpy.QtCore import QCoreApplication, QRect, Qt
+from qtpy.QtWidgets import (
+    QAbstractItemView,
+    QAction,
+    QApplication,
+    QFileDialog,
+    QMainWindow,
+    QMenu,
+    QMenuBar,
+    QTableWidget,
+    QTableWidgetItem,
+    QVBoxLayout,
+    QWidget,
+)
 
 
 class GEMspaPlottingWindow(QMainWindow):
     """Main window for showing plots"""
 
     def __init__(self, napari_viewer, figsize=(8, 3), *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -43,235 +52,285 @@
 
         for i, row in enumerate(df.iterrows()):
             for j, col in enumerate(df.columns):
                 val = row[1][col]
                 t.setItem(i, j, QTableWidgetItem(str(val)))
 
     def plot_locate_results(self, df):
-
         self.canvas.figure.clear()
         axs = self.canvas.figure.subplots(1, 3)
 
         # Show Mass histogram
-        axs[0].hist(df['mass'], bins=20)
-        axs[0].set(xlabel='mass', ylabel='count')
-        axs[0].set_title('mass')
+        axs[0].hist(df["mass"], bins=20)
+        axs[0].set(xlabel="mass", ylabel="count")
+        axs[0].set_title("mass")
 
         # Show subpixel bias (histogram fractional part of x/y positions)
-        axs[1].hist(np.modf(df['x'])[0], bins=20)
-        axs[1].set(xlabel='x', ylabel='count')
-        axs[1].set_title('sub px bias (x)')
-
-        axs[2].hist(np.modf(df['y'])[0], bins=20)
-        axs[2].set(xlabel='y', ylabel='count')
-        axs[2].set_title('sub px bias (y)')
+        axs[1].hist(np.modf(df["x"])[0], bins=20)
+        axs[1].set(xlabel="x", ylabel="count")
+        axs[1].set_title("sub px bias (x)")
+
+        axs[2].hist(np.modf(df["y"])[0], bins=20)
+        axs[2].set(xlabel="y", ylabel="count")
+        axs[2].set_title("sub px bias (y)")
 
         self.canvas.figure.tight_layout()
 
     def plot_link_results(self, df):
-
         self.canvas.figure.clear()
         axs = self.canvas.figure.subplots(1, 3)
 
         # Show plots of mass vs. size and mass vs. eccentricity
-        mean_t = df.groupby('track_id').mean()
+        mean_t = df.groupby("track_id").mean()
 
-        axs[0].plot(mean_t['mass'], mean_t['size'], 'ko', alpha=0.1)
-        axs[0].set(xlabel='mass', ylabel='size')
-        axs[0].set_title('mass vs size')
-
-        axs[1].plot(mean_t['mass'], mean_t['ecc'], 'ko', alpha=0.3)
-        axs[1].set(xlabel='mass', ylabel='eccentricity (0=circular)')
-        axs[1].set_title('mass vs eccentricity')
+        axs[0].plot(mean_t["mass"], mean_t["size"], "ko", alpha=0.3)
+        axs[0].set(xlabel="mass", ylabel="size")
+        axs[0].set_title("mass vs size")
+
+        axs[1].plot(mean_t["mass"], mean_t["ecc"], "ko", alpha=0.3)
+        axs[1].set(xlabel="mass", ylabel="eccentricity (0=circular)")
+        axs[1].set_title("mass vs eccentricity")
 
         # Show track length histogram
-        track_lengths = df['track_id'].value_counts(sort=False)
+        track_lengths = df["track_id"].value_counts(sort=False)
 
-        axs[2].hist(track_lengths, bins=range(0, track_lengths.max()+1, 1)) #, histtype='step')
-        axs[2].set(xlabel='track length', ylabel='counts')
-        axs[2].set_title('Track lengths histogram')
+        axs[2].hist(track_lengths, bins=30)
+        axs[2].set(xlabel="track length", ylabel="counts")
+        axs[2].set_title("Track lengths histogram")
 
         self.canvas.figure.tight_layout()
 
-    def plot_rainbow_tracks(self, df, img_shape=None, color_by="track_id", color_range=None):
+    def plot_rainbow_tracks(
+        self, df, img_shape=None, color_by="track_id", color_range=None
+    ):
         self.canvas.figure.clear()
         ax = self.canvas.figure.subplots(1, 1)
 
         if color_range is not None:
             min_val = color_range[0]
             max_val = color_range[1]
 
             if max_val < min_val:
                 print("Rainbow tracks: Max/Min are invalid, using defaults...")
                 color_range = None
 
         if color_range is None:
             min_val = 0
-            if color_by in ['step_size', 'frame']:
+            if color_by in ["step_size", "frame", "track_length"]:
                 max_val = df[color_by].max()
             elif color_by == "D":
                 max_val = 2
             elif color_by == "a":
                 max_val = 2
             elif color_by == "r_sq (lin)":
                 max_val = 1
 
         if img_shape is not None:
             max_y = img_shape[0]
         else:
-            max_y = df['y'].max()
+            max_y = df["y"].max()
 
         def get_color(v):
             if v < min_val:
                 v = min_val
             if v > max_val:
                 v = max_val
             return (v - min_val) / (max_val - min_val)
 
         # Plot all tracks
-        for group in df.groupby('track_id'):
+        for group in df.groupby("track_id"):
             track_data = group[1]
-            if color_by == 'track_id':
-                ax.plot(track_data['x'], track_data['y'], '-')
-            elif color_by in ['D', 'a', 'r_sq (lin)']:
+            if color_by == "track_id":
+                ax.plot(track_data["x"], track_data["y"], "-")
+            elif color_by in ["D", "a", "r_sq (lin)", "track_length"]:
                 val = track_data.iloc[0][color_by]
                 if not np.isnan(val):
-                    ax.plot(track_data['x'], track_data['y'],
-                            '-', color=mpl.cm.jet(get_color(val)))
-            elif color_by in ['step_size', 'frame']:
+                    ax.plot(
+                        track_data["x"],
+                        track_data["y"],
+                        "-",
+                        color=mpl.cm.jet(get_color(val)),
+                    )
+            elif color_by in ["step_size", "frame"]:
                 for step_i in range(1, len(track_data), 1):
                     val = track_data.iloc[step_i][color_by]
                     if not np.isnan(val):
-                        ax.plot([track_data.iloc[step_i-1]['x'], track_data.iloc[step_i]['x']],
-                                [track_data.iloc[step_i-1]['y'], track_data.iloc[step_i]['y']],
-                                '-', color=mpl.cm.jet(get_color(val)))
+                        ax.plot(
+                            [
+                                track_data.iloc[step_i - 1]["x"],
+                                track_data.iloc[step_i]["x"],
+                            ],
+                            [
+                                track_data.iloc[step_i - 1]["y"],
+                                track_data.iloc[step_i]["y"],
+                            ],
+                            "-",
+                            color=mpl.cm.jet(get_color(val)),
+                        )
             elif color_by == "t":
                 max_val = len(track_data)
                 for step_i in range(1, max_val, 1):
                     show_color = step_i / max_val
-                    ax.plot([track_data.iloc[step_i - 1]['x'], track_data.iloc[step_i]['x']],
-                            [track_data.iloc[step_i - 1]['y'], track_data.iloc[step_i]['y']],
-                            '-', color=mpl.cm.jet(show_color))
+                    ax.plot(
+                        [
+                            track_data.iloc[step_i - 1]["x"],
+                            track_data.iloc[step_i]["x"],
+                        ],
+                        [
+                            track_data.iloc[step_i - 1]["y"],
+                            track_data.iloc[step_i]["y"],
+                        ],
+                        "-",
+                        color=mpl.cm.jet(show_color),
+                    )
             else:
                 print("Rainbow tracks: Unknown color_by option, using track_id...")
-                ax.plot(group[1]['x'], group[1]['y'], '-')
+                ax.plot(group[1]["x"], group[1]["y"], "-")
 
         if img_shape is not None and len(img_shape) > 1:
             ax.set_xlim(0, img_shape[1])
             ax.set_ylim(0, img_shape[0])
 
         ax.set_ylim(max_y, 0)
 
-        if color_by != 'track_id':
-            if color_by == 't':
+        if color_by != "track_id":
+            if color_by == "t":
                 norm = mpl.colors.Normalize(vmin=0, vmax=1)
-                cmap = mpl.cm.ScalarMappable(norm=norm, cmap='jet')
-                cbar = self.canvas.figure.colorbar(cmap)
+                cmap = mpl.cm.ScalarMappable(norm=norm, cmap="jet")
+                cbar = self.canvas.figure.colorbar(cmap, ax=ax)
                 cbar.set_ticks([0, 1])
-                cbar.set_ticklabels(['Start', 'End'])
+                cbar.set_ticklabels(["Start", "End"])
             else:
                 norm = mpl.colors.Normalize(vmin=min_val, vmax=max_val)
-                cmap = mpl.cm.ScalarMappable(norm=norm, cmap='jet')
-                cbar = self.canvas.figure.colorbar(cmap)
+                cmap = mpl.cm.ScalarMappable(norm=norm, cmap="jet")
+                self.canvas.figure.colorbar(cmap, ax=ax)
 
         self.canvas.figure.tight_layout()
 
     def plot_tracks_info(self, out_data):
-
-        df = out_data['df']
+        df = out_data["df"]
 
         self.canvas.figure.clear()
         axs = self.canvas.figure.subplots(1, 3)
 
         # Show track length histogram
-        track_lengths = df['track_id'].value_counts(sort=False)
+        track_lengths = df["track_id"].value_counts(sort=False)
 
-        axs[0].hist(track_lengths, bins=range(0, track_lengths.max() + 1, 1))  # , histtype='step')
-        axs[0].set(xlabel='track length', ylabel='counts')
-        axs[0].set_title('Track lengths (# frames)')
+        axs[0].hist(track_lengths, bins=30)
+        axs[0].set(xlabel="track length", ylabel="counts")
+        axs[0].set_title("Track lengths (# frames)")
 
         # Show r of g histogram - only final r of g
-        df = df.drop_duplicates(subset='track_id', keep='last')
-        rg = df['radius_gyration']
+        df = df.drop_duplicates(subset="track_id", keep="last")
+        rg = df["radius_gyration"]
 
-        axs[1].hist(rg, bins=np.linspace(0, rg.max(), 30))  # , histtype='step')
-        axs[1].set(xlabel='radius', ylabel='counts')
-        axs[1].set_title('Radius of gyration (microns)')
+        axs[1].hist(rg, bins=30)
+        axs[1].set(xlabel="radius", ylabel="counts")
+        axs[1].set_title("Radius of gyration (microns)")
 
         # Scatter
-        axs[2].scatter(track_lengths, rg, s=4)
-        axs[2].set(xlabel='Track length', ylabel='Radius of gyration')
-        axs[2].set_title('Scatter')
+        axs[2].plot(track_lengths, rg, "ko", alpha=0.3)
+        axs[2].set(xlabel="Track length", ylabel="Radius of gyration")
+        axs[2].set_title("Scatter")
 
         self.canvas.figure.tight_layout()
 
     def plot_analyze_results(self, out_data):
-
         summary_table = QTableWidget()
         self.verticalLayout.addWidget(summary_table)
 
-        if 'ens_fit_results' in out_data['summary_data'] and 'ens_msd' in out_data['summary_data']:
-            plot_data = out_data['summary_data']
+        if (
+            "ens_fit_results" in out_data["summary_data"]
+            and "ens_msd" in out_data["summary_data"]
+        ):
+            plot_data = out_data["summary_data"]
 
-            msd = plot_data['ens_msd']
-            df = plot_data['ens_fit_results']
+            msd = plot_data["ens_msd"]
+            df = plot_data["ens_fit_results"]
 
             # Table of data
             self._fill_table(summary_table, df)
 
-            D = df.iloc[0]['D']
-            alpha = df.iloc[0]['a']
+            D = df.iloc[0]["D"]
+            alpha = df.iloc[0]["a"]
 
             # Ensemble MSD plot
             self.canvas.figure.clear()
             axs = self.canvas.figure.subplots(1, 2)
             axs[0].scatter(msd[:, 0], msd[:, 1])
             axs[1].scatter(msd[:, 0], msd[:, 1])
-            axs[1].set_xscale('log', base=10)
-            axs[1].set_yscale('log', base=10)
-            axs[0].set(xlabel=r'$\tau$ $(s)$', ylabel=r'$MSD$ ($\mu m^{2}$)')
-            axs[1].set(xlabel=r'$log_{10}$ $\tau$ $(s)$', ylabel=r'$log_{10}$ $MSD$ ($\mu m^{2}$)')
+            axs[1].set_xscale("log", base=10)
+            axs[1].set_yscale("log", base=10)
+            axs[0].set(xlabel=r"$\tau$ $(s)$", ylabel=r"$MSD$ ($\mu m^{2}$)")
+            axs[1].set(
+                xlabel=r"$log_{10}$ $\tau$ $(s)$",
+                ylabel=r"$log_{10}$ $MSD$ ($\mu m^{2}$)",
+            )
             axs[0].set_title(f"ens-avg MSD (2d)\nD = {D} " + r"$\mu m^{2}$/s")
-            axs[1].set_title(f"ens-avg log-log MSD (2d)\n" + r"$\alpha$ = " + f"{alpha}")
+            axs[1].set_title("ens-avg log-log MSD (2d)\n" + r"$\alpha$ = " + f"{alpha}")
 
-        elif 'fit_results' in out_data['summary_data'] and 'msd' in out_data['summary_data']:
-
-            plot_data = out_data['summary_data']
-            msd = plot_data['msd']
-            df = plot_data['fit_results']
+        elif (
+            "fit_results" in out_data["summary_data"]
+            and "msd" in out_data["summary_data"]
+        ):
+            plot_data = out_data["summary_data"]
+            df = out_data["df"]
+            msd = plot_data["msd"]
+            summary_df = plot_data["fit_results"]
 
             # Table of data
-            self._fill_table(summary_table, df)
+            self._fill_table(summary_table, summary_df)
 
-            D = df[df.dim == 'sum'].iloc[0]['D']
-            alpha = df[df.dim == 'sum'].iloc[0]['a']
-            track_id = int(df.iloc[0]['track_id'])
+            D = summary_df[summary_df.dim == "sum"].iloc[0]["D"]
+            alpha = summary_df[summary_df.dim == "sum"].iloc[0]["a"]
+            track_id = int(summary_df.iloc[0]["track_id"])
 
             # Make plots (MSD of track, with fit line, linear and loglog scale)
             self.canvas.figure.clear()
-            axs = self.canvas.figure.subplots(1, 3)
+            axs = self.canvas.figure.subplots(1, 4)
             axs[0].scatter(msd[:, 0], msd[:, 1])
             axs[1].scatter(msd[:, 0], msd[:, 1])
-            axs[1].set_xscale('log', base=10)
-            axs[1].set_yscale('log', base=10)
-            axs[0].set(xlabel=r'$\tau$ $(s)$', ylabel=r'$MSD$ ($\mu m^{2}$)')
-            axs[1].set(xlabel=r'$log_{10}$ $\tau$ $(s)$', ylabel=r'$log_{10}$ $MSD$ ($\mu m^{2}$)')
-            axs[0].set_title(f'track {track_id} MSD (2d)\nD = {D} ' + r'$\mu m^{2}$/s')
-            axs[1].set_title(f'track {track_id} log-log MSD (2d)\n' + r'$\alpha$ = ' + f'{alpha}')
+            axs[1].set_xscale("log", base=10)
+            axs[1].set_yscale("log", base=10)
+            axs[0].set(xlabel=r"$\tau$ $(s)$", ylabel=r"$MSD$ ($\mu m^{2}$)")
+            axs[1].set(
+                xlabel=r"$log_{10}$ $\tau$ $(s)$",
+                ylabel=r"$log_{10}$ $MSD$ ($\mu m^{2}$)",
+            )
+            axs[0].set_title(f"track {track_id} MSD (2d)\nD = {D} " + r"$\mu m^{2}$/s")
+            axs[1].set_title(
+                f"track {track_id} log-log MSD (2d)\n" + r"$\alpha$ = " + f"{alpha}"
+            )
 
-            # Make plot of the track itself...
-            df = out_data['df']
-            x_min = df['x'].min()
-            y_min = df['y'].min()
-
-            axs[2].plot(df['x']-x_min, df['y']-y_min)
-            axs[2].plot(df.iloc[0]['x']-x_min, df.iloc[0]['y']-y_min, '.', color='green')
-            axs[2].plot(df.iloc[-1]['x']-x_min, df.iloc[-1]['y']-y_min, '.', color='red')
+            # Make plot of radius of gyration...
+            axs[2].plot(df["t"], df["radius_gyration"])
             axs[2].set_title(f"track {track_id}")
-            axs[2].set(xlabel="x", ylabel="y")
+            axs[2].set(xlabel="t (s)", ylabel="radius gyration " + r"($\mu m$)")
+
+            # Make plot of the track itself...
+            x_values = df["x (microns)"].to_numpy()
+            y_values = df["y (microns)"].to_numpy()
+            x_min = np.min(x_values)
+            y_min = np.min(y_values)
+
+            axs[3].plot(x_values - x_min, y_values - y_min)
+            axs[3].plot(
+                x_values[0] - x_min,
+                y_values[0] - y_min,
+                ".",
+                color="green",
+            )
+            axs[3].plot(
+                x_values[-1] - x_min,
+                y_values[-1] - y_min,
+                ".",
+                color="red",
+            )
+            axs[3].set_title(f"track {track_id}")
+            axs[3].set(xlabel=r"x ($\mu m$)", ylabel=r"y ($\mu m$)")
 
         self.canvas.figure.tight_layout()
 
 
 class GEMspaTableWidget(QTableWidget):
     """
     this class extends QTableWidget
@@ -279,24 +338,23 @@
     * formatted specifically to work with multiple-cell paste into programs
       like google sheets, excel, or numbers
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def copy_selection_to_clipboard(self, sep='\t'):
+    def copy_selection_to_clipboard(self, sep="\t"):
         copied_cells = sorted(self.selectedIndexes())
-        if(len(copied_cells) > 0):
-
-            copy_text = ''
+        if len(copied_cells) > 0:
+            copy_text = ""
             max_column = copied_cells[-1].column()
             for c in copied_cells:
                 copy_text += self.item(c.row(), c.column()).text()
                 if c.column() == max_column:
-                    copy_text += '\n'
+                    copy_text += "\n"
                 else:
                     copy_text += sep
 
             QApplication.clipboard().setText(copy_text)
 
     def save_to_file(self, fname):
         nrows = self.rowCount()
@@ -309,27 +367,28 @@
         for i in range(nrows):
             data = []
             for j in range(ncols):
                 data.append(self.item(i, j).text())
             full_data.append(data)
 
         df = pd.DataFrame(full_data, columns=headers)
-        df.to_csv(fname, sep='\t', index=False)
+        df.to_csv(fname, sep="\t", index=False)
 
     def select_all(self):
         self.selectAll()
 
     def keyPressEvent(self, event):
         super().keyPressEvent(event)
-        if event.key() == Qt.Key_C and (QApplication.keyboardModifiers() & Qt.ControlModifier):
+        if event.key() == Qt.Key_C and (
+            QApplication.keyboardModifiers() & Qt.ControlModifier
+        ):
             self.copy_selection_to_clipboard()
 
 
 class GEMspaTableWindow(QMainWindow):
-
     def __init__(self, napari_viewer):
         super().__init__()
         self.viewer = napari_viewer
 
         self.setGeometry(QRect(100, 100, 600, 200))
 
         self.centralWidget = QWidget(self)
@@ -398,15 +457,17 @@
     def select_all(self):
         self.tableWidget.select_all()
 
     def save(self):
         pass
 
     def save_as(self):
-        file_name = QFileDialog.getSaveFileName(self, "Save file...", "", "Text, tab-delimited (*.txt)")
+        file_name = QFileDialog.getSaveFileName(
+            self, "Save file...", "", "Text, tab-delimited (*.txt)"
+        )
         print(f"Saving {file_name}...")
         self.tableWidget.save_to_file(file_name[0])
 
     def reload_from_pandas(self, df):
         """Fill the table with the data in a pandas data frame"""
         self.tableWidget.clearContents()
         self.tableWidget.setColumnCount(len(df.columns))
@@ -419,39 +480,45 @@
 
     def reload_from_layer(self, layer_name):
         """Reload the properties from the layer to the table widget"""
 
         data = self.viewer.layers[layer_name].data
         properties = self.viewer.layers[layer_name].properties
         headers = []
-        if isinstance(self.viewer.layers[layer_name], napari.layers.points.points.Points):
+        if isinstance(
+            self.viewer.layers[layer_name], napari.layers.points.points.Points
+        ):
             if data.shape[1] == 3:
-                headers = ['frame', 'y', 'x']
+                headers = ["frame", "y", "x"]
             elif data.shape[1] == 4:
-                headers = ['frame', 'z', 'y', 'x']
+                headers = ["frame", "z", "y", "x"]
 
-        elif isinstance(self.viewer.layers[layer_name], napari.layers.tracks.tracks.Tracks):
+        elif isinstance(
+            self.viewer.layers[layer_name], napari.layers.tracks.tracks.Tracks
+        ):
             if data.shape[1] == 4:
-                headers = ['track_id', 'frame', 'y', 'x']
+                headers = ["track_id", "frame", "y", "x"]
             elif data.shape[1] == 5:
-                headers = ['track_id', 'frame', 'z', 'y', 'x']
+                headers = ["track_id", "frame", "z", "y", "x"]
 
             # Avoid repeated column: napari adds track_id column to properties
-            del properties['track_id']
+            del properties["track_id"]
 
         for key in properties:
             headers.append(key)
 
         self.tableWidget.setColumnCount(len(headers))
         self.tableWidget.setHorizontalHeaderLabels(headers)
         self.tableWidget.setRowCount(data.shape[0])
 
         for line in range(data.shape[0]):
             for col in range(data.shape[1]):
-                self.tableWidget.setItem(line, col, QTableWidgetItem(str(data[line, col])))
+                self.tableWidget.setItem(
+                    line, col, QTableWidgetItem(str(data[line, col]))
+                )
 
         # properties
         col = data.shape[1]
         for key in properties:
             prop = properties[key]
             for line in range(len(prop)):
                 self.tableWidget.setItem(line, col, QTableWidgetItem(str(prop[line])))
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_file_import_widget.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_file_import_widget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,166 @@
-from qtpy.QtWidgets import (QGridLayout, QVBoxLayout, QFileDialog, QRadioButton, QPushButton, QWidget,
-                            QLabel, QGroupBox)
-from ._utils import show_error
+"""Defines: GEMspaFileImport, GEMspaFileImportWidget"""
+
 import os
-import pandas as pd
-import nd2
-from skimage import io
+
 import napari
+import nd2
 import numpy as np
+import pandas as pd
 from gemspa_spt import ParticleTracks
+from qtpy.QtWidgets import (
+    QFileDialog,
+    QGridLayout,
+    QGroupBox,
+    QLabel,
+    QPushButton,
+    QRadioButton,
+    QVBoxLayout,
+    QWidget,
+)
+from skimage import io
 
-
-"""Defines: GEMspaFileImport, GEMspaFileImportWidget"""
+from ._utils import show_error
 
 
 class GEMspaFileImport:
-
     def __init__(self, path, data_format):
-
         if data_format not in ParticleTracks.file_columns.keys():
-            raise ValueError(f"Unexpected file format: {data_format} when importing file.")
+            raise ValueError(
+                f"Unexpected file format: {data_format} when importing file."
+            )
 
         self.file_path = path
         self.file_format = data_format
         file_ext = os.path.splitext(self.file_path)[1].lower()
-        if file_ext == '.csv':
-            self.file_sep = ','
-        elif file_ext == '.txt' or file_ext == '.tsv':
-            self.file_sep = '\t'
+        if file_ext == ".csv":
+            self.file_sep = ","
+        elif file_ext == ".txt" or file_ext == ".tsv":
+            self.file_sep = "\t"
         else:
-            print(f"Unknown extension found for '{self.file_path}'. Attempting to open as a tab-delimited text file.")
-            self.file_sep = '\t'
+            print(
+                f"Unknown extension found for '{self.file_path}'. Attempting to open as a tab-delimited text file."
+            )
+            self.file_sep = "\t"
+
+        self.file_df = pd.read_csv(
+            self.file_path,
+            sep=self.file_sep,
+            header=0,
+            skiprows=ParticleTracks.skip_rows[data_format],
+        )
 
-        self.file_df = pd.read_csv(self.file_path, sep=self.file_sep, header=0,
-                                   skiprows=ParticleTracks.skip_rows[data_format])
-        self.file_df.columns = [item.lower() for item in self.file_df.columns]
+    def find_col(self, target_string):
+        lower_target = target_string.lower()
+        for col in self.file_df.columns:
+            if col.lower() == lower_target:
+                return col
+        return None
 
     def get_layer_data(self):
-
         all_cols = ParticleTracks.file_columns[self.file_format]
-        cols = all_cols[3:5]  # ['y','x']: mandatory
-        for col in cols:
-            if col not in self.file_df.columns:
-                raise Exception(f"Error in importing file: required column {col} is missing.")
-
-        if all_cols[2] in self.file_df.columns:  # 'z': optional, add if it exists
-            cols.insert(0, all_cols[2])
-
-        if all_cols[1] in self.file_df.columns:  # 'frame': optional, add if it exists
-            cols.insert(0, all_cols[1])
+        orig_cols = []
 
-        if all_cols[0] in self.file_df.columns:  # 'track_id': optional, if it exists this is tracks data (not points)
-            if cols[0] != all_cols[1]:  # must have 'frame' column if there is a 'track_id' column
+        # 'x' is mandatory
+        col = self.find_col(all_cols[4])
+        if col is None:
+            raise Exception(
+                f"Error in importing file: required column {all_cols[4]} is missing."
+            )
+        orig_cols.insert(0, col)
+
+        # 'y' is mandatory
+        col = self.find_col(all_cols[3])
+        if col is None:
+            raise Exception(
+                f"Error in importing file: required column {all_cols[3]} is missing."
+            )
+        orig_cols.insert(0, col)
+
+        # 'z' is optional
+        col = self.find_col(all_cols[2])
+        if col:
+            orig_cols.insert(0, col)
+
+        # 'frame' is optional
+        frame_col = self.find_col(all_cols[1])
+        if frame_col:
+            orig_cols.insert(0, frame_col)
+
+        # 'track_id' is optional; if it exists this is tracks data (not points)
+        track_id_col = self.find_col(all_cols[0])
+        if track_id_col:
+            if frame_col is None:
                 raise Exception(
-                    f"Error in importing file data: data appears to be tracks layer but frame column is missing.")
-            cols.insert(0, all_cols[0])
+                    "Error in importing file data: data appears to be tracks layer but frame column is missing."
+                )
+            orig_cols.insert(0, track_id_col)
             layer_type = "tracks"
         else:
             layer_type = "points"
 
         # data and properties for the layer data tuple
-        data = self.file_df[cols].to_numpy()
+        data = self.file_df[orig_cols].to_numpy()
         props = {}
         for col in self.file_df.columns:
-            if col not in cols:
-                props[col] = self.file_df[col].to_numpy()
+            if col not in orig_cols:
+                # nan_to_num because napari properties does not handle nan data
+                props[col] = np.nan_to_num(self.file_df[col].to_numpy())
 
         # add properties and other keyword args
-        add_kwargs = {'properties': props,
-                      'name': os.path.split(self.file_path)[1]}
-        if layer_type == 'points':
-            add_kwargs['face_color'] = 'transparent'
-            add_kwargs['edge_color'] = 'red'
-        elif layer_type == 'tracks':
-            add_kwargs['blending'] = 'translucent'
-            add_kwargs['tail_length'] = data[:, 1].max()
+        add_kwargs = {"properties": props, "name": os.path.split(self.file_path)[1]}
+        if layer_type == "points":
+            add_kwargs["face_color"] = "transparent"
+            add_kwargs["edge_color"] = "red"
+        elif layer_type == "tracks":
+            add_kwargs["blending"] = "translucent"
+            add_kwargs["tail_length"] = int(data[:, 1].max())
 
         return data, add_kwargs, layer_type
 
 
 class GEMspaFileImportWidget(QWidget):
     """Widget for Import file plugin"""
 
-    name = 'GEMspaFileImportWidget'
+    name = "GEMspaFileImportWidget"
 
     def __init__(self, napari_viewer):
         super().__init__()
 
         self.viewer = napari_viewer
 
-        self._track_file_format_rbs = [QRadioButton("GEMspa", self),
-                                       QRadioButton("Mosaic", self),
-                                       QRadioButton("Trackmate", self),
-                                       QRadioButton("Trackpy", self)
-                                       ]
+        self._track_file_format_rbs = [
+            QRadioButton("GEMspa", self),
+            QRadioButton("Mosaic", self),
+            QRadioButton("Trackmate", self),
+            QRadioButton("Trackpy", self),
+        ]
 
         self._open_tracks_file_btn = QPushButton("Open file...", self)
         self._open_image_file_btn = QPushButton("Open file...", self)
         self._open_labels_file_btn = QPushButton("Open file...", self)
         self._new_labels_layer_btn = QPushButton("Add layer", self)
 
         self.init_ui()
 
     def init_ui(self):
-
         layout = QVBoxLayout()
 
         group = QGroupBox("Add image layer")
         group_layout = QVBoxLayout()
         group_layout.addWidget(QLabel("Open image file (nd2/tif time-lapse movie):"))
         group_layout.addWidget(self._open_image_file_btn)
         group.setLayout(group_layout)
         layout.addWidget(group)
 
         group = QGroupBox("Add labels layer")
         group_layout = QGridLayout()
-        group_layout.addWidget(QLabel("Create blank 2D labels layer for selected image:"), 0, 0)
+        group_layout.addWidget(
+            QLabel("Create blank 2D labels layer for selected image:"), 0, 0
+        )
         group_layout.addWidget(self._new_labels_layer_btn, 0, 1)
         group_layout.addWidget(QLabel("Open labels file:"), 1, 0)
         group_layout.addWidget(self._open_labels_file_btn, 1, 1)
         group.setLayout(group_layout)
         layout.addWidget(group)
 
         group = QGroupBox("Add tracks layer")
@@ -147,68 +189,64 @@
 
         found_image = False
         if len(selected_layers) > 0:
             for layer in selected_layers:
                 if isinstance(layer, napari.layers.image.image.Image):
                     # get final 2 image dimensions and create mask
                     dims = layer.data.shape[-2:]
-                    new_mask = np.zeros(dims, dtype='int64')
+                    new_mask = np.zeros(dims, dtype="int64")
                     self.viewer.add_labels(new_mask)
                     found_image = True
                     break
 
         if not found_image:
             show_error("Cannot create labels layer: no selected image layer found.")
 
     def _load_image_file(self):
         filename, _ = QFileDialog.getOpenFileName(
-            self,
-            "time-lapse movies (*.tif *.tiff *.nd2)"
+            self, "time-lapse movies (*.tif *.tiff *.nd2)"
         )
         if filename:
             ext = os.path.splitext(filename)[1]
             if ext == ".nd2":
                 f = nd2.ND2File(filename)
                 images = f.asarray()
                 f.close()
-            elif ext == '.tif' or ext == '.tiff':
+            elif ext == ".tif" or ext == ".tiff":
                 images = io.imread(filename)
             else:
                 raise ValueError(f"Unrecognized file extension for image file {ext}")
 
             self.viewer.add_image(images, name=os.path.split(filename)[1])
 
     def _load_labels_file(self):
         filename, _ = QFileDialog.getOpenFileName(
             self,
-            "images with integer labels (*.png *.jpg *.jpeg *.bmp *.gif *.tif *.tiff *.jp2)"
+            "images with integer labels (*.png *.jpg *.jpeg *.bmp *.gif *.tif *.tiff *.jp2)",
         )
         if filename:
             labeled_image = io.imread(filename)
             self.viewer.add_labels(labeled_image, name=os.path.split(filename)[1])
 
     def _load_tracks_file(self):
-
         filename, _ = QFileDialog.getOpenFileName(
-            self,
-            "tab or comma delimited text files (*.txt *.tsv *.csv)"
+            self, "tab or comma delimited text files (*.txt *.tsv *.csv)"
         )
         if filename:
-
             # Get selected format for imported file
-            data_format = self._format_rbs[0].text()
-            for rb in self._format_rbs:
+            data_format = self._track_file_format_rbs[0].text()
+            for rb in self._track_file_format_rbs:
                 if rb.isChecked():
                     data_format = rb.text()
                     break
             data_format = data_format.lower()
 
             file_import = GEMspaFileImport(filename, data_format)
             layer_data = file_import.get_layer_data()
 
             # Add layer (points or tracks)
-            if layer_data[2] == 'points':
+            if layer_data[2] == "points":
                 self.viewer.add_points(layer_data[0], **layer_data[1])
-            elif layer_data[2] == 'tracks':
+            elif layer_data[2] == "tracks":
                 self.viewer.add_tracks(layer_data[0], **layer_data[1])
             else:
                 pass
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_filter_links_widget.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_filter_links_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,173 @@
-from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+"""Defines: GEMspaFilterLinksWidget, GEMspaFilterLinksWorker"""
+
 import trackpy as tp
-from qtpy.QtWidgets import QLineEdit
 from qtpy.QtCore import Slot
-from ._utils import show_error, convert_to_int, convert_to_float
+from qtpy.QtWidgets import QLineEdit
 
-"""Defines: GEMspaFilterLinksWidget, GEMspaFilterLinksWorker"""
+from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+from ._utils import convert_to_float, convert_to_int, show_error
 
 
 class GEMspaFilterLinksWorker(GEMspaWorker):
-    """Worker for the Link Features plugin
-
-    """
+    """Worker for the Link Features plugin"""
 
     def __init__(self):
         super().__init__()
 
     @Slot(dict)
     def run(self, state):
         """Execute the processing"""
 
-        input_params = state['inputs']
-        state_params = state['parameters']
+        input_params = state["inputs"]
+        state_params = state["parameters"]
 
-        min_frames = state_params['min_frames']
-        min_mass = state_params['min_mass']
-        max_mass = state_params['max_mass']
-        min_size = state_params['min_size']
-        max_size = state_params['max_size']
-        min_ecc = state_params['min_ecc']
-        max_ecc = state_params['max_ecc']
-
-        tracks_layer_data = input_params['tracks_layer_data']
-        scale = input_params['tracks_layer_scale']
-        tracks_layer_props = input_params['tracks_layer_props']
+        min_frames = state_params["min_frames"]
+        min_mass = state_params["min_mass"]
+        max_mass = state_params["max_mass"]
+        min_size = state_params["min_size"]
+        max_size = state_params["max_size"]
+        min_ecc = state_params["min_ecc"]
+        max_ecc = state_params["max_ecc"]
+
+        tracks_layer_data = input_params["tracks_layer_data"]
+        scale = input_params["tracks_layer_scale"]
+        tracks_layer_props = input_params["tracks_layer_props"]
 
         # Make trackpy table from layer data
         out_data = dict()
         t = self._make_trackpy_table("tracks", tracks_layer_data, tracks_layer_props)
         if t is not None:
             self.log.emit(f"Number of particles: {t['particle'].nunique()}")
 
             tp.quiet()
 
             # filter by min frames
             if min_frames is not None and min_frames > 1:
                 t = tp.filter_stubs(t, threshold=min_frames)
-                self.log.emit(f"After filter for Min frames, number of particles: {t['particle'].nunique()}")
+                self.log.emit(
+                    f"After filter for Min frames, number of particles: {t['particle'].nunique()}"
+                )
 
             # filter by mass, size, eccentricity
-            mean_t = t.groupby('particle').mean()
+            mean_t = t.groupby("particle").mean()
 
             if min_mass is not None and min_mass > 0:
-                mean_t = mean_t[mean_t['mass'] >= min_mass]
+                mean_t = mean_t[mean_t["mass"] >= min_mass]
             if max_mass is not None:
-                mean_t = mean_t[mean_t['mass'] <= max_mass]
+                mean_t = mean_t[mean_t["mass"] <= max_mass]
 
             if min_size is not None and min_size > 0:
-                mean_t = mean_t[mean_t['size'] >= min_size]
+                mean_t = mean_t[mean_t["size"] >= min_size]
             if max_size is not None:
-                mean_t = mean_t[mean_t['size'] <= max_size]
+                mean_t = mean_t[mean_t["size"] <= max_size]
 
             if min_ecc is not None and min_ecc > 0:
-                mean_t = mean_t[mean_t['ecc'] >= min_ecc]
+                mean_t = mean_t[mean_t["ecc"] >= min_ecc]
             if max_ecc is not None and max_ecc < 1:
-                mean_t = mean_t[mean_t['ecc'] <= max_ecc]
+                mean_t = mean_t[mean_t["ecc"] <= max_ecc]
 
-            t = t[t['particle'].isin(mean_t.index)]
-            self.log.emit(f"After filter for mass/size/eccentricity, number of particles: {t['particle'].nunique()}")
+            t = t[t["particle"].isin(mean_t.index)]
+            self.log.emit(
+                f"After filter for mass/size/eccentricity, number of particles: {t['particle'].nunique()}"
+            )
 
             # emit the output data after sorting by track_id (particle) and frame (needed for tracks layer)
-            t.index.name = 'index'  # pandas complains when index name and column name are the same
-            t = t.sort_values(by=['particle', 'frame'], axis=0, ascending=True)
+            t.index.name = (
+                "index"  # pandas complains when index name and column name are the same
+            )
+            t = t.sort_values(by=["particle", "frame"], axis=0, ascending=True)
 
             # change column name from 'particle' to 'track_id' to identify the track for consistency with napari layer
-            t.rename(columns={'particle': 'track_id'}, inplace=True)
+            t.rename(columns={"particle": "track_id"}, inplace=True)
 
-            out_data = {'df': t,
-                        'scale': scale}
+            out_data = {"df": t, "scale": scale}
         else:
-            self.log.emit(f"Error: The tracks layer properties do not contain the required columns for filtering.")
+            self.log.emit(
+                "Error: The tracks layer properties do not contain the required columns for filtering."
+            )
 
         self.update_data.emit(out_data)
         super().run()
 
 
 class GEMspaFilterLinksWidget(GEMspaWidget):
     """Widget for Filter links plugin"""
 
     name = "GEMspaFilterLinksWidget"
 
     def __init__(self, napari_viewer, title="Filter links with trackpy:"):
         super().__init__(napari_viewer, title)
 
-        self._input_values = {'Min frames': QLineEdit('3'),
-                              'Min mass': QLineEdit('0'),
-                              'Max mass': QLineEdit(''),
-                              'Min size': QLineEdit('0'),
-                              'Max size': QLineEdit(''),
-                              'Min eccentricity': QLineEdit('0'),
-                              'Max eccentricity': QLineEdit('1'),
-                              }
+        self._input_values = {
+            "Min frames": QLineEdit("3"),
+            "Min mass": QLineEdit("0"),
+            "Max mass": QLineEdit(""),
+            "Min size": QLineEdit("0"),
+            "Max size": QLineEdit(""),
+            "Min eccentricity": QLineEdit("0"),
+            "Max eccentricity": QLineEdit("1"),
+        }
 
         self._required_inputs = []
 
         self.init_ui()
 
     def start_task(self, layer_names, log_widget):
         # initialize worker and start task
         self.worker = GEMspaFilterLinksWorker()
         super().start_task(layer_names, log_widget)
 
     def state(self, layer_names) -> dict:
-
-        return {'name': self.name,
-                'inputs': {'tracks_layer_name': layer_names['tracks'],
-                           'tracks_layer_data': self.viewer.layers[layer_names['tracks']].data,
-                           'tracks_layer_scale': self.viewer.layers[layer_names['tracks']].scale,
-                           'tracks_layer_props': self.viewer.layers[layer_names['tracks']].properties
-                           },
-                'parameters': {'min_frames': convert_to_int(self._input_values['Min frames'].text()),
-                               'min_mass': convert_to_float(self._input_values['Min mass'].text()),
-                               'max_mass': convert_to_float(self._input_values['Max mass'].text()),
-                               'min_size': convert_to_float(self._input_values['Min size'].text()),
-                               'max_size': convert_to_float(self._input_values['Max size'].text()),
-                               'min_ecc': convert_to_float(self._input_values['Min eccentricity'].text()),
-                               'max_ecc': convert_to_float(self._input_values['Max eccentricity'].text()),
-                               },
-                }
+        return {
+            "name": self.name,
+            "inputs": {
+                "tracks_layer_name": layer_names["tracks"],
+                "tracks_layer_data": self.viewer.layers[layer_names["tracks"]].data,
+                "tracks_layer_scale": self.viewer.layers[layer_names["tracks"]].scale,
+                "tracks_layer_props": self.viewer.layers[
+                    layer_names["tracks"]
+                ].properties,
+            },
+            "parameters": {
+                "min_frames": convert_to_int(self._input_values["Min frames"].text()),
+                "min_mass": convert_to_float(self._input_values["Min mass"].text()),
+                "max_mass": convert_to_float(self._input_values["Max mass"].text()),
+                "min_size": convert_to_float(self._input_values["Min size"].text()),
+                "max_size": convert_to_float(self._input_values["Max size"].text()),
+                "min_ecc": convert_to_float(
+                    self._input_values["Min eccentricity"].text()
+                ),
+                "max_ecc": convert_to_float(
+                    self._input_values["Max eccentricity"].text()
+                ),
+            },
+        }
 
     def update_data(self, out_dict):
         """Set the worker outputs to napari layers"""
 
-        if 'df' in out_dict:
-            df = out_dict['df']
-            kwargs = {'scale': out_dict['scale'],
-                      'blending': 'translucent',
-                      'tail_length': df['frame'].max(),
-                      'name': 'Linked features (filtered)'}
+        if "df" in out_dict:
+            df = out_dict["df"]
+            kwargs = {
+                "scale": out_dict["scale"],
+                "blending": "translucent",
+                "tail_length": int(df["frame"].max()),
+                "name": "Linked features (filtered)",
+            }
             if len(df) == 0:
                 show_error("No particles were linked!")
             else:
                 layer = self._add_napari_layer("tracks", df, **kwargs)
 
                 plots_viewer = self._new_plots_viewer(layer.name)
                 properties_viewer = self._new_properties_viewer(layer.name)
 
                 plots_viewer.plot_link_results(df)
                 plots_viewer.show()
 
                 if self.display_table_view:
                     # Fixing column ordering for display on table view
-                    df.insert(0, 'frame', df.pop('frame'))
-                    df.insert(0, 'track_id', df.pop('track_id'))
+                    df.insert(0, "frame", df.pop("frame"))
+                    df.insert(0, "track_id", df.pop("track_id"))
                     properties_viewer.reload_from_pandas(df)
                     properties_viewer.show()
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_link_widget.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_link_widget.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,135 +1,161 @@
-from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+"""Defines: GEMspaLinkWidget, GEMspaLinkWorker"""
+
+import warnings
+
 import trackpy as tp
-from qtpy.QtWidgets import QLineEdit
 from qtpy.QtCore import Slot
-from ._utils import show_error, convert_to_int, convert_to_float
+from qtpy.QtWidgets import QLineEdit
 
-"""Defines: GEMspaLinkWidget, GEMspaLinkWorker"""
+from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+from ._utils import convert_to_float, convert_to_int, show_error
 
 
 class GEMspaLinkWorker(GEMspaWorker):
-    """Worker for the Link Features plugin
-
-    """
+    """Worker for the Link Features plugin"""
 
     def __init__(self):
         super().__init__()
 
     @Slot(dict)
     def run(self, state):
         """Execute the processing"""
 
-        input_params = state['inputs']
-        state_params = state['parameters']
+        input_params = state["inputs"]
+        state_params = state["parameters"]
 
-        search_range = state_params['search_range']
+        search_range = state_params["search_range"]
 
-        memory = state_params['memory']
+        memory = state_params["memory"]
         if memory is None:
             memory = 0
 
-        min_frames = state_params['min_frames']
+        min_frames = state_params["min_frames"]
 
-        points_layer_data = input_params['points_layer_data']
-        scale = input_params['points_layer_scale']
-        points_layer_props = input_params['points_layer_props']
+        points_layer_data = input_params["points_layer_data"]
+        scale = input_params["points_layer_scale"]
+        points_layer_props = input_params["points_layer_props"]
 
         out_data = dict()
         if len(points_layer_data.shape) > 1 and points_layer_data.shape[1] >= 3:
-
             # Make trackpy table from layer data
-            f = self._make_trackpy_table("points", points_layer_data, points_layer_props)
+            f = self._make_trackpy_table(
+                "points", points_layer_data, points_layer_props
+            )
             if f is not None:
-                tp.quiet()  # trackpy to quiet mode
+                # tp.quiet()  # trackpy to quiet mode
+
+                # When a Warning is raised by trackpy, napari freezes and below message is printed to the console.
+                # Ignoring trackpy warnings prevents this.
+                # The process has forked and you cannot use this CoreFoundation functionality safely. You MUST exec().
+                # Break on
+                # __THE_PROCESS_HAS_FORKED_AND_YOU_CANNOT_USE_THIS_COREFOUNDATION_FUNCTIONALITY___YOU_MUST_EXEC__()
+                # to debug.
+                warnings.filterwarnings("ignore", module="trackpy")
 
                 # perform linking
                 t = tp.link(f, search_range=search_range, memory=memory)
                 self.log.emit(f"Number of particles: {t['particle'].nunique()}")
 
                 # Filter spurious trajectories
                 if min_frames is not None and min_frames > 1:
                     t = tp.filter_stubs(t, threshold=min_frames)
-                    self.log.emit(f"After filter for Min frames, number of particles: {t['particle'].nunique()}")
+                    self.log.emit(
+                        f"After filter for Min frames, number of particles: {t['particle'].nunique()}"
+                    )
 
                 # emit the output data after sorting by track_id (particle) and frame (needed for tracks layer)
-                t.index.name = 'index'  # pandas complains when index name and column name are the same
-                t = t.sort_values(by=['particle', 'frame'], axis=0, ascending=True)
+                t.index.name = "index"  # pandas complains when index name and column name are the same
+                t = t.sort_values(by=["particle", "frame"], axis=0, ascending=True)
 
                 # change column name from 'particle' to 'track_id' to identify the track for consistency with napari
-                t.rename(columns={'particle': 'track_id'}, inplace=True)
+                t.rename(columns={"particle": "track_id"}, inplace=True)
+
+                warnings.resetwarnings()
 
-                out_data = {'df': t,
-                            'scale': scale}
+                out_data = {"df": t, "scale": scale}
             else:
-                self.log.emit(f"Error: The points layer properties do not contain the required columns for linking.")
+                self.log.emit(
+                    "Error: The points layer properties do not contain the required columns for linking."
+                )
         else:
-            self.log.emit(f"The data does not have a dimension for linking.")
+            self.log.emit("The data does not have a dimension for linking.")
 
         self.update_data.emit(out_data)
         super().run()
 
 
 class GEMspaLinkWidget(GEMspaWidget):
     """Widget for Link features plugin"""
 
     name = "GEMspaLinkWidget"
 
     def __init__(self, napari_viewer, title="Link features with trackpy:"):
         super().__init__(napari_viewer, title)
 
-        self._input_values = {'Link range': QLineEdit('5'),
-                              'Memory': QLineEdit('0'),
-                              'Min frames': QLineEdit('3')
-                              }
+        self._input_values = {
+            "Link range": QLineEdit("5"),
+            "Memory": QLineEdit("0"),
+            "Min frames": QLineEdit("3"),
+        }
 
         # Link range does not have a default value in trackpy and must be input by the user
-        self._required_inputs = ['Link range', ]
+        self._required_inputs = [
+            "Link range",
+        ]
 
         self.init_ui()
 
     def start_task(self, layer_names, log_widget):
         # initialize worker and start task
         self.worker = GEMspaLinkWorker()
         super().start_task(layer_names, log_widget)
 
     def state(self, layer_names) -> dict:
-
-        return {'name': self.name,
-                'inputs': {'points_layer_name': layer_names['points'],
-                           'points_layer_data': self.viewer.layers[layer_names['points']].data,
-                           'points_layer_scale': self.viewer.layers[layer_names['points']].scale,
-                           'points_layer_props': self.viewer.layers[layer_names['points']].properties
-                           },
-                'parameters': {'search_range': convert_to_float(self._input_values['Link range'].text()),
-                               'memory': convert_to_int(self._input_values['Memory'].text()),
-                               'min_frames': convert_to_int(self._input_values['Min frames'].text()),
-                               },
-                }
+        return {
+            "name": self.name,
+            "inputs": {
+                "points_layer_name": layer_names["points"],
+                "points_layer_data": self.viewer.layers[layer_names["points"]].data,
+                "points_layer_scale": self.viewer.layers[layer_names["points"]].scale,
+                "points_layer_props": self.viewer.layers[
+                    layer_names["points"]
+                ].properties,
+            },
+            "parameters": {
+                "search_range": convert_to_float(
+                    self._input_values["Link range"].text()
+                ),
+                "memory": convert_to_int(self._input_values["Memory"].text()),
+                "min_frames": convert_to_int(self._input_values["Min frames"].text()),
+            },
+        }
 
     def update_data(self, out_dict):
         """Set the worker outputs to napari layers"""
 
-        if 'df' in out_dict:
-            df = out_dict['df']
-            kwargs = {'scale': out_dict['scale'],
-                      'blending': 'translucent',
-                      'tail_length': df['frame'].max(),
-                      'name': 'Linked features'}
+        if "df" in out_dict:
+            df = out_dict["df"]
+            kwargs = {
+                "scale": out_dict["scale"],
+                "blending": "translucent",
+                "tail_length": int(df["frame"].max()),
+                "name": "Linked features",
+            }
 
             if len(df) == 0:
                 show_error("No particles were linked!")
             else:
                 layer = self._add_napari_layer("tracks", df, **kwargs)
 
                 plots_viewer = self._new_plots_viewer(layer.name)
                 properties_viewer = self._new_properties_viewer(layer.name)
 
                 plots_viewer.plot_link_results(df)
                 plots_viewer.show()
 
                 # Fixing column ordering for display on table view
                 if self.display_table_view:
-                    df.insert(0, 'frame', df.pop('frame'))
-                    df.insert(0, 'track_id', df.pop('track_id'))
+                    df.insert(0, "frame", df.pop("frame"))
+                    df.insert(0, "track_id", df.pop("track_id"))
                     properties_viewer.reload_from_pandas(df)
                     properties_viewer.show()
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_locate_widget.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_locate_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,140 @@
-from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+"""Defines: GEMspaLocateWidget, GEMspaLocateWorker"""
+
+import warnings
+
 import trackpy as tp
-from qtpy.QtWidgets import (QGridLayout, QLabel, QLineEdit, QCheckBox, QVBoxLayout)
 from qtpy.QtCore import Slot
-from ._utils import show_error, convert_to_float, convert_to_int, remove_outside_mask, fix_frame_limits
+from qtpy.QtWidgets import QCheckBox, QGridLayout, QLabel, QLineEdit, QVBoxLayout
 
-
-"""Defines: GEMspaLocateWidget, GEMspaLocateWorker"""
+from ._gemspa_widget import GEMspaWidget, GEMspaWorker
+from ._utils import (
+    convert_to_float,
+    convert_to_int,
+    fix_frame_limits,
+    remove_outside_mask,
+    show_error,
+)
 
 
 class GEMspaLocateWorker(GEMspaWorker):
-    """Worker for the Locate Features plugin
-
-    """
+    """Worker for the Locate Features plugin"""
 
     def __init__(self):
         super().__init__()
 
     @Slot(dict)
     def run(self, state):
         """Execute the processing"""
 
-        input_params = state['inputs']
-        state_params = state['parameters']
+        input_params = state["inputs"]
+        state_params = state["parameters"]
 
-        current_frame = state_params['current_frame']
-        del state_params['current_frame']
+        current_frame = state_params["current_frame"]
+        del state_params["current_frame"]
 
-        frame_start = state_params['frame_start']
-        del state_params['frame_start']
+        frame_start = state_params["frame_start"]
+        del state_params["frame_start"]
 
-        frame_end = state_params['frame_end']
-        del state_params['frame_end']
+        frame_end = state_params["frame_end"]
+        del state_params["frame_end"]
 
-        diameter = state_params['diameter']
-        del state_params['diameter']
+        diameter = state_params["diameter"]
+        del state_params["diameter"]
 
         keys = list(state_params.keys())
         for key in keys:
             if state_params[key] is None:
                 del state_params[key]
 
-        image = input_params['image_layer_data']
-        scale = input_params['image_layer_scale']
+        image = input_params["image_layer_data"]
+        scale = input_params["image_layer_scale"]
+
+        # tp.quiet()  # trackpy to quiet mode
+
+        # When a Warning is raised by trackpy, napari freezes and below message is printed to the console.
+        # Ignoring trackpy warnings prevents this.
+        # The process has forked and you cannot use this CoreFoundation functionality safely. You MUST exec().
+        # Break on
+        # __THE_PROCESS_HAS_FORKED_AND_YOU_CANNOT_USE_THIS_COREFOUNDATION_FUNCTIONALITY___YOU_MUST_EXEC__()
+        # to debug.
+        warnings.filterwarnings("ignore", module="trackpy")
 
-        tp.quiet()  # trackpy to quiet mode
         if current_frame:
             # Only process the current frame
-            t = input_params['frame']
+            t = input_params["frame"]
             f = tp.locate(image[t], diameter, **state_params)
+            if "frame" not in f.columns:
+                f["frame"] = t
             self.log.emit(f"Processed frame {t}, number of particles: {len(f)}")
         else:
             # process the entire movie - limited by frame start/end
             frame_offset = 0
             if len(image.shape) >= 3:
-                frame_start, frame_end = fix_frame_limits(frame_start, frame_end, len(image))
-                image = image[frame_start:frame_end+1]
+                frame_start, frame_end = fix_frame_limits(
+                    frame_start, frame_end, len(image)
+                )
+                image = image[frame_start : frame_end + 1]
                 frame_offset = frame_start
-
             f = tp.batch(image, diameter, **state_params)
-            f['frame'] = f['frame']+frame_offset
-            self.log.emit(f"Processed {len(image)} frames, number of particles: {len(f)}")
+            if "frame" in f.columns:
+                f["frame"] = f["frame"] + frame_offset
+            self.log.emit(
+                f"Processed {len(image)} frames, number of particles: {len(f)}"
+            )
 
-        if 'frame' not in f.columns:
-            f['frame'] = t
+        warnings.resetwarnings()
 
         # if labels layer was chosen, remove all points that are outside labeled regions
-        if 'labels_layer_data' in input_params:
-            labeled_mask = input_params['labels_layer_data']
+        if "labels_layer_data" in input_params:
+            labeled_mask = input_params["labels_layer_data"]
             f = remove_outside_mask(f, labeled_mask)
-            self.log.emit(f"Removed particles outside of mask region, number of particles: {len(f)}")
+            self.log.emit(
+                f"Removed particles outside of mask region, number of particles: {len(f)}"
+            )
 
-        out_data = {'df': f,
-                    'scale': scale,
-                    'diameter': diameter}
+        out_data = {"df": f, "scale": scale, "diameter": diameter}
 
         self.update_data.emit(out_data)
         super().run()
 
 
 class GEMspaLocateWidget(GEMspaWidget):
     """Widget for Locate Features plugin"""
 
-    name = 'GEMspaLocateWidget'
+    name = "GEMspaLocateWidget"
 
     def __init__(self, napari_viewer, title="Locate features with trackpy:"):
         super().__init__(napari_viewer, title)
 
-        self._current_frame_check = QCheckBox('Process only current frame')
-        self._invert_check = QCheckBox('Invert')
-        self._preprocess_check = QCheckBox('Preprocess')
-
-        self._input_values = {'Frame start': QLineEdit(''),
-                              'Frame end': QLineEdit(''),
-                              'Diameter': QLineEdit('11'),
-                              'Min mass': QLineEdit('125'),
-                              'Max size': QLineEdit(''),
-                              'Separation': QLineEdit(''),
-                              'Noise size': QLineEdit('1'),
-                              'Smoothing size': QLineEdit(''),
-                              'Threshold': QLineEdit(''),
-                              'Percentile': QLineEdit('64'),
-                              'Top n': QLineEdit('')
-                              }
+        self._current_frame_check = QCheckBox("Process only current frame")
+        self._invert_check = QCheckBox("Invert")
+        self._preprocess_check = QCheckBox("Preprocess")
+
+        self._input_values = {
+            "Frame start": QLineEdit(""),
+            "Frame end": QLineEdit(""),
+            "Diameter": QLineEdit("11"),
+            "Min mass": QLineEdit("125"),
+            "Max size": QLineEdit(""),
+            "Separation": QLineEdit(""),
+            "Noise size": QLineEdit("1"),
+            "Smoothing size": QLineEdit(""),
+            "Threshold": QLineEdit(""),
+            "Percentile": QLineEdit("64"),
+            "Top n": QLineEdit(""),
+        }
         # Diameter does not have a default value in trackpy and must be input by the user
-        self._required_inputs = ['Diameter', ]
+        self._required_inputs = [
+            "Diameter",
+        ]
 
         self.init_ui()
 
     def init_ui(self):
-
         layout = QVBoxLayout()
 
         grid_layout = QGridLayout()
         grid_layout.setContentsMargins(0, 0, 0, 0)
         i = 0
 
         if self.title is not None:
@@ -139,53 +161,61 @@
 
     def start_task(self, layer_names, log_widget):
         # initialize worker and start task
         self.worker = GEMspaLocateWorker()
         super().start_task(layer_names, log_widget)
 
     def state(self, layer_names) -> dict:
-
-        inputs_dict = {'image_layer_name': layer_names['image'],
-                       'image_layer_data': self.viewer.layers[layer_names['image']].data,
-                       'image_layer_scale': self.viewer.layers[layer_names['image']].scale,
-                       'frame': self.viewer.dims.current_step[0]
-                       }
-        if 'labels' in layer_names:
-            inputs_dict['labels_layer_name'] = layer_names['labels']
-            inputs_dict['labels_layer_data'] = self.viewer.layers[layer_names['labels']].data
-
-        return {'name': self.name,
-                'inputs': inputs_dict,
-                'parameters': {'frame_start': convert_to_int(self._input_values['Frame start'].text()),
-                               'frame_end': convert_to_int(self._input_values['Frame end'].text()),
-                               'diameter': convert_to_float(self._input_values['Diameter'].text()),
-                               'minmass': convert_to_float(self._input_values['Min mass'].text()),
-                               'maxsize': convert_to_float(self._input_values['Max size'].text()),
-                               'separation': convert_to_float(self._input_values['Separation'].text()),
-                               'noise_size': convert_to_float(self._input_values['Noise size'].text()),
-                               'smoothing_size': convert_to_float(self._input_values['Smoothing size'].text()),
-                               'threshold': convert_to_float(self._input_values['Threshold'].text()),
-                               'percentile': convert_to_float(self._input_values['Percentile'].text()),
-                               'topn': convert_to_float(self._input_values['Top n'].text()),
-                               'invert': self._invert_check.isChecked(),
-                               'preprocess': self._preprocess_check.isChecked(),
-                               'current_frame': self._current_frame_check.isChecked()
-                               },
-                }
+        inputs_dict = {
+            "image_layer_name": layer_names["image"],
+            "image_layer_data": self.viewer.layers[layer_names["image"]].data,
+            "image_layer_scale": self.viewer.layers[layer_names["image"]].scale,
+            "frame": self.viewer.dims.current_step[0],
+        }
+        if "labels" in layer_names:
+            inputs_dict["labels_layer_name"] = layer_names["labels"]
+            inputs_dict["labels_layer_data"] = self.viewer.layers[
+                layer_names["labels"]
+            ].data
+
+        return {
+            "name": self.name,
+            "inputs": inputs_dict,
+            "parameters": {
+                "frame_start": convert_to_int(self._input_values["Frame start"].text()),
+                "frame_end": convert_to_int(self._input_values["Frame end"].text()),
+                "diameter": convert_to_float(self._input_values["Diameter"].text()),
+                "minmass": convert_to_float(self._input_values["Min mass"].text()),
+                "maxsize": convert_to_float(self._input_values["Max size"].text()),
+                "separation": convert_to_float(self._input_values["Separation"].text()),
+                "noise_size": convert_to_float(self._input_values["Noise size"].text()),
+                "smoothing_size": convert_to_float(
+                    self._input_values["Smoothing size"].text()
+                ),
+                "threshold": convert_to_float(self._input_values["Threshold"].text()),
+                "percentile": convert_to_float(self._input_values["Percentile"].text()),
+                "topn": convert_to_float(self._input_values["Top n"].text()),
+                "invert": self._invert_check.isChecked(),
+                "preprocess": self._preprocess_check.isChecked(),
+                "current_frame": self._current_frame_check.isChecked(),
+            },
+        }
 
     def update_data(self, out_dict):
         """Set the worker outputs to napari layer"""
 
-        if 'df' in out_dict:
-            kwargs = {'scale': out_dict['scale'],
-                      'size': out_dict['diameter'],
-                      'name': 'Feature Locations',
-                      'face_color': 'transparent',
-                      'edge_color': 'red'}
-            df = out_dict['df']
+        if "df" in out_dict:
+            kwargs = {
+                "scale": out_dict["scale"],
+                "size": out_dict["diameter"],
+                "name": "Feature Locations",
+                "face_color": "transparent",
+                "edge_color": "red",
+            }
+            df = out_dict["df"]
 
             if len(df) == 0:
                 show_error("No particles were located!")
             else:
                 layer = self._add_napari_layer("points", df, **kwargs)
 
                 plots_viewer = self._new_plots_viewer(layer.name)
@@ -193,10 +223,10 @@
 
                 # viewer for the graphical output
                 plots_viewer.plot_locate_results(df)
                 plots_viewer.show()
 
                 if self.display_table_view:
                     # viewer for feature properties
-                    df.insert(0, 'frame', df.pop('frame'))
+                    df.insert(0, "frame", df.pop("frame"))
                     properties_viewer.reload_from_pandas(df)
                     properties_viewer.show()
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_plugin.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         if self.allow_none:
             self._input_layer_box.addItem("")
 
         for layer in self.viewer.layers:
             if self._is_layer_type_instance(layer):
                 self._input_layer_box.addItem(layer.name)
 
-
     def _is_layer_type_instance(self, layer):
         if ((self.layer_type == 'image' and isinstance(layer, napari.layers.image.image.Image)) or
                 (self.layer_type == 'points' and isinstance(layer, napari.layers.points.points.Points)) or
                 (self.layer_type == 'tracks' and isinstance(layer, napari.layers.tracks.tracks.Tracks)) or
                 (self.layer_type == 'labels' and isinstance(layer, napari.layers.labels.labels.Labels))):
             return True
         return False
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_gemspa_widget.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_widget.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from qtpy.QtWidgets import (QWidget, QVBoxLayout, QTextEdit, QGridLayout, QLabel)
-from qtpy.QtCore import Signal, QObject, QThread
-from ._gemspa_data_views import GEMspaTableWindow, GEMspaPlottingWindow
+"""Defines: GEMspaWidget, GEMspaWorker, GEMspaLogWidget"""
+
+import numpy as np
 import pandas as pd
-from ._utils import show_error
+from qtpy.QtCore import QObject, QThread, Signal
+from qtpy.QtWidgets import QGridLayout, QLabel, QTextEdit, QVBoxLayout, QWidget
 
-"""Defines: GEMspaWidget, GEMspaWorker, GEMspaLogWidget"""
+from ._gemspa_data_views import GEMspaPlottingWindow, GEMspaTableWindow
+from ._utils import show_error
 
 
 class GEMspaWorker(QObject):
     """Definition of a GEMspaWorker
 
     Receives and Sends input/output as a dictionary
 
@@ -20,64 +22,62 @@
     log = Signal(str)
 
     def __init__(self):
         super().__init__()
 
     @staticmethod
     def _make_trackpy_table(layer_type, data, props):
-        req_cols = ['mass', 'size', 'ecc', 'signal', 'raw_mass', 'ep']
+        req_cols = ["mass", "size", "ecc", "signal", "raw_mass", "ep"]
         for col in req_cols:
             if col not in props.keys():
                 return None
-        if layer_type == 'points':
+        if layer_type == "points":
             df = pd.DataFrame()
             if data.shape[1] == 2:
                 i = 0
             elif data.shape[1] == 3:
-                df['frame'] = data[:, 0]
+                df["frame"] = data[:, 0]
                 i = 1
             else:  # data.shape[1] >= 4
-                df['frame'] = data[:, 0]
-                df['z'] = data[:, 1]
+                df["frame"] = data[:, 0]
+                df["z"] = data[:, 1]
                 i = 2
-            df['y'] = data[:, i]
-            df['x'] = data[:, i + 1]
+            df["y"] = data[:, i]
+            df["x"] = data[:, i + 1]
             for col in props.keys():
                 df[col] = props[col]
-        elif layer_type == 'tracks':
+        elif layer_type == "tracks":
             df = pd.DataFrame()
-            df['particle'] = data[:, 0]
-            df['frame'] = data[:, 1]
+            df["particle"] = data[:, 0]
+            df["frame"] = data[:, 1]
             if data.shape[1] == 4:
                 i = 2
             else:  # data.shape[1] >= 5
-                df['z'] = data[:, 2]
+                df["z"] = data[:, 2]
                 i = 3
-            df['y'] = data[:, i]
-            df['x'] = data[:, i+1]
+            df["y"] = data[:, i]
+            df["x"] = data[:, i + 1]
             for col in props.keys():
-                if col != 'track_id':
+                if col != "track_id":
                     df[col] = props[col]
         else:
             raise ValueError(f"Invalid layer type: {layer_type}")
 
         return df
 
     def run(self):
         """Exec the data processing"""
 
         self.finished.emit()
 
 
 class GEMspaWidget(QWidget):
-    """Definition of a GEMspa napari widget
-
-    """
+    """Definition of a GEMspa napari widget"""
 
-    name = 'GEMspaWidget'
+    name = "GEMspaWidget"
 
     def __init__(self, napari_viewer, title=None):
         super().__init__()
 
         self.viewer = napari_viewer
         self.title = title
         self.thread = None
@@ -91,15 +91,14 @@
 
         self.display_table_view = False
 
         self._input_values = {}
         self._required_inputs = []
 
     def init_ui(self):
-
         layout = QVBoxLayout()
 
         # Set up the input GUI items
         grid_layout = QGridLayout()
         grid_layout.setContentsMargins(0, 0, 0, 0)
         i = 0
 
@@ -129,47 +128,46 @@
             viewer.deleteLater()
 
         while self.properties_viewers:
             viewer = self.properties_viewers.pop()
             viewer.close()
             viewer.deleteLater()
 
-    def _new_plots_viewer(self, title='Plot view', figsize=(8, 3), close_last=True):
+    def _new_plots_viewer(self, title="Plot view", figsize=(8, 3), close_last=True):
         if close_last and len(self.plots_viewers) >= 1:
             viewer = self.plots_viewers.pop()
             viewer.close()
             viewer.deleteLater()
 
         i = len(self.plots_viewers)
         self.plots_viewers.append(GEMspaPlottingWindow(self.viewer, figsize=figsize))
         self.plots_viewers[i].setWindowTitle(title)
         return self.plots_viewers[i]
 
-    def _new_properties_viewer(self, title='Table view', close_last=True):
+    def _new_properties_viewer(self, title="Table view", close_last=True):
         if close_last and len(self.properties_viewers) >= 1:
             viewer = self.properties_viewers.pop()
             viewer.close()
             viewer.deleteLater()
 
         i = len(self.properties_viewers)
         self.properties_viewers.append(GEMspaTableWindow(self.viewer))
         self.properties_viewers[i].setWindowTitle(title)
         return self.properties_viewers[i]
 
     def start_task(self, layer_names, log_widget):
-
         # Perform startup tasks and start thread: worker must be initialized before this function is called
 
-        # connect worker log signal to the GEMspaLogWidget all_log method
-        self.worker.log.connect(log_widget.add_log)
-
         # Thread for this worker
         self.thread = QThread()
         self.worker.moveToThread(self.thread)
 
+        # connect worker log signal to the GEMspaLogWidget all_log method
+        self.worker.log.connect(log_widget.add_log)
+
         # when thread is started, worker is run with the current state of the widget as input
         self.thread.started.connect(lambda: self.worker.run(self.state(layer_names)))
 
         # when the worker sends update_data signal, update_data of the widget will execute to update the GUI
         self.worker.update_data.connect(self.update_data)
 
         # Cleanup (as chatGPT suggested)
@@ -190,40 +188,43 @@
                     _ = float(text)
                 except ValueError:
                     show_error(f"{key} input must be a number")
                     valid = False
         return valid
 
     def _add_napari_layer(self, layer_type, df, **kwargs):
-
         if layer_type == "points":
-            if 'z' in df.columns:
-                data_cols = ['frame', 'z', 'y', 'x']
+            if "z" in df.columns:
+                data_cols = ["frame", "z", "y", "x"]
             else:
-                data_cols = ['frame', 'y', 'x']
+                data_cols = ["frame", "y", "x"]
         elif layer_type == "tracks":
-            if 'z' in df.columns:
-                data_cols = ['track_id', 'frame', 'z', 'y', 'x']
+            if "z" in df.columns:
+                data_cols = ["track_id", "frame", "z", "y", "x"]
             else:
-                data_cols = ['track_id', 'frame', 'y', 'x']
+                data_cols = ["track_id", "frame", "y", "x"]
         else:
-            raise ValueError(f"Unrecognized layer type: {layer_type}.  Expected points or tracks.")
+            raise ValueError(
+                f"Unrecognized layer type: {layer_type}.  Expected points or tracks."
+            )
 
         data = df[data_cols].to_numpy()
         props = {}
         for col in df.columns:
             if col not in data_cols:
-                props[col] = df[col].to_numpy()
+                # nan_to_num because napari properties does not handle nan data
+                props[col] = np.nan_to_num(df[col].to_numpy())
 
         add_layer = getattr(self.viewer, f"add_{layer_type}")
         return add_layer(data, properties=props, **kwargs)
 
 
 class GEMspaLogWidget(QWidget):
     """Widget to log the GEMspa plugin messages in the graphical interface"""
+
     def __init__(self):
         super().__init__()
 
         layout = QVBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         self.log_area = QTextEdit()
         layout.addWidget(self.log_area)
@@ -232,10 +233,7 @@
     def add_log(self, value: str):
         """Callback to add a new message in the log area"""
         self.log_area.append(value)
 
     def clear_log(self):
         """Callback to clear all the log area"""
         self.log_area.clear()
-
-
-
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_reader.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_utils.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/_writer.py` & `napari-gemspa-0.0.2/src/napari_gemspa/_writer.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 It implements the Writer specification.
 see: https://napari.org/stable/plugins/guides.html?#writers
 
 Replace code below according to your needs.
 """
 from __future__ import annotations
 
+import os
 from typing import TYPE_CHECKING, Any, List, Sequence, Tuple, Union
 
+import numpy as np
 import pandas as pd
-import os
 
 if TYPE_CHECKING:
     DataType = Union[Any, Sequence[Any]]
     FullLayerData = Tuple[DataType, dict, str]
 
 
 def _save_data(df, path):
     ext = os.path.splitext(path)[1]
-    if ext == '.csv':
-        sep = ','
-    elif ext == '.txt' or ext == '.tsv':
-        sep = '\t'
+    if ext == ".csv":
+        sep = ","
+    elif ext == ".txt" or ext == ".tsv":
+        sep = "\t"
     else:
         raise ValueError(f"{path}: file extension is invalid")
 
     df.to_csv(path, sep=sep, index=False)
 
 
 def write_points(path: str, data: Any, meta: dict) -> List[str]:
@@ -40,27 +41,27 @@
     # if dimension is 4: [t, z, y, x]
 
     if data.shape[1] < 2:
         raise ValueError("Points layer data cannot be saved with GEMspa.")
 
     df = pd.DataFrame()
     if data.shape[1] == 2:
-        #df['frame'] = np.zeros(data.shape[0], dtype=int)
+        # df['frame'] = np.zeros(data.shape[0], dtype=int)
         i = 0
     elif data.shape[1] == 3:
-        df['frame'] = data[:, 0]
+        df["frame"] = data[:, 0]
         i = 1
     else:  # data.shape[1] >= 4
-        df['frame'] = data[:, 0]
-        df['z'] = data[:, 1]
+        df["frame"] = data[:, 0]
+        df["z"] = data[:, 1]
         i = 2
-    df['y'] = data[:, i]
-    df['x'] = data[:, i+1]
-    for col in meta['properties'].keys():
-        df[col] = meta['properties'][col]
+    df["y"] = data[:, i]
+    df["x"] = data[:, i + 1]
+    for col in meta["properties"].keys():
+        df[col] = meta["properties"][col]
 
     _save_data(df, path)
 
     # return path to any file(s) that were successfully written
     return [path]
 
 
@@ -71,26 +72,40 @@
     # we assume a specific order to axes that is expected in GEMspa tracks data:
     # if dimension is 4: [track_id, t, z, y, x]
     # if dimension is 3: [track_id, t, y, x]
     if data.shape[1] < 4:
         raise ValueError("Tracks layer data cannot be saved with GEMspa.")
 
     df = pd.DataFrame()
-    df['track_id'] = data[:, 0]
-    df['frame'] = data[:, 1]
+    df["track_id"] = data[:, 0]
+    df["frame"] = data[:, 1]
     if data.shape[1] == 4:
         i = 2
     else:  # data.shape[1] >= 5
-        df['z'] = data[:, 2]
+        df["z"] = data[:, 2]
         i = 3
 
-    df['y'] = data[:, i]
-    df['x'] = data[:, i+1]
-    for col in meta['properties'].keys():
-        df[col] = meta['properties'][col]
+    df["y"] = data[:, i]
+    df["x"] = data[:, i + 1]
+    for col in meta["properties"].keys():
+        df[col] = meta["properties"][col]
+
+    # If columns for msd/step-size/radius_gyration, set first frame to empty instead of 0
+    # If columns for MSD_fitted and fitting data, set fitting data to empty where MSD_fitted==0
+
+    for col in ["msd", "step_size", "radius_gyration"]:
+        if col in df.columns:
+            df[col].where(df["frame"] > df["frame_start"], other=np.nan, inplace=True)
+
+    fitting_columns = ["D", "E", "r_sq (lin)", "K", "a", "r_sq (log)"]
+
+    if set(fitting_columns).issubset(set(df.columns)) and "MSD_fitted" in df.columns:
+        df[fitting_columns] = df[fitting_columns].where(
+            df["MSD_fitted"] == 1, other=np.nan
+        )
 
     _save_data(df, path)
 
     # return path to any file(s) that were successfully written
     return [path]
```

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa/napari.yaml` & `napari-gemspa-0.0.2/src/napari_gemspa/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.1/src/napari_gemspa.egg-info/SOURCES.txt` & `napari-gemspa-0.0.2/src/napari_gemspa.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+src/_tests/__init__.py
+src/_tests/run_napari.py
+src/_tests/test_gemspa_locate_worker.py
 src/napari_gemspa/__init__.py
 src/napari_gemspa/_gemspa_analyze_widget.py
 src/napari_gemspa/_gemspa_data_views.py
 src/napari_gemspa/_gemspa_file_import_widget.py
 src/napari_gemspa/_gemspa_filter_links_widget.py
 src/napari_gemspa/_gemspa_link_widget.py
 src/napari_gemspa/_gemspa_locate_widget.py
 src/napari_gemspa/_gemspa_plugin.py
 src/napari_gemspa/_gemspa_widget.py
 src/napari_gemspa/_reader.py
-src/napari_gemspa/_sample_data.py
 src/napari_gemspa/_utils.py
 src/napari_gemspa/_writer.py
 src/napari_gemspa/napari.yaml
 src/napari_gemspa.egg-info/PKG-INFO
 src/napari_gemspa.egg-info/SOURCES.txt
 src/napari_gemspa.egg-info/dependency_links.txt
 src/napari_gemspa.egg-info/entry_points.txt
```

