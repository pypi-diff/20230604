# Comparing `tmp/extremitypathfinder-2.5.0.tar.gz` & `tmp/extremitypathfinder-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extremitypathfinder-2.5.0.tar", max compression
+gzip compressed data, was "extremitypathfinder-2.6.0.tar", max compression
```

## Comparing `extremitypathfinder-2.5.0.tar` & `extremitypathfinder-2.6.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      200 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/.editorconfig
--rw-r--r--   0        0        0     2043 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     4071 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3091 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1056 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/LICENSE
--rw-r--r--   0        0        0      759 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/Makefile
--rw-r--r--   0        0        0     2447 2023-05-05 11:43:19.731766 extremitypathfinder-2.5.0/README.rst
--rw-r--r--   0        0        0      574 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/example.json
--rw-r--r--   0        0        0      132 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/__init__.py
--rw-r--r--   0        0        0     2234 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/command_line.py
--rw-r--r--   0        0        0      151 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/configs.py
--rw-r--r--   0        0        0    14688 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/extremitypathfinder.py
--rw-r--r--   0        0        0     6866 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/plotting.py
--rw-r--r--   0        0        0      379 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/types.py
--rw-r--r--   0        0        0    41506 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/extremitypathfinder/utils.py
--rw-r--r--   0        0        0     1906 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/__init__.py
--rw-r--r--   0        0        0      580 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/cli_test.py
--rwxr-xr-x   0        0        0     6871 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/helper_fcts_test.py
--rwxr-xr-x   0        0        0      838 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/helpers.py
--rwxr-xr-x   0        0        0     7352 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/main_test.py
--rw-r--r--   0        0        0    10758 2023-05-05 11:43:19.739766 extremitypathfinder-2.5.0/tests/test_cases.py
--rwxr-xr-x   0        0        0      318 2023-05-05 11:43:19.743766 extremitypathfinder-2.5.0/tox.ini
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 extremitypathfinder-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/.editorconfig
+-rw-r--r--   0        0        0     2043 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     4627 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     3091 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1056 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/LICENSE
+-rw-r--r--   0        0        0      759 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/Makefile
+-rw-r--r--   0        0        0     2447 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/README.rst
+-rw-r--r--   0        0        0      574 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/example.json
+-rw-r--r--   0        0        0      132 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/command_line.py
+-rw-r--r--   0        0        0      151 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/configs.py
+-rw-r--r--   0        0        0    14688 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/extremitypathfinder.py
+-rw-r--r--   0        0        0     6902 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/plotting.py
+-rw-r--r--   0        0        0      379 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/types.py
+-rw-r--r--   0        0        0    51145 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/utils.py
+-rw-r--r--   0        0        0     1906 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/cli_test.py
+-rwxr-xr-x   0        0        0     6914 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/helper_fcts_test.py
+-rwxr-xr-x   0        0        0      839 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/helpers.py
+-rwxr-xr-x   0        0        0     7351 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/main_test.py
+-rw-r--r--   0        0        0    10817 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/test_cases.py
+-rw-r--r--   0        0        0    12701 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/test_find_visible.py
+-rwxr-xr-x   0        0        0      318 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tox.ini
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 extremitypathfinder-2.6.0/PKG-INFO
```

### Comparing `extremitypathfinder-2.5.0/.pre-commit-config.yaml` & `extremitypathfinder-2.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/CHANGELOG.rst` & `extremitypathfinder-2.6.0/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+2.6.0 (2023-06-04)
+-------------------
+
+internal:
+
+* implemented an optimised visibility graph algorithm: sort edges and candidates after their representation to always only check the relevant fraction of candidates for each edge. Runtime complexity O(n^2 log_2 n).
+* added visibility computation tests
+* automatically skip GitHub actions publishing when the version already exists. useful for minor improvements without publishing a version. build would always fail otherwise
+* updated pinned dependencies to fix security alerts
+* minor code refactoring
+
 
 2.5.0 (2023-05-05)
 -------------------
 
 * removed need for separate ``.prepare()`` call. Storing environment boundary data automatically triggers the preparation of the visibility graph. This is a non-breaking change. The ``.prepare()`` method is still available, but it is not needed anymore.
 
 internal:
