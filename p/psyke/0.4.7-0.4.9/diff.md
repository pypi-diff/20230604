# Comparing `tmp/psyke-0.4.7.tar.gz` & `tmp/psyke-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.4.7.tar", last modified: Sun Jun  4 18:38:09 2023, max compression
+gzip compressed data, was "psyke-0.4.9.tar", last modified: Sun Jun  4 20:34:32 2023, max compression
```

## Comparing `psyke-0.4.7.tar` & `psyke-0.4.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-04 18:36:38.000000 psyke-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-04 18:36:38.000000 psyke-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-04 18:38:09.717284 psyke-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-04 18:36:38.000000 psyke-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 18:38:09.000000 psyke-0.4.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.709284 psyke-0.4.7/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-04 18:38:02.000000 psyke-0.4.7/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/gridrex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/extraction/trepan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-04 18:36:38.000000 psyke-0.4.7/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.713284 psyke-0.4.7/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-04 18:38:09.000000 psyke-0.4.7/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-04 18:38:09.000000 psyke-0.4.7/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:38:09.000000 psyke-0.4.7/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:38:09.000000 psyke-0.4.7/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 18:38:09.000000 psyke-0.4.7/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 18:38:09.000000 psyke-0.4.7/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 18:36:38.000000 psyke-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 18:38:09.717284 psyke-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-04 18:36:38.000000 psyke-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.709284 psyke-0.4.7/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-04 18:36:38.000000 psyke-0.4.7/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-04 18:36:42.000000 psyke-0.4.7/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-04 18:36:42.000000 psyke-0.4.7/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 18:36:42.000000 psyke-0.4.7/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 18:38:09.717284 psyke-0.4.7/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-04 18:36:42.000000 psyke-0.4.7/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-06-04 20:32:44.000000 psyke-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-04 20:32:44.000000 psyke-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-04 20:34:32.467380 psyke-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-04 20:32:44.000000 psyke-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 20:34:32.000000 psyke-0.4.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.455380 psyke-0.4.9/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)    14626 2023-06-04 20:34:24.000000 psyke-0.4.9/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.455380 psyke-0.4.9/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.455380 psyke-0.4.9/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.455380 psyke-0.4.9/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.455380 psyke-0.4.9/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/gridrex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/extraction/trepan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.459380 psyke-0.4.9/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-04 20:32:44.000000 psyke-0.4.9/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.455380 psyke-0.4.9/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-04 20:34:32.000000 psyke-0.4.9/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-04 20:34:32.000000 psyke-0.4.9/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:34:32.000000 psyke-0.4.9/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:34:32.000000 psyke-0.4.9/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-04 20:34:32.000000 psyke-0.4.9/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-04 20:34:32.000000 psyke-0.4.9/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 20:32:44.000000 psyke-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:34:32.467380 psyke-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-06-04 20:32:44.000000 psyke-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.451380 psyke-0.4.9/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.463380 psyke-0.4.9/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14273 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-04 20:32:44.000000 psyke-0.4.9/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-04 20:32:49.000000 psyke-0.4.9/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-04 20:32:49.000000 psyke-0.4.9/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-04 20:32:49.000000 psyke-0.4.9/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:34:32.467380 psyke-0.4.9/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-04 20:32:49.000000 psyke-0.4.9/test/resources/tests/__init__.py
```

### Comparing `psyke-0.4.7/LICENSE` & `psyke-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/PKG-INFO` & `psyke-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.4.7
+Version: 0.4.9
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.4.7/README.md` & `psyke-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/__init__.py` & `psyke-0.4.9/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/clustering/cream/__init__.py` & `psyke-0.4.9/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/clustering/exact/__init__.py` & `psyke-0.4.9/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/clustering/utils.py` & `psyke-0.4.9/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/cart/__init__.py` & `psyke-0.4.9/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/cart/predictor.py` & `psyke-0.4.9/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/__init__.py` & `psyke-0.4.9/psyke/extraction/hypercubic/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.4.9/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.4.9/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.4.9/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.4.9/psyke/extraction/hypercubic/hypercube.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,50 @@
 from psyke.utils.logic import create_term, to_rounded_real, linear_function_creator
 from sklearn.linear_model import LinearRegression
 from tuprolog.core import Var, Struct
 from random import Random
 import numpy as np
 
 
