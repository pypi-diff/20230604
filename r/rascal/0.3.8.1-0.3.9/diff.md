# Comparing `tmp/rascal-0.3.8.1.tar.gz` & `tmp/rascal-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rascal-0.3.8.1.tar", last modified: Tue Nov 29 15:43:27 2022, max compression
+gzip compressed data, was "rascal-0.3.9.tar", last modified: Thu Jan 12 00:26:53 2023, max compression
```

## Comparing `rascal-0.3.8.1.tar` & `rascal-0.3.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:43:27.603367 rascal-0.3.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1540 2022-11-29 15:42:21.000000 rascal-0.3.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-29 15:42:21.000000 rascal-0.3.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2022-11-29 15:43:27.603367 rascal-0.3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4054 2022-11-29 15:42:21.000000 rascal-0.3.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      115 2022-11-29 15:42:22.000000 rascal-0.3.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1357 2022-11-29 15:43:27.603367 rascal-0.3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       86 2022-11-29 15:42:22.000000 rascal-0.3.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:43:27.583367 rascal-0.3.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:43:27.587367 rascal-0.3.8.1/src/rascal/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:43:27.595367 rascal-0.3.8.1/src/rascal/arc_lines/
--rw-r--r--   0 runner    (1001) docker     (122)   660892 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/all_nist.csv
--rw-r--r--   0 runner    (1001) docker     (122)     4790 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/ar.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1921 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/convolve_lines.py
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/cu.csv
--rw-r--r--   0 runner    (1001) docker     (122)      991 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/cuar.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1411 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/cuar_unknown.csv
--rw-r--r--   0 runner    (1001) docker     (122)    13027 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/cunear_high.csv
--rw-r--r--   0 runner    (1001) docker     (122)     3798 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/cunear_low.csv
--rw-r--r--   0 runner    (1001) docker     (122)      528 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/efosc.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1183 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/he.csv
--rw-r--r--   0 runner    (1001) docker     (122)      815 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/hg.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1655 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/kr.csv
--rw-r--r--   0 runner    (1001) docker     (122)     7012 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/ne.csv
--rw-r--r--   0 runner    (1001) docker     (122)   255601 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/nist_clean.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2004 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/xe.csv
--rw-r--r--   0 runner    (1001) docker     (122)      576 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/arc_lines/xe_strong.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12252 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/atlas.py
--rw-r--r--   0 runner    (1001) docker     (122)    74951 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11029 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/houghtransform.py
--rw-r--r--   0 runner    (1001) docker     (122)     2675 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    41207 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     4537 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (122)    14966 2022-11-29 15:42:22.000000 rascal-0.3.8.1/src/rascal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:43:27.591367 rascal-0.3.8.1/src/rascal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2022-11-29 15:43:27.000000 rascal-0.3.8.1/src/rascal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1230 2022-11-29 15:43:27.000000 rascal-0.3.8.1/src/rascal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 15:43:27.000000 rascal-0.3.8.1/src/rascal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 15:43:27.000000 rascal-0.3.8.1/src/rascal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-11-29 15:43:27.000000 rascal-0.3.8.1/src/rascal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2022-11-29 15:43:27.000000 rascal-0.3.8.1/src/rascal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 15:43:27.603367 rascal-0.3.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2284 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_arclines.py
--rw-r--r--   0 runner    (1001) docker     (122)     2268 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_effective_pixel.py
--rw-r--r--   0 runner    (1001) docker     (122)     3816 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_hough_transform.py
--rw-r--r--   0 runner    (1001) docker     (122)     6909 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_lt_sprat_manual_atlas.py
--rw-r--r--   0 runner    (1001) docker     (122)     1561 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (122)     9399 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_polynomial_fit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2649 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (122)     3465 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_synthetic_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3653 2022-11-29 15:42:22.000000 rascal-0.3.8.1/test/test_xe_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:26:53.665686 rascal-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-01-12 00:25:40.000000 rascal-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-12 00:25:40.000000 rascal-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-01-12 00:26:53.665686 rascal-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-01-12 00:25:40.000000 rascal-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-12 00:25:41.000000 rascal-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-01-12 00:26:53.665686 rascal-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-12 00:25:41.000000 rascal-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:26:53.653686 rascal-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:26:53.657686 rascal-0.3.9/src/rascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:26:53.661686 rascal-0.3.9/src/rascal/arc_lines/
+-rw-r--r--   0 runner    (1001) docker     (123)   660892 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/all_nist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/ar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/convolve_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/cu.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/cuar.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/cuar_unknown.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/cunear_high.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/cunear_low.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/efosc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/he.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/hg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/kr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/ne.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   255601 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/nist_clean.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/xe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/arc_lines/xe_strong.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75486 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/houghtransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41232 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-01-12 00:25:41.000000 rascal-0.3.9/src/rascal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:26:53.657686 rascal-0.3.9/src/rascal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-01-12 00:26:53.000000 rascal-0.3.9/src/rascal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-01-12 00:26:53.000000 rascal-0.3.9/src/rascal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 00:26:53.000000 rascal-0.3.9/src/rascal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 00:26:53.000000 rascal-0.3.9/src/rascal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-12 00:26:53.000000 rascal-0.3.9/src/rascal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-12 00:26:53.000000 rascal-0.3.9/src/rascal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 00:26:53.665686 rascal-0.3.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_arclines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_effective_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_hough_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_lt_sprat_manual_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_polynomial_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_synthetic_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-01-12 00:25:41.000000 rascal-0.3.9/test/test_xe_calibration.py
```

### Comparing `rascal-0.3.8.1/LICENSE` & `rascal-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/PKG-INFO` & `rascal-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rascal
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: The Pyhton Automated Wavelenmgth Calibrator.
 Home-page: https://rascal.readthedocs.io/en/latest/?badge=latest
 Download-URL: https://github.com/jveitchmichaelis/rascal
 Author: Josh Veitch-Michaelis, Marco C Lam
 Author-email: j.veitchmichaelis@gmail.com, lam@mail.tau.ac.il
 Maintainer: Josh Veitch-Michaelis, Marco C Lam
 Maintainer-email: j.veitchmichaelis@gmail.com, lam@mail.tau.ac.il
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -43,19 +42,20 @@
 
 You don't need to know the dispersion and start wavelength exactly. Often this information is provided by the observatory, but if you don't know it, you can take a rough guess. The closer you are to the actual system settings, the more likely it is that Rascal will be able to solve the calibration. Blind calibration, where no parameters are known, is possible but challenging currently. If you don't know the lamp, you can try iterating over the various combinations of sources. Generally when you do get a correct fit, with most astronomical instruments the errors will be extremely low.
 
 More background information can be referred to this [arXiv article](https://ui.adsabs.harvard.edu/abs/2019arXiv191205883V/abstract).
 
 
 ## Dependencies
-* python >= 3.6
-* numpy
-* scipy
-* pynverse
-* matplotlib
+* python >= 3.7
+* numpy>=1.16,<1.24
+* scipy>=1.3.3
+* pynverse>=0.1.4
+* matplotlib>=3.0.3
+* tqdm>=4.48.0
 
 ## Optional Dependencies
 * [plotly](https://github.com/plotly/plotly.py) >= 4.0
 
 ## Installation
 Instructions can be found [here](https://rascal.readthedocs.io/en/latest/installation/installation.html).
```

### Comparing `rascal-0.3.8.1/README.md` & `rascal-0.3.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 
 You don't need to know the dispersion and start wavelength exactly. Often this information is provided by the observatory, but if you don't know it, you can take a rough guess. The closer you are to the actual system settings, the more likely it is that Rascal will be able to solve the calibration. Blind calibration, where no parameters are known, is possible but challenging currently. If you don't know the lamp, you can try iterating over the various combinations of sources. Generally when you do get a correct fit, with most astronomical instruments the errors will be extremely low.
 
 More background information can be referred to this [arXiv article](https://ui.adsabs.harvard.edu/abs/2019arXiv191205883V/abstract).
 
 
 ## Dependencies
-* python >= 3.6
-* numpy
-* scipy
-* pynverse
-* matplotlib
+* python >= 3.7
+* numpy>=1.16,<1.24
+* scipy>=1.3.3
+* pynverse>=0.1.4
+* matplotlib>=3.0.3
+* tqdm>=4.48.0
 
 ## Optional Dependencies
 * [plotly](https://github.com/plotly/plotly.py) >= 4.0
 
 ## Installation
 Instructions can be found [here](https://rascal.readthedocs.io/en/latest/installation/installation.html).
```

### Comparing `rascal-0.3.8.1/setup.cfg` & `rascal-0.3.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rascal
-version = 0.3.8.1
+version = 0.3.9
 license = BSD-3-Clause
 license_files = LICENSE
 description = The Pyhton Automated Wavelenmgth Calibrator.
 long_description = file: README.md
 long_description_content_type = text/markdown
 readme = README.md
 author = Josh Veitch-Michaelis, Marco C Lam
@@ -12,15 +12,14 @@
 maintainer = Josh Veitch-Michaelis, Marco C Lam
 maintainer_email = j.veitchmichaelis@gmail.com, lam@mail.tau.ac.il
 url = https://rascal.readthedocs.io/en/latest/?badge=latest
 download_url = https://github.com/jveitchmichaelis/rascal
 classifiers = 
 	License :: OSI Approved :: BSD License
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 
@@ -28,15 +27,15 @@
 zip_safe = False
 package_dir = 
 	=src
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
-	numpy>=1.16
+	numpy>=1.16,<1.24
 	scipy>=1.3.3
 	pynverse>=0.1.4
 	matplotlib>=3.0.3
 	tqdm>=4.48.0
 setup_requires = 
 	astropy>=4.0
 	plotly>=4.0
```

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/all_nist.csv` & `rascal-0.3.9/src/rascal/arc_lines/all_nist.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/ar.csv` & `rascal-0.3.9/src/rascal/arc_lines/ar.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/convolve_lines.py` & `rascal-0.3.9/src/rascal/arc_lines/convolve_lines.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/cu.csv` & `rascal-0.3.9/src/rascal/arc_lines/cu.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/cuar.csv` & `rascal-0.3.9/src/rascal/arc_lines/cuar.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/cuar_unknown.csv` & `rascal-0.3.9/src/rascal/arc_lines/cuar_unknown.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/cunear_high.csv` & `rascal-0.3.9/src/rascal/arc_lines/cunear_high.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/cunear_low.csv` & `rascal-0.3.9/src/rascal/arc_lines/cunear_low.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/efosc.csv` & `rascal-0.3.9/src/rascal/arc_lines/efosc.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/he.csv` & `rascal-0.3.9/src/rascal/arc_lines/he.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/hg.csv` & `rascal-0.3.9/src/rascal/arc_lines/hg.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/kr.csv` & `rascal-0.3.9/src/rascal/arc_lines/kr.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/ne.csv` & `rascal-0.3.9/src/rascal/arc_lines/ne.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/nist_clean.csv` & `rascal-0.3.9/src/rascal/arc_lines/nist_clean.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/xe.csv` & `rascal-0.3.9/src/rascal/arc_lines/xe.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/arc_lines/xe_strong.csv` & `rascal-0.3.9/src/rascal/arc_lines/xe_strong.csv`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/atlas.py` & `rascal-0.3.9/src/rascal/atlas.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/calibrator.py` & `rascal-0.3.9/src/rascal/calibrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1434,27 +1434,44 @@
 
             min_atlas_wavelength = self.min_wavelength - self.range_tolerance
 
         if max_atlas_wavelength is None:
 
             max_atlas_wavelength = self.max_wavelength + self.range_tolerance
 
-        new_atlas = Atlas(
-            elements,
-            min_atlas_wavelength=min_atlas_wavelength,
-            max_atlas_wavelength=max_atlas_wavelength,
-            min_intensity=min_intensity,
-            min_distance=min_distance,
-            range_tolerance=self.range_tolerance,
-            vacuum=vacuum,
-            pressure=pressure,
-            temperature=temperature,
-            relative_humidity=relative_humidity,
-        )
-        self.atlas = new_atlas
+        if self.atlas is None:
+
+            new_atlas = Atlas(
+                elements,
+                min_atlas_wavelength=min_atlas_wavelength,
+                max_atlas_wavelength=max_atlas_wavelength,
+                min_intensity=min_intensity,
+                min_distance=min_distance,
+                range_tolerance=self.range_tolerance,
+                vacuum=vacuum,
+                pressure=pressure,
+                temperature=temperature,
+                relative_humidity=relative_humidity,
+            )
+            self.atlas = new_atlas
+
+        else:
+
+            self.atlas.add(
+                elements,
+                min_atlas_wavelength=min_atlas_wavelength,
+                max_atlas_wavelength=max_atlas_wavelength,
+                min_intensity=min_intensity,
+                min_distance=min_distance,
+                vacuum=vacuum,
+                pressure=pressure,
+                temperature=temperature,
+                relative_humidity=relative_humidity,
+            )
+
         self.candidate_tolerance = candidate_tolerance
         self.constrain_poly = constrain_poly
 
         self._generate_pairs()
 
     def remove_atlas_lines_range(self, wavelength, tolerance=10):
         """
```

### Comparing `rascal-0.3.8.1/src/rascal/houghtransform.py` & `rascal-0.3.9/src/rascal/houghtransform.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/models.py` & `rascal-0.3.9/src/rascal/models.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/plotting.py` & `rascal-0.3.9/src/rascal/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -986,14 +986,18 @@
                     yaxis="y3",
                     name="Arc Spectrum",
                 )
             )
 
             spec_max = np.nanmax(spectrum) * 1.05
 
+        else:
+
+            spec_max = vline_max
+
         fitted_peaks = []
         fitted_peaks_adu = []
         fitted_diff = []
         all_diff = []
 
         for p in calibrator.peaks:
 
@@ -1022,20 +1026,20 @@
             if np.abs(diff[idx]) < tolerance:
 
                 fitted_peaks.append(p)
                 if spectrum is not None:
                     fitted_peaks_adu.append(
                         spectrum[int(calibrator.pix_to_rawpix(p))]
                     )
-                    fitted_diff.append(diff[idx])
-                    calibrator.logger.info(
-                        "- matched to {} A".format(
-                            calibrator.atlas.get_lines()[idx]
-                        )
+                fitted_diff.append(diff[idx])
+                calibrator.logger.info(
+                    "- matched to {} A".format(
+                        calibrator.atlas.get_lines()[idx]
                     )
+                )
 
         x_fitted = calibrator.polyval(fitted_peaks, fit_coeff)
 
         fig.add_trace(
             go.Scatter(
                 x=x_fitted,
                 y=fitted_peaks_adu,
```

### Comparing `rascal-0.3.8.1/src/rascal/synthetic.py` & `rascal-0.3.9/src/rascal/synthetic.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal/util.py` & `rascal-0.3.9/src/rascal/util.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/src/rascal.egg-info/PKG-INFO` & `rascal-0.3.9/src/rascal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rascal
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: The Pyhton Automated Wavelenmgth Calibrator.
 Home-page: https://rascal.readthedocs.io/en/latest/?badge=latest
 Download-URL: https://github.com/jveitchmichaelis/rascal
 Author: Josh Veitch-Michaelis, Marco C Lam
 Author-email: j.veitchmichaelis@gmail.com, lam@mail.tau.ac.il
 Maintainer: Josh Veitch-Michaelis, Marco C Lam
 Maintainer-email: j.veitchmichaelis@gmail.com, lam@mail.tau.ac.il
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -43,19 +42,20 @@
 
 You don't need to know the dispersion and start wavelength exactly. Often this information is provided by the observatory, but if you don't know it, you can take a rough guess. The closer you are to the actual system settings, the more likely it is that Rascal will be able to solve the calibration. Blind calibration, where no parameters are known, is possible but challenging currently. If you don't know the lamp, you can try iterating over the various combinations of sources. Generally when you do get a correct fit, with most astronomical instruments the errors will be extremely low.
 
 More background information can be referred to this [arXiv article](https://ui.adsabs.harvard.edu/abs/2019arXiv191205883V/abstract).
 
 
 ## Dependencies
-* python >= 3.6
-* numpy
-* scipy
-* pynverse
-* matplotlib
+* python >= 3.7
+* numpy>=1.16,<1.24
+* scipy>=1.3.3
+* pynverse>=0.1.4
+* matplotlib>=3.0.3
+* tqdm>=4.48.0
 
 ## Optional Dependencies
 * [plotly](https://github.com/plotly/plotly.py) >= 4.0
 
 ## Installation
 Instructions can be found [here](https://rascal.readthedocs.io/en/latest/installation/installation.html).
```

### Comparing `rascal-0.3.8.1/src/rascal.egg-info/SOURCES.txt` & `rascal-0.3.9/src/rascal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_arclines.py` & `rascal-0.3.9/test/test_arclines.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_effective_pixel.py` & `rascal-0.3.9/test/test_effective_pixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     c.set_calibrator_properties(pixel_list=effective_pixel)
 
     # Setup the Hough transform parameters
     c.set_hough_properties(
         range_tolerance=100.0, min_wavelength=100.0, max_wavelength=1300.0
     )
 
-    c.set_ransac_properties(linear=False, minimum_fit_error=1e-12)
+    c.set_ransac_properties(linear=False, minimum_fit_error=1e-14)
 
     # Add our fake lines as the atlas
     a.add_user_atlas(elements=["Test"] * len(waves), wavelengths=waves)
     c.set_atlas(a)
     assert len(c.atlas.atlas_lines) > 0
 
     # And let's try and fit...
```

### Comparing `rascal-0.3.8.1/test/test_hough_transform.py` & `rascal-0.3.9/test/test_hough_transform.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_lt_sprat_manual_atlas.py` & `rascal-0.3.9/test/test_lt_sprat_manual_atlas.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_plotting.py` & `rascal-0.3.9/test/test_plotting.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_polynomial_fit.py` & `rascal-0.3.9/test/test_polynomial_fit.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_synthetic.py` & `rascal-0.3.9/test/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_synthetic_calibration.py` & `rascal-0.3.9/test/test_synthetic_calibration.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_util.py` & `rascal-0.3.9/test/test_util.py`

 * *Files identical despite different names*

### Comparing `rascal-0.3.8.1/test/test_xe_calibration.py` & `rascal-0.3.9/test/test_xe_calibration.py`

 * *Files identical despite different names*

