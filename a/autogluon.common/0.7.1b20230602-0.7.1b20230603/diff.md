# Comparing `tmp/autogluon.common-0.7.1b20230602.tar.gz` & `tmp/autogluon.common-0.7.1b20230603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230602.tar", last modified: Fri Jun  2 09:03:37 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230603.tar", last modified: Sat Jun  3 09:03:32 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230602.tar` & `autogluon.common-0.7.1b20230603.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.929129 autogluon.common-0.7.1b20230602/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-06-02 09:03:37.929129 autogluon.common-0.7.1b20230602/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:03:37.929129 autogluon.common-0.7.1b20230602/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/autogluon/common/model_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/model_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/model_filter/_model_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.929129 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.929129 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-02 09:03:27.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:37.925128 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:03:37.000000 autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.608435 autogluon.common-0.7.1b20230603/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-03 09:03:32.608435 autogluon.common-0.7.1b20230603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 09:03:32.608435 autogluon.common-0.7.1b20230603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.600435 autogluon.common-0.7.1b20230603/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.600435 autogluon.common-0.7.1b20230603/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.604435 autogluon.common-0.7.1b20230603/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.604435 autogluon.common-0.7.1b20230603/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.604435 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.604435 autogluon.common-0.7.1b20230603/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.604435 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.608435 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-03 09:03:22.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:32.604435 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:32.000000 autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230602/LICENSE` & `autogluon.common-0.7.1b20230603/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/PKG-INFO` & `autogluon.common-0.7.1b20230603/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.common-0.7.1b20230602/setup.py` & `autogluon.common-0.7.1b20230603/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/model_filter/_model_filter.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/model_filter/_model_filter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230603/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.common-0.7.1b20230602/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230603/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

