# Comparing `tmp/psyke-0.4.5.tar.gz` & `tmp/psyke-0.4.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.4.5.tar", last modified: Sat Jun  3 23:16:24 2023, max compression
+gzip compressed data, was "psyke-0.4.6.dev5.tar", last modified: Sun Jun  4 16:23:05 2023, max compression
```

## Comparing `psyke-0.4.5.tar` & `psyke-0.4.6.dev5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.485432 psyke-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-03 23:15:08.000000 psyke-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 23:15:08.000000 psyke-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-03 23:16:24.485432 psyke-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-03 23:15:08.000000 psyke-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-03 23:16:24.000000 psyke-0.4.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-03 23:16:17.000000 psyke-0.4.5/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/gridrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/extraction/trepan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-03 23:15:08.000000 psyke-0.4.5/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-03 23:16:24.000000 psyke-0.4.5/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-03 23:16:24.000000 psyke-0.4.5/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:16:24.000000 psyke-0.4.5/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:16:24.000000 psyke-0.4.5/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-03 23:16:24.000000 psyke-0.4.5/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-03 23:16:24.000000 psyke-0.4.5/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 23:15:08.000000 psyke-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 23:16:24.485432 psyke-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-03 23:15:08.000000 psyke-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.473432 psyke-0.4.5/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.477432 psyke-0.4.5/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.485432 psyke-0.4.5/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-03 23:15:08.000000 psyke-0.4.5/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.485432 psyke-0.4.5/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 23:15:11.000000 psyke-0.4.5/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.485432 psyke-0.4.5/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-03 23:15:11.000000 psyke-0.4.5/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.485432 psyke-0.4.5/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-03 23:15:11.000000 psyke-0.4.5/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 23:16:24.485432 psyke-0.4.5/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-03 23:15:12.000000 psyke-0.4.5/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.348032 psyke-0.4.6.dev5/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-04 16:22:58.000000 psyke-0.4.6.dev5/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.348032 psyke-0.4.6.dev5/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.348032 psyke-0.4.6.dev5/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.348032 psyke-0.4.6.dev5/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/gridrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/extraction/trepan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.348032 psyke-0.4.6.dev5/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 16:23:05.000000 psyke-0.4.6.dev5/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.344031 psyke-0.4.6.dev5/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.352032 psyke-0.4.6.dev5/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-04 16:21:44.000000 psyke-0.4.6.dev5/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-04 16:21:48.000000 psyke-0.4.6.dev5/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-04 16:21:48.000000 psyke-0.4.6.dev5/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 16:21:48.000000 psyke-0.4.6.dev5/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 16:23:05.356032 psyke-0.4.6.dev5/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-04 16:21:48.000000 psyke-0.4.6.dev5/test/resources/tests/__init__.py
```

### Comparing `psyke-0.4.5/LICENSE` & `psyke-0.4.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/PKG-INFO` & `psyke-0.4.6.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.4.5
+Version: 0.4.6.dev5
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.4.5/README.md` & `psyke-0.4.6.dev5/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/__init__.py` & `psyke-0.4.6.dev5/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/clustering/cream/__init__.py` & `psyke-0.4.6.dev5/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/clustering/exact/__init__.py` & `psyke-0.4.6.dev5/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/clustering/utils.py` & `psyke-0.4.6.dev5/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/cart/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/cart/predictor.py` & `psyke-0.4.6.dev5/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             output if output is not None else Target.CONSTANT
         self.__generator = Random(seed)
 
     def _best_cube(self, dataframe: pd.DataFrame, cube: GenericCube, cubes: Iterable[Expansion]) -> Expansion | None:
         expansions = []
         for limit in cubes:
             count = limit.cube.count(dataframe)
-            dataframe = dataframe.append(limit.cube.create_samples(self.min_examples - count, self.__generator))
+            dataframe = pd.concat([dataframe, limit.cube.create_samples(self.min_examples - count, self.__generator)])
             limit.cube.update(dataframe, self.predictor)
             expansions.append(Expansion(
                 limit.cube, limit.feature, limit.direction,
                 abs(cube.output - limit.cube.output) if self._output is Target.CONSTANT else
                 1 - int(cube.output == limit.cube.output)
             ))
         if len(expansions) > 0:
```

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/strategy.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/hypercubic/utils.py` & `psyke-0.4.6.dev5/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/real/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/real/utils.py` & `psyke-0.4.6.dev5/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/trepan/__init__.py` & `psyke-0.4.6.dev5/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/extraction/trepan/utils.py` & `psyke-0.4.6.dev5/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/schema/__init__.py` & `psyke-0.4.6.dev5/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/tuning/__init__.py` & `psyke-0.4.6.dev5/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/tuning/crash/__init__.py` & `psyke-0.4.6.dev5/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/tuning/orchid/__init__.py` & `psyke-0.4.6.dev5/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/tuning/pedro/__init__.py` & `psyke-0.4.6.dev5/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/utils/__init__.py` & `psyke-0.4.6.dev5/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/utils/dataframe.py` & `psyke-0.4.6.dev5/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/utils/logic.py` & `psyke-0.4.6.dev5/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/utils/metrics.py` & `psyke-0.4.6.dev5/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/utils/plot.py` & `psyke-0.4.6.dev5/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke/utils/sorted.py` & `psyke-0.4.6.dev5/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/psyke.egg-info/PKG-INFO` & `psyke-0.4.6.dev5/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.4.5
+Version: 0.4.6.dev5
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.4.5/psyke.egg-info/SOURCES.txt` & `psyke-0.4.6.dev5/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/setup.py` & `psyke-0.4.6.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 
 EPOCHS: int = 50
 BATCH_SIZE: int = 16
 REQUIREMENTS = [
-    'numpy~=1.24.0',
-    'pandas~=1.5.0',
+    'numpy~=1.23.5',
+    'pandas~=2.0.2',
     'scikit-learn~=1.2.0',
     '2ppy~=0.4.0',
     'kneed~=0.8.1',
     'sympy~=1.11'
 ]  # Optional
```

### Comparing `psyke-0.4.5/test/psyke/__init__.py` & `psyke-0.4.6.dev5/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/cart/test_cart.py` & `psyke-0.4.6.dev5/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.4.6.dev5/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.4.6.dev5/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/real/test_real.py` & `psyke-0.4.6.dev5/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/real/test_rule.py` & `psyke-0.4.6.dev5/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/trepan/test_node.py` & `psyke-0.4.6.dev5/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/extraction/trepan/test_split.py` & `psyke-0.4.6.dev5/test/psyke/extraction/trepan/test_split.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class TestSplit(unittest.TestCase):
 
     dataset: pd.DataFrame = get_dataset('iris')
     n_examples = dataset.shape[0]
     all_node = Node(dataset, n_examples)
     setosa_40 = Node(dataset.iloc[10:70, :], n_examples)
-    setosa_40_complementar = Node(dataset.iloc[:10, :].append(dataset.iloc[70:, :]), n_examples)
+    setosa_40_complementar = Node(pd.concat([dataset.iloc[:10, :], dataset.iloc[70:, :]]), n_examples)
     versicolor_25 = Node(dataset.iloc[40:75, :], n_examples)
     versicolor_25_complementar = Node(dataset.iloc[75:110, :], n_examples)
 
     def test_priority(self):
         self.assertTrue(math.isclose(-40/60-50/90-100,
                                      Split(self.all_node, (self.setosa_40, self.setosa_40_complementar)).priority))
         self.assertTrue(math.isclose((25 / 35) * - 2 - 200 + 200,
```

### Comparing `psyke-0.4.5/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.4.6.dev5/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/utils/test_prune.py` & `psyke-0.4.6.dev5/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/utils/test_simplify.py` & `psyke-0.4.6.dev5/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.4.6.dev5/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.5/test/resources/tests/__init__.py` & `psyke-0.4.6.dev5/test/resources/tests/__init__.py`

 * *Files identical despite different names*