-Point = dict[str, float]
-
-
 class FeatureNotFoundException(Exception):
 
     def __init__(self, feature: str):
         super().__init__(f'Feature {feature} not found.')
 
 
+class Point:
+    """
+    An N-dimensional point.
+    """
+
+    EPSILON = get_default_precision()
+
+    def __init__(self, dimensions: list[str], values: list[float]):
+        self._dimensions = {dimension: value for (dimension, value) in zip(dimensions, values)}
+
+    def __getitem__(self, feature: str) -> float:
+        if feature in self._dimensions.keys():
+            return self._dimensions[feature]
+        else:
+            raise FeatureNotFoundException(feature)
+
+    def __setitem__(self, key: str, value: float) -> None:
+        self._dimensions[key] = value
+
+    def __eq__(self, other: Point) -> bool:
+        return all([abs(self[dimension] - other[dimension]) < Point.EPSILON for dimension in self._dimensions])
+
+    @property
+    def dimensions(self) -> dict[str, float]:
+        return self._dimensions
+
+
 class HyperCube:
     """
-    A N-dimensional cube holding a numeric value.
+    An N-dimensional cube holding a numeric value.
     """
 
     EPSILON = get_default_precision()  # Precision used when comparing two hypercubes
     INT_PRECISION = get_int_precision()
 
     def __init__(self, dimension: dict[str, tuple[float, float]] = None, limits: set[Limit] = None,
                  output: float | LinearRegression = 0.0):
@@ -57,15 +81,15 @@
 
     def __getitem__(self, feature: str) -> Dimension:
         if feature in self._dimensions.keys():
             return self._dimensions[feature]
         else:
             raise FeatureNotFoundException(feature)
 
-    def __setitem__(self, key, value) -> None:
+    def __setitem__(self, key: str, value: tuple[float, float] | list[float]) -> None:
         self._dimensions[key] = value
 
     def __hash__(self) -> int:
         result = [hash(name + str(dimension[0]) + str(dimension[1])) for name, dimension in self.dimensions.items()]
         return sum(result)
 
     @property
@@ -222,20 +246,20 @@
 
     def diagonal(self) -> float:
         return reduce(
             lambda a, b: a + b, [(dimension[1] - dimension[0]) ** 2 for dimension in self._dimensions.values()], 0
         ) ** 0.5
 
     def center(self) -> Point:
-        return {dimension: (interval[0] + interval[1]) / 2 for dimension, interval in self._dimensions.items()}
+        return Point(list(self._dimensions.keys()),
+                     [(interval[0] + interval[1]) / 2 for interval in self._dimensions.values()])
 
     def corners(self) -> Iterable[Point]:
         return [
-            {dimension: value for (dimension, value) in zip(self._dimensions.keys(), values)}
-            for values in itertools.product(*self._dimensions.values())
+            Point(list(self._dimensions.keys()), values) for values in itertools.product(*self._dimensions.values())
         ]
 
     def is_adjacent(self, cube: HyperCube) -> str | None:
         adjacent = None
         for (feature, [a1, b1]) in self._dimensions.items():
             if self[feature] == cube[feature]:
                 continue