```

### Comparing `extremitypathfinder-2.5.0/CONTRIBUTING.rst` & `extremitypathfinder-2.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/LICENSE` & `extremitypathfinder-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/Makefile` & `extremitypathfinder-2.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/README.rst` & `extremitypathfinder-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/example.json` & `extremitypathfinder-2.6.0/example.json`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/extremitypathfinder/command_line.py` & `extremitypathfinder-2.6.0/extremitypathfinder/command_line.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/extremitypathfinder/extremitypathfinder.py` & `extremitypathfinder-2.6.0/extremitypathfinder/extremitypathfinder.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -192,17 +192,17 @@
         return utils.find_visible(
             origin,
             candidates,
             edge_idxs2check,
             coords,
             vert_idx2repr,
             vert_idx2dist,
-            self.extremity_mask,
             self.edge_vertex_idxs,
             self.vertex_edge_idxs,
+            self.extremity_mask,
         )
 
     def find_shortest_path(
         self,
         start_coordinates: InputCoord,
         goal_coordinates: InputCoord,
         free_space_after: bool = True,
```

### Comparing `extremitypathfinder-2.5.0/extremitypathfinder/plotting.py` & `extremitypathfinder-2.6.0/extremitypathfinder/plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,19 @@
     "edgecolor": "black",
     "fill": False,
     "linewidth": 1.0,
 }
 
 SHOW_PLOTS = False
 PLOTTING_DIR = "all_plots"
+PLOT_FILE_ENDING = ".svg"
 
 
 def get_plot_name(file_name="plot"):
-    return abspath(join(PLOTTING_DIR, file_name + "_" + str(time.time())[:-7] + ".png"))
+    return abspath(join(PLOTTING_DIR, file_name + "_" + str(time.time())[:-7] + PLOT_FILE_ENDING))
 
 
 def export_plot(fig, file_name):
     fig.set_size_inches(EXPORT_SIZE_X, EXPORT_SIZE_Y, forward=True)
     plt.savefig(get_plot_name(file_name), dpi=EXPORT_RESOLUTION)
     plt.close()
```

### Comparing `extremitypathfinder-2.5.0/pyproject.toml` & `extremitypathfinder-2.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extremitypathfinder"
-version = "2.5.0"
+version = "2.6.0"
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/jannikmi/extremitypathfinder"
 homepage = "https://extremitypathfinder.readthedocs.io/en/latest/"
 documentation = "https://extremitypathfinder.readthedocs.io/en/latest/"
 keywords = ["path-planning", "path-finding", "shortest-path", "visibility", "graph", "polygon", "grid", "map", "robotics", "navigation", "offline"]
 classifiers = [
```

### Comparing `extremitypathfinder-2.5.0/tests/cli_test.py` & `extremitypathfinder-2.6.0/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.5.0/tests/helper_fcts_test.py` & `extremitypathfinder-2.6.0/tests/helper_fcts_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 from typing import Dict, Set
 
 import numpy as np
 import pytest
 
 from extremitypathfinder import PolygonEnvironment
 from extremitypathfinder.utils import (
-    clean_visibles,
-    compute_extremity_idxs,
-    compute_repr_n_dist,
-    has_clockwise_numbering,
-    inside_polygon,
+    _compute_extremity_idxs,
+    _compute_repr_n_dist,
+    _has_clockwise_numbering,
+    _inside_polygon,
     read_json,
 )
 from tests.helpers import proto_test_case
+from tests.test_find_visible import _clean_visibles
 
 
 def test_inside_polygon():
     for border_value in [True, False]:
 
         def test_fct(input):
             polygon_test_case = np.array([(-1.0, -1.0), (1.0, -1.0), (1.0, 1.0), (-1.0, 1.0)])
             p = np.array(input, dtype=float)
-            return inside_polygon(p, polygon_test_case, border_value)
+            return _inside_polygon(p, polygon_test_case, border_value)
 
         p_test_cases = [
             # (x,y),
             # inside
             (0.0, 0.0),
             # # outside
             (-2.0, 2.0),
@@ -104,15 +104,15 @@
         ({0, 1}, {0: 0.0, 1: 0.0}, {0: 1.0, 1: 0.0}, {1}),
         ({0, 1}, {0: 0.0, 1: 0.0}, {0: 1.1, 1: 0.0}, {1}),
     ],
 )
 def test_clean_visible_idxs(
     visible_idxs: Set[int], cand_idx2repr: Dict[int, float], vert_idx2dist: Dict[int, float], expected: Set[int]
 ):
-    res = clean_visibles(visible_idxs, cand_idx2repr, vert_idx2dist)
+    res = _clean_visibles(visible_idxs, cand_idx2repr, vert_idx2dist)
     assert res == expected
 
 
 @pytest.mark.parametrize(
     "coords, expected",
     [
         (
@@ -146,15 +146,15 @@
             ],
             {6, 1},
         ),
     ],
 )
 def test_compute_extremity_idxs(coords, expected):
     coords = np.array(coords)
