# Comparing `tmp/lokii-1.1.1.tar.gz` & `tmp/lokii-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokii-1.1.1.tar", last modified: Sat Jun  3 07:19:42 2023, max compression
+gzip compressed data, was "lokii-1.1.2.tar", last modified: Sun Jun  4 11:02:05 2023, max compression
```

## Comparing `lokii-1.1.1.tar` & `lokii-1.1.2.tar`

### file list

```diff
@@ -1,69 +1,68 @@
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.1/LICENSE
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-03 07:19:42.140868 lokii-1.1.1/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.1/README.md
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        5 2023-06-03 07:18:59.000000 lokii-1.1.1/VERSION
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       55 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/__main__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.1/lokii/cli.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2287 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/config.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/exec/node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii/logger/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/logger/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-06-02 08:52:49.000000 lokii-1.1.1/lokii/logger/color.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/logger/context.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2023-06-03 07:10:34.000000 lokii-1.1.1/lokii/logger/formatter.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/logger/progress.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     7475 2023-06-03 06:05:24.000000 lokii-1.1.1/lokii/main.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii/model/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/model/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.1/lokii/model/group_module.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/model/node_module.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/parse/base_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3109 2023-06-03 07:18:23.000000 lokii-1.1.1/lokii/parse/group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2928 2023-06-03 07:15:57.000000 lokii-1.1.1/lokii/parse/node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.1/lokii/storage/batch_iterator.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4924 2023-06-02 09:34:04.000000 lokii-1.1.1/lokii/storage/data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      835 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/storage/temp_storage.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/lokii/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/util/graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.1/lokii/util/module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.1/lokii/util/perf_timer_context.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.136868 lokii-1.1.1/lokii.egg-info/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-03 07:19:42.000000 lokii-1.1.1/lokii.egg-info/PKG-INFO
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1339 2023-06-03 07:19:42.000000 lokii-1.1.1/lokii.egg-info/SOURCES.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-03 07:19:42.000000 lokii-1.1.1/lokii.egg-info/dependency_links.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-03 07:19:42.000000 lokii-1.1.1/lokii.egg-info/entry_points.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.1/lokii.egg-info/not-zip-safe
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-03 07:19:42.000000 lokii-1.1.1/lokii.egg-info/requires.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-03 07:19:42.000000 lokii-1.1.1/lokii.egg-info/top_level.txt
--rw-rw-r--   0 doruk     (1000) doruk     (1000)       38 2023-06-03 07:19:42.140868 lokii-1.1.1/setup.cfg
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1801 2023-06-02 08:01:36.000000 lokii-1.1.1/setup.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/tests/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.1/tests/conftest.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/tests/exec/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/exec/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.1/tests/exec/test_node_executor.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/tests/parse/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/parse/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.1/tests/parse/test_group_parser.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.1/tests/parse/test_node_parser.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/tests/storage/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/storage/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     4195 2023-06-02 09:34:04.000000 lokii-1.1.1/tests/storage/test_data_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/storage/test_temp_storage.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     3345 2023-06-03 05:56:09.000000 lokii-1.1.1/tests/test_cli.py
-drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-03 07:19:42.140868 lokii-1.1.1/tests/util/
--rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/util/__init__.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.1/tests/util/test_graph_analyzer.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/util/test_module_file_loader.py
--rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.1/tests/util/test_perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-26 20:12:04.000000 lokii-1.1.2/LICENSE
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-04 11:02:05.917296 lokii-1.1.2/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     5434 2023-06-02 08:01:36.000000 lokii-1.1.2/README.md
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.913296 lokii-1.1.2/lokii/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       77 2023-06-04 11:02:04.000000 lokii-1.1.2/lokii/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       78 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/__main__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3176 2023-06-02 08:01:36.000000 lokii-1.1.2/lokii/cli.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2142 2023-06-04 11:01:51.000000 lokii-1.1.2/lokii/config.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/lokii/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2620 2023-05-31 14:39:03.000000 lokii-1.1.2/lokii/exec/node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/lokii/logger/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/logger/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1268 2023-06-02 08:52:49.000000 lokii-1.1.2/lokii/logger/color.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1756 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/logger/context.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      877 2023-06-03 07:10:34.000000 lokii-1.1.2/lokii/logger/formatter.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      639 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/logger/progress.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     7475 2023-06-03 06:05:24.000000 lokii-1.1.2/lokii/main.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/lokii/model/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/model/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      943 2023-06-02 08:01:36.000000 lokii-1.1.2/lokii/model/group_module.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1083 2023-05-31 14:39:03.000000 lokii-1.1.2/lokii/model/node_module.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/lokii/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      709 2023-05-31 14:39:03.000000 lokii-1.1.2/lokii/parse/base_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3109 2023-06-03 07:18:23.000000 lokii-1.1.2/lokii/parse/group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2928 2023-06-03 07:15:57.000000 lokii-1.1.2/lokii/parse/node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/lokii/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      983 2023-06-02 08:01:36.000000 lokii-1.1.2/lokii/storage/batch_iterator.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4924 2023-06-02 09:34:04.000000 lokii-1.1.2/lokii/storage/data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      835 2023-05-31 14:39:03.000000 lokii-1.1.2/lokii/storage/temp_storage.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/lokii/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2160 2023-05-31 14:39:03.000000 lokii-1.1.2/lokii/util/graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1464 2023-05-31 14:39:03.000000 lokii-1.1.2/lokii/util/module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      610 2023-05-26 20:12:04.000000 lokii-1.1.2/lokii/util/perf_timer_context.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.913296 lokii-1.1.2/lokii.egg-info/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     6557 2023-06-04 11:02:05.000000 lokii-1.1.2/lokii.egg-info/PKG-INFO
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1341 2023-06-04 11:02:05.000000 lokii-1.1.2/lokii.egg-info/SOURCES.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-06-04 11:02:05.000000 lokii-1.1.2/lokii.egg-info/dependency_links.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       45 2023-06-04 11:02:05.000000 lokii-1.1.2/lokii.egg-info/entry_points.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2021-03-08 06:45:18.000000 lokii-1.1.2/lokii.egg-info/not-zip-safe
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       71 2023-06-04 11:02:05.000000 lokii-1.1.2/lokii.egg-info/requires.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       12 2023-06-04 11:02:05.000000 lokii-1.1.2/lokii.egg-info/top_level.txt
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)       84 2023-06-04 11:02:05.917296 lokii-1.1.2/setup.cfg
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1700 2023-06-04 11:01:51.000000 lokii-1.1.2/setup.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/tests/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        1 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2501 2023-06-02 08:01:36.000000 lokii-1.1.2/tests/conftest.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/tests/exec/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/exec/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1098 2023-05-31 14:39:03.000000 lokii-1.1.2/tests/exec/test_node_executor.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/tests/parse/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/parse/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     2230 2023-06-02 08:01:36.000000 lokii-1.1.2/tests/parse/test_group_parser.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3165 2023-05-31 14:39:03.000000 lokii-1.1.2/tests/parse/test_node_parser.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/tests/storage/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/storage/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     4195 2023-06-02 09:34:04.000000 lokii-1.1.2/tests/storage/test_data_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      369 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/storage/test_temp_storage.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     3345 2023-06-03 05:56:09.000000 lokii-1.1.2/tests/test_cli.py
+drwxrwxr-x   0 doruk     (1000) doruk     (1000)        0 2023-06-04 11:02:05.917296 lokii-1.1.2/tests/util/
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)        0 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/util/__init__.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      953 2023-05-31 14:39:03.000000 lokii-1.1.2/tests/util/test_graph_analyzer.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)     1007 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/util/test_module_file_loader.py
+-rw-rw-r--   0 doruk     (1000) doruk     (1000)      629 2023-05-26 20:12:04.000000 lokii-1.1.2/tests/util/test_perf_timer_context.py
```

### Comparing `lokii-1.1.1/LICENSE` & `lokii-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/PKG-INFO` & `lokii-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.1.1
+Version: 1.1.2
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lokii-1.1.1/README.md` & `lokii-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/cli.py` & `lokii-1.1.2/lokii/cli.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/config.py` & `lokii-1.1.2/lokii/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,9 @@
 from os import path, environ, cpu_count
