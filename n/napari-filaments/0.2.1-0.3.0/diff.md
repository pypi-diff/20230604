# Comparing `tmp/napari_filaments-0.2.1.tar.gz` & `tmp/napari_filaments-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_filaments-0.2.1.tar", last modified: Sat Jul 16 06:21:47 2022, max compression
+gzip compressed data, was "napari_filaments-0.3.0.tar", last modified: Sun Jun  4 13:10:34 2023, max compression
```

## Comparing `napari_filaments-0.2.1.tar` & `napari_filaments-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:47.009842 napari_filaments-0.2.1/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.924156 napari_filaments-0.2.1/.tox/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.926531 napari_filaments-0.2.1/.tox/.package/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.925189 napari_filaments-0.2.1/.tox/.package/Lib/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.926531 napari_filaments-0.2.1/.tox/.package/Lib/idlelib/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.946399 napari_filaments-0.2.1/.tox/.package/Lib/idlelib/Icons/
--rw-rw-rw-   0        0        0     1031 2022-03-23 21:12:08.000000 napari_filaments-0.2.1/.tox/.package/Lib/idlelib/Icons/idle_16.png
--rw-rw-rw-   0        0        0    39205 2022-03-23 21:12:08.000000 napari_filaments-0.2.1/.tox/.package/Lib/idlelib/Icons/idle_256.png
--rw-rw-rw-   0        0        0     2036 2022-03-23 21:12:08.000000 napari_filaments-0.2.1/.tox/.package/Lib/idlelib/Icons/idle_32.png
--rw-rw-rw-   0        0        0     3977 2022-03-23 21:12:08.000000 napari_filaments-0.2.1/.tox/.package/Lib/idlelib/Icons/idle_48.png
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.927527 napari_filaments-0.2.1/.tox/.package/tcl/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.927992 napari_filaments-0.2.1/.tox/.package/tcl/tk8.6/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.928556 napari_filaments-0.2.1/.tox/.package/tcl/tk8.6/demos/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.948389 napari_filaments-0.2.1/.tox/.package/tcl/tk8.6/demos/images/
--rw-rw-rw-   0        0        0     8157 2021-11-08 21:12:37.000000 napari_filaments-0.2.1/.tox/.package/tcl/tk8.6/demos/images/earthmenu.png
--rw-rw-rw-   0        0        0    54257 2021-11-08 21:12:37.000000 napari_filaments-0.2.1/.tox/.package/tcl/tk8.6/demos/images/ouster.png
--rw-rw-rw-   0        0        0     1513 2022-06-20 11:37:18.000000 napari_filaments-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      126 2022-07-01 07:58:33.000000 napari_filaments-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4814 2022-07-16 06:21:47.009842 napari_filaments-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3512 2022-07-16 05:58:44.000000 napari_filaments-0.2.1/README.md
--rw-rw-rw-   0        0        0      192 2022-06-20 11:37:18.000000 napari_filaments-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1659 2022-07-16 06:21:47.012836 napari_filaments-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0       40 2022-07-01 07:26:07.000000 napari_filaments-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.930710 napari_filaments-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.962700 napari_filaments-0.2.1/src/napari_filaments/
--rw-rw-rw-   0        0        0      169 2022-07-03 07:22:39.000000 napari_filaments-0.2.1/src/napari_filaments/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:47.001887 napari_filaments-0.2.1/src/napari_filaments/_icon/
--rw-rw-rw-   0        0        0        0 2022-07-01 07:39:21.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/__init__.py
--rw-rw-rw-   0        0        0     5981 2022-06-21 08:30:26.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/clip_l.png
--rw-rw-rw-   0        0        0     6000 2022-06-21 08:30:37.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/clip_r.png
--rw-rw-rw-   0        0        0     2336 2022-06-21 12:20:44.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/del.png
--rw-rw-rw-   0        0        0     8068 2022-06-21 09:07:18.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/erf2.png
--rw-rw-rw-   0        0        0     7526 2022-06-21 08:21:08.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/erf_l.png
--rw-rw-rw-   0        0        0     7095 2022-06-21 08:21:37.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/erf_r.png
--rw-rw-rw-   0        0        0     9881 2022-06-21 08:47:48.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/ext_l.png
--rw-rw-rw-   0        0        0    10651 2022-06-21 08:47:40.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/ext_r.png
--rw-rw-rw-   0        0        0    11465 2022-06-21 08:50:03.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/extfit_l.png
--rw-rw-rw-   0        0        0    11990 2022-06-21 08:49:52.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/extfit_r.png
--rw-rw-rw-   0        0        0     3602 2022-06-21 09:12:10.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/fit.png
--rw-rw-rw-   0        0        0     8954 2022-06-21 12:38:49.000000 napari_filaments-0.2.1/src/napari_filaments/_icon/undo.png
--rw-rw-rw-   0        0        0     5329 2022-07-03 05:29:22.000000 napari_filaments-0.2.1/src/napari_filaments/_optimizer.py
--rw-rw-rw-   0        0        0    12963 2022-07-03 05:03:24.000000 napari_filaments-0.2.1/src/napari_filaments/_spline.py
--rw-rw-rw-   0        0        0     2358 2022-07-03 07:22:57.000000 napari_filaments-0.2.1/src/napari_filaments/_table_stack.py
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:47.007850 napari_filaments-0.2.1/src/napari_filaments/_tests/
--rw-rw-rw-   0        0        0        0 2022-06-20 11:37:18.000000 napari_filaments-0.2.1/src/napari_filaments/_tests/__init__.py
--rw-rw-rw-   0        0        0      778 2022-07-01 07:14:49.000000 napari_filaments-0.2.1/src/napari_filaments/_tests/test_optimizer.py
--rw-rw-rw-   0        0        0     5611 2022-07-06 13:36:03.000000 napari_filaments-0.2.1/src/napari_filaments/_tests/test_widget.py
--rw-rw-rw-   0        0        0      175 2022-06-21 07:08:14.000000 napari_filaments-0.2.1/src/napari_filaments/_types.py
--rw-rw-rw-   0        0        0    34902 2022-07-06 14:46:55.000000 napari_filaments-0.2.1/src/napari_filaments/_widget.py
--rw-rw-rw-   0        0        0      418 2022-06-21 14:13:39.000000 napari_filaments-0.2.1/src/napari_filaments/core.py
--rw-rw-rw-   0        0        0      327 2022-06-22 16:50:52.000000 napari_filaments-0.2.1/src/napari_filaments/napari.yaml
-drwxrwxrwx   0        0        0        0 2022-07-16 06:21:46.978118 napari_filaments-0.2.1/src/napari_filaments.egg-info/
--rw-rw-rw-   0        0        0     4814 2022-07-16 06:21:46.000000 napari_filaments-0.2.1/src/napari_filaments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2022-07-16 06:21:46.000000 napari_filaments-0.2.1/src/napari_filaments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-16 06:21:46.000000 napari_filaments-0.2.1/src/napari_filaments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2022-07-16 06:21:46.000000 napari_filaments-0.2.1/src/napari_filaments.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      112 2022-07-16 06:21:46.000000 napari_filaments-0.2.1/src/napari_filaments.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-07-16 06:21:46.000000 napari_filaments-0.2.1/src/napari_filaments.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 13:10:34.223250 napari_filaments-0.3.0/
+-rw-rw-rw-   0        0        0     1513 2022-06-20 11:37:18.000000 napari_filaments-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      126 2022-07-01 07:58:33.000000 napari_filaments-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4956 2023-06-04 13:10:34.223250 napari_filaments-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3831 2022-08-21 03:47:14.000000 napari_filaments-0.3.0/README.md
+-rw-rw-rw-   0        0        0      747 2023-06-04 13:02:43.000000 napari_filaments-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1559 2023-06-04 13:10:34.229242 napari_filaments-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       40 2022-07-01 07:26:07.000000 napari_filaments-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:10:34.057363 napari_filaments-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 13:10:34.125628 napari_filaments-0.3.0/src/napari_filaments/
+-rw-rw-rw-   0        0        0      320 2023-06-04 05:39:23.000000 napari_filaments-0.3.0/src/napari_filaments/__init__.py
+-rw-rw-rw-   0        0        0      101 2023-06-04 05:39:23.000000 napari_filaments-0.3.0/src/napari_filaments/_consts.py
+-rw-rw-rw-   0        0        0     2119 2023-06-04 06:22:08.000000 napari_filaments-0.3.0/src/napari_filaments/_custom_layers.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:10:34.206196 napari_filaments-0.3.0/src/napari_filaments/_icon/
+-rw-rw-rw-   0        0        0        0 2022-07-01 07:39:21.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/__init__.py
+-rw-rw-rw-   0        0        0     5981 2022-06-21 08:30:26.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/clip_l.png
+-rw-rw-rw-   0        0        0     6000 2022-06-21 08:30:37.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/clip_r.png
+-rw-rw-rw-   0        0        0     2336 2022-06-21 12:20:44.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/del.png
+-rw-rw-rw-   0        0        0     8068 2022-06-21 09:07:18.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/erf2.png
+-rw-rw-rw-   0        0        0     7526 2022-06-21 08:21:08.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/erf_l.png
+-rw-rw-rw-   0        0        0     7095 2022-06-21 08:21:37.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/erf_r.png
+-rw-rw-rw-   0        0        0     9881 2022-06-21 08:47:48.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/ext_l.png
+-rw-rw-rw-   0        0        0    10651 2022-06-21 08:47:40.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/ext_r.png
+-rw-rw-rw-   0        0        0    11465 2022-06-21 08:50:03.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/extfit_l.png
+-rw-rw-rw-   0        0        0    11990 2022-06-21 08:49:52.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/extfit_r.png
+-rw-rw-rw-   0        0        0     3602 2022-06-21 09:12:10.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/fit.png
+-rw-rw-rw-   0        0        0     9660 2023-06-04 05:39:23.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/redo.png
+-rw-rw-rw-   0        0        0     8954 2022-06-21 12:38:49.000000 napari_filaments-0.3.0/src/napari_filaments/_icon/undo.png
+-rw-rw-rw-   0        0        0     5409 2023-04-07 14:56:30.000000 napari_filaments-0.3.0/src/napari_filaments/_optimizer.py
+-rw-rw-rw-   0        0        0    12983 2023-06-04 06:41:14.000000 napari_filaments-0.3.0/src/napari_filaments/_spline.py
+-rw-rw-rw-   0        0        0     4783 2023-06-04 05:39:23.000000 napari_filaments-0.3.0/src/napari_filaments/_subwidgets.py
+-rw-rw-rw-   0        0        0     2358 2022-07-03 07:22:57.000000 napari_filaments-0.3.0/src/napari_filaments/_table_stack.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:10:34.220244 napari_filaments-0.3.0/src/napari_filaments/_tests/
+-rw-rw-rw-   0        0        0        0 2022-06-20 11:37:18.000000 napari_filaments-0.3.0/src/napari_filaments/_tests/__init__.py
+-rw-rw-rw-   0        0        0      778 2022-07-01 07:14:49.000000 napari_filaments-0.3.0/src/napari_filaments/_tests/test_optimizer.py
+-rw-rw-rw-   0        0        0     9298 2023-06-04 07:02:22.000000 napari_filaments-0.3.0/src/napari_filaments/_tests/test_widget.py
+-rw-rw-rw-   0        0        0      175 2022-06-21 07:08:14.000000 napari_filaments-0.3.0/src/napari_filaments/_types.py
+-rw-rw-rw-   0        0        0    40837 2023-06-04 07:21:12.000000 napari_filaments-0.3.0/src/napari_filaments/_widget.py
+-rw-rw-rw-   0        0        0      501 2023-04-07 15:07:37.000000 napari_filaments-0.3.0/src/napari_filaments/core.py
+-rw-rw-rw-   0        0        0      327 2022-06-22 16:50:52.000000 napari_filaments-0.3.0/src/napari_filaments/napari.yaml
+drwxrwxrwx   0        0        0        0 2023-06-04 13:10:34.151915 napari_filaments-0.3.0/src/napari_filaments.egg-info/
+-rw-rw-rw-   0        0        0     4956 2023-06-04 13:10:33.000000 napari_filaments-0.3.0/src/napari_filaments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1348 2023-06-04 13:10:33.000000 napari_filaments-0.3.0/src/napari_filaments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:10:33.000000 napari_filaments-0.3.0/src/napari_filaments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-04 13:10:33.000000 napari_filaments-0.3.0/src/napari_filaments.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      120 2023-06-04 13:10:33.000000 napari_filaments-0.3.0/src/napari_filaments.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-04 13:10:33.000000 napari_filaments-0.3.0/src/napari_filaments.egg-info/top_level.txt
```

### Comparing `napari_filaments-0.2.1/LICENSE` & `napari_filaments-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/PKG-INFO` & `napari_filaments-0.3.0/src/napari_filaments.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
-Name: napari_filaments
-Version: 0.2.1
+Name: napari-filaments
+Version: 0.3.0
 Summary: A napari plugin for filament analysis
 Home-page: https://github.com/hanjinliu/napari-filaments
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hanjinliu/napari-filaments/issues
 Project-URL: Documentation, https://github.com/hanjinliu/napari-filaments#README.md
 Project-URL: Source Code, https://github.com/hanjinliu/napari-filaments
 Project-URL: User Support, https://github.com/hanjinliu/napari-filaments/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-filaments
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-filaments.svg?color=green)](https://github.com/hanjinliu/napari-filaments/raw/main/LICENSE)
@@ -52,22 +48,32 @@
 - Import paths from ImageJ ROI file.
 
 Basic Usage
 -----------
 
 Click `Layers > open image` to open a tif file. You'll find the image you chose and a shapes layer are added to the layer list.
 
-![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig.png)
+![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig-1.png)
 
 - The "target filaments" box shows the working shapes layer.
 - The "target image" box shows the image layer on which fitting and quantification will be conducted.
 - The "filament" box shows currently selected shape (initially this box is empty).
 
 Add path shapes and push key `F1` to fit the shape to the filament in the target image layer.
 
+- In the "Spline" tab, you can cut/extend or re-fit splines.
+- In the "Measure" tab, click "measure property" to measure mean instensity etc along each spline.
+
+How it works
+------------
+
+Spline fitting is done as following.
+
+![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig-2.png)
+
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 
 ## Installation
@@ -110,9 +116,7 @@
 
 [file an issue]: https://github.com/hanjinliu/napari-filaments/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

### Comparing `napari_filaments-0.2.1/README.md` & `napari_filaments-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,32 @@
 - Import paths from ImageJ ROI file.
 
 Basic Usage
 -----------
 
 Click `Layers > open image` to open a tif file. You'll find the image you chose and a shapes layer are added to the layer list.
 
-![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig.png)
+![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig-1.png)
 
 - The "target filaments" box shows the working shapes layer.
 - The "target image" box shows the image layer on which fitting and quantification will be conducted.
 - The "filament" box shows currently selected shape (initially this box is empty).
 
 Add path shapes and push key `F1` to fit the shape to the filament in the target image layer.
 
+- In the "Spline" tab, you can cut/extend or re-fit splines.
+- In the "Measure" tab, click "measure property" to measure mean instensity etc along each spline.
+
+How it works
+------------
+
+Spline fitting is done as following.
+
+![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig-2.png)
+
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 
 ## Installation
```

### Comparing `napari_filaments-0.2.1/setup.cfg` & `napari_filaments-0.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 695f 6669 6c61 6d65   = napari_filame
 00000020: 6e74 730d 0a76 6572 7369 6f6e 203d 2030  nts..version = 0
-00000030: 2e32 2e31 0d0a 6465 7363 7269 7074 696f  .2.1..descriptio
+00000030: 2e33 2e30 0d0a 6465 7363 7269 7074 696f  .3.0..descriptio
 00000040: 6e20 3d20 4120 6e61 7061 7269 2070 6c75  n = A napari plu
 00000050: 6769 6e20 666f 7220 6669 6c61 6d65 6e74  gin for filament
 00000060: 2061 6e61 6c79 7369 730d 0a6c 6f6e 675f   analysis..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 000000a0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
@@ -37,68 +37,62 @@
 00000240: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000250: 6167 6520 3a3a 2050 7974 686f 6e0d 0a09  age :: Python...
 00000260: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000270: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 00000280: 3a20 330d 0a09 5072 6f67 7261 6d6d 696e  : 3...Programmin
 00000290: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
 000002a0: 7468 6f6e 203a 3a20 3320 3a3a 204f 6e6c  thon :: 3 :: Onl
-000002b0: 790d 0a09 5072 6f67 7261 6d6d 696e 6720  y...Programming 
-000002c0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000002d0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-000002e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000002f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000300: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000310: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000320: 6f6e 203a 3a20 332e 3130 0d0a 0954 6f70  on :: 3.10...Top
-00000330: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-00000340: 6576 656c 6f70 6d65 6e74 203a 3a20 5465  evelopment :: Te
-00000350: 7374 696e 670d 0a70 726f 6a65 6374 5f75  sting..project_u
-00000360: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-00000370: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000380: 6974 6875 622e 636f 6d2f 6861 6e6a 696e  ithub.com/hanjin
-00000390: 6c69 752f 6e61 7061 7269 2d66 696c 616d  liu/napari-filam
-000003a0: 656e 7473 2f69 7373 7565 730d 0a09 446f  ents/issues...Do
-000003b0: 6375 6d65 6e74 6174 696f 6e20 3d20 6874  cumentation = ht
-000003c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003d0: 2f68 616e 6a69 6e6c 6975 2f6e 6170 6172  /hanjinliu/napar
-000003e0: 692d 6669 6c61 6d65 6e74 7323 5245 4144  i-filaments#READ
-000003f0: 4d45 2e6d 640d 0a09 536f 7572 6365 2043  ME.md...Source C
-00000400: 6f64 6520 3d20 6874 7470 733a 2f2f 6769  ode = https://gi
-00000410: 7468 7562 2e63 6f6d 2f68 616e 6a69 6e6c  thub.com/hanjinl
-00000420: 6975 2f6e 6170 6172 692d 6669 6c61 6d65  iu/napari-filame
-00000430: 6e74 730d 0a09 5573 6572 2053 7570 706f  nts...User Suppo
-00000440: 7274 203d 2068 7474 7073 3a2f 2f67 6974  rt = https://git
-00000450: 6875 622e 636f 6d2f 6861 6e6a 696e 6c69  hub.com/hanjinli
-00000460: 752f 6e61 7061 7269 2d66 696c 616d 656e  u/napari-filamen
-00000470: 7473 2f69 7373 7565 730d 0a0d 0a5b 6f70  ts/issues....[op
-00000480: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
-00000490: 203d 2066 696e 643a 0d0a 696e 7374 616c   = find:..instal
-000004a0: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-000004b0: 6d61 6769 632d 636c 6173 733e 3d30 2e36  magic-class>=0.6
-000004c0: 2e37 0d0a 096d 6167 6963 6775 690d 0a09  .7...magicgui...
-000004d0: 6d61 7470 6c6f 746c 6962 0d0a 096e 756d  matplotlib...num
-000004e0: 7079 0d0a 0971 7470 790d 0a09 7363 6970  py...qtpy...scip
-000004f0: 790d 0a70 7974 686f 6e5f 7265 7175 6972  y..python_requir
-00000500: 6573 203d 203e 3d33 2e38 0d0a 696e 636c  es = >=3.8..incl
-00000510: 7564 655f 7061 636b 6167 655f 6461 7461  ude_package_data
-00000520: 203d 2054 7275 650d 0a70 6163 6b61 6765   = True..package
-00000530: 5f64 6972 203d 200d 0a09 3d73 7263 0d0a  _dir = ...=src..
-00000540: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-00000550: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-00000560: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-00000570: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000580: 0d0a 6e61 7061 7269 2e6d 616e 6966 6573  ..napari.manifes
-00000590: 7420 3d20 0d0a 096e 6170 6172 692d 6669  t = ...napari-fi
-000005a0: 6c61 6d65 6e74 7320 3d20 6e61 7061 7269  laments = napari
-000005b0: 5f66 696c 616d 656e 7473 3a6e 6170 6172  _filaments:napar
-000005c0: 692e 7961 6d6c 0d0a 0d0a 5b6f 7074 696f  i.yaml....[optio
-000005d0: 6e73 2e65 7874 7261 735f 7265 7175 6972  ns.extras_requir
-000005e0: 655d 0d0a 7465 7374 696e 6720 3d20 0d0a  e]..testing = ..
-000005f0: 096e 6170 6172 690d 0a09 7079 7174 350d  .napari...pyqt5.
-00000600: 0a09 7079 7465 7374 0d0a 0970 7974 6573  ..pytest...pytes
-00000610: 742d 636f 760d 0a09 7079 7465 7374 2d71  t-cov...pytest-q
-00000620: 740d 0a09 746f 780d 0a0d 0a5b 6f70 7469  t...tox....[opti
-00000630: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000640: 5d0d 0a2a 203d 202a 2e79 616d 6c0d 0a0d  ]..* = *.yaml...
-00000650: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-00000660: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-00000670: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+000002b0: 790d 0a09 546f 7069 6320 3a3a 2053 6f66  y...Topic :: Sof
+000002c0: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
+000002d0: 7420 3a3a 2054 6573 7469 6e67 0d0a 7072  t :: Testing..pr
+000002e0: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+000002f0: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+00000300: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000310: 2f68 616e 6a69 6e6c 6975 2f6e 6170 6172  /hanjinliu/napar
+00000320: 692d 6669 6c61 6d65 6e74 732f 6973 7375  i-filaments/issu
+00000330: 6573 0d0a 0944 6f63 756d 656e 7461 7469  es...Documentati
+00000340: 6f6e 203d 2068 7474 7073 3a2f 2f67 6974  on = https://git
+00000350: 6875 622e 636f 6d2f 6861 6e6a 696e 6c69  hub.com/hanjinli
+00000360: 752f 6e61 7061 7269 2d66 696c 616d 656e  u/napari-filamen
+00000370: 7473 2352 4541 444d 452e 6d64 0d0a 0953  ts#README.md...S
+00000380: 6f75 7263 6520 436f 6465 203d 2068 7474  ource Code = htt
+00000390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000003a0: 6861 6e6a 696e 6c69 752f 6e61 7061 7269  hanjinliu/napari
+000003b0: 2d66 696c 616d 656e 7473 0d0a 0955 7365  -filaments...Use
+000003c0: 7220 5375 7070 6f72 7420 3d20 6874 7470  r Support = http
+000003d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+000003e0: 616e 6a69 6e6c 6975 2f6e 6170 6172 692d  anjinliu/napari-
+000003f0: 6669 6c61 6d65 6e74 732f 6973 7375 6573  filaments/issues
+00000400: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000410: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
+00000420: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000430: 7320 3d20 0d0a 096d 6167 6963 2d63 6c61  s = ...magic-cla
+00000440: 7373 3e3d 302e 372e 330d 0a09 6d61 6769  ss>=0.7.3...magi
+00000450: 6367 7569 0d0a 096d 6174 706c 6f74 6c69  cgui...matplotli
+00000460: 620d 0a09 6e75 6d70 790d 0a09 7174 7079  b...numpy...qtpy
+00000470: 0d0a 0973 6369 7079 0d0a 7079 7468 6f6e  ...scipy..python
+00000480: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000490: 390d 0a69 6e63 6c75 6465 5f70 6163 6b61  9..include_packa
+000004a0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+000004b0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000004c0: 093d 7372 630d 0a0d 0a5b 6f70 7469 6f6e  .=src....[option
+000004d0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000004e0: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+000004f0: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
+00000500: 706f 696e 7473 5d0d 0a6e 6170 6172 692e  points]..napari.
+00000510: 6d61 6e69 6665 7374 203d 200d 0a09 6e61  manifest = ...na
+00000520: 7061 7269 2d66 696c 616d 656e 7473 203d  pari-filaments =
+00000530: 206e 6170 6172 695f 6669 6c61 6d65 6e74   napari_filament
+00000540: 733a 6e61 7061 7269 2e79 616d 6c0d 0a0d  s:napari.yaml...
+00000550: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000560: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+00000570: 6e67 203d 200d 0a09 6e61 7061 7269 0d0a  ng = ...napari..
+00000580: 0970 7971 7435 0d0a 0970 7974 6573 740d  .pyqt5...pytest.
+00000590: 0a09 7079 7465 7374 2d63 6f76 0d0a 0970  ..pytest-cov...p
+000005a0: 7974 6573 742d 7174 0d0a 0972 6f69 6669  ytest-qt...roifi
+000005b0: 6c65 0d0a 0974 6f78 0d0a 0d0a 5b6f 7074  le...tox....[opt
+000005c0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+000005d0: 615d 0d0a 2a20 3d20 0d0a 092a 2e79 616d  a]..* = ...*.yam
+000005e0: 6c0d 0a09 2a2e 706e 670d 0a0d 0a5b 6567  l...*.png....[eg
+000005f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000600: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000610: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/clip_l.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/clip_l.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/clip_r.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/clip_r.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/del.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/del.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/erf2.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/erf2.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/erf_l.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/erf_l.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/erf_r.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/erf_r.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/ext_l.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/ext_l.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/ext_r.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/ext_r.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/extfit_l.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/extfit_l.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/extfit_r.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/extfit_r.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/fit.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/fit.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_icon/undo.png` & `napari_filaments-0.3.0/src/napari_filaments/_icon/undo.png`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_optimizer.py` & `napari_filaments-0.3.0/src/napari_filaments/_optimizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, NamedTuple, Tuple, Union
 
 import numpy as np
 from numpy.typing import ArrayLike
 from scipy.optimize import curve_fit
 from scipy.special import erf
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import Self
 
 
 sq2 = np.sqrt(2)
 Bounds = Tuple[Union[ArrayLike, float], Union[ArrayLike, float]]
 
 
@@ -86,15 +86,15 @@
 class GaussianOptimizer(Optimizer):
     class Parameters(NamedTuple):
         mu: float
         sg: float
         a: float
         b: float
 
-    if TYPE_CHECKING:
+    if TYPE_CHECKING:  # pragma: no cover
 
         @property
         def params(self) -> Parameters:
             ...
 
     @staticmethod
     def model(xdata: np.ndarray, mu, sg, a, b):
@@ -117,15 +117,15 @@
 class ErfOptimizer(Optimizer):
     class Parameters(NamedTuple):
         mu: float
         sg: float
         a: float
         b: float
 
-    if TYPE_CHECKING:
+    if TYPE_CHECKING:  # pragma: no cover
 
         @property
         def params(self) -> Parameters:
             ...
 
     @staticmethod
     def model(xdata: np.ndarray, mu, sg, a, b):
@@ -160,15 +160,15 @@
         mu1: float
         sg0: float
         sg1: float
         a: float
         b0: float
         b1: float
 
-    if TYPE_CHECKING:
+    if TYPE_CHECKING:  # pragma: no cover
 
         @property
         def params(self) -> Parameters:
             ...
 
     @staticmethod
     def model(xdata: np.ndarray, mu0, mu1, sg0, sg1, a, b0, b1):
```

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_spline.py` & `napari_filaments-0.3.0/src/napari_filaments/_spline.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import cached_property, lru_cache
 from typing import TYPE_CHECKING, Any, Callable, Sequence
 
 import numpy as np
 from scipy import ndimage as ndi
 from scipy.interpolate import splev, splprep
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import Self
 
     _TCK = tuple[tuple[np.ndarray, list[np.ndarray], int], np.ndarray]
 
 from . import _optimizer as _opt
```

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_table_stack.py` & `napari_filaments-0.3.0/src/napari_filaments/_table_stack.py`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_tests/test_optimizer.py` & `napari_filaments-0.3.0/src/napari_filaments/_tests/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_tests/test_widget.py` & `napari_filaments-0.3.0/src/napari_filaments/_tests/test_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from pathlib import Path
+import pytest
 
 import napari
 import numpy as np
 from numpy.testing import assert_allclose
 
-from napari_filaments import FilamentAnalyzer
+from napari_filaments import FilamentAnalyzer, start
+from magicclass import get_button
+import magicclass.testing as mcls_testing
 
 IMAGE_PATH = Path(__file__).parent / "image.tif"
 SAVE_PATH = Path(__file__).parent / "result"
+ROI_PATH = Path(__file__).parent / "_roi"
 DUMMY_PATH = Path(__file__).parent / "test.tif"
 
 rng = np.random.default_rng(1234)
 
 
 def _get_dock_widget(make_napari_viewer) -> FilamentAnalyzer:
     viewer: napari.Viewer = make_napari_viewer()
@@ -24,33 +28,49 @@
 
 def test_widget(make_napari_viewer):
     ui = _get_dock_widget(make_napari_viewer)
 
     assert ui.parent_viewer is not None
 
 
+def test_magicclass_stuff(make_napari_viewer):
+    ui = _get_dock_widget(make_napari_viewer)
+    mcls_testing.check_function_gui_buildable(ui)
+    mcls_testing.check_tooltip(ui)
+
+
+def test_start(make_napari_viewer):
+    ui = start(make_napari_viewer())
+    ui.parent_viewer.close()
+
+
 def test_fit(make_napari_viewer):
     ui = _get_dock_widget(make_napari_viewer)
     ui.open_image(IMAGE_PATH)
 
-    ui.target_filaments.add([[48, 31], [55, 86]], shape_type="path")
+    ui.add_filament_data([[48, 31], [55, 86]])
     ui.fit_filament(ui.parent_viewer.layers[0])
 
-    ui.clip_left()
-    ui.clip_right()
+    ui.truncate_left()
+    ui.truncate_right()
     ui.extend_left()
     ui.extend_right()
 
+    for _ in range(5):
+        ui.undo()
+    for _ in range(5):
+        ui.redo()
+
 
 def test_io(make_napari_viewer):
     ui = _get_dock_widget(make_napari_viewer)
     ui.open_image(IMAGE_PATH)
     img_layer = ui.target_image
 
-    ui.target_filaments.add([[48, 31], [55, 86]], shape_type="path")
+    ui.add_filament_data([[48, 31], [55, 86]])
     ui.fit_filament(img_layer)
 
     data0 = ui.target_filaments.data
 
     ui.save_filaments(ui.target_filaments, SAVE_PATH)
     ui.open_filaments(SAVE_PATH)
 
@@ -61,15 +81,15 @@
 
 
 def test_measure(make_napari_viewer):
     ui = _get_dock_widget(make_napari_viewer)
     ui.open_image(IMAGE_PATH)
     img_layer = ui.target_image
 
-    ui.target_filaments.add([[48, 31], [55, 86]], shape_type="path")
+    ui.add_filament_data([[48, 31], [55, 86]])
     ui.fit_filament(img_layer)
 
     ui.target_filaments.add([[10, 10], [10, 50]], shape_type="path")
 
     from napari_filaments._spline import Measurement
 
     ui.measure_properties(img_layer, properties=Measurement.PROPERTIES)
@@ -111,22 +131,22 @@
     ui.filament = 0
     assert ui.target_filaments.selected_data == {0}
     assert ui.parent_viewer.dims.current_step[0] == 0
     ui.filament = 2
     assert ui.target_filaments.selected_data == {2}
     assert ui.parent_viewer.dims.current_step[0] == 2
 
-    ui["delete_current"].changed()
+    get_button(ui.delete_filament).changed()
     assert ui["filament"].choices == (0, 1)
     assert ui.filament == 1
     assert ui.target_filaments.selected_data == {1}
     assert ui.parent_viewer.dims.current_step[0] == 0
 
     ui.filament = 0
-    ui["delete_current"].changed()
+    get_button(ui.delete_filament).changed()
     assert ui["filament"].choices == (0,)
     assert ui.target_filaments.selected_data == {0}
     assert ui.filament == 0
 
 
 def test_target_change(make_napari_viewer):
     ui = _get_dock_widget(make_napari_viewer)
@@ -147,28 +167,122 @@
     ui["target_filaments"].value = ui["target_filaments"].choices[0]
     assert ui.filament is None
     assert ui.parent_viewer.dims.current_step[0] == 2
     ui.target_filaments.add_paths([[0, 10, 10], [0, 10, 40]])
     ui.target_filaments.add_paths([[1, 10, 10], [1, 10, 40]])
     assert ui.filament == 1
     ui.parent_viewer.dims.set_current_step(0, 1)
+    assert ui.filament == 1
 
     ui["target_filaments"].value = ui["target_filaments"].choices[1]
     assert ui.filament == 1
     assert ui.parent_viewer.dims.current_step[0] == 1
     ui.filament = 2
 
     ui["target_filaments"].value = ui["target_filaments"].choices[0]
+    # 0-th filaments layer has less filaments. Set to the last filament.
     assert ui.filament == 1
 
 
 def test_add_filament_layer(make_napari_viewer):
-    from napari.layers import Shapes
+    from napari_filaments._custom_layers import FilamentsLayer
 
     ui = _get_dock_widget(make_napari_viewer)
     img = rng.normal(size=(5, 100, 100))
     ui._add_image(img, "TYX", DUMMY_PATH)
     ui.add_filaments()
 
-    assert type(ui.parent_viewer.layers[-1]) is Shapes
-    assert type(ui.parent_viewer.layers[-2]) is Shapes
+    assert type(ui.parent_viewer.layers[-1]) is FilamentsLayer
+    assert type(ui.parent_viewer.layers[-2]) is FilamentsLayer
     assert ui.parent_viewer.layers[0].visible
+
+
+def test_extend_and_fit(make_napari_viewer):
+    ui = _get_dock_widget(make_napari_viewer)
+    ui.open_image(IMAGE_PATH)
+
+    ui.add_filament_data([[48, 31], [55, 86]])
+    image_layer = ui.parent_viewer.layers[0]
+    ui.fit_filament(image_layer)
+
+    ui.truncate_left()
+    ui.truncate_right()
+    ui.extend_and_fit_left(image_layer)
+    ui.extend_and_fit_right(image_layer)
+
+
+def test_clip_inflection(make_napari_viewer):
+    ui = _get_dock_widget(make_napari_viewer)
+    ui.open_image(IMAGE_PATH)
+
+    ui.add_filament_data([[48, 31], [55, 86]])
+    ui.fit_filament()
+
+    ui.extend_left(dx=20)
+    ui.extend_right(dx=20)
+    ui.truncate_left_at_inflection()
+    ui.truncate_right_at_inflection()
+    assert ui.get_spline(0).length() == pytest.approx(62.7, abs=0.1)
+    ui.undo()
+    ui.undo()
+    ui.truncate_at_inflections()
+    assert ui.get_spline(0).length() == pytest.approx(62.7, abs=0.2)
+
+
+def test_read_roi_files(make_napari_viewer):
+    ui = _get_dock_widget(make_napari_viewer)
+    ui.open_image(IMAGE_PATH)
+    for path in (ROI_PATH).glob("*"):
+        ui.from_roi(path)
+        for i in range(ui.target_filaments.nshapes):
+            _, prof = ui.get_profile(i)
+            assert prof.mean() > 80
+
+
+def test_plot(make_napari_viewer):
+    ui = _get_dock_widget(make_napari_viewer)
+    ui.open_image(IMAGE_PATH)
+    ui.add_filament_data([[48, 31], [55, 86]])
+    ui.fit_filament()
+    ui.plot_profile()
+    ui.plot_curvature()
+
+
+def test_delete(make_napari_viewer):
+    from napari_filaments._consts import ROI_ID
+
+    ui = _get_dock_widget(make_napari_viewer)
+    ui.open_image(IMAGE_PATH)
+    ui.add_filament_data([[48, 30], [55, 86]])
+    ui.fit_filament()
+    ui.add_filament_data([[48, 31], [55, 86]])
+    ui.fit_filament()
+    ui.add_filament_data([[48, 32], [55, 86]])
+    ui.fit_filament()
+    ui.filament = 1
+    data = ui.target_filaments.data.copy()
+    ui.delete_filament(1)
+    assert ui.target_filaments.nshapes == len(data) - 1
+    assert_allclose(ui.target_filaments.data[0], data[0])
+    assert_allclose(ui.target_filaments.data[1], data[2])
+    assert list(ui.target_filaments.features[ROI_ID]) == [0, 1]
+
+    ui.undo()
+    assert ui.target_filaments.nshapes == len(data)
+    assert_allclose(ui.target_filaments.data[0], data[0])
+    assert_allclose(ui.target_filaments.data[1], data[1])
+    assert_allclose(ui.target_filaments.data[2], data[2])
+    assert list(ui.target_filaments.features[ROI_ID]) == [0, 1, 2]
+
+    ui.redo()
+    assert ui.target_filaments.nshapes == len(data) - 1
+    assert_allclose(ui.target_filaments.data[0], data[0])
+    assert_allclose(ui.target_filaments.data[1], data[2])
+    assert list(ui.target_filaments.features[ROI_ID]) == [0, 1]
+
+
+def test_kymograph(make_napari_viewer):
+    ui = _get_dock_widget(make_napari_viewer)
+    img = rng.normal(size=(5, 100, 100))
+    ui._add_image(img, "TYX", DUMMY_PATH)
+    ui.add_filament_data([[0, 10, 10], [0, 90, 90]])
+    ui.kymograph(idx=0, time_axis="T")
```

### Comparing `napari_filaments-0.2.1/src/napari_filaments/_widget.py` & `napari_filaments-0.3.0/src/napari_filaments/_widget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,471 +1,279 @@
 import re
 import weakref
-from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, List, Set, Tuple, TypeVar, Union
+from typing import TYPE_CHECKING, Iterable, TypeVar, Annotated
 
 import numpy as np
+from numpy.typing import NDArray
+import pandas as pd
+import macrokit as mk
 from magicclass import (
     MagicTemplate,
     bind_key,
+    defaults,
     do_not_record,
     field,
     magicclass,
-    magicmenu,
-    magictoolbar,
     nogui,
     set_design,
     set_options,
     vfield,
 )
-from magicclass.types import Bound, OneOf, SomeOf
-from magicclass.widgets import Figure, Separator
-from napari.layers import Image, Shapes
+from magicclass.types import Path
+from magicclass.undo import undo_callback
+from magicclass.widgets import Figure
+import napari
+from napari.layers import Image
 
-from . import _optimizer as _opt
+from . import _optimizer as _opt, _subwidgets
 from ._spline import Measurement, Spline
 from ._table_stack import TableStack
 from ._types import weight
+from ._custom_layers import FilamentsLayer
+from ._consts import ROI_ID, TARGET_IMG_LAYERS, IMAGE_AXES, SOURCE
 
-if TYPE_CHECKING:
-    from magicclass.fields import MagicValueField
+if TYPE_CHECKING:  # pragma: no cover
     from magicgui.widgets import ComboBox
 
 ICON_DIR = Path(__file__).parent / "_icon"
-ICON_KWARGS = dict(text="", min_width=42, min_height=42)
+ICON_KW = dict(text="", min_width=42, min_height=42, max_height=45)
+SMALL_ICON_KW = dict(text="", min_width=20, min_height=28, max_height=30)
 
-# global metadata keys
-TARGET_IMG_LAYERS = "target-image-layer"
+ROI_FMT = "[{" + ROI_ID + "}]"
 
-ROI_ID = "ROI-ID"
-SOURCE = "source"
-IMAGE_AXES = "axes"
+defaults["macro-highlight"] = True
+del defaults
 
-ROI_FMT = "[{" + ROI_ID + "}]"
 
+@mk.register_type(np.ndarray)
+def _format_ndarray(x: np.ndarray):
+    if x.ndim != 2:
+        raise RuntimeError(
+            f"{x.ndim}D arrays are not supposed to be an input."
+        )
+    return str(x.tolist())
 
-@magicclass
+
+@magicclass(widget_type="scrollable")
 class FilamentAnalyzer(MagicTemplate):
     """
     Filament Analyzer widget.
 
     Attributes
     ----------
-    target_filament : Shapes
+    target_filaments : Shapes
         The target Shapes layer.
     target_image : Image
         The target Image layer. Fitting/analysis will be performed on this
         layer.
+    filament : int
+        The selected filament ID. Operations such as filament fitting,
+        extension, clipping will be performed on this filament.
     """
 
-    def _get_available_filament_id(self, w=None) -> List[int]:
+    def _get_available_filament_id(self, w=None) -> "list[int]":
         if self.target_filaments is None:
             return []
         return list(range(self.target_filaments.nshapes))
 
-    _tablestack = field(TableStack, name="Filament Analyzer Tables")
-    target_filaments: "MagicValueField[ComboBox, Shapes]" = vfield(Shapes)
-    target_image: "MagicValueField[ComboBox, Image]" = vfield(Image)
-    filament = vfield(OneOf[_get_available_filament_id])
-
-    # fmt: off
-    @magictoolbar
-    class Tools(MagicTemplate):
-        @magicmenu
-        class Layers(MagicTemplate):
-            def open_image(self): ...
-            def open_filaments(self): ...
-            def add_filaments(self): ...
-
-            @magicmenu
-            class Import(MagicTemplate):
-                def from_roi(self): ...
-            sep0 = field(Separator)
-            def save_filaments(self): ...
-            sep1 = field(Separator)
-            def create_total_intensity(self): ...
-            # def export_roi(self): ...
-
-        @magicmenu
-        class Parameters(MagicTemplate):
-            """
-            Global parameters of Filament Analyzer.
-
-            Attributes
-            ----------
-            lattice_width : int
-                The width of the image lattice along a filament.
-            dx : float
-                Delta x of filament clipping and extension.
-            sigma_range : (float, float)
-                The range of sigma to be used for fitting.
-
-            """
-            lattice_width = vfield(17, options={"min": 5, "max": 49}, record=False)  # noqa
-            dx = vfield(5.0, options={"min": 1, "max": 50.0}, record=False)
-            sigma_range = vfield((0.5, 5.0), record=False)
-            target_image_filter = vfield(True, record=False)
-
-        @magicmenu
-        class Others(MagicTemplate):
-            def create_macro(self): ...
-            def send_widget_to_viewer(self): ...
-
-    @magicclass(widget_type="tabbed")
-    class Tabs(MagicTemplate):
-        @magicclass(layout="horizontal")
-        class Spline(MagicTemplate):
-            def __post_init__(self):
-                self.margins = (2, 2, 2, 2)
-
-            @magicclass(widget_type="groupbox")
-            class Left(MagicTemplate):
-                def extend_left(self): ...
-                def extend_and_fit_left(self): ...
-                def clip_left(self): ...
-                def clip_left_at_inflection(self): ...
-
-            @magicclass(widget_type="frame")
-            class Both(MagicTemplate):
-                def fit_filament(self): ...
-                def delete_current(self): ...
-                def undo_spline(self): ...
-                def clip_at_inflections(self): ...
-
-            @magicclass(widget_type="groupbox")
-            class Right(MagicTemplate):
-                def extend_right(self): ...
-                def extend_and_fit_right(self): ...
-                def clip_right(self): ...
-                def clip_right_at_inflection(self): ...
-
-        @magicclass(widget_type="scrollable")
-        class Measure(MagicTemplate):
-            def measure_properties(self): ...
-            def plot_profile(self): ...
-            def plot_curvature(self): ...
-            def kymograph(self): ...
-
-    # fmt: on
-
-    @magicclass
-    class Output(MagicTemplate):
-        plt = field(Figure)
-
-        def __post_init__(self):
-            self._xdata = []
-            self._ydata = []
-            self.min_height = 200
-
-        @do_not_record
-        def view_data(self):
-            """View plot data in a table."""
-            xlabel = self.plt.ax.get_xlabel() or "x"
-            ylabel = self.plt.ax.get_ylabel() or "y"
-            if isinstance(self._ydata, list):
-                data = {xlabel: self._xdata}
-                for i, y in enumerate(self._ydata):
-                    data[f"{ylabel}-{i}"] = y
-            else:
-                data = {xlabel: self._xdata, ylabel: self._ydata}
-            tstack = self.find_ancestor(FilamentAnalyzer)._tablestack
-            tstack.add_table(data, name="Plot data")
-            tstack.show()
-
-        def _plot(self, x, y, clear=True, **kwargs):
-            if clear:
-                self.plt.cla()
-            self.plt.plot(x, y, **kwargs)
-            self._xdata = x
-            if clear:
-                self._ydata = y
-            else:
-                if isinstance(self._ydata, list):
-                    self._ydata.append(y)
-                else:
-                    self._ydata = [self._ydata, y]
-
-        def _set_labels(self, x: str, y: str):
-            self.plt.xlabel(x)
-            self.plt.ylabel(y)
+    _tablestack = field(TableStack, name="_Filament Analyzer Tables")
+    target_filaments = vfield(FilamentsLayer, record=False)
+    target_image = vfield(Image, record=False)
+    filament = vfield(int, record=False).with_choices(
+        _get_available_filament_id
+    )
+
+    Tabs = _subwidgets.Tabs
+    Tools = _subwidgets.Tools
+    Output = _subwidgets.Output
 
     def __init__(self):
         self._last_target_filaments = None
         self._color_default = np.array([0.973, 1.000, 0.412, 1.000])
-        self._last_data: Tuple[int, np.ndarray] = None
-        self._dims_slider_changing = False
         self._nfilaments = 0
+        self.objectName()  # activate napari namespace
 
-    def _get_idx(self, w=None) -> Union[int, Set[int]]:
+    def _get_idx(self, w=None) -> "int | set[int]":
         if self.target_filaments is None:
             return 0
         sel = self.target_filaments.selected_data
         if len(sel) == 0:
+            if self.target_filaments.nshapes == 0:
+                raise ValueError("No filament is selected.")
             return self.target_filaments.nshapes - 1
         return sel
 
     @property
-    def last_target_filaments(self) -> Union[Shapes, None]:
+    def last_target_filaments(self) -> "FilamentsLayer | None":
         if self._last_target_filaments is None:
             return None
         return self._last_target_filaments()
 
     @last_target_filaments.setter
-    def last_target_filaments(self, val: Union[Shapes, None]):
+    def last_target_filaments(self, val: "FilamentsLayer | None"):
         if val is None:
             self._last_target_filaments = None
             return
 
-        if not isinstance(val, Shapes):
+        if not isinstance(val, FilamentsLayer):
             raise TypeError(
                 f"Cannot set type {type(val)} to `last_target_filaments`."
             )
         self._last_target_filaments = weakref.ref(val)
+        return None
 
     @target_filaments.connect
-    def _on_change(self):
+    def _on_target_filament_change(self):
         # old parameters
         _sl = self.parent_viewer.dims.current_step[:-2]
         _fil = self.filament
         if self.last_target_filaments is not None:
             _mode = self.last_target_filaments.mode
             _toggle_target_images(self.last_target_filaments, False)
         else:
             _mode = "pan_zoom"
 
-        self._last_data = None
         _toggle_target_images(self.target_filaments, True)
         self.last_target_filaments = self.target_filaments
         self.parent_viewer.layers.selection = {self.target_filaments}
 
         self._filter_image_choices()
         cbox: ComboBox = self["filament"]
         cbox.reset_choices()
 
         # restore old parameters
         self.target_filaments.mode = _mode
         if _fil in cbox.choices:
             cbox.value = _fil
+        else:
+            try:
+                cbox.value = max(cbox.choices)
+            except Exception:
+                pass
         self.parent_viewer.dims.set_current_step(np.arange(len(_sl)), _sl)
+        self._on_filament_change(self.filament)
+        return None
 
     @filament.connect
-    def _on_filament_change(self, idx: int):
-        data = self.target_filaments.data[idx]
+    def _on_filament_change(self, idx: "int | None"):
+        if idx is None:
+            return
+        layer = self.target_filaments
+        data = layer.data[idx]
         _sl, _ = _split_slice_and_path(data)
-        self._dims_slider_changing = True
         self.parent_viewer.dims.set_current_step(np.arange(len(_sl)), _sl)
-        self._dims_slider_changing = False
-        self.target_filaments.selected_data = {idx}
+        layer.selected_data = {idx}
 
-        props = self.target_filaments.current_properties
-        next_id = self.target_filaments.nshapes
+        props = layer.current_properties
+        next_id = layer.nshapes
         props[ROI_ID] = next_id
-        self.target_filaments.current_properties = props
+        layer.current_properties = props
 
-    def _filter_image_choices(self):
-        if not self.Tools.Parameters.target_image_filter:
-            return
-        target_image_widget: ComboBox = self["target_image"]
-        if target_image_widget.value is None:
-            return
-        cbox_idx = target_image_widget.choices.index(target_image_widget.value)
-        img_layers = _get_connected_target_image_layers(self.target_filaments)
-        if len(img_layers) > 0:
-            target_image_widget.choices = img_layers
-            cbox_idx = min(cbox_idx, len(img_layers) - 1)
-            target_image_widget.value = target_image_widget.choices[cbox_idx]
+        # update text color
+        colors = np.full((layer.nshapes, 4), 1.0)
+        colors[idx] = layer.edge_color[idx]
+        layer.text.color = colors
+        if layer.text.color.encoding_type == "ManualColorEncoding":
+            layer.text.color.default = "white"
+        return None
 
     @Tools.Layers.wraps
-    def open_image(self, path: Path):
+    @bind_key("Ctrl+K, Ctrl+O")
+    def open_image(self, path: Path.Read["*.tif;*.tiff"]):
         """Open a TIF."""
         path = Path(path)
         from tifffile import TiffFile
 
         with TiffFile(path) as tif:
             series0 = tif.series[0]
             axes = getattr(series0, "axes", "")
             img: np.ndarray = tif.asarray()
-        self._add_image(img, axes, path)
-
-    def _add_image(self, img: np.ndarray, axes: str, path: Path):
-        if "C" in axes:
-            ic = axes.find("C")
-            nchn = img.shape[ic]
-            axis_labels: Tuple[str] = tuple(c for c in axes if c != "C")
-            img_layers: List[Image] = self.parent_viewer.add_image(
-                img,
-                channel_axis=ic,
-                name=[f"[C{i}] {path.stem}" for i in range(nchn)],
-                metadata={IMAGE_AXES: axis_labels, SOURCE: path},
-            )
-        else:
-            axis_labels = tuple(axes)
-            _layer = self.parent_viewer.add_image(
-                img,
-                name=path.stem,
-                metadata={IMAGE_AXES: axis_labels, SOURCE: path},
-            )
-            img_layers = [_layer]
-
-        self._add_filament_layer(img_layers, path.stem)
-        ndim = self.parent_viewer.dims.ndim
-        if ndim == len(axis_labels):
-            self.parent_viewer.dims.set_axis_label(
-                list(range(ndim)), axis_labels
-            )
+        return self._add_image(img, axes, path)
 
     @Tools.Layers.wraps
-    @set_options(path={"mode": "d"})
-    def open_filaments(self, path: Path):
+    @bind_key("Ctrl+K, Ctrl+F")
+    def open_filaments(self, path: Path.Dir):
         """Open a directory with csv files as a filament layer."""
         import pandas as pd
 
         path = Path(path)
 
-        all_csv: List[np.ndarray] = []
+        all_csv: "list[np.ndarray]" = []
         for p in path.glob("*.csv"):
             df = pd.read_csv(p)
             all_csv.append(df.values)
         self._load_filament_coordinates(all_csv, f"[F] {path.stem}")
-
-    def _load_filament_coordinates(self, data: List[np.ndarray], name: str):
-        ndata = len(data)
-        layer_paths = self.parent_viewer.add_shapes(
-            data,
-            edge_color=self._color_default,
-            name=name,
-            shape_type="path",
-            edge_width=0.5,
-            properties={ROI_ID: np.arange(ndata, dtype=np.uint32)},
-            text=dict(string=ROI_FMT, color="white", size=8),
-        )
-
-        self._set_filament_layer(layer_paths)
-        layer_paths.current_properties = {ROI_ID: ndata}
-        self.target_filaments.metadata[TARGET_IMG_LAYERS] = list(
-            filter(lambda x: isinstance(x, Image), self.parent_viewer.layers)
-        )
+        return None
 
     @Tools.Layers.wraps
     def add_filaments(self):
         images = self.target_filaments.metadata[TARGET_IMG_LAYERS]
         name = self.target_filaments.name.lstrip("[F] ")
         return self._add_filament_layer(images, name)
 
-    def _add_filament_layer(self, images: List[Image], name: str):
-        """Add a Shapes layer for the target image."""
-        # check input images
-        ndim: int = _get_unique_value(img.ndim for img in images)
-        axes: Tuple[str] = _get_unique_value(
-            img.metadata[IMAGE_AXES] for img in images
-        )
-        layer = self.parent_viewer.add_shapes(
-            ndim=ndim,
-            edge_color=self._color_default,
-            name=f"[F] {name}",
-            metadata={IMAGE_AXES: axes, TARGET_IMG_LAYERS: images},
-            edge_width=0.5,
-            properties={ROI_ID: 0},
-            text=dict(string=ROI_FMT, color="white", size=8),
-        )
-
-        return self._set_filament_layer(layer)
-
-    def _set_filament_layer(self, new_filaments_layer: Shapes):
-        @new_filaments_layer.events.set_data.connect
-        def _on_data_changed(e):
-            if (
-                self.target_filaments is not new_filaments_layer
-                or self.target_filaments._is_moving
-                or self._dims_slider_changing
-            ):
-                return
-            # delete undo history
-            self._last_data = None
-
-            # update current filament ROI ID
-            next_id = self.target_filaments.nshapes
-            if self._nfilaments >= next_id:
-                features = self.target_filaments.features
-                features[ROI_ID] = np.arange(next_id)
-                self.target_filaments.features = features
-            props = self.target_filaments.current_properties
-            props[ROI_ID] = next_id
-            self.target_filaments.current_properties = props
-            self["filament"].reset_choices()
-            next_id = self.target_filaments.nshapes
-            try:
-                self.filament = next_id - 1
-            except Exception:
-                pass
-
-            self._nfilaments = next_id
-
-        new_filaments_layer.current_properties = {ROI_ID: 0}
-        self.target_filaments = new_filaments_layer
-        if self.last_target_filaments is None:
-            self.last_target_filaments = new_filaments_layer
-
-        new_filaments_layer.mode = "add_path"
-
-        return new_filaments_layer
-
     @Tools.Layers.Import.wraps
     @set_design(text="From ImageJ ROI")
-    def from_roi(self, path: Path):
+    def from_roi(
+        self,
+        path: Path.Read["*.zip;*.roi;;All files (*)"],
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+    ):
         """Import ImageJ Roi zip file as filaments."""
         from roifile import ROI_TYPE, roiread
 
+        _, filaments = self._check_layers(None, filaments)
         path = Path(path)
         rois = roiread(path)
         if not isinstance(rois, list):
             rois = [rois]
 
-        shapes = self.target_filaments
-        axes = shapes.metadata[IMAGE_AXES]
+        axes = filaments.metadata[IMAGE_AXES]
 
         for roi in rois:
             if roi.roitype not in (ROI_TYPE.LINE, ROI_TYPE.POLYLINE):
                 raise ValueError(f"ROI type {roi.roitype.name} not supported")
             # load coordinates
             yx: np.ndarray = roi.coordinates()[:, ::-1]
             p = roi.position
             t = roi.t_position if "T" in axes else -1
             z = roi.z_position if "Z" in axes else -1
 
             d = np.array([x - 1 for x in [p, t, z] if x > 0])
             stacked = np.stack([d] * yx.shape[0], axis=0)
             multi_coords = np.concatenate([stacked, yx], axis=1)
-            self.target_filaments.add_paths(multi_coords)
+            filaments.add_paths(multi_coords)
+        return None
 
     @Tools.Layers.wraps
-    @set_options(path={"mode": "w"})
-    def save_filaments(self, layer: Shapes, path: Path):
+    @bind_key("Ctrl+K, Ctrl+S")
+    def save_filaments(self, layer: FilamentsLayer, path: Path.Save):
         """Save a Shapes layer as a directory of CSV files."""
         import datetime
         import json
 
         import magicclass as mcls
-        import napari
         import pandas as pd
 
         from . import __version__
 
         path = Path(path)
         path.mkdir(exist_ok=True)
         labels = self.parent_viewer.dims.axis_labels
         roi_id = layer.features[ROI_ID]
 
+        ndigits = max(len(str(layer.nshapes)), 2)
         # save filaments
         for idx in range(layer.nshapes):
             data: np.ndarray = layer.data[idx]
             ndim = data.shape[1]
             df = pd.DataFrame(data, columns=list(labels[-ndim:]))
             df.to_csv(
-                path / f"Filament-{roi_id[idx]}.csv",
+                path / f"Filament-{roi_id[idx]:0>{ndigits}}.csv",
                 index=False,
                 float_format="%.3f",
             )
 
         # save other info
         info = {
             "versions": {
@@ -476,327 +284,350 @@
             "date": datetime.datetime.now().isoformat(sep=" "),
             "images": _get_image_sources(layer),
         }
         with open(path / "info.json", "w") as f:
             json.dump(info, f, indent=2)
         return None
 
-    def _update_paths(
-        self, idx: int, spl: Spline, current_slice: Tuple[int, ...] = ()
-    ):
-        if idx < 0:
-            idx += self.target_filaments.nshapes
-        if spl.length() > 1000:
-            raise ValueError("Spline is too long.")
-        sampled = spl.sample(interval=1.0)
-        if current_slice:
-            sl = np.stack([np.array(current_slice)] * sampled.shape[0], axis=0)
-            sampled = np.concatenate([sl, sampled], axis=1)
-
-        hist = self.target_filaments.data[idx]
-        self._replace_data(idx, sampled)
-        self._last_data = (idx, hist)
-
-    def _fit_i_2d(self, width, img, coords) -> Spline:
-        spl = Spline.fit(coords, degree=1, err=0.0)
-        length = spl.length()
-        interv = min(8.0, length / 4)
-        rough = spl.fit_filament(
-            img, width=width, interval=interv, spline_error=0.0
-        )
-        return rough.fit_filament(img, width=7, spline_error=3e-2)
-
     @Tabs.Spline.Both.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "fit.png")
+    @set_design(**ICON_KW, icon=ICON_DIR / "fit.png")
     @bind_key("F1")
     def fit_filament(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
-        width: Bound[Tools.Parameters.lattice_width] = 9,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        width: Annotated[float, {"bind": Tools.Parameters.lattice_width}] = 9,
     ):
         """Fit current spline to the image."""
-        if not isinstance(image, Image):
-            raise TypeError("'image' must be a Image layer.")
-        self.target_filaments._finish_drawing()
-        indices = _arrange_selection(idx)
-        for i in indices:
-            data: np.ndarray = self.target_filaments.data[i]
-            current_slice, data = _split_slice_and_path(data)
-            fit = self._fit_i_2d(width, image.data[current_slice], data)
-            self._update_paths(i, fit, current_slice)
-
-    def _get_slice_and_spline(
-        self, idx: int
-    ) -> Tuple[Tuple[int, ...], Spline]:
-        data: np.ndarray = self.target_filaments.data[idx]
+        image, filaments = self._check_layers(image, filaments)
+        filaments._finish_drawing()
+        i = _assert_single_selection(idx)
+        data: np.ndarray = filaments.data[i]
         current_slice, data = _split_slice_and_path(data)
-        if data.shape[0] < 4:
-            data = Spline.fit(data, degree=1, err=0).sample(interval=1.0)
-        spl = Spline.fit(data, err=0.0)
-        return current_slice, spl
+        fit = self._fit_i_2d(width, image.data[current_slice], data)
+        return self._update_paths(i, fit, filaments, current_slice)
 
-    @Tabs.Spline.Both.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "undo.png")
-    def undo_spline(self):
-        """Undo the last spline fit."""
-        if self._last_data is None:
-            return
-        self._replace_data(*self._last_data)
-
-    def _replace_data(self, idx: int, new_data: np.ndarray):
-        """Replace the idx-th data to the new one."""
-        data = self.target_filaments.data
-        data[idx] = new_data
-        self.target_filaments.data = data
-        self._last_data = None
-        self.filament = idx
+    @Tabs.Spline.Both.VBox.wraps
+    @set_design(**SMALL_ICON_KW, icon=ICON_DIR / "undo.png")
+    @bind_key("Ctrl+Z")
+    @do_not_record(recursive=False)
+    def undo(self):
+        """Undo the last operation."""
+        return self.macro.undo()
+
+    @Tabs.Spline.Both.VBox.wraps
+    @set_design(**SMALL_ICON_KW, icon=ICON_DIR / "redo.png")
+    @bind_key("Ctrl+Y")
+    @do_not_record(recursive=False)
+    def redo(self):
+        """Redo the last spline fit."""
+        return self.macro.redo()
 
     @Tabs.Spline.Left.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "ext_l.png")
+    @set_design(**ICON_KW, icon=ICON_DIR / "ext_l.png")
     def extend_left(
-        self, idx: Bound[_get_idx] = -1, dx: Bound[Tools.Parameters.dx] = 5.0
+        self,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        dx: Annotated[float, {"bind": Tools.Parameters.dx}] = 5.0,
     ):
         """Extend spline at the starting edge."""
+        _, filaments = self._check_layers(None, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         out = spl.extend_left(dx)
-        self._update_paths(idx, out, current_slice)
+        return self._update_paths(idx, out, filaments, current_slice)
 
     @Tabs.Spline.Right.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "ext_r.png")
+    @set_design(**ICON_KW, icon=ICON_DIR / "ext_r.png")
     def extend_right(
-        self, idx: Bound[_get_idx] = -1, dx: Bound[Tools.Parameters.dx] = 5.0
+        self,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        dx: Annotated[float, {"bind": Tools.Parameters.dx}] = 5.0,
     ):
         """Extend spline at the ending edge."""
+        _, filaments = self._check_layers(None, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         out = spl.extend_right(dx)
-        self._update_paths(idx, out, current_slice)
+        return self._update_paths(idx, out, filaments, current_slice)
 
     @Tabs.Spline.Left.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "extfit_l.png")
+    @set_design(**ICON_KW, icon=ICON_DIR / "extfit_l.png")
     def extend_and_fit_left(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
-        dx: Bound[Tools.Parameters.dx] = 5.0,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        dx: Annotated[float, {"bind": Tools.Parameters.dx}] = 5.0,
     ):
         """Extend spline and fit to the filament at the starting edge."""
+        image, filaments = self._check_layers(image, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         fit = spl.extend_filament_left(
             image.data[current_slice], dx, width=11, spline_error=3e-2
         )
-        self._update_paths(idx, fit, current_slice)
+        return self._update_paths(idx, fit, filaments, current_slice)
 
     @Tabs.Spline.Right.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "extfit_r.png")
+    @set_design(**ICON_KW, icon=ICON_DIR / "extfit_r.png")
     def extend_and_fit_right(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
-        dx: Bound[Tools.Parameters.dx] = 5.0,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        dx: Annotated[float, {"bind": Tools.Parameters.dx}] = 5.0,
     ):
         """Extend spline and fit to the filament at the ending edge."""
+        image, filaments = self._check_layers(image, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         fit = spl.extend_filament_right(
             image.data[current_slice], dx, width=11, spline_error=3e-2
         )
-        self._update_paths(idx, fit, current_slice)
+        return self._update_paths(idx, fit, filaments, current_slice)
 
     @Tabs.Spline.Left.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "clip_l.png")
-    def clip_left(
-        self, idx: Bound[_get_idx] = -1, dx: Bound[Tools.Parameters.dx] = 5.0
+    @set_design(**ICON_KW, icon=ICON_DIR / "clip_l.png")
+    def truncate_left(
+        self,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        dx: Annotated[float, {"bind": Tools.Parameters.dx}] = 5.0,
     ):
-        """Clip spline at the starting edge."""
+        """Truncate spline by constant lenght at the starting edge."""
+        _, filaments = self._check_layers(None, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         start = dx / spl.length()
         fit = spl.clip(start, 1.0)
-        self._update_paths(idx, fit, current_slice)
+        return self._update_paths(idx, fit, filaments, current_slice)
 
     @Tabs.Spline.Right.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "clip_r.png")
-    def clip_right(
-        self, idx: Bound[_get_idx] = -1, dx: Bound[Tools.Parameters.dx] = 5.0
+    @set_design(**ICON_KW, icon=ICON_DIR / "clip_r.png")
+    def truncate_right(
+        self,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        dx: Annotated[float, {"bind": Tools.Parameters.dx}] = 5.0,
     ):
-        """Clip spline at the ending edge."""
+        """Truncate spline by constant lenght at the ending edge."""
+        _, filaments = self._check_layers(None, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         stop = 1.0 - dx / spl.length()
         fit = spl.clip(0.0, stop)
-        self._update_paths(idx, fit, current_slice)
+        return self._update_paths(idx, fit, filaments, current_slice)
 
     @Tabs.Spline.Left.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "erf_l.png")
-    def clip_left_at_inflection(
+    @set_design(**ICON_KW, icon=ICON_DIR / "erf_l.png")
+    def truncate_left_at_inflection(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
     ):
-        """Clip spline at the inflection point at starting edge."""
+        """Truncate spline at the inflection point at starting edge."""
+        image, filaments = self._check_layers(image, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         fit = spl.clip_at_inflection_left(
             image.data[current_slice],
             callback=self._show_fitting_result,
         )
-        self._update_paths(idx, fit, current_slice)
+        return self._update_paths(idx, fit, filaments, current_slice)
 
     @Tabs.Spline.Right.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "erf_r.png")
-    def clip_right_at_inflection(
+    @set_design(**ICON_KW, icon=ICON_DIR / "erf_r.png")
+    def truncate_right_at_inflection(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
     ):
-        """Clip spline at the inflection point at ending edge."""
+        """Truncate spline at the inflection point at ending edge."""
+        image, filaments = self._check_layers(image, filaments)
         idx = _assert_single_selection(idx)
-        current_slice, spl = self._get_slice_and_spline(idx)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
         fit = spl.clip_at_inflection_right(
             image.data[current_slice],
             callback=self._show_fitting_result,
         )
-        self._update_paths(idx, fit, current_slice)
+        return self._update_paths(idx, fit, filaments, current_slice)
 
     @Tabs.Spline.Both.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "erf2.png")
-    @bind_key("F2")
-    def clip_at_inflections(
+    @set_design(**ICON_KW, icon=ICON_DIR / "erf2.png")
+    def truncate_at_inflections(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
     ):
-        """Clip spline at the inflection points at both ends."""
+        """Truncate spline at the inflection points at both ends."""
+        image, filaments = self._check_layers(image, filaments)
         indices = _arrange_selection(idx)
         for i in indices:
-            current_slice, spl = self._get_slice_and_spline(i)
+            current_slice, spl = self._get_slice_and_spline(i, filaments)
             out = spl.clip_at_inflections(
                 image.data[current_slice],
                 callback=self._show_fitting_result,
             )
-            self._update_paths(i, out, current_slice)
-
-    def _show_fitting_result(self, opt: _opt.Optimizer, prof: np.ndarray):
-        """Callback function for error function fitting"""
-        sg_min, sg_max = self.Tools.Parameters.sigma_range
-        if isinstance(opt, (_opt.GaussianOptimizer, _opt.ErfOptimizer)):
-            valid = sg_min <= opt.params.sg <= sg_max
-        elif isinstance(opt, _opt.TwosideErfOptimizer):
-            valid0 = sg_min <= opt.params.sg0 <= sg_max
-            valid1 = sg_min <= opt.params.sg1 <= sg_max
-            valid = valid0 and valid1
-        else:
-            raise NotImplementedError
-        ndata = prof.size
-        xdata = np.arange(ndata)
-        ydata = opt.sample(xdata)
-        self.Output._plot(xdata, prof, color="gray", alpha=0.7, lw=1)
-        self.Output._plot(xdata, ydata, clear=False, color="red", lw=2)
-        if not valid:
-            self.Output.plt.text(
-                0, np.min(ydata), "Sigma out of range.", color="crimson"
-            )
-        self.Output._set_labels("Data points", "Intensity")
+            self._update_paths(i, out, filaments, current_slice)
+        return None
 
     @Tabs.Measure.wraps
     def measure_properties(
         self,
-        image: Bound[target_image],
-        properties: SomeOf[Measurement.PROPERTIES] = ("length", "mean"),
-        slices: bool = False,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+        properties: Annotated[
+            list[str],
+            {"choices": Measurement.PROPERTIES, "widget_type": "Select"},
+        ] = ("length", "mean"),
+        slices: Annotated[bool, {"label": "Record slice numbers"}] = False,
     ):
         """Measure properties of all the splines."""
         import pandas as pd
 
+        image, filaments = self._check_layers(image, filaments)
         if slices:
             # Record slice numbers in columns such as "index_T"
             ndim = len(image.data.shape)
             labels = self.parent_viewer.dims.axis_labels[-ndim:-2]
             sl_data = {f"index_{lname}": [] for lname in labels}
         else:
             sl_data = {}
         data = {p: [] for p in properties}
 
         image_data = image.data
-        for idx in range(self.target_filaments.nshapes):
-            sl, spl = self._get_slice_and_spline(idx)
+        for idx in range(filaments.nshapes):
+            sl, spl = self._get_slice_and_spline(idx, filaments)
             measure = Measurement(spl, image_data[sl])
             for v, s0 in zip(sl_data.values(), sl):
                 v.append(s0)
             for k, v in data.items():
                 v.append(getattr(measure, k)())
 
         sl_data.update(data)
         tstack = self._tablestack
-        tstack.add_table(sl_data, name=self.target_filaments.name)
+        tstack.add_table(sl_data, name=filaments.name)
         tstack.show()
+
+        # NOTE: Updating features are not safe. If user added new filaments
+        # after measuring, new filaments will initialized with duplicated
+        # features.
+        # feat = filaments.features
+        # filaments.features = feat.assign(**sl_data)
+        # defaults = filaments.current_properties
+        # for key in defaults.keys():
+        #     if key in Measurement.PROPERTIES:
+        #         defaults[key] = [np.nan]
+        # filaments.current_properties = defaults
+
         return pd.DataFrame(sl_data)
 
     @Tabs.Measure.wraps
     def plot_curvature(
         self,
-        idx: Bound[_get_idx] = -1,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
     ):
         """Plot curvature of filament."""
-        _, spl = self._get_slice_and_spline(idx)
+        _, filaments = self._check_layers(None, filaments)
+        _, spl = self._get_slice_and_spline(idx, filaments)
         length = spl.length()
         x = np.linspace(0, 1, int(spl.length()))
         cv = spl.curvature(x)
         self.Output._plot(x * length, cv)
         self.Output._set_labels("Position (px)", "Curvature")
+        return None
 
     @Tabs.Measure.wraps
     def plot_profile(
         self,
-        image: Bound[target_image],
-        idx: Bound[_get_idx] = -1,
+        idx: Annotated[int, {"bind": _get_idx}] = -1,
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
     ):
-        """Plot intensity profile."""
-        current_slice, spl = self._get_slice_and_spline(idx)
-        prof = spl.get_profile(image.data[current_slice])
-        length = spl.length()
-        x = np.linspace(0, 1, int(length)) * length
-        self.Output._plot(x, prof)
+        """Plot intensity profile using the selected image layer and the filament."""
+        image, filaments = self._check_layers(image, filaments)
+        x, prof = self.get_profile(idx, image, filaments)
+        self.Output._plot(x, prof, color=_cmap_to_color(image))
         self.Output._set_labels("Position (px)", "Intensity")
+        return None
 
     def _get_axes(self, w=None):
         return self.parent_viewer.dims.axis_labels[:-2]
 
     @Tabs.Measure.wraps
     def kymograph(
         self,
-        image: Bound[target_image],
-        time_axis: OneOf[_get_axes],
-        idx: Bound[_get_idx] = -1,
+        idx: Annotated[int, {"bind": _get_idx}],
+        time_axis: Annotated[str, {"bind": _get_axes}],
+        image: Annotated[Image, {"bind": target_image}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
     ):
-        """Plot kymograph."""
-        current_slice, spl = self._get_slice_and_spline(idx)
+        """Plot kymograph using the selected image layer and the filament."""
+        image, filaments = self._check_layers(image, filaments)
+        sl, spl = self._get_slice_and_spline(idx, filaments)
+        if time_axis is None:
+            if image.ndim < 3:
+                raise ValueError("Cannot build a kymograph with a 2D image.")
+            t0 = image.metadata[IMAGE_AXES][0]
         if isinstance(time_axis, str):
             t0 = image.metadata[IMAGE_AXES].index(time_axis)
         else:
             t0 = time_axis
         ntime = image.data.shape[t0]
-        profiles: List[np.ndarray] = []
+        profiles: "list[np.ndarray]" = []
         for t in range(ntime):
             t1 = t0 + 1
-            sl = current_slice[:t0] + (t,) + current_slice[t1:]
+            sl = sl[:t0] + (t,) + sl[t1:]
             prof = spl.get_profile(image.data[sl])
             profiles.append(prof)
         kymo = np.stack(profiles, axis=0)
         plt = Figure()
-        plt.imshow(kymo, cmap="gray")
-        plt.show()
+        plt.imshow(kymo, cmap=_cmap_to_mpl_cmap(image))
+        self.parent_viewer.window.add_dock_widget(plt, name="kymograph")
+        return None
 
     @Tools.Layers.wraps
     @set_options(wlayers={"layout": "vertical", "label": "weight x layer"})
-    def create_total_intensity(self, wlayers: List[Tuple[weight, Image]]):
+    def create_total_intensity(self, wlayers: list[tuple[weight, Image]]):
         """Create a total intensity layer from multiple images."""
         weights = [t[0] for t in wlayers]
         imgs = [t[1].data for t in wlayers]
         names = [t[1].name for t in wlayers]
         tot = sum(w * img for w, img in zip(weights, imgs))
 
         outs = set()
@@ -811,27 +642,28 @@
 
         tot_layer = self.parent_viewer.add_image(
             tot, name=new_name, visible=False
         )
 
         # update target images
         for layer in self.parent_viewer.layers:
-            if not isinstance(layer, Shapes):
+            if not isinstance(layer, FilamentsLayer):
                 continue
             # if all the input images belongs to the same shapes layer, update
             # the target image list.
             img_layers = _get_connected_target_image_layers(layer)
             target_names = [target.name for target in img_layers]
             if all(img_name in target_names for img_name in names):
                 img_layers.append(tot_layer)
+        return None
 
     # TODO: how to save at subpixel resolution?
     # @Tools.Layers.wraps
     # @set_options(path={"mode": "w", "filter": ".zip"})
-    # def export_roi(self, layer: Shapes, path: Path):
+    # def export_roi(self, layer: FilamentsLayer, path: Path):
     #     """Export filament layer as a ImageJ ROI.zip file."""
     #
     #     from roifile import roiwrite, ImagejRoi, ROI_TYPE, ROI_OPTIONS
     #     roilist: List[ImagejRoi] = []
     #     multi_labels = self.parent_viewer.dims.axis_labels[:-2]
     #     roi_id = layer.features[ROI_ID]
     #     for i, data in enumerate(layer.data):
@@ -858,93 +690,396 @@
     #             **dim_kwargs,
     #             **edge_kwargs,
     #         )
     #         roilist.append(roi)
     #     roiwrite(path, roilist)
 
     @Tabs.Spline.Both.wraps
-    @set_design(**ICON_KWARGS, icon=ICON_DIR / "del.png")
-    def delete_current(self, idx: Bound[_get_idx]):
+    @set_design(**ICON_KW, icon=ICON_DIR / "del.png")
+    def delete_filament(
+        self,
+        idx: Annotated[int, {"bind": _get_idx}] = None,
+        filaments: Annotated[
+            FilamentsLayer, {"bind": target_filaments}
+        ] = None,
+    ):
         """Delete selected (or the last) path."""
+        _, filaments = self._check_layers(None, filaments)
+        if idx is None:
+            idx = {self.filament}
         if isinstance(idx, int):
             idx = {idx}
-        self.target_filaments.selected_data = idx
-        self.target_filaments.remove_selected()
-        if len(idx) == 1 and self.target_filaments.nshapes > 0:
-            self.filament = min(
-                list(idx)[0], len(self.target_filaments.data) - 1
+        # keep current state for undoing
+        data_info = {
+            i: (
+                filaments.data[i],
+                filaments.features.iloc[i : i + 1, :],
+                filaments.edge_color[i],
             )
-            self.target_filaments.selected_data = {self.filament}
+            for i in idx
+        }
+
+        # select and remove
+        filaments.selected_data = idx
+        filaments.remove_selected()
+        if len(idx) == 1 and filaments.nshapes > 0:
+            self.filament = min(list(idx)[0], len(filaments.data) - 1)
+            filaments.selected_data = {self.filament}
+
+        @undo_callback
+        def _undo():
+            shapes = filaments.data
+            cur_feat = filaments.features
+            cur_ec = filaments.edge_color
+            for i, (d, feat, ec) in sorted(
+                data_info.items(), key=lambda x: x[0], reverse=True
+            ):
+                shapes.insert(i, d)
+                np.insert(cur_ec, i, ec, axis=0)
+                cur_feat = pd.concat(
+                    [cur_feat.iloc[:i], feat, cur_feat.iloc[i:]],
+                    axis=1,
+                    ignore_index=True,
+                )
+
+            filaments.data = shapes
+            filaments._relabel()
+
+        return _undo
 
     @Tools.Others.wraps
     @do_not_record
+    @bind_key("Ctrl+Shift+M")
     def create_macro(self):
         """Create an executable Python script."""
         import macrokit as mk
 
         new = self.macro.widget.duplicate()
         v = mk.Expr("getattr", [mk.symbol(self), "parent_viewer"])
-        new.value = self.macro.format([(mk.symbol(self.parent_viewer), v)])
+        new.textedit.value = self.macro.format(
+            [(mk.symbol(self.parent_viewer), v)]
+        )
         new.show()
         return None
 
     @Tools.Others.wraps
     @do_not_record
+    def show_macro(self):
+        """Show the macro widget."""
+        self.macro.widget.show()
+        return None
+
+    @Tools.Others.wraps
+    @do_not_record
     def send_widget_to_viewer(self):
-        self.parent_viewer.update_console({"ui": self})
+        """Add this widget to the viewer console as identifier 'ui'."""
+        return self.parent_viewer.update_console({"ui": self})
+
+    @nogui
+    def add_filament_data(
+        self, data: np.ndarray, layer: "FilamentsLayer | None" = None
+    ):
+        data = np.asarray(data)
+        _, layer = self._check_layers(None, layer)
+        with layer.data_added.blocked():
+            layer.add_paths(data)
+
+        @undo_callback
+        def _undo():
+            layer.data = layer.data[:-1]
+
+        @_undo.with_redo
+        def _undo():
+            with layer.data_added.blocked():
+                layer.add_paths(data)
+
+        return _undo
 
     @nogui
     @do_not_record
-    def get_spline(self, idx: int) -> Spline:
-        _, spl = self._get_slice_and_spline(idx)
+    def get_spline(
+        self, idx: int, filaments: "FilamentsLayer | None" = None
+    ) -> Spline:
+        """Get the idx-th spline object."""
+        _, filaments = self._check_layers(None, filaments)
+        _, spl = self._get_slice_and_spline(idx, filaments)
         return spl
 
+    @nogui
+    @do_not_record
+    def get_profile(
+        self,
+        idx: int = -1,
+        image: "Image | None" = None,
+        filaments: "FilamentsLayer | None" = None,
+    ) -> tuple[NDArray[np.float32], NDArray[np.float32]]:
+        """Get intensity profile using the selected image layer and the filament."""
+        image, filaments = self._check_layers(image, filaments)
+        current_slice, spl = self._get_slice_and_spline(idx, filaments)
+        prof = spl.get_profile(image.data[current_slice])
+        length = spl.length()
+        x = np.linspace(0, 1, int(length), dtype=np.float32) * length
+        return x, prof
+
+    def _show_fitting_result(self, opt: _opt.Optimizer, prof: np.ndarray):
+        """Callback function for error function fitting"""
+        sg_min, sg_max = self.Tools.Parameters.sigma_range
+        if isinstance(opt, (_opt.GaussianOptimizer, _opt.ErfOptimizer)):
+            valid = sg_min <= opt.params.sg <= sg_max
+        elif isinstance(opt, _opt.TwosideErfOptimizer):
+            valid0 = sg_min <= opt.params.sg0 <= sg_max
+            valid1 = sg_min <= opt.params.sg1 <= sg_max
+            valid = valid0 and valid1
+        else:
+            raise NotImplementedError
+        ndata = prof.size
+        xdata = np.arange(ndata)
+        ydata = opt.sample(xdata)
+        self.Output._plot(xdata, prof, color="gray", alpha=0.7, lw=1)
+        self.Output._plot(xdata, ydata, clear=False, color="red", lw=2)
+        if not valid:
+            self.Output.plt.text(
+                0, np.min(ydata), "Sigma out of range.", color="crimson"
+            )
+        return self.Output._set_labels("Data points", "Intensity")
+
+    def _replace_data(
+        self, idx: int, new_data: np.ndarray, filaments: FilamentsLayer
+    ):
+        """Replace the idx-th data to the new one."""
+        data = filaments.data
+        data[idx] = new_data
+        filaments.data = data
+        self.filament = idx
+        return None
+
+    def _update_paths(
+        self,
+        idx: int,
+        spl: Spline,
+        filaments: FilamentsLayer,
+        current_slice: tuple[int, ...] = (),
+    ):
+        """
+        Update the filament path shape at `idx`-th index of `filaments` layer to the spline
+        `spl`. If the layer is >3D, `current_slice` will be the slice index of the 2D image.
+        """
+        if idx < 0:
+            idx += filaments.nshapes
+        if spl.length() > 1000:
+            raise ValueError("Spline is too long.")
+        sampled = spl.sample(interval=1.0)
+        if current_slice:
+            sl = np.stack([np.array(current_slice)] * sampled.shape[0], axis=0)
+            sampled = np.concatenate([sl, sampled], axis=1)
+
+        old_data = filaments.data[idx]
+        self._replace_data(idx, sampled, filaments)
+
+        @undo_callback
+        def _out():
+            self._replace_data(idx, old_data, filaments)
+
+        @_out.with_redo
+        def _out():
+            self._replace_data(idx, sampled, filaments)
+            filaments.selected_data = {}
+            filaments.refresh()
+
+        return _out
+
+    def _fit_i_2d(
+        self, width: float, img: np.ndarray, coords: np.ndarray
+    ) -> Spline:
+        spl = Spline.fit(coords, degree=1, err=0.0)
+        length = spl.length()
+        interv = min(8.0, length / 4)
+        rough = spl.fit_filament(
+            img, width=width, interval=interv, spline_error=0.0
+        )
+        return rough.fit_filament(img, width=7, spline_error=3e-2)
+
+    def _load_filament_coordinates(self, data: "list[np.ndarray]", name: str):
+        ndata = len(data)
+        layer = FilamentsLayer(
+            data,
+            edge_color=self._color_default,
+            name=name,
+            shape_type="path",
+            edge_width=0.5,
+            properties={ROI_ID: np.arange(ndata, dtype=np.uint32)},
+            text=dict(string=ROI_FMT, color="white", size=8),
+        )
+        self.parent_viewer.add_layer(layer)
+
+        self._set_filament_layer(layer)
+        layer.current_properties = {ROI_ID: ndata}
+        self.target_filaments.metadata[TARGET_IMG_LAYERS] = list(
+            filter(lambda x: isinstance(x, Image), self.parent_viewer.layers)
+        )
+        return None
+
+    def _filter_image_choices(self):
+        if not self.Tools.Parameters.target_image_filter:
+            return
+        target_image_widget: ComboBox = self["target_image"]
+        if target_image_widget.value is None:
+            return
+        cbox_idx = target_image_widget.choices.index(target_image_widget.value)
+        img_layers = _get_connected_target_image_layers(self.target_filaments)
+        if len(img_layers) > 0:
+            target_image_widget.choices = img_layers
+            cbox_idx = min(cbox_idx, len(img_layers) - 1)
+            target_image_widget.value = target_image_widget.choices[cbox_idx]
+        return None
+
+    def _add_image(self, img: np.ndarray, axes: str, path: Path):
+        if "C" in axes:
+            ic = axes.find("C")
+            nchn = img.shape[ic]
+            axis_labels: "tuple[str, ...]" = tuple(c for c in axes if c != "C")
+            img_layers: "list[Image]" = self.parent_viewer.add_image(
+                img,
+                channel_axis=ic,
+                name=[f"[C{i}] {path.stem}" for i in range(nchn)],
+                metadata={IMAGE_AXES: axis_labels, SOURCE: path},
+            )
+        else:
+            axis_labels = tuple(axes)
+            _layer = self.parent_viewer.add_image(
+                img,
+                name=path.stem,
+                metadata={IMAGE_AXES: axis_labels, SOURCE: path},
+            )
+            img_layers = [_layer]
+
+        self._add_filament_layer(img_layers, path.stem)
+        ndim = self.parent_viewer.dims.ndim
+        if ndim == len(axis_labels):
+            self.parent_viewer.dims.set_axis_label(
+                list(range(ndim)), axis_labels
+            )
+        self._on_target_filament_change()  # initialize
+        return None
+
+    def _on_data_added(self):
+        self["filament"].reset_choices()
+        if self.target_filaments.nshapes > 0:
+            self.filament = self.target_filaments.nshapes - 1
+            self.target_filaments.selected_data = {}
+            self.target_filaments.refresh()
+
+    def _on_data_removed(self):
+        self["filament"].reset_choices()
+        self._on_filament_change(self.filament)
+
+    def _on_data_draw_finished(self, layer: FilamentsLayer):
+        with layer.draw_finished.blocked():
+            added_data = np.round(layer.data[-1], 2)
+            layer.data = layer.data[:-1]
+            self.add_filament_data(added_data, layer=layer)
+            if layer.nshapes > 0:
+                self._on_filament_change(layer.nshapes - 1)
+        self["filament"].reset_choices()
+
+    def _set_filament_layer(self, layer: FilamentsLayer):
+        layer.data_added.connect(self._on_data_added)
+        layer.data_removed.connect(self._on_data_removed)
+        layer.draw_finished.connect(self._on_data_draw_finished)
+        layer.mode = "add_path"
+        self.target_filaments = layer
+        return layer
+
+    def _add_filament_layer(self, images: "list[Image]", name: str):
+        """Add a Filaments layer for the target image."""
+        # check input images
+        ndim: int = _get_unique_value(img.ndim for img in images)
+        axes: "tuple[str]" = _get_unique_value(
+            img.metadata[IMAGE_AXES] for img in images
+        )
+        layer = FilamentsLayer(
+            ndim=ndim,
+            edge_color=self._color_default,
+            name=f"[F] {name}",
+            metadata={IMAGE_AXES: axes, TARGET_IMG_LAYERS: images},
+            edge_width=0.5,
+            properties={ROI_ID: 0},
+            text=dict(string=ROI_FMT, color="white", size=8),
+        )
+        self.parent_viewer.add_layer(layer)
+        return self._set_filament_layer(layer)
+
+    def _get_slice_and_spline(
+        self, idx: int, filaments: FilamentsLayer
+    ) -> "tuple[tuple[int, ...], Spline]":
+        data: np.ndarray = filaments.data[idx]
+        current_slice, data = _split_slice_and_path(data)
+        if data.shape[0] < 4:
+            data = Spline.fit(data, degree=1, err=0).sample(interval=1.0)
+        spl = Spline.fit(data, err=0.0)
+        return current_slice, spl
+
+    def _check_layers(
+        self, image: "Image | None", filaments: "FilamentsLayer | None"
+    ):
+        if image is None:
+            image = self.target_image
+        if filaments is None:
+            filaments = self.target_filaments
+        if not isinstance(image, Image):
+            raise TypeError(f"Invalid image type: {type(image)}")
+        if not isinstance(filaments, FilamentsLayer):
+            raise TypeError(f"Invalid filament type: {type(filaments)}")
+        return image, filaments
+
 
 def _split_slice_and_path(
     data: np.ndarray,
-) -> Tuple[Tuple[int, ...], np.ndarray]:
+) -> "tuple[tuple[int, ...], np.ndarray]":
     if data.shape[1] == 2:
         return (), data
     sl: np.ndarray = np.unique(data[:, :-2], axis=0)
     if sl.shape[0] != 1:
         raise ValueError("Spline is not in 2D")
     return tuple(sl.ravel().astype(np.int64)), data[:, -2:]
 
 
-def _get_connected_target_image_layers(shapes: Shapes) -> List[Image]:
+def _get_connected_target_image_layers(
+    shapes: FilamentsLayer,
+) -> "list[Image]":
     """Return all connected target image layers."""
     return shapes.metadata.get(TARGET_IMG_LAYERS, [])
 
 
-def _toggle_target_images(shapes: Shapes, visible: bool):
+def _toggle_target_images(shapes: FilamentsLayer, visible: bool):
     """Set target images to visible or invisible."""
     img_layers = _get_connected_target_image_layers(shapes)
     for img_layer in img_layers:
         if img_layer.name.startswith("[Total]"):
             continue
         img_layer.visible = visible
     shapes.visible = visible
 
 
-def _assert_single_selection(idx: Union[int, Set[int]]) -> int:
+def _assert_single_selection(idx: "int | set[int]") -> int:
     if isinstance(idx, set):
         if len(idx) != 1:
             raise ValueError("Multiple selection")
-        return idx.pop()
+        return next(iter(idx))
     return idx
 
 
-def _arrange_selection(idx: Union[int, Set[int]]) -> List[int]:
+def _arrange_selection(idx: "int | set[int]") -> "list[int]":
     if isinstance(idx, int):
         return [idx]
     else:
         return sorted(list(idx), reverse=True)
 
 
-def _get_image_sources(shapes: Shapes) -> Union[List[str], None]:
+def _get_image_sources(shapes: FilamentsLayer) -> "list[str] | None":
     """Extract image sources from a shapes layer."""
     img_layers = _get_connected_target_image_layers(shapes)
     if not img_layers:
         return None
     sources = []
     for img in img_layers:
         source = img.metadata.get(SOURCE) or img.source.path
@@ -959,7 +1094,21 @@
 
 
 def _get_unique_value(vals: Iterable[_V]) -> _V:
     s = set(vals)
     if len(s) != 1:
         raise ValueError(f"Not a unique value: {s}")
     return next(iter(s))
+
+
+def _cmap_to_color(image: Image) -> np.ndarray:
+    """Convert colormap to color."""
+    cmap = image.colormap
+    return cmap.map(1)
+
+
+def _cmap_to_mpl_cmap(image: Image, name="no-name"):
+    """Convert colormap to matplotlib colormap."""
+    from matplotlib.colors import LinearSegmentedColormap
+
+    cmap = image.colormap
+    return LinearSegmentedColormap.from_list("custom", cmap.colors)
```

### Comparing `napari_filaments-0.2.1/src/napari_filaments.egg-info/PKG-INFO` & `napari_filaments-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
-Name: napari-filaments
-Version: 0.2.1
+Name: napari_filaments
+Version: 0.3.0
 Summary: A napari plugin for filament analysis
 Home-page: https://github.com/hanjinliu/napari-filaments
 Author: Hanjin Liu
 Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hanjinliu/napari-filaments/issues
 Project-URL: Documentation, https://github.com/hanjinliu/napari-filaments#README.md
 Project-URL: Source Code, https://github.com/hanjinliu/napari-filaments
 Project-URL: User Support, https://github.com/hanjinliu/napari-filaments/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: napari
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # napari-filaments
 
 [![License BSD-3](https://img.shields.io/pypi/l/napari-filaments.svg?color=green)](https://github.com/hanjinliu/napari-filaments/raw/main/LICENSE)
@@ -52,22 +48,32 @@
 - Import paths from ImageJ ROI file.
 
 Basic Usage
 -----------
 
 Click `Layers > open image` to open a tif file. You'll find the image you chose and a shapes layer are added to the layer list.
 
-![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig.png)
+![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig-1.png)
 
 - The "target filaments" box shows the working shapes layer.
 - The "target image" box shows the image layer on which fitting and quantification will be conducted.
 - The "filament" box shows currently selected shape (initially this box is empty).
 
 Add path shapes and push key `F1` to fit the shape to the filament in the target image layer.
 
+- In the "Spline" tab, you can cut/extend or re-fit splines.
+- In the "Measure" tab, click "measure property" to measure mean instensity etc along each spline.
+
+How it works
+------------
+
+Spline fitting is done as following.
+
+![](https://github.com/hanjinliu/napari-filaments/raw/main/resources/fig-2.png)
+
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 
 ## Installation
@@ -110,9 +116,7 @@
 
 [file an issue]: https://github.com/hanjinliu/napari-filaments/issues
 
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
-
-
```