```

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.4.9/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/strategy.py` & `psyke-0.4.9/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/hypercubic/utils.py` & `psyke-0.4.9/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/real/__init__.py` & `psyke-0.4.9/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/real/utils.py` & `psyke-0.4.9/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/trepan/__init__.py` & `psyke-0.4.9/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/extraction/trepan/utils.py` & `psyke-0.4.9/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/schema/__init__.py` & `psyke-0.4.9/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/tuning/__init__.py` & `psyke-0.4.9/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/tuning/crash/__init__.py` & `psyke-0.4.9/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/tuning/orchid/__init__.py` & `psyke-0.4.9/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/tuning/pedro/__init__.py` & `psyke-0.4.9/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/utils/__init__.py` & `psyke-0.4.9/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/utils/dataframe.py` & `psyke-0.4.9/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/utils/logic.py` & `psyke-0.4.9/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/utils/metrics.py` & `psyke-0.4.9/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/utils/plot.py` & `psyke-0.4.9/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke/utils/sorted.py` & `psyke-0.4.9/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/psyke.egg-info/PKG-INFO` & `psyke-0.4.9/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.4.7
+Version: 0.4.9
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.4.7/psyke.egg-info/SOURCES.txt` & `psyke-0.4.9/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/setup.py` & `psyke-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/__init__.py` & `psyke-0.4.9/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/cart/test_cart.py` & `psyke-0.4.9/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.4.9/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.4.9/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.4.9/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.4.9/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 import unittest
 import pandas as pd
 from sklearn.linear_model import LinearRegression
 
 from psyke.extraction.hypercubic.hypercube import FeatureNotFoundException, ClosedRegressionCube, \
-    ClosedClassificationCube, ClosedCube, ClassificationCube, RegressionCube
+    ClosedClassificationCube, ClosedCube, ClassificationCube, RegressionCube, Point
 from psyke.extraction.hypercubic.utils import MinUpdate, Expansion, ZippedDimension
 from psyke.utils import get_int_precision
 from sklearn.neighbors import KNeighborsRegressor
 from test.psyke import Predictor
 from psyke.extraction.hypercubic import HyperCube
 from test.resources.datasets import get_dataset_path
 
@@ -221,21 +221,20 @@
     def test_volume(self):
         self.assertEqual(self.cube.volume(), (self.x[1] - self.x[0]) * (self.y[1] - self.y[0]))
 
     def test_diagonal(self):
         self.assertEqual(self.cube.diagonal(), ((self.x[1] - self.x[0])**2 + (self.y[1] - self.y[0])**2)**0.5)
 
     def test_center(self):
-        self.assertEqual(self.cube.center(), {dim: (val[0] + val[1]) / 2 for dim, val in self.dimensions.items()})
+        self.assertEqual(self.cube.center(), Point(list(self.dimensions.keys()),
+                                                   [(val[0] + val[1]) / 2 for val in self.dimensions.values()]))
 
     def test_corners(self):
         self.assertEqual(self.cube.corners(), [
-            {dim: value for (dim, value) in zip(self.dimensions.keys(), values)}
-            for values in itertools.product(*self.dimensions.values())
-        ])
+            Point(list(self.dimensions.keys()), values) for values in itertools.product(*self.dimensions.values())])
 
     def test_is_adjacent(self):
         cube_adj = HyperCube({'X': (0.6, 0.9), 'Y': self.y}, set(), self.mean)
         self.assertTrue(self.cube.is_adjacent(cube_adj))
         cube_not_adj = HyperCube({'X': self.y, 'Y': self.x}, set(), self.mean)
         self.assertFalse(self.cube.is_adjacent(cube_not_adj))
```

### Comparing `psyke-0.4.7/test/psyke/extraction/real/test_real.py` & `psyke-0.4.9/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/real/test_rule.py` & `psyke-0.4.9/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/trepan/test_node.py` & `psyke-0.4.9/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/trepan/test_split.py` & `psyke-0.4.9/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.4.9/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/utils/test_prune.py` & `psyke-0.4.9/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/utils/test_simplify.py` & `psyke-0.4.9/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.4.9/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.4.7/test/resources/tests/__init__.py` & `psyke-0.4.9/test/resources/tests/__init__.py`

 * *Files identical despite different names*