-
-root = path.dirname(path.dirname(__file__))
-# read app version from root of the project
-f = open(path.join(root, "VERSION"), "r")
-VERSION = f.read().strip()
-f.close()
+import lokii
 
 # temp directory that contains generated runtime files and database
 TEMP_DIR_PATH = environ.get("LOKII__TEMP_DIR_PATH", ".temp")
 # duckdb database that stores generated data in relational tables
 TEMP_DB_FILE = environ.get("LOKII__TEMP_DB_FILE", "lokii.duckdb")
 # name of the temp data file that contains generated runtime files
 TEMP_DATA_DIR = environ.get("LOKII__TEMP_DATA_DIR", "data")
@@ -66,15 +61,15 @@
 
         @property
         def chunk_size(self) -> int:
             return int(GEN_CHUNK_SIZE)
 
     @property
     def version(self):
-        return VERSION
+        return lokii.__version__
 
     @property
     def temp(self):
         return self.__TempConfig()
 
     @property
     def gen(self):
```

### Comparing `lokii-1.1.1/lokii/exec/node_executor.py` & `lokii-1.1.2/lokii/exec/node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/logger/color.py` & `lokii-1.1.2/lokii/logger/color.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/logger/context.py` & `lokii-1.1.2/lokii/logger/context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/logger/formatter.py` & `lokii-1.1.2/lokii/logger/formatter.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/logger/progress.py` & `lokii-1.1.2/lokii/logger/progress.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/main.py` & `lokii-1.1.2/lokii/main.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/model/group_module.py` & `lokii-1.1.2/lokii/model/group_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/model/node_module.py` & `lokii-1.1.2/lokii/model/node_module.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/parse/base_parser.py` & `lokii-1.1.2/lokii/parse/base_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/parse/group_parser.py` & `lokii-1.1.2/lokii/parse/group_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/parse/node_parser.py` & `lokii-1.1.2/lokii/parse/node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/storage/batch_iterator.py` & `lokii-1.1.2/lokii/storage/batch_iterator.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/storage/data_storage.py` & `lokii-1.1.2/lokii/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/storage/temp_storage.py` & `lokii-1.1.2/lokii/storage/temp_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/util/graph_analyzer.py` & `lokii-1.1.2/lokii/util/graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/util/module_file_loader.py` & `lokii-1.1.2/lokii/util/module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii/util/perf_timer_context.py` & `lokii-1.1.2/lokii/util/perf_timer_context.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/lokii.egg-info/PKG-INFO` & `lokii-1.1.2/lokii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lokii
-Version: 1.1.1
+Version: 1.1.2
 Summary: Generate, Load, Develop and Test with consistent relational datasets!
 Home-page: https://github.com/dorukerenaktas/lokii
 Author: Doruk Eren Aktaş
 Author-email: dorukerenaktas@gmail.com
 License: MIT License
 Keywords: data generation,relational datasets,development environment,testing,database
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lokii-1.1.1/lokii.egg-info/SOURCES.txt` & `lokii-1.1.2/lokii.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-VERSION
+setup.cfg
 setup.py
 lokii/__init__.py
 lokii/__main__.py
 lokii/cli.py
 lokii/config.py
 lokii/main.py
 lokii.egg-info/PKG-INFO