-    res = compute_extremity_idxs(coords)
+    res = _compute_extremity_idxs(coords)
     assert set(res) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
     [
         # clockwise numbering!
@@ -166,15 +166,15 @@
         ([(0.0, 0.0), (10.0, 0.0), (10.0, 10.0), (0.0, 10.0)], False),
         ([(0.0, 0.0), (10.0, 0.0), (10.0, 5.0), (10.0, 10.0), (0.0, 10.0)], False),
         ([(0.0, 0.0), (10.0, 0.0), (9.0, 5.0), (10.0, 10.0), (0.0, 10.0)], False),
     ],
 )
 def test_clockwise_numering(input, expected):
     def clockwise_test_fct(input):
-        return has_clockwise_numbering(np.array(input))
+        return _has_clockwise_numbering(np.array(input))
 
     assert clockwise_test_fct(input) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
     [
@@ -185,15 +185,15 @@
         ([0.0, 1.0], (1.0, 1.0)),
         ([-6.0, -5.0], (2.64018439966448, 7.810249675906654)),
         ([-5.0, -6.0], (2.768221279597376, 7.810249675906654)),
     ],
 )
 def test_compute_repr_n_dist(input, expected):
     def test_fct(input):
-        return compute_repr_n_dist(np.array(input))
+        return _compute_repr_n_dist(np.array(input))
 
     assert test_fct(input) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
     [
@@ -205,15 +205,15 @@
         ([0.0, 2.0], 1.0),
         ([-2.0, 0.0], 2.0),
         ([0.0, -2.0], 3.0),
     ],
 )
 def test_angle_representation(input, expected):
     def func(input):
-        repr, dist = compute_repr_n_dist(np.array(input))
+        repr, dist = _compute_repr_n_dist(np.array(input))
         return repr
 
     assert func(input) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
@@ -238,13 +238,13 @@
         ([-0.00001, 1.0], 1.0),
         ([-1.0, -0.00001], 2.0),
         ([-0.00001, -1.0], 2.0),
     ],
 )
 def test_angle_repr_quadrant(input, expected):
     def func(input):
-        repr, dist = compute_repr_n_dist(np.array(input))
+        repr, dist = _compute_repr_n_dist(np.array(input))
         return repr
 
     res = func(input)
     assert res >= expected
     assert res < expected + 1
```

### Comparing `extremitypathfinder-2.5.0/tests/helpers.py` & `extremitypathfinder-2.6.0/tests/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     p2 = coords[n2]
     for i1, i2 in edge_vertex_idxs:
         if i1 == n1 or i2 == n2:
             # no not check the same edge
             continue
         q1 = coords[i1]
         q2 = coords[i2]
-        if utils.get_intersection_status(p1, p2, q1, q2) == 1:
+        if utils._get_intersection_status(p1, p2, q1, q2) == 1:
             return True
     return False
```

### Comparing `extremitypathfinder-2.5.0/tests/main_test.py` & `extremitypathfinder-2.6.0/tests/main_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
         path, length = expected_output
         expected_output_reversed = list(reversed(path)), length
         validate(goal_coordinates, start_coordinates, expected_output_reversed)
 
 
 def test_grid_env():
     grid_env = ENVIRONMENT_CLASS(**CONSTRUCTION_KWARGS)
-
     grid_env.store_grid_world(*GRID_ENV_PARAMS, simplify=False, validate=False)
     nr_extremities = len(grid_env.all_extremities)
     assert nr_extremities == 17, "extremities do not get detected correctly!"
     nr_graph_nodes = len(grid_env.graph.nodes)
     assert nr_graph_nodes == 16, "identical nodes should get joined in the graph!"
 
     # test if points outside the map are being rejected
```

### Comparing `extremitypathfinder-2.5.0/tests/test_cases.py` & `extremitypathfinder-2.6.0/tests/test_cases.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # size_x, size_y, obstacle_iter
 from math import sqrt
 
+import numpy as np
+
+from extremitypathfinder import utils
+
 GRID_ENV_PARAMS = (
     19,
     10,
     [
         # (x,y),
         # obstacles changing boundary
         (0, 1),
```

### Comparing `extremitypathfinder-2.5.0/PKG-INFO` & `extremitypathfinder-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extremitypathfinder
-Version: 2.5.0
+Version: 2.6.0
 Summary: python package for fast shortest path computation on 2D polygon or grid maps
 Home-page: https://extremitypathfinder.readthedocs.io/en/latest/
 License: MIT
 Keywords: path-planning,path-finding,shortest-path,visibility,graph,polygon,grid,map,robotics,navigation,offline
 Author: jannikmi
 Author-email: github@michelfe.it
 Requires-Python: >=3.8,<4.0
```