```

### Comparing `lokii-1.1.1/setup.py` & `lokii-1.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 #!/usr/bin/env python
 
 from os import path
 from setuptools import setup, find_packages
 
 root = path.dirname(__file__)
-with open(path.join(root, "VERSION"), "r") as f:
-    VERSION = f.read().strip()
 with open(path.join(root, "README.md"), "r") as f:
     README = f.read().strip()
 
 setup(
     name="lokii",
-    version=VERSION,
     packages=find_packages(where="."),
     description="Generate, Load, Develop and Test with consistent relational datasets!",
     long_description=README,
     long_description_content_type="text/markdown",
     keywords="data generation, relational datasets, development environment, testing, database",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `lokii-1.1.1/tests/conftest.py` & `lokii-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/exec/test_node_executor.py` & `lokii-1.1.2/tests/exec/test_node_executor.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/parse/test_group_parser.py` & `lokii-1.1.2/tests/parse/test_group_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/parse/test_node_parser.py` & `lokii-1.1.2/tests/parse/test_node_parser.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/storage/test_data_storage.py` & `lokii-1.1.2/tests/storage/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/test_cli.py` & `lokii-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/util/test_graph_analyzer.py` & `lokii-1.1.2/tests/util/test_graph_analyzer.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/util/test_module_file_loader.py` & `lokii-1.1.2/tests/util/test_module_file_loader.py`

 * *Files identical despite different names*

### Comparing `lokii-1.1.1/tests/util/test_perf_timer_context.py` & `lokii-1.1.2/tests/util/test_perf_timer_context.py`

 * *Files identical despite different names*

