# Comparing `tmp/py-dbcn-0.3.1.tar.gz` & `tmp/py-dbcn-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-dbcn-0.3.1.tar", last modified: Mon Nov 21 13:25:45 2022, max compression
+gzip compressed data, was "py-dbcn-0.3.2.tar", last modified: Sun Jun  4 20:02:04 2023, max compression
```

## Comparing `py-dbcn-0.3.1.tar` & `py-dbcn-0.3.2.tar`

### file list

```diff
@@ -1,106 +1,110 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-06-24 02:45:26.000000 py-dbcn-0.3.1/LICENSE
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       34 2022-06-24 02:45:26.000000 py-dbcn-0.3.1/MANIFEST.in
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2414 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.273221 py-dbcn-0.3.1/py_dbcn/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/py_dbcn/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.273221 py-dbcn-0.3.1/py_dbcn/connectors/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1780 2022-09-19 13:36:44.000000 py-dbcn-0.3.1/py_dbcn/connectors/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.273221 py-dbcn-0.3.1/py_dbcn/connectors/core/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4957 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7142 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    14682 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3061 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    11639 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13633 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      750 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    30557 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/py_dbcn/connectors/core/validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.273221 py-dbcn-0.3.1/py_dbcn/connectors/mysql/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      165 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3345 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      784 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      825 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      747 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5949 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      740 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3811 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4584 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/py_dbcn/connectors/mysql/validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.273221 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      175 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3526 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5624 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      864 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      858 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7270 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1632 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      613 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3533 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/py_dbcn/connectors/postgresql/validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2033 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      641 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      658 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      602 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      609 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      593 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/connectors/sqlite/validate.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1731 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/py_dbcn/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    11749 2022-09-19 13:36:44.000000 py-dbcn-0.3.1/py_dbcn/logging.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.273221 py-dbcn-0.3.1/py_dbcn.egg-info/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2414 2022-11-21 13:25:45.000000 py-dbcn-0.3.1/py_dbcn.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3221 2022-11-21 13:25:45.000000 py-dbcn-0.3.1/py_dbcn.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2022-11-21 13:25:45.000000 py-dbcn-0.3.1/py_dbcn.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       87 2022-11-21 13:25:45.000000 py-dbcn-0.3.1/py_dbcn.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       14 2022-11-21 13:25:45.000000 py-dbcn-0.3.1/py_dbcn.egg-info/top_level.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1152 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/pyproject.toml
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      193 2022-07-30 21:10:41.000000 py-dbcn-0.3.1/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      852 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/setup.cfg
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/tests/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/tests/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/tests/connectors/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/tests/connectors/__init__.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/tests/connectors/core/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/tests/connectors/core/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10445 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/tests/connectors/core/test_core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10633 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/core/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    42489 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/core/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      850 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/core/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    80989 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/tests/connectors/core/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13108 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/core/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      554 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/core/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   197639 2022-11-21 13:22:29.000000 py-dbcn-0.3.1/tests/connectors/core/test_validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/tests/connectors/mysql/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/tests/connectors/mysql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      755 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/tests/connectors/mysql/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    19375 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/expected_display_output.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1305 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2645 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3984 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1009 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5281 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3009 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3750 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2339 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/tests/connectors/mysql/test_validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/tests/connectors/postgresql/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/tests/connectors/postgresql/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      783 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/tests/connectors/postgresql/constants.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    20058 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/expected_display_output.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1362 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_core.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2674 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3974 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1034 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7228 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3005 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      597 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2369 2022-11-21 13:22:26.000000 py-dbcn-0.3.1/tests/connectors/postgresql/test_validate.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2022-11-21 13:25:45.277221 py-dbcn-0.3.1/tests/connectors/sqlite/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-06-11 01:40:25.000000 py-dbcn-0.3.1/tests/connectors/sqlite/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      482 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_database.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      479 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_display.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      473 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_query.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      478 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_records.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      475 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_tables.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      582 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_utils.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      542 2022-10-04 14:41:52.000000 py-dbcn-0.3.1/tests/connectors/sqlite/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-07-30 11:57:47.000000 py-dbcn-0.3.2/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       34 2022-07-30 11:57:47.000000 py-dbcn-0.3.2/MANIFEST.in
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2425 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn/connectors/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1780 2022-10-02 00:19:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn/connectors/core/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    40695 2023-06-04 19:48:07.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6174 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7142 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    14494 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3061 2023-01-27 02:21:04.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     8696 2023-06-04 04:51:57.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13633 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      750 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    24893 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/core/validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/py_dbcn/connectors/mysql/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      165 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3945 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      784 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      825 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      747 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5949 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      740 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3811 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4584 2022-12-06 23:14:49.000000 py-dbcn-0.3.2/py_dbcn/connectors/mysql/validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      175 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     4126 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5624 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      864 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      858 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     6058 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1632 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      613 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3533 2022-12-06 23:14:49.000000 py-dbcn-0.3.2/py_dbcn/connectors/postgresql/validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      167 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2033 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      641 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      658 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      602 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      609 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      593 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      652 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/connectors/sqlite/validate.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1731 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/py_dbcn/constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    11749 2023-01-29 18:59:14.000000 py-dbcn-0.3.2/py_dbcn/logging.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.877746 py-dbcn-0.3.2/py_dbcn.egg-info/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2425 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3377 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       75 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       14 2023-06-04 20:02:04.000000 py-dbcn-0.3.2/py_dbcn.egg-info/top_level.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1302 2023-06-04 19:56:46.000000 py-dbcn-0.3.2/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      193 2022-09-11 11:43:55.000000 py-dbcn-0.3.2/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      852 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2021-11-18 14:09:53.000000 py-dbcn-0.3.2/tests/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/connectors/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2021-11-18 14:11:07.000000 py-dbcn-0.3.2/tests/connectors/__init__.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/connectors/core/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:34:33.000000 py-dbcn-0.3.2/tests/connectors/core/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    72483 2023-06-04 19:24:42.000000 py-dbcn-0.3.2/tests/connectors/core/test_clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10445 2022-12-06 23:14:49.000000 py-dbcn-0.3.2/tests/connectors/core/test_core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10633 2023-01-26 23:43:57.000000 py-dbcn-0.3.2/tests/connectors/core/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    43158 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/core/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      850 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/core/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    93193 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/core/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    13108 2023-01-27 01:26:18.000000 py-dbcn-0.3.2/tests/connectors/core/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      554 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/core/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   198103 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/core/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.881746 py-dbcn-0.3.2/tests/connectors/mysql/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:55:45.000000 py-dbcn-0.3.2/tests/connectors/mysql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      755 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/mysql/constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    19375 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/expected_display_output.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      665 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1305 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2645 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3984 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1009 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5281 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3009 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3750 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2339 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/mysql/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/tests/connectors/postgresql/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:58:12.000000 py-dbcn-0.3.2/tests/connectors/postgresql/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      783 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/postgresql/constants.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    20613 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/postgresql/expected_display_output.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      711 2023-06-03 03:17:14.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_clauses.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1362 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_core.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2674 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3974 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1034 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7228 2023-01-23 09:41:06.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3005 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      597 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2369 2022-11-14 00:44:20.000000 py-dbcn-0.3.2/tests/connectors/postgresql/test_validate.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-04 20:02:04.885746 py-dbcn-0.3.2/tests/connectors/sqlite/
+-rw-r--r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-01-23 12:58:19.000000 py-dbcn-0.3.2/tests/connectors/sqlite/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      482 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_database.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      479 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_display.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      473 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_query.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      478 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_records.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      475 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_tables.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      582 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_utils.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      542 2022-10-11 03:13:18.000000 py-dbcn-0.3.2/tests/connectors/sqlite/test_validate.py
```

### Comparing `py-dbcn-0.3.1/LICENSE` & `py-dbcn-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/PKG-INFO` & `py-dbcn-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbcn
-Version: 0.3.1
+Version: 0.3.2
 Summary: Connector for Pythonic interaction with multiple database types.
 Home-page: https://github.com/brodriguez8774/py-dbcn
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Brandon Rodriguez
@@ -24,15 +24,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/brodriguez8774/py-dbcn
-Keywords: database,mysql
+Keywords: database,mysql,postgresql
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/__init__.py` & `py-dbcn-0.3.2/py_dbcn/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/core.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,122 @@
 """
-"Core" DB Connector class.
+MySQL DB Connector class.
 
-Contains generalized database connection logic.
-Should be inherited by language-specific connectors.
+Contains database connection logic specific to MySQL databases.
 """
 
 # System Imports.
-from abc import ABC, abstractmethod
+
+# Third-party Imports.
+import MySQLdb
 
 # Internal Imports.
-from .database import BaseDatabase
-from .display import BaseDisplay
-from .query import BaseQuery
-from .records import BaseRecords
-from .tables import BaseTables
-from .utils import BaseUtils
-from .validate import BaseValidate
+from .database import MysqlDatabase
+from .display import MysqlDisplay
+from .query import MysqlQuery
+from .records import MysqlRecords
+from .tables import MysqlTables
+from .utils import MysqlUtils
+from .validate import MysqlValidate
+from py_dbcn.connectors.core import AbstractDbConnector
 from py_dbcn.logging import init_logging
 
 
 # Import logger.
 logger = init_logging(__name__)
 
 
-class AbstractDbConnector(ABC):
+class MysqlDbConnector(AbstractDbConnector):
     """
-    Abstract/generalized database connector logic, that is universal to all database classes.
-
-    (As this project develops, logic will likely start here,
-    and then be gradually moved to specific connectors as needed.)
+    Database connector logic for MySQL databases.
     """
-    @abstractmethod
-    def __init__(
-        self,
-        db_host, db_port, db_user, db_pass, db_name, *args,
-        display_connection_output=True, debug=False, **kwargs,
-    ):
-        logger.debug('Generating (core) Connector class.')
-        db_port = int(db_port)
-
-        self._connection = None
-        self._debug = debug
-
-        # region Config Initialization
-
-        # Define class to hold config values.
-        class Config:
-            pass
-
-        # Initialize config.
-        self._config = Config()
-        # Values for connecting.
-        self._config.display_connection_output = display_connection_output
-        self._config.db_host = db_host
-        self._config.db_port = db_port
-        self._config.db_user = db_user
-        self._config.db_pass = db_pass
-        self._config.db_name = db_name
-        # Values for managing connector state.
-        self._config.db_type = None
-        self._config._implemented_db_types = ['MySQL', 'PostgreSQL']
-
-        # endregion Config Initialization
-
-        # region Error Handler Setup
-
-        # Define class to hold error handler references.
-        class Errors:
-            pass
-
-        self.errors = Errors()
-        self.errors.handler = None
-        self.errors.database_does_not_exist = None
-        self.errors.database_already_exists = None
-        self.errors.table_does_not_exist = None
-        self.errors.table_already_exists = None
-
-        # endregion Error Handler Setup
-
-        # region Child Sub-Class Initialization
-
-        # Create references to related subclasses.
-        self.database = self._get_related_database_class()
-        self.databases = self._get_related_database_class()
-        self.display = self._get_related_display_class()
-        self.query = self._get_related_query_class()
-        self.record = self._get_related_records_class()
-        self.records = self._get_related_records_class()
-        self.table = self._get_related_tables_class()
-        self.tables = self._get_related_tables_class()
-        self.utils = self._get_related_utils_class()
-        self.validate = self._get_related_validate_class()
-
-        # endregion Child Sub-Class Initialization
-
-    def __del__(self):
-        """
-        Close database connection on exit.
-        """
-        self.close_connection()
+    def __init__(self, *args, **kwargs):
+        # Call parent logic.
+        super().__init__(*args, **kwargs)
+
+        # Initialize error handlers.
+        self.errors.handler = MySQLdb
+        self.errors.database_does_not_exist = self.errors.handler.OperationalError
+        self.errors.database_already_exists = self.errors.handler.ProgrammingError
+        self.errors.table_does_not_exist = self.errors.handler.OperationalError
+        self.errors.table_already_exists = self.errors.handler.OperationalError
+
+        # Initialize database connection.
+        self._config.db_type = 'MySQL'
+        self.create_connection()
 
     def create_connection(self, db_name=None):
-        """Attempts to create database connection, using config values."""
-        raise NotImplementedError('Please override the connection.create_connection() function.')
+        """Attempts to create database connection, using config values.
 
-    def close_connection(self):
-        """Attempts to close database connection, if open.
-
-        :param display_output: Bool indicating if output should display.
+        :param db_name: Name of database to connect to.
         """
-        try:
-            self._connection.close()
-        except:
-            pass
+        if db_name is None or str(db_name).strip() == '':
+            # Empty value provided. Fallback to config value.
+            db_name = self._config.db_name
+        else:
+            # Update selected db in config.
+            self._config.db_name = db_name
+
+        self._connection = MySQLdb.connect(
+            host=self._config.db_host,
+            port=self._config.db_port,
+            user=self._config.db_user,
+            password=self._config.db_pass,
+            db=db_name,
+        )
 
         if self._config.display_connection_output:
-            logger.info('Closed {0} database connection.'.format(self._config.db_type))
+            logger.info('Created MySQL database connection.')
 
     def _get_related_database_class(self):
         """
         Overridable method to get the related "database functionality" class.
         """
-        return BaseDatabase(self)
+        return MysqlDatabase(self)
 
     def _get_related_display_class(self):
         """
         Overridable method to get the related "display functionality" class.
         """
-        return BaseDisplay(self)
+        return MysqlDisplay(self)
 
     def _get_related_query_class(self):
         """
         Overridable method to get the related "query functionality" class.
         """
-        return BaseQuery(self)
+        return MysqlQuery(self)
 
     def _get_related_records_class(self):
         """
-        Overridable method to get the related "record functionality" class.
+        Overridable method to get the related "records functionality" class.
         """
-        return BaseRecords(self)
+        return MysqlRecords(self)
 
     def _get_related_tables_class(self):
         """
         Overridable method to get the related "tables functionality" class.
         """
-        return BaseTables(self)
+        return MysqlTables(self)
 
     def _get_related_utils_class(self):
         """
-        Overridable method to get the related "utility functionality" class.
+        Overridable method to get the related "utils functionality" class.
         """
-        return BaseUtils(self)
+        return MysqlUtils(self)
 
-    def _get_related_validate_class(self):
+    def _get_related_validate_class(
+        self,
+        enable_identifier_validators, enable_where_validators, enable_column_validators,
+        enable_values_validators, enable_order_by_validators, enable_limit_validators,
+    ):
         """
         Overridable method to get the related "validation functionality" class.
         """
-        return BaseValidate(self)
+        return MysqlValidate(
+            self,
+            enable_identifier_validators=enable_identifier_validators,
+            enable_where_validators=enable_where_validators,
+            enable_column_validators=enable_column_validators,
+            enable_values_validators=enable_values_validators,
+            enable_order_by_validators=enable_order_by_validators,
+            enable_limit_validators=enable_limit_validators,
+        )
```

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/database.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/display.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/display.py`

 * *Files 10% similar despite different names*

```diff
@@ -290,50 +290,44 @@
 
     def select(self, results, logger, table_name, select_clause=None):
         """Display logic for records.select()."""
         if not self._base.validate._quote_column_format:
             raise ValueError('Column quote format is not defined.')
 
         if results:
-            # Check select clause, which directly affects desired output columns.
-            # First we initialize to a default str.
-            if select_clause is None:
-                select_clause = '*'
-            else:
-                select_clause = str(select_clause).strip()
-
             if self._base._config.db_type == 'MySQL':
                 col_name_index = 0
             elif self._base._config.db_type == 'PostgreSQL':
                 col_name_index = 3
             else:
                 raise NotImplementedError('Please define expected index to find column name.')
 
             # Handle based on star or specific cols.
             # TODO: Probably need to tokenize this, to properly compare.
-            if select_clause == '*' or '(*)' in select_clause:
+            if len(select_clause.array) ==  1 and select_clause.array[0] == '*':
                 # Calculate column header values, using all columns.
                 table_cols = [
                     x[col_name_index]
                     for x in self._base.tables.describe(table_name, display_query=False, display_results=False)
                 ]
             else:
-                select_clause = select_clause.split(',')
+                # Calculate column header values, using only provided columns.
                 table_cols = []
                 table_describe = self._base.tables.describe(table_name, display_query=False, display_results=False)
-                for index in range(len(select_clause)):
+                select_clause_arr = select_clause.array
+                for index in range(len(select_clause_arr)):
                     # Sanitize select clause values.
-                    clause = select_clause[index].strip()
-                    if len(clause) > 1 and clause[0] == clause[-1] and clause[0] in ['`', '"', "'"]:
-                        clause = clause[1:-1]
-                    select_clause[index] = clause
-
-                # Calculate column header values, filtered by select clause.
-                table_cols = copy.deepcopy(select_clause)
+                    if select_clause.is_quoted(select_clause_arr[index]):
+                        clause = select_clause_arr[index][1:-1]
+                    else:
+                        clause = select_clause_arr[index]
+                    # if clause in table_describe:
+                    table_cols.append(clause)
 
+            # Calculate column header values with determined columns.
             col_len_array = []
             total_col_len = 0
             for table_col in table_cols:
                 col_len = len(table_col)
                 if not any(keyword_str in table_col for keyword_str in self._base.validate._reserved_function_names):
                     record_len = self._base.query.execute(
                         self._parent.max_col_length_query.format(
```

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/query.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/records.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/records.py`

 * *Files 21% similar despite different names*

```diff
@@ -69,14 +69,15 @@
         query = 'SELECT {0} FROM {1}{2}{3}{4};'.format(
             select_clause,
             table_name,
             where_clause,
             order_by_clause,
             limit_clause,
         )
+
         results = self._base.query.execute(query, display_query=display_query)
         if display_results:
             self._base.display.records.select(results, logger, table_name, select_clause)
 
         return results
 
     def insert(self, table_name, values_clause, columns_clause=None, display_query=True, display_results=True):
@@ -90,104 +91,59 @@
         """
         # Check that provided table name is valid format.
         if not self._base.validate.table_name(table_name):
             raise ValueError('Invalid table name of "{0}".'.format(table_name))
 
         # Check that provided COLUMNS clause is valid format.
         columns_clause = self._base.validate.sanitize_columns_clause(columns_clause)
-        if len(columns_clause) > 0:
-            columns_clause = ' ({0})'.format(columns_clause)
 
         # Check that provided VALUES clause is valid format.
         values_clause = self._base.validate.sanitize_values_clause(values_clause)
 
-        # Check for values that might need formatting.
-        # For example, if we find date/datetime objects, we automatically convert to a str value that won't error.
-        if isinstance(values_clause, list) or isinstance(values_clause, tuple):
-            updated_values_clause = ()
-            for item in values_clause:
-
-                if isinstance(item, datetime.datetime):
-                    # Is a datetime object. Convert to string.
-                    item = item.strftime('%Y-%m-%d %H:%M:%S')
-                elif isinstance(item, datetime.date):
-                    # Is a date object. Convert to string.
-                    item = item.strftime('%Y-%m-%d')
-
-                # Add item to updated clause.
-                updated_values_clause += (item,)
-
-            # Replace original clause.
-            values_clause = updated_values_clause
-
         # Insert record.
         query = textwrap.dedent(
             """
             INSERT INTO {0}{1}
-            VALUES {2};
-            """.format(table_name, columns_clause, values_clause)
+            VALUES ({2});
+            """.format(table_name, columns_clause, values_clause.context)
         )
-        results = self._base.query.execute(query, display_query=display_query)
+
+        results = self._base.query.execute(query, data=values_clause.data, display_query=display_query)
         if display_results:
             self._base.display.results('{0}'.format(results))
 
         return results
 
     def insert_many(self, table_name, values_clause, columns_clause=None, display_query=True, display_results=True):
         """"Inserts multiple records into provided table with one query."""
         # Check that provided table name is valid format.
         if not self._base.validate.table_name(table_name):
             raise ValueError('Invalid table name of "{0}".'.format(table_name))
 
         # Check that provided COLUMNS clause is valid format.
         columns_clause = self._base.validate.sanitize_columns_clause(columns_clause)
-        if columns_clause != '':
-            columns_clause = ' ({0})'.format(columns_clause)
 
         # Check that provided VALUES clause is valid format.
         # Must be array format.
         if not isinstance(values_clause, list) and not isinstance(values_clause, tuple):
             raise ValueError('VALUES clause for INSERT_MANY queries must be in list/tuple format.')
         if len(values_clause) < 1:
             raise ValueError('VALUES clause cannot be empty for INSERT_MANY queries.')
-        values_clause = self._base.validate.sanitize_values_clause(values_clause)
-
-        # Check for values that might need formatting.
-        # For example, if we find date/datetime objects, we automatically convert to a str value that won't error.
-        if isinstance(values_clause, list) or isinstance(values_clause, tuple):
-            updated_values_clause = ()
-
-            # Check each sub-item.
-            for item in values_clause:
-
-                if isinstance(item, datetime.datetime):
-                    # Is a datetime object. Convert to string.
-                    item = item.strftime('%Y-%m-%d %H:%M:%S')
-                elif isinstance(item, datetime.date):
-                    # Is a date object. Convert to string.
-                    item = item.strftime('%Y-%m-%d')
-
-                # Add item to updated clause.
-                updated_values_clause += (item,)
-
-            # Replace original clause.
-            values_clause = updated_values_clause
-        else:
-            raise ValueError('In an execute_many, values clause must be a list or tuple.')
-
-        values_context = ', '.join('%s' for i in range(len(values_clause[0])))
+        values_clause = self._base.validate.sanitize_values_many_clause(values_clause)
 
         # Insert record.
         query = textwrap.dedent(
             """
             INSERT INTO {0}{1}
-            VALUES ({2});
-            """.format(table_name, columns_clause, values_context)
+            VALUES
+            {2};
+            """.format(table_name, columns_clause, values_clause.context)
         )
-        results = self._base.query.execute_many(query, values_clause, display_query=display_query)
+
+        results = self._base.query.execute(query, data=values_clause.data, display_query=display_query)
         if display_results:
             self._base.display.results('{0}'.format(results))
 
         return results
 
     def update(self, table_name, values_clause, where_clause, display_query=True, display_results=True):
         """Updates record in provided table.
@@ -199,43 +155,24 @@
         :param display_results: Bool indicating if results should output to console. Defaults to True.
         """
         # Check that provided table name is valid format.
         if not self._base.validate.table_name(table_name):
             raise ValueError('Invalid table name of "{0}".'.format(table_name))
 
         # Check that provided VALUES clause is valid format.
-        values_clause = self._base.validate.sanitize_values_clause(values_clause)
+        values_clause = self._base.validate.sanitize_set_clause(values_clause)
 
         # Check that provided WHERE clause is valid format.
         where_clause = self._base.validate.sanitize_where_clause(where_clause)
 
-        # Check for values that might need formatting.
-        # For example, if we find date/datetime objects, we automatically convert to a str value that won't error.
-        if isinstance(values_clause, list) or isinstance(values_clause, tuple):
-            updated_values_clause = ()
-            for item in values_clause:
-
-                if isinstance(item, datetime.datetime):
-                    # Is a datetime object. Convert to string.
-                    item = item.strftime('%Y-%m-%d %H:%M:%S')
-                elif isinstance(item, datetime.date):
-                    # Is a date object. Convert to string.
-                    item = item.strftime('%Y-%m-%d')
-
-                # Add item to updated clause.
-                updated_values_clause += (item,)
-
-            # Replace original clause.
-            values_clause = updated_values_clause
-
         # Update record.
         query = textwrap.dedent(
             """
             UPDATE {0}
-            SET {1}{2};
+            {1}{2};
             """.format(table_name, values_clause, where_clause)
         )
         self._base.query.execute(query, display_query=display_query)
 
         # Do a select to get the updated values as results.
         results = self.select(
             table_name,
```

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/tables.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/utils.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/core/validate.py` & `py-dbcn-0.3.2/py_dbcn/connectors/core/validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,48 +3,55 @@
 
 Contains generalized database connection logic.
 Should be inherited by language-specific connectors.
 """
 
 # System Imports.
 import copy, re
-from io import StringIO
-from tokenize import (
-    generate_tokens,
-    ENDMARKER,
-    NAME,
-    NEWLINE,
-    NUMBER,
-    OP,
-    STRING,
-)
 
 # Internal Imports.
+from . import clauses
 from py_dbcn.logging import init_logging
 
 
 # Import logger.
 logger = init_logging(__name__)
 
 
 class BaseValidate:
     """
     Abstract/generalized logic, for validating various queries and query subsections.
 
     (As this project develops, logic will likely start here,
     and then be gradually moved to specific connectors as needed.)
     """
-    def __init__(self, parent, *args, **kwargs):
+    def __init__(
+        self,
+        parent,
+        *args,
+        enable_identifier_validators=True, enable_where_validators=True, enable_column_validators=True,
+        enable_values_validators=True, enable_order_by_validators=True, enable_limit_validators=True,
+        **kwargs,
+    ):
         logger.debug('Generating related (core) Validate class.')
 
         # Define connector root object.
         self._base = parent
 
         # Define provided direct parent object.
         self._parent = parent
+        self.clauses = clauses
+
+        # Save provided values.
+        self._enable_identifier_validators = enable_identifier_validators
+        self._enable_where_validators = enable_where_validators
+        self._enable_column_validators = enable_column_validators
+        self._enable_values_validators = enable_values_validators
+        self._enable_order_by_validators = enable_order_by_validators
+        self._enable_limit_validators = enable_limit_validators
 
         # Define inheritance variables.
         self._reserved_function_names = None
         self._quote_column_format = None
         self._quote_identifier_format = None
         self._quote_order_by_format = None
         self._quote_str_literal_format = None
@@ -330,237 +337,83 @@
     def validate_limit_by_clause(self, identifier):
         """"""
 
     # endregion Validation Functions
 
     # region Sanitization Functions
 
-    def sanitize_select_identifier_clause(self, clause, as_str=True):
+    def sanitize_select_identifier_clause(self, clause):
         """
         Validates that provided clause follows acceptable format.
         :param clause: SELECT clause to validate.
         :param as_str: Bool indicating if return value should be formatted as a str. Otherwise is list.
         :return: Properly formatted clause if possible, otherwise error.
         """
-        if not self._reserved_function_names:
-            raise ValueError('Reserved keyword list is not defined.')
-
-        # Sanitize overall clause.
-        clause = self._inner_sanitize_columns(clause, allow_wildcard=True)
-
-        # Check that each inner clause item is valid.
-        for item in clause:
-            self.validate_select_clause(item)
-
-        # All items in clause were valid. Return validated and sanitized SELECT clause.
-        if as_str:
-            # Re-concatenate into single expected str format.
-            return ', '.join(clause)
+        if self._enable_identifier_validators:
+            return clauses.SelectClauseBuilder(self, clause)
         else:
-            # Return as list.
             return clause
 
     def sanitize_where_clause(self, clause):
         """
         Validates that provided clause follows acceptable format.
         :param clause: WHERE clause to validate.
         :return: Properly formatted clause if possible, otherwise error.
         """
-        # TODO: Implement proper sanitization.
-
-        # Handle if none.
-        if clause is None:
-            clause = ''
-
-        # Convert to str.
-        clause = str(clause).strip()
-
-        # Remove prefix, if present.
-        if clause.lower().startswith('where'):
-            clause = clause[5:]
-
-        # Strip now that prefix is gone.
-        clause = clause.strip()
-
-        # Put into expected format.
-        if len(clause) > 1:
-            clause = '\nWHERE {0}'.format(clause)
-
-        return clause
+        if self._enable_where_validators:
+            return clauses.WhereClauseBuilder(self, clause)
+        else:
+            return clause
 
-    def sanitize_columns_clause(self, clause, as_str=True):
+    def sanitize_columns_clause(self, clause):
         """
         Validates that provided clause follows acceptable format.
         :param clause: COLUMNS clause to validate.
         :param as_str: Bool indicating if return value should be formatted as a str. Otherwise is list.
         :return: Properly formatted clause if possible, otherwise error.
         """
-        if not self._reserved_function_names:
-            raise ValueError('Reserved keyword list is not defined.')
-
-        # Sanitize overall clause.
-        clause = self._inner_sanitize_columns(clause, allow_wildcard=False)
-
-        # Check that each inner clause item is valid.
-        for item in clause:
-            self.validate_columns_clause(item)
-
-        # All items in clause were valid. Return validated and sanitized SELECT clause.
-        if as_str:
-            # Re-concatenate into single expected str format.
-            return ', '.join(clause)
+        if self._enable_column_validators:
+            return clauses.ColumnsClauseBuilder(self, clause)
         else:
-            # Return as list.
             return clause
 
     def sanitize_values_clause(self, clause):
         """
         Validates that provided clause follows acceptable format.
 
         :param clause: VALUES clause to validate.
         :return: Properly formatted clause if possible, otherwise error.
         """
-        # For now, always return as valid.
-        return clause
+        if self._enable_values_validators:
+            return clauses.ValuesClauseBuilder(self, clause)
+        else:
+            return clause
+
+    def sanitize_values_many_clause(self, clause):
+        if self._enable_values_validators:
+            return clauses.ValuesManyClauseBuilder(self, clause)
+        else:
+            return clause
 
-        # # TODO: Attempted to have full, dynamic validation of entire clause and all inner values.
-        # #   However, had too many cases where it would break, due to being able to essentially put in anything.
-        # #   It may be possible to magically validate the "values clause", but it's too much time/work
-        # #   to implement right now. Potentially look into again in the future.
-        # #
-        # #   Also, due to the nature of this logic, it almost seems like this should either do the
-        # #   "full dynamic validation" or have no validation at all for this clause. Unsure how best to handle this
-        # #   at the current date...
-        # #
-        # print('\n\n\n\n')
-        # print('orig clause: "{0}"'.format(clause))
-        #
-        # if not self._reserved_function_names:
-        #     raise ValueError('Reserved keyword list is not defined.')
-        #
-        # # Convert to array format.
-        # if isinstance(clause, list) or isinstance(clause, tuple):
-        #     # Format we want.
-        #     pass
-        # else:
-        #     print('as str: {0}')
-        #
-        #     # Handle for None type.
-        #     if clause is None:
-        #         clause = ''
-        #     else:
-        #         clause = str(clause).strip()
-        #
-        #     # Remove clause starting value.
-        #     if clause.lower().startswith('values'):
-        #         clause = clause[6:].strip()
-        #
-        #     # Ensure not empty when prefix was provided.
-        #     if len(clause) < 1:
-        #         raise ValueError('Invalid VALUES clause. Must have one or more items.')
-        #
-        #     # Due to possible amount of variation (particularly in quoted string values),
-        #     # we have to tokenize in order to attempt to properly parse.
-        #     # Via tokenization, we can effectively avoid outer parens.
-        #     tokens = generate_tokens(StringIO(clause).readline)
-        #     print('\nas tokens:')
-        #     clause = []
-        #     for token in tokens:
-        #         print('    {0}'.format(token))
-        #         if token.exact_type == 1:
-        #             # Direct value, missing quotes.
-        #             token = str(token.string).strip()
-        #             clause.append('{0}{1}{0}'.format(self._quote_str_literal_format, token))
-        #         elif token.exact_type == 3:
-        #             # String type. Convert to expected quote type.
-        #             token = str(token.string).strip()[1:-1]
-        #             clause.append('{0}{1}{0}'.format(self._quote_str_literal_format, token))
-        #
-        # print('as array: {0}'.format(clause))
-        #
-        # # Loop through each item in array and ensure proper formatting.
-        # updated_clause = []
-        # for index in range(len(clause)):
-        #     item = clause[index]
-        #     print('    type: {0}    val: {1}'.format(type(item), item))
-        #
-        #     # Sanitize for null.
-        #     if item is None:
-        #         item = 'Null'
-        #
-        #     # Sanitize str outer quoting.
-        #     elif isinstance(item, str):
-        #         print('    formatted: {0}'.format("""{0}""".format(item)))
-        #
-        #         # TODO: Unsure of if this part is required? Seemed to be having issues parsing when multiple quotes are
-        #         # put in a row.
-        #         tokens = generate_tokens(StringIO("""{0}""".format(item)).readline)
-        #         print('    tokens:')
-        #         for token in tokens:
-        #             print('        {0}'.format(token))
-        #
-        #         if len(item) > 1:
-        #             if item[0] != self._quote_str_literal_format or item[-1] != self._quote_str_literal_format:
-        #                 item = '{0}{1}{0}'.format(self._quote_str_literal_format, item)
-        #
-        #     # Set all others to str equivalent.
-        #     else:
-        #         item = str(item)
-        #
-        #     # Append item.
-        #     updated_clause.append(item)
-        # clause = updated_clause
-        #
-        # # Handle empty clause.
-        # if clause == '':
-        #     return ''
-        #
-        # # Return formatted clause.
-        # return ' VALUES ({0})'.format(', '.join(clause))
+    def sanitize_set_clause(self, clause):
+        if self._enable_values_validators:
+            return clauses.SetClauseBuilder(self, clause)
+        else:
+            return clause
 
-    def sanitize_order_by_clause(self, clause, as_str=True):
+    def sanitize_order_by_clause(self, clause):
         """
         Validates that provided clause follows acceptable format.
         :param clause: ORDER_BY clause to validate.
         :param as_str: Bool indicating if return value should be formatted as a str. Otherwise is list.
         :return: Properly formatted clause if possible, otherwise error.
         """
-        if not self._reserved_function_names:
-            raise ValueError('Reserved keyword list is not defined.')
-
-        # Quickly sanitize if string format.
-        if isinstance(clause, str):
-            clause = clause.strip()
-
-            # Remove clause starting value.
-            if clause.lower().startswith('order by'):
-                clause = clause[8:].strip()
-
-                # Ensure not empty when prefix was provided.
-                if len(clause) < 1:
-                    raise ValueError('Invalid ORDER BY clause.')
-
-        # Validate.
-        clause = self._inner_sanitize_columns(clause, allow_wildcard=False, order_by=True)
-
-        # Handle empty clause.
-        if clause == '':
-            return ''
-
-        # Check that each inner clause item is valid.
-        for item in clause:
-            self.validate_order_by_clause(item)
-
-        # All items in clause were valid. Return validated and sanitized SELECT clause.
-        if as_str:
-            # Re-concatenate into single expected str format.
-            clause = ', '.join(clause)
-            return '\nORDER BY {0}'.format(clause)
+        if self._enable_order_by_validators:
+            return clauses.OrderByClauseBuilder(self, clause)
         else:
-            # Return as list.
             return clause
 
     def sanitize_limit_clause(self, clause):
         """
         Validates that provided clause follows acceptable format.
         :param clause: LIMIT clause to validate.
         :return: Properly formatted clause if possible, otherwise error.
```

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/database.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/display.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/query.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/records.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/tables.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/utils.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/mysql/validate.py` & `py-dbcn-0.3.2/py_dbcn/connectors/mysql/validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/postgresql/database.py` & `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/postgresql/display.py` & `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/postgresql/query.py` & `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/postgresql/tables.py` & `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/postgresql/utils.py` & `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/postgresql/validate.py` & `py-dbcn-0.3.2/py_dbcn/connectors/postgresql/validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/core.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/database.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/display.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/query.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/records.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/tables.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/utils.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/connectors/sqlite/validate.py` & `py-dbcn-0.3.2/py_dbcn/connectors/sqlite/validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/constants.py` & `py-dbcn-0.3.2/py_dbcn/constants.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn/logging.py` & `py-dbcn-0.3.2/py_dbcn/logging.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/py_dbcn.egg-info/PKG-INFO` & `py-dbcn-0.3.2/py_dbcn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dbcn
-Version: 0.3.1
+Version: 0.3.2
 Summary: Connector for Pythonic interaction with multiple database types.
 Home-page: https://github.com/brodriguez8774/py-dbcn
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Brandon Rodriguez
@@ -24,15 +24,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/brodriguez8774/py-dbcn
-Keywords: database,mysql
+Keywords: database,mysql,postgresql
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `py-dbcn-0.3.1/py_dbcn.egg-info/SOURCES.txt` & `py-dbcn-0.3.2/py_dbcn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 py_dbcn.egg-info/PKG-INFO
 py_dbcn.egg-info/SOURCES.txt
 py_dbcn.egg-info/dependency_links.txt
 py_dbcn.egg-info/requires.txt
 py_dbcn.egg-info/top_level.txt
 py_dbcn/connectors/__init__.py
 py_dbcn/connectors/core/__init__.py
+py_dbcn/connectors/core/clauses.py
 py_dbcn/connectors/core/core.py
 py_dbcn/connectors/core/database.py
 py_dbcn/connectors/core/display.py
 py_dbcn/connectors/core/query.py
 py_dbcn/connectors/core/records.py
 py_dbcn/connectors/core/tables.py
 py_dbcn/connectors/core/utils.py
@@ -47,36 +48,39 @@
 py_dbcn/connectors/sqlite/records.py
 py_dbcn/connectors/sqlite/tables.py
 py_dbcn/connectors/sqlite/utils.py
 py_dbcn/connectors/sqlite/validate.py
 tests/__init__.py
 tests/connectors/__init__.py
 tests/connectors/core/__init__.py
+tests/connectors/core/test_clauses.py
 tests/connectors/core/test_core.py
 tests/connectors/core/test_database.py
 tests/connectors/core/test_display.py
 tests/connectors/core/test_query.py
 tests/connectors/core/test_records.py
 tests/connectors/core/test_tables.py
 tests/connectors/core/test_utils.py
 tests/connectors/core/test_validate.py
 tests/connectors/mysql/__init__.py
 tests/connectors/mysql/constants.py
 tests/connectors/mysql/expected_display_output.py
+tests/connectors/mysql/test_clauses.py
 tests/connectors/mysql/test_core.py
 tests/connectors/mysql/test_database.py
 tests/connectors/mysql/test_display.py
 tests/connectors/mysql/test_query.py
 tests/connectors/mysql/test_records.py
 tests/connectors/mysql/test_tables.py
 tests/connectors/mysql/test_utils.py
 tests/connectors/mysql/test_validate.py
 tests/connectors/postgresql/__init__.py
 tests/connectors/postgresql/constants.py
 tests/connectors/postgresql/expected_display_output.py
+tests/connectors/postgresql/test_clauses.py
 tests/connectors/postgresql/test_core.py
 tests/connectors/postgresql/test_database.py
 tests/connectors/postgresql/test_display.py
 tests/connectors/postgresql/test_query.py
 tests/connectors/postgresql/test_records.py
 tests/connectors/postgresql/test_tables.py
 tests/connectors/postgresql/test_utils.py
```

### Comparing `py-dbcn-0.3.1/pyproject.toml` & `py-dbcn-0.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "py-dbcn"
-version = "0.3.1"
+version = "0.3.2"
 description = "Connector for Pythonic interaction with multiple database types."
 readme = "readme.md"
 authors = [{ name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -20,17 +20,19 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 keywords = [
     "database",
     "mysql",
+    "postgresql",
 ]
 dependencies = [
-    "mysqlclient",
+#    "mysqlclient",         # Required if connecting to MySQL databases.
+#    "psycopg2-binary",     # Required if connecting to PostgreSQL databases.
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = [
     "pip-tools",
 ]
```

### Comparing `py-dbcn-0.3.1/setup.cfg` & `py-dbcn-0.3.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-dbcn
-version = 0.3.1
+version = 0.3.2
 description = Connector for Pythonic interaction with multiple database types.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/py-dbcn
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_core.py` & `py-dbcn-0.3.2/tests/connectors/core/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_database.py` & `py-dbcn-0.3.2/tests/connectors/core/test_database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_display.py` & `py-dbcn-0.3.2/tests/connectors/core/test_display.py`

 * *Files 9% similar despite different names*

```diff
@@ -199,118 +199,118 @@
         self.connector.database.create(db_name, display_query=False)
         self.connector.database.use(db_name, display_query=False)
 
         with self.subTest('With no tables present'):
             # Capture logging output.
             with self.assertLogs(None, 'QUERY') as qlog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(qlog, 0), show_tables_query)
-            self.assertText(self.get_logging_output(qlog, 1), '{0}Empty Set{1}'.format(OUTPUT_RESULTS, OUTPUT_RESET))
+            self.assertText(show_tables_query, self.get_logging_output(qlog, 0))
+            self.assertText('{0}Empty Set{1}'.format(OUTPUT_RESULTS, OUTPUT_RESET), self.get_logging_output(qlog, 1))
 
         with self.subTest('Db name longer - Pt 1'):
             # Create table.
             self.connector.tables.create('category', self._columns_clause__basic, display_query=False)
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__DB_LONGER__PT_1, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('Db name longer - Pt 2'):
             # Create table.
             self.connector.tables.create('priority', self._columns_clause__basic, display_query=False)
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__DB_LONGER__PT_2, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('Db name longer - Pt 3'):
             # Create table.
             self.connector.tables.create('a', self._columns_clause__basic, display_query=False)
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__DB_LONGER__PT_3, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('Db name and table name equal length'):
             # Create table.
             self.connector.tables.create(
                 'test___{0}___this_is_a_really_long_table_name__test_'.format(self.db_type.lower()),
                 self._columns_clause__basic,
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__EQUAL_LENGTH, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('Table name longer - Pt 1'):
             # Create table.
             self.connector.tables.create(
                 'test___{0}___this_is_a_really_long_table_name__test__'.format(self.db_type.lower()),
                 self._columns_clause__basic,
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__TABLE_LONGER__PT_1, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('Table name longer - Pt 2'):
             # Create table.
             self.connector.tables.create('zzz', self._columns_clause__basic, display_query=False)
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__TABLE_LONGER__PT_2, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('Table name longer - Pt 3'):
             # Create table.
             self.connector.tables.create(
                 'test___{0}___this_is_a_really_long_table_name__testing__'.format(self.db_type.lower()),
                 self._columns_clause__basic,
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.show()
-            self.assertText(self.get_logging_output(ilog, 0), show_tables_query)
+            self.assertText(show_tables_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.SHOW__TABLE_LONGER__PT_3, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
     def test__display__describe_tables(self):
         """"""
         describe_table_query = '{0}{1}{2}'.format(OUTPUT_QUERY, self._describe_table_query, OUTPUT_RESET)
 
         # Since this directly tests display of tables, ensure we use a fresh database.
@@ -321,44 +321,44 @@
         # Create initial table to describe.
         self.connector.tables.create('category', self._columns_clause__minimal, display_query=False)
 
         with self.subTest('With only id'):
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.describe('category')
-            self.assertText(self.get_logging_output(ilog, 0), describe_table_query)
+            self.assertText(describe_table_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.DESCRIBE__COLS_ID, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With id, name'):
             # Add new table column.
             self.connector.tables.add_column('category', 'name VARCHAR(100)', display_query=False)
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.describe('category')
-            self.assertText(self.get_logging_output(ilog, 0), describe_table_query)
+            self.assertText(describe_table_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.DESCRIBE__COLS_ID_NAME, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With id, name, desc'):
             # Add new table column.
             self.connector.tables.add_column('category', 'description VARCHAR(100)', display_query=False)
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.tables.describe('category')
-            self.assertText(self.get_logging_output(ilog, 0), describe_table_query)
+            self.assertText(describe_table_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.tables.DESCRIBE__COLS_ID_NAME_DESC, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
 
 class CoreDisplayRecordsMixin:
     """
     Tests "Core" DB Connector class display logic.
     """
@@ -379,205 +379,205 @@
 
         self.connector.tables.create('category', self._columns_clause__basic, display_query=False)
 
         with self.subTest('With no records present'):
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}Empty Set{1}'.format(OUTPUT_RESULTS, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 1 record present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(1, {0}tn{0}, {0}td{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_1, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 2 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(2, {0}t n{0}, {0}t d{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_2, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 3 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(3, {0}te n{0}, {0}te d{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_3, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 4 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(4, {0}tes n{0}, {0}tes d{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_4, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 5 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(5, {0}test n{0}, {0}test d{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_5, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 6 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(6, {0}test na{0}, {0}test de{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_6, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 7 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(7, {0}test nam{0}, {0}test des{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_7, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 8 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(8, {0}test name{0}, {0}test desc{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_8, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 9 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(9, {0}test name{0}, {0}test descr{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_9, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 10 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(10, {0}test name{0}, {0}test descri{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_10, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 11 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(101, {0}test name{0}, {0}test descrip{0})'.format(self.connector.validate._quote_str_literal_format),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_11, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 12 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(1010, {0}test name{0}, {0}test descript{0})'.format(
@@ -585,18 +585,18 @@
                 ),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_12, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 13 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(10101, {0}test name{0}, {0}test descripti{0})'.format(
@@ -604,18 +604,18 @@
                 ),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_13, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 14 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(101010, {0}test name{0}, {0}test descriptio{0})'.format(
@@ -623,18 +623,18 @@
                 ),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_14, OUTPUT_RESET),
+                self.get_logging_output(ilog, 1),
             )
 
         with self.subTest('With 15 records present'):
             # Create record.
             self.connector.records.insert(
                 'category',
                 '(1010101, {0}test name{0}, {0}test description{0})'.format(
@@ -642,302 +642,302 @@
                 ),
                 display_query=False,
             )
 
             # Capture logging output.
             with self.assertLogs(None, 'INFO') as ilog:
                 self.connector.records.select('category')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query)
+            self.assertText(select_from_query, self.get_logging_output(ilog, 0))
             self.assertText(
-                self.get_logging_output(ilog, 1),
                 '{0}{1}{2}'.format(OUTPUT_RESULTS, self.expected_output.records.SELECT__PT_15, OUTPUT_RESET),
-            )
-
-    def test__display__select_records__limited(self):
-        """"""
-        select_from_query = '{0}SELECT {1} FROM category2;{2}'.format(OUTPUT_QUERY, '{0}', OUTPUT_RESET)
-        quoted_id = '{0}id{0}'.format(self.connector.validate._quote_identifier_format)
-        quoted_name = '{0}name{0}'.format(self.connector.validate._quote_identifier_format)
-        quoted_desc = '{0}description{0}'.format(self.connector.validate._quote_identifier_format)
-
-        # Create table.
-        self.connector.tables.create('category2', self._columns_clause__basic, display_query=False)
-
-        # Create record.
-        self.connector.records.insert(
-            'category2',
-            '(1, {0}longer name value{0}, {0}short desc{0})'.format(
-                self.connector.validate._quote_str_literal_format,
-            ),
-            display_query=False,
-        )
-
-        with self.subTest('With basic column types - Pull all'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query.format('*'))
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__ALL,
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With basic column types - Exclude id'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'name, description')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_name, quoted_desc))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__OMIT_ID,
-                    OUTPUT_RESET
-                ),
-            )
-
-        with self.subTest('With basic column types - Exclude name'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'id, description')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_id, quoted_desc))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__OMIT_NAME,
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With basic column types - Exclude description'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'id, name')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_id, quoted_name))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__OMIT_DESC,
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With basic column types - Pull all reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'description, name, id')
-            curr_select_clause = select_from_query.format('{0}, {1}, {2}'.format(quoted_desc, quoted_name, quoted_id))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
                 self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_ALL,
-                    OUTPUT_RESET,
-                ),
             )
 
-        with self.subTest('With basic column types - Exclude id reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'description, name')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_desc, quoted_name))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_OMIT_ID,
-                    OUTPUT_RESET
-                ),
-            )
-
-        with self.subTest('With basic column types - Exclude name reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'description, id')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_desc, quoted_id))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_OMIT_NAME,
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With basic column types - Exclude description reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category2', 'name, id')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_name, quoted_id))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_OMIT_DESC,
-                    OUTPUT_RESET,
-                ),
-            )
-
-        datetime_now = datetime.now()
-        select_from_query = '{0}SELECT {1} FROM category3;{2}'.format(OUTPUT_QUERY, '{0}', OUTPUT_RESET)
-        quoted_datetime = '{0}test_datetime{0}'.format(self.connector.validate._quote_identifier_format)
-        quoted_date = '{0}test_date{0}'.format(self.connector.validate._quote_identifier_format)
-
-        # Create table.
-        self.connector.tables.create('category3', self._columns_clause__datetime, display_query=False)
-
-        # Create record.
-        self.connector.records.insert('category3', [1, datetime_now, datetime_now], display_query=False)
-
-        with self.subTest('With datetime column types - Pull all'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3')
-            self.assertText(self.get_logging_output(ilog, 0), select_from_query.format('*'))
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__ALL.format(
-                        datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
-                        datetime_now.date(),
-                    ),
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With datetime column types - Exclude id'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'test_datetime, test_date')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_datetime, quoted_date))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__OMIT_ID.format(
-                        datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
-                        datetime_now.date(),
-                    ),
-                    OUTPUT_RESET
-                ),
-            )
-
-        with self.subTest('With datetime column types - Exclude datetime'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'id, test_date')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_id, quoted_date))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__OMIT_DATETIME.format(
-                        datetime_now.date(),
-                    ),
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With datetime column types - Exclude date'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'id, test_datetime')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_id, quoted_datetime))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__OMIT_DATE.format(
-                        datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
-                    ),
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With datetime column types - Pull all reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'test_date, test_datetime, id')
-            curr_select_clause = select_from_query.format(
-                '{0}, {1}, {2}'.format(quoted_date, quoted_datetime, quoted_id),
-            )
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_ALL.format(
-                        datetime_now.date(),
-                        datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
-                    ),
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With datetime column types - Exclude id reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'test_date, test_datetime')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_date, quoted_datetime))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_OMIT_ID.format(
-                        datetime_now.date(),
-                        datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
-                    ),
-                    OUTPUT_RESET
-                ),
-            )
-
-        with self.subTest('With datetime column types - Exclude datetime reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'test_date, id')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_date, quoted_id))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_OMIT_DATETIME.format(
-                        datetime_now.date(),
-                    ),
-                    OUTPUT_RESET,
-                ),
-            )
-
-        with self.subTest('With datetime column types - Exclude date reversed'):
-            # Capture logging output.
-            with self.assertLogs(None, 'INFO') as ilog:
-                self.connector.records.select('category3', 'test_datetime, id')
-            curr_select_clause = select_from_query.format('{0}, {1}'.format(quoted_datetime, quoted_id))
-            self.assertText(self.get_logging_output(ilog, 0), curr_select_clause)
-            self.assertText(
-                self.get_logging_output(ilog, 1),
-                '{0}{1}{2}'.format(
-                    OUTPUT_RESULTS,
-                    self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_OMIT_DATE.format(
-                        datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
-                    ),
-                    OUTPUT_RESET,
-                ),
-            )
+    # def test__display__select_records__limited(self):
+    #     """"""
+    #     select_from_query = '{0}SELECT {1} FROM category2;{2}'.format(OUTPUT_QUERY, '{0}', OUTPUT_RESET)
+    #     quoted_id = '{0}id{0}'.format(self.connector.validate._quote_identifier_format)
+    #     quoted_name = '{0}name{0}'.format(self.connector.validate._quote_identifier_format)
+    #     quoted_desc = '{0}description{0}'.format(self.connector.validate._quote_identifier_format)
+    #
+    #     # Create table.
+    #     self.connector.tables.create('category2', self._columns_clause__basic, display_query=False)
+    #
+    #     # Create record.
+    #     self.connector.records.insert(
+    #         'category2',
+    #         '(1, {0}longer name value{0}, {0}short desc{0})'.format(
+    #             self.connector.validate._quote_str_literal_format,
+    #         ),
+    #         display_query=False,
+    #     )
+    #
+    #     with self.subTest('With basic column types - Pull all'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2')
+    #         self.assertText(select_from_query.format('*'), self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             self.get_logging_output(ilog, 1),
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__ALL,
+    #                 OUTPUT_RESET,
+    #             ),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Exclude id'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'name, description')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_name, quoted_desc))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__OMIT_ID,
+    #                 OUTPUT_RESET
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Exclude name'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'id, description')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_id, quoted_desc))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__OMIT_NAME,
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Exclude description'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'id, name')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_id, quoted_name))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__OMIT_DESC,
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Pull all reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'description, name, id')
+    #         curr_select_clause = select_from_query.format('({0}, {1}, {2})'.format(quoted_desc, quoted_name, quoted_id))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_ALL,
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Exclude id reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'description, name')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_desc, quoted_name))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_OMIT_ID,
+    #                 OUTPUT_RESET
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Exclude name reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'description, id')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_desc, quoted_id))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_OMIT_NAME,
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With basic column types - Exclude description reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category2', 'name, id')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_name, quoted_id))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__BASIC__REVERSED_OMIT_DESC,
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     datetime_now = datetime.now()
+    #     select_from_query = '{0}SELECT {1} FROM category3;{2}'.format(OUTPUT_QUERY, '{0}', OUTPUT_RESET)
+    #     quoted_datetime = '{0}test_datetime{0}'.format(self.connector.validate._quote_identifier_format)
+    #     quoted_date = '{0}test_date{0}'.format(self.connector.validate._quote_identifier_format)
+    #
+    #     # Create table.
+    #     self.connector.tables.create('category3', self._columns_clause__datetime, display_query=False)
+    #
+    #     # Create record.
+    #     self.connector.records.insert('category3', [1, datetime_now, datetime_now], display_query=False)
+    #
+    #     with self.subTest('With datetime column types - Pull all'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3')
+    #         self.assertText(select_from_query.format('*'), self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__ALL.format(
+    #                     datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
+    #                     datetime_now.date(),
+    #                 ),
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Exclude id'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'test_datetime, test_date')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_datetime, quoted_date))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__OMIT_ID.format(
+    #                     datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
+    #                     datetime_now.date(),
+    #                 ),
+    #                 OUTPUT_RESET
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Exclude datetime'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'id, test_date')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_id, quoted_date))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__OMIT_DATETIME.format(
+    #                     datetime_now.date(),
+    #                 ),
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Exclude date'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'id, test_datetime')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_id, quoted_datetime))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__OMIT_DATE.format(
+    #                     datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
+    #                 ),
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Pull all reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'test_date, test_datetime, id')
+    #         curr_select_clause = select_from_query.format(
+    #             '({0}, {1}, {2})'.format(quoted_date, quoted_datetime, quoted_id),
+    #         )
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_ALL.format(
+    #                     datetime_now.date(),
+    #                     datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
+    #                 ),
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Exclude id reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'test_date, test_datetime')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_date, quoted_datetime))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_OMIT_ID.format(
+    #                     datetime_now.date(),
+    #                     datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
+    #                 ),
+    #                 OUTPUT_RESET
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Exclude datetime reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'test_date, id')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_date, quoted_id))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_OMIT_DATETIME.format(
+    #                     datetime_now.date(),
+    #                 ),
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
+    #
+    #     with self.subTest('With datetime column types - Exclude date reversed'):
+    #         # Capture logging output.
+    #         with self.assertLogs(None, 'INFO') as ilog:
+    #             self.connector.records.select('category3', 'test_datetime, id')
+    #         curr_select_clause = select_from_query.format('({0}, {1})'.format(quoted_datetime, quoted_id))
+    #         self.assertText(curr_select_clause, self.get_logging_output(ilog, 0))
+    #         self.assertText(
+    #             '{0}{1}{2}'.format(
+    #                 OUTPUT_RESULTS,
+    #                 self.expected_output.records.LIMITED_SELECT__DATETIME__REVERSED_OMIT_DATE.format(
+    #                     datetime_now.strftime('%Y-%m-%d %H:%M:%S'),
+    #                 ),
+    #                 OUTPUT_RESET,
+    #             ),
+    #             self.get_logging_output(ilog, 1),
+    #         )
```

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_query.py` & `py-dbcn-0.3.2/tests/connectors/core/test_query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_records.py` & `py-dbcn-0.3.2/tests/connectors/core/test_records.py`

 * *Files 11% similar despite different names*

```diff
@@ -871,14 +871,19 @@
         self.assertIn(row, results)
 
         # Works for 0, 1, and 2. Assume works for all further n+1 values.
 
         # Test with columns defined.
         row = (3, 'test_name_3', 'test_desc_3')
         self.connector.records.insert(table_name, row, columns_clause='id, name, description')
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+
+        # Verify two records returned.
+        self.assertEqual(len(results), 3)
+        self.assertIn(row, results)
 
     def test__insert__datetime__success(self):
         """
         Test `INSERT` query with datetime values.
         """
         table_name = 'test_queries__insert__datetime__success'
 
@@ -900,16 +905,16 @@
             day=15,
             hour=7,
             minute=12,
             second=52,
             microsecond=29,
         )
         test_date__2020 = test_datetime__2020.date()
-        test_datetime_str__2020 = test_datetime__2020.strftime('%Y-%m-%d %H:%M:%S')
-        test_date_str__2020 = test_date__2020.strftime('%Y-%m-%d')
+        test_datetime_str__2020 = "'{0}'".format(test_datetime__2020.strftime('%Y-%m-%d %H:%M:%S'))
+        test_date_str__2020 = "'{0}'".format(test_date__2020.strftime('%Y-%m-%d'))
 
         # Run test query, using string values.
         row_1 = (1, test_datetime_str__2020, test_date_str__2020)
         self.connector.records.insert(table_name, row_1)
         results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
 
         # Verify record returned.
@@ -934,19 +939,52 @@
         results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
 
         # Verify two records returned.
         self.assertEqual(len(results), 2)
         self.assertIn((1, test_datetime__2020.replace(microsecond=0), test_date__2020), results)
         self.assertIn((2, test_datetime__2021.replace(microsecond=0), test_date__2021), results)
 
-    def test__insert_many__success(self):
+    def test__insert__with_quote_types(self):
+        """"""
+        table_name = 'test_queries__insert__with_quote_types'
+
+        # Verify table exists.
+        try:
+            self.connector.query.execute('CREATE TABLE {0}{1};'.format(table_name, self._columns_clause__basic))
+        except self.connector.errors.table_already_exists:
+            # Table already exists, as we want.
+            pass
+
+        # Verify starting state.
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+        self.assertEqual(len(results), 0)
+
+        # Run test query.
+        row = (1, """2" nail""", """2 inch nail""")
+        self.connector.records.insert(table_name, row)
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+
+        # Verify one record returned.
+        self.assertEqual(len(results), 1)
+        self.assertIn(row, results)
+
+        # Run test query.
+        row = (2, """1' ruler""", """1 foot ruler""")
+        self.connector.records.insert(table_name, row)
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+
+        # Verify two records returned.
+        self.assertEqual(len(results), 2)
+        self.assertIn(row, results)
+
+    def test__insert_many__basic__success(self):
         """
         Test execute_many `INSERT` query.
         """
-        table_name = 'test_queries__insert_many__success'
+        table_name = 'test_queries__insert_many__basic__success'
 
         # Verify table exists.
         try:
             self.connector.query.execute('CREATE TABLE {0}{1};'.format(table_name, self._columns_clause__basic))
         except self.connector.errors.table_already_exists:
             # Table already exists, as we want.
             pass
@@ -1051,14 +1089,183 @@
             self.assertIn(row_5, results)
             self.assertIn(row_6, results)
             self.assertIn(row_7, results)
             self.assertIn(row_8, results)
             self.assertIn(row_9, results)
             self.assertIn(row_10, results)
 
+    def test__insert_many__datetime__success(self):
+        """
+        Test execute_many `UPDATE` query with datetime values.
+        """
+        table_name = 'test_queries__insert_many__datetime__success'
+
+        # Verify table exists.
+        try:
+            self.connector.query.execute('CREATE TABLE {0}{1};'.format(table_name, self._columns_clause__datetime))
+        except self.connector.errors.table_already_exists:
+            # Table already exists, as we want.
+            pass
+
+        # Verify starting state.
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+        self.assertEqual(len(results), 0)
+
+        # Generate datetime objects.
+        test_datetime__2020 = datetime.datetime(
+            year=2020,
+            month=6,
+            day=15,
+            hour=7,
+            minute=12,
+            second=52,
+            microsecond=0,
+        )
+        test_date__2020 = test_datetime__2020.date()
+        test_datetime__2021 = datetime.datetime(
+            year=2021,
+            month=7,
+            day=16,
+            hour=8,
+            minute=13,
+            second=53,
+            microsecond=0,
+        )
+        test_date__2021 = test_datetime__2021.date()
+        test_datetime__2022 = datetime.datetime(
+            year=2022,
+            month=8,
+            day=17,
+            hour=9,
+            minute=14,
+            second=54,
+            microsecond=0,
+        )
+        test_date__2022 = test_datetime__2022.date()
+
+        # Generate row values.
+        row_1 = (1, test_datetime__2020, test_date__2020)
+        row_2 = (2, test_datetime__2021, test_date__2021)
+        row_3 = (3, test_datetime__2022, test_date__2022)
+
+        # Generate initial rows.
+        rows = [
+            row_1,
+            row_2,
+            row_3,
+        ]
+
+        with self.subTest('With one insert'):
+            # Run test query.
+            rows = [
+                row_1,
+            ]
+            self.connector.records.insert_many(table_name, rows)
+
+            # Verify one record returned.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            self.assertEqual(len(results), 1)
+            self.assertIn(row_1, results)
+
+        # Reset table.
+        self.connector.tables.drop(table_name)
+        self.connector.tables.create(table_name, self._columns_clause__datetime)
+
+        with self.subTest('With two inserts'):
+            # Run test query.
+            rows = [
+                row_1,
+                row_2,
+            ]
+            self.connector.records.insert_many(table_name, rows)
+
+            # Verify one record returned.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            self.assertEqual(len(results), 2)
+            self.assertIn(row_1, results)
+            self.assertIn(row_2, results)
+
+        # Reset table.
+        self.connector.tables.drop(table_name)
+        self.connector.tables.create(table_name, self._columns_clause__datetime)
+
+        with self.subTest('With three inserts'):
+            # Run test query.
+            rows = [
+                row_1,
+                row_2,
+                row_3,
+            ]
+            self.connector.records.insert_many(table_name, rows)
+
+            # Verify five records returned.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            self.assertEqual(len(results), 3)
+            self.assertIn(row_1, results)
+            self.assertIn(row_2, results)
+            self.assertIn(row_3, results)
+
+        # Reset table.
+        self.connector.tables.drop(table_name)
+        self.connector.tables.create(table_name, self._columns_clause__datetime)
+
+    def test__insert_many__with_quote_types(self):
+        """"""
+        table_name = 'test_queries__insert_many__with_quote_types'
+
+        # Verify table exists.
+        try:
+            self.connector.query.execute('CREATE TABLE {0}{1};'.format(table_name, self._columns_clause__basic))
+        except self.connector.errors.table_already_exists:
+            # Table already exists, as we want.
+            pass
+
+        # Verify starting state.
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+        self.assertEqual(len(results), 0)
+
+        # Run test query.
+        row_1 = (1, """1" nail""", """1 inch nail""")
+        row_2 = (2, """2" nail""", """2 inch nail""")
+        row_3 = (3, """3" nail""", """3 inch nail""")
+        rows = [
+            row_1,
+            row_2,
+            row_3,
+        ]
+        self.connector.records.insert_many(table_name, rows)
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+
+        # Verify three records returned.
+        self.assertEqual(len(results), 3)
+        self.assertIn(row_1, results)
+        self.assertIn(row_2, results)
+        self.assertIn(row_3, results)
+
+        # Run test query.
+        row_4 = (4, """4' ruler""", """4 foot ruler""")
+        row_5 = (5, """5' ruler""", """5 foot ruler""")
+        row_6 = (6, """6' ruler""", """6 foot ruler""")
+        rows = [
+            row_4,
+            row_5,
+            row_6,
+        ]
+        self.connector.records.insert_many(table_name, rows)
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+
+        # Verify six records returned.
+        self.assertEqual(len(results), 6)
+        self.assertIn(row_1, results)
+        self.assertIn(row_2, results)
+        self.assertIn(row_3, results)
+        self.assertIn(row_4, results)
+        self.assertIn(row_5, results)
+        self.assertIn(row_6, results)
+
     def test__update__basic__success(self):
         """
         Test `UPDATE` query with basic values.
         """
         table_name = 'test_queries__update__basic__success'
 
         # Verify table exists.
@@ -1225,19 +1432,19 @@
             updated_test_datetime_str__2021 = updated_test_datetime__2021.strftime('%Y-%m-%d %H:%M:%S')
             updated_test_date_str__2021 = updated_test_date__2021.strftime('%Y-%m-%d')
 
             # Update row 2 and verify change. Use datetime str.
             self.connector.records.update(
                 table_name,
                 (
-                    'test_datetime = {1}{0}{1}, '.format(
+                    """test_datetime = {1}{0}{1}, """.format(
                         updated_test_datetime_str__2021,
                         self.connector.validate._quote_str_literal_format,
                     )
-                    + 'test_date = {1}{0}{1}'.format(
+                    + """test_date = {1}{0}{1}""".format(
                         updated_test_date_str__2021,
                         self.connector.validate._quote_str_literal_format,
                     )
                 ),
                 'id = 2',
             )
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
@@ -1268,19 +1475,19 @@
 
             # Update row 3 and verify change. Use datetime objects.
             # TODO: This isn't very useful when placed directly after above assertions.
             #   Is basically just checking for str format again. Rework after where clause is handled better.
             self.connector.records.update(
                 table_name,
                 (
-                    'test_datetime = {1}{0}{1}, '.format(
+                    """test_datetime = {1}{0}{1}, """.format(
                         updated_test_datetime__2022,
                         self.connector.validate._quote_str_literal_format,
                     )
-                    + 'test_date = {1}{0}{1}'.format(
+                    + """test_date = {1}{0}{1}""".format(
                         updated_test_date__2022,
                         self.connector.validate._quote_str_literal_format,
                     )
                 ),
                 'id = 3',
             )
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
@@ -1370,15 +1577,15 @@
             columns_clause = ['id', 'name', 'description']
             values_clause = [
                 updated_row_1,
             ]
             where_columns_clause = ['id']
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify one record returned.
+            # Verify one record updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(updated_row_1, results)
             self.assertIn(row_2, results)
             self.assertIn(row_3, results)
             self.assertIn(row_4, results)
             self.assertIn(row_5, results)
@@ -1400,15 +1607,15 @@
             values_clause = [
                 updated_row_2,
                 updated_row_3,
             ]
             where_columns_clause = ['id']
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify one record returned.
+            # Verify two records updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(row_1, results)
             self.assertIn(updated_row_2, results)
             self.assertIn(updated_row_3, results)
             self.assertIn(row_4, results)
             self.assertIn(row_5, results)
@@ -1438,15 +1645,15 @@
                 updated_row_6,
                 updated_row_7,
                 updated_row_8,
             ]
             where_columns_clause = ['name']
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify five records returned.
+            # Verify five records updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(row_1, results)
             self.assertIn(row_2, results)
             self.assertIn(row_3, results)
             self.assertIn(updated_row_4, results)
             self.assertIn(updated_row_5, results)
@@ -1466,24 +1673,24 @@
             row_5 = updated_row_5
             row_6 = updated_row_6
             row_7 = updated_row_7
             row_8 = updated_row_8
 
         with self.subTest('With ten updates'):
             # Run test query.
-            updated_row_1 = (1, '"110"', '"10010"')
-            updated_row_2 = (2, '"109"', '"10009"')
-            updated_row_3 = (3, '"108"', '"10008"')
-            updated_row_4 = (4, '"107"', '"10007"')
-            updated_row_5 = (5, '"106"', '"10006"')
-            updated_row_6 = (6, '"105"', '"10005"')
-            updated_row_7 = (7, '"104"', '"10004"')
-            updated_row_8 = (8, '"103"', '"10003"')
-            updated_row_9 = (9, '"102"', '"10002"')
-            updated_row_10 = (10, '"101"', '"10001"')
+            updated_row_1 = (1, '110', '10010')
+            updated_row_2 = (2, '109', '10009')
+            updated_row_3 = (3, '108', '10008')
+            updated_row_4 = (4, '107', '10007')
+            updated_row_5 = (5, '106', '10006')
+            updated_row_6 = (6, '105', '10005')
+            updated_row_7 = (7, '104', '10004')
+            updated_row_8 = (8, '103', '10003')
+            updated_row_9 = (9, '102', '10002')
+            updated_row_10 = (10, '101', '10001')
             columns_clause = 'id, name, description'
             values_clause = [
                 updated_row_1,
                 updated_row_2,
                 updated_row_3,
                 updated_row_4,
                 updated_row_5,
@@ -1492,15 +1699,15 @@
                 updated_row_8,
                 updated_row_9,
                 updated_row_10,
             ]
             where_columns_clause = 'id'
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify ten records returned.
+            # Verify ten records updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(updated_row_1, results)
             self.assertIn(updated_row_2, results)
             self.assertIn(updated_row_3, results)
             self.assertIn(updated_row_4, results)
             self.assertIn(updated_row_5, results)
@@ -1538,15 +1745,15 @@
             columns_clause = ['name', 'description', 'id']
             values_clause = [
                 ('name as first', 'desc as second', 3)
             ]
             where_columns_clause = ['id']
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify one record returned.
+            # Verify one record updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(row_1, results)
             self.assertIn(row_2, results)
             self.assertIn(updated_row_3, results)
             self.assertIn(row_4, results)
             self.assertIn(row_5, results)
@@ -1570,15 +1777,15 @@
                 (updated_row_5[0], updated_row_5[2]),
                 (updated_row_6[0], updated_row_6[2]),
                 (updated_row_7[0], updated_row_7[2]),
             ]
             where_columns_clause = ['id']
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify one record returned.
+            # Verify three records updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(row_1, results)
             self.assertIn(row_2, results)
             self.assertIn(row_3, results)
             self.assertIn(row_4, results)
             self.assertIn(updated_row_5, results)
@@ -1602,15 +1809,15 @@
             columns_clause = ['id', 'name', 'description']
             values_clause = [
                 updated_row_8,
             ]
             where_columns_clause = ['id', 'name']
             self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
 
-            # Verify one record returned.
+            # Verify one record updated.
             results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
             self.assertEqual(len(results), 10)
             self.assertIn(row_1, results)
             self.assertIn(row_2, results)
             self.assertIn(row_3, results)
             self.assertIn(row_4, results)
             self.assertIn(row_5, results)
@@ -1813,14 +2020,137 @@
             self.assertNotIn(row_3, results)
 
             # Update row variables.
             row_1 = updated_row_1
             row_2 = updated_row_2
             row_3 = updated_row_3
 
+    def test__update_many__with_quote_types(self):
+        """"""
+        table_name = 'test_queries__update_many__with_quote_types'
+
+        # Verify table exists.
+        try:
+            self.connector.query.execute('CREATE TABLE {0}{1};'.format(table_name, self._columns_clause__basic))
+        except self.connector.errors.table_already_exists:
+            # Table already exists, as we want.
+            pass
+
+        # Verify starting state.
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+        self.assertEqual(len(results), 0)
+
+        # Run test query.
+        row_1 = (1, """1" nail""", """1 inch nail""")
+        row_2 = (2, """2" nail""", """2 inch nail""")
+        row_3 = (3, """3" nail""", """3 inch nail""")
+        row_4 = (4, """4' ruler""", """4 foot ruler""")
+        row_5 = (5, """5' ruler""", """5 foot ruler""")
+        row_6 = (6, """6' ruler""", """6 foot ruler""")
+        rows = [
+            row_1,
+            row_2,
+            row_3,
+            row_4,
+            row_5,
+            row_6,
+        ]
+        self.connector.records.insert_many(table_name, rows)
+        results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+
+        # Verify six records returned.
+        self.assertEqual(len(results), 6)
+        self.assertIn(row_1, results)
+        self.assertIn(row_2, results)
+        self.assertIn(row_3, results)
+        self.assertIn(row_4, results)
+        self.assertIn(row_5, results)
+        self.assertIn(row_6, results)
+
+        with self.subTest('When updating away from quote types'):
+            # Run test query.
+            updated_row_2 = (2, """Some nail""", """2 inch nail""")
+            updated_row_5 = (5, """Some ruler""", """5 foot ruler""")
+            columns_clause = ['id', 'name', 'description']
+            values_clause = [
+                updated_row_2,
+                updated_row_5,
+            ]
+            where_columns_clause = ['id', 'description']
+            self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
+
+            # Verify two records updated.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            self.assertIn(row_1, results)
+            self.assertIn(updated_row_2, results)
+            self.assertIn(row_3, results)
+            self.assertIn(row_4, results)
+            self.assertIn(updated_row_5, results)
+            self.assertIn(row_6, results)
+            self.assertNotIn(row_2, results)
+            self.assertNotIn(row_5, results)
+
+            # Update row variables.
+            row_2 = updated_row_2
+            row_5 = updated_row_5
+
+        with self.subTest('When updating to use quote types'):
+            # Run test query.
+            updated_row_2 = (2, """2" nail""", """2 inch nail""")
+            updated_row_5 = (5, """5' ruler""", """5 foot ruler""")
+            columns_clause = ['id', 'name', 'description']
+            values_clause = [
+                updated_row_2,
+                updated_row_5,
+            ]
+            where_columns_clause = ['id', 'description']
+            self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
+
+            # Verify two records updated.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            self.assertIn(row_1, results)
+            self.assertIn(updated_row_2, results)
+            self.assertIn(row_3, results)
+            self.assertIn(row_4, results)
+            self.assertIn(updated_row_5, results)
+            self.assertIn(row_6, results)
+            self.assertNotIn(row_2, results)
+            self.assertNotIn(row_5, results)
+
+            # Update row variables.
+            row_2 = updated_row_2
+            row_5 = updated_row_5
+
+        with self.subTest('When matching by value with quote types'):
+            # Run test query.
+            updated_row_2 = (2, """2" nail""", """A nail description""")
+            updated_row_5 = (5, """5' ruler""", """A ruler description""")
+            columns_clause = ['id', 'name', 'description']
+            values_clause = [
+                updated_row_2,
+                updated_row_5,
+            ]
+            where_columns_clause = ['id', 'name']
+            self.connector.records.update_many(table_name, columns_clause, values_clause, where_columns_clause)
+
+            # Verify two records updated.
+            results = self.connector.query.execute('SELECT * FROM {0};'.format(table_name))
+            self.assertIn(row_1, results)
+            self.assertIn(updated_row_2, results)
+            self.assertIn(row_3, results)
+            self.assertIn(row_4, results)
+            self.assertIn(updated_row_5, results)
+            self.assertIn(row_6, results)
+            self.assertNotIn(row_2, results)
+            self.assertNotIn(row_5, results)
+
+            # Update row variables.
+            row_2 = updated_row_2
+            row_5 = updated_row_5
+
     def test__delete__success(self):
         """
         Test `DELETE` query.
         """
         table_name = 'test_queries__delete__success'
 
         # Verify table exists.
```

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_tables.py` & `py-dbcn-0.3.2/tests/connectors/core/test_tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_utils.py` & `py-dbcn-0.3.2/tests/connectors/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/core/test_validate.py` & `py-dbcn-0.3.2/tests/connectors/core/test_validate.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,16 +38,14 @@
     #             self.connector.
     #             self.connector.validate.validate_select_clause('DROP DATABASE {0}'.format(self.test_db_name_start))
     #
     #     with self.subTest('SQL Injection - Drop table'):
     #         with self.assertRaises():
     #             self.connector.validate.validate_select_clause('DROP DATABASE {0}'.format(self.test_db_name_start))
 
-
-
     def test__column_quote_format(self):
         raise NotImplementedError('Check for column quote formatting not implemented.')
 
     def test__select_identifier_quote_format(self):
         raise NotImplementedError('Check for SELECT identifier quote formatting not implemented.')
 
     def test__order_by_quote_format(self):
@@ -920,997 +918,989 @@
         converts it to the actual type/format as expected by the given database.
         """
         if self._quote_select_identifier_format is None:
             TypeError('Invalid _select_identifier_clause_format_str variable. Is None.')
 
         # None provided. Defaults back to "*".
         result = self.connector.validate.sanitize_select_identifier_clause(None)
-        self.assertText(result, '*')
+        self.assertText('*', result)
 
         # All flag provided.
         result = self.connector.validate.sanitize_select_identifier_clause('*')
-        self.assertText(result, '*')
+        self.assertText('*', result)
 
         with self.subTest('Values as str - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause('id')
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause(' id ')
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause('id, name')
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name')
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause(' id ,  name ')
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause('id, name, code')
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause(' id ,  name ,  code ')
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as triple str - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause("""id""")
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause(""" id """)
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause("""id, name""")
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause(""" id ,  name """)
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause("""id, name, code""")
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause(""" id ,  name ,  code """)
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['id'])
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause([' id '])
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['id', 'name'])
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause([' id ', ' name '])
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['id', 'name', 'code'])
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause([' id ', ' name ', ' code '])
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('id',))
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause((' id ',))
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('id', 'name'))
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause((' id ', ' name '))
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('id', 'name', 'code'))
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_select_identifier_clause((' id ', ' name ', ' code '))
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause("'id'")
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause("'id', 'name'")
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause("'id', 'name', 'code'")
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code')
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(["'id'"])
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(["'id'", "'name'"])
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(["'id'", "'name'", "'code'"])
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(("'id'",))
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(("'id'", "'name'"))
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(("'id'", "'name'", "'code'"))
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause('"id"')
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause('"id", "name"')
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause('"id", "name", code')
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['"id"'])
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['"id"', '"name"'])
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['"id"', '"name"', '"code"'])
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('"id"',))
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('"id"', '"name"'))
             self.assertText(
-                result, '{0}, {1}'.format(
+                '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('"id"', '"name"', '"code"'))
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause('`id`')
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause('`id`, `name`')
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause('`id`, `name`, `code`')
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['`id`'])
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['`id`', '`name`'])
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(['`id`', '`name`', '`code`'])
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('`id`',))
-            self.assertText(result, self._quote_select_identifier_format.format('id'))
+            self.assertText('{0}'.format(self._quote_select_identifier_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('`id`', '`name`'))
             self.assertText(
-                result,
                 '{0}, {1}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_select_identifier_clause(('`id`', '`name`', '`code`'))
             self.assertText(
-                result,
                 '{0}, {1}, {2}'.format(
                     self._quote_select_identifier_format.format('id'),
                     self._quote_select_identifier_format.format('name'),
                     self._quote_select_identifier_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as non-standard types'):
             result = self.connector.validate.sanitize_select_identifier_clause((1, True))
-            self.assertText(
-                result,
-                '{0}, {1}'.format(
-                    self._quote_select_identifier_format.format(1),
-                    self._quote_select_identifier_format.format(True),
-                ),
-            )
+            self.assertText('{0}, {1}'.format(1, True), result)
 
         with self.subTest('Values with function calls'):
             # Uppercase.
             result = self.connector.validate.sanitize_select_identifier_clause('COUNT(*)')
-            self.assertText(result, 'COUNT(*)')
+            self.assertText('COUNT(*)', result)
 
             # Lowercase.
             result = self.connector.validate.sanitize_select_identifier_clause('count(*)')
-            self.assertText(result, 'COUNT(*)')
+            self.assertText('COUNT(*)', result)
 
     def test__sanitize_select_identifier_clause__failure(self):
         """
         Test sanitizing a SELECT clause, in cases when it should fail.
         """
         # Param "*" provided with other values.
         with self.assertRaises(ValueError) as err:
             self.connector.validate.sanitize_select_identifier_clause('* , id')
         self.assertText('SELECT clause provided * with other params. * is only valid alone.', str(err.exception))
 
-        # Mistmatching quotes - double then single.
-        identifier = """\"id'"""
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_select_identifier_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier "id\'',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - single then double.
-        identifier = """'id\""""
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_select_identifier_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier \'id"',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - backtick then single.
-        identifier = "`id'"
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_select_identifier_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier `id\'',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - single then backtick.
-        identifier = "'id`"
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_select_identifier_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier \'id`',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - double then backtick.
-        identifier = '"id`'
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_select_identifier_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier "id`',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - backtick then double.
-        identifier = '`id"'
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_select_identifier_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier `id"',
-            str(err.exception),
-        )
+        # # For now, we are no longer testing this.
+        # # While uncommon, there might be legitimate cases where a string starts/ends with one quote.
+        # # Mistmatching quotes - double then single.
+        # identifier = """\"id'"""
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_select_identifier_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier "id\'',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - single then double.
+        # identifier = """'id\""""
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_select_identifier_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier \'id"',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - backtick then single.
+        # identifier = "`id'"
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_select_identifier_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier `id\'',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - single then backtick.
+        # identifier = "'id`"
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_select_identifier_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier \'id`',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - double then backtick.
+        # identifier = '"id`'
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_select_identifier_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier "id`',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - backtick then double.
+        # identifier = '`id"'
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_select_identifier_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier `id"',
+        #     str(err.exception),
+        # )
 
     def test__sanitize_columns_clause__success(self):
         """
         Test sanitizing a COLUMNS clause, in cases when it should succeed.
 
         For the most part, we test that the library gracefully handles any of
         the "standard" database quote types (', ", and `), and then properly
         converts it to the actual type/format as expected by the given database.
         """
         if self._quote_columns_format is None:
             TypeError('Invalid _columns_clause_format_str variable. Is None.')
 
         # None provided. Defaults back to empty string.
         result = self.connector.validate.sanitize_columns_clause(None)
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (single-quote str).
         result = self.connector.validate.sanitize_columns_clause('')
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (double-quote str).
         result = self.connector.validate.sanitize_columns_clause("")
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (triple double-quote str).
         result = self.connector.validate.sanitize_columns_clause("""""")
-        self.assertText(result, '')
+        self.assertText('', result)
 
         with self.subTest('Values as str - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause('id')
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(' id ')
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Single val provided and COLUMNS.
             result = self.connector.validate.sanitize_columns_clause('COLUMNS (id)')
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(' COLUMNS ( id ) ')
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause('id, name')
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name')
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(' id ,  name ')
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause('id, name, code')
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(' id ,  name ,  code ')
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as triple str - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause("""id""")
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(""" id """)
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause("""id, name""")
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(""" id ,  name """)
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause("""id, name, code""")
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause(""" id ,  name ,  code """)
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(['id'])
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause([' id '])
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(['id', 'name'])
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause([' id ', ' name '])
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(['id', 'name', 'code'])
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause([' id ', ' name ', ' code '])
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(('id',))
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause((' id ',))
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(('id', 'name'))
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause((' id ', ' name '))
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(('id', 'name', 'code'))
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_columns_clause((' id ', ' name ', ' code '))
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause("'id'")
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause("'id', 'name'")
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause("'id', 'name', 'code'")
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code')
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(["'id'"])
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(["'id'", "'name'"])
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(["'id'", "'name'", "'code'"])
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(("'id'",))
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(("'id'", "'name'"))
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(("'id'", "'name'", "'code'"))
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause('"id"')
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause('"id", "name"')
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause('"id", "name", code')
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(['"id"'])
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(['"id"', '"name"'])
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(['"id"', '"name"', '"code"'])
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(('"id"',))
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(('"id"', '"name"'))
             self.assertText(
-                result, '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(('"id"', '"name"', '"code"'))
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause('`id`')
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause('`id`, `name`')
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause('`id`, `name`, `code`')
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(['`id`'])
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(['`id`', '`name`'])
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(['`id`', '`name`', '`code`'])
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_columns_clause(('`id`',))
-            self.assertText(result, self._quote_columns_format.format('id'))
+            self.assertText('({0})'.format(self._quote_columns_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_columns_clause(('`id`', '`name`'))
             self.assertText(
-                result,
-                '{0}, {1}'.format(
+                '({0}, {1})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_columns_clause(('`id`', '`name`', '`code`'))
             self.assertText(
-                result,
-                '{0}, {1}, {2}'.format(
+                '({0}, {1}, {2})'.format(
                     self._quote_columns_format.format('id'),
                     self._quote_columns_format.format('name'),
                     self._quote_columns_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as non-standard types'):
             # TODO: Should these fail? These probably should fail.
             #  I think only literal column names should work.
             result = self.connector.validate.sanitize_columns_clause((1, True))
-            self.assertText(
-                result,
-                '{0}, {1}'.format(
-                    self._quote_columns_format.format(1),
-                    self._quote_columns_format.format(True),
-                ),
-            )
+            self.assertText('({0}, {1})'.format(1, True), result)
 
     def test__sanitize_columns_clause__failure(self):
         """
         Test sanitizing a COLUMNS clause, in cases when it should fail.
         """
         # Param "*" provided.
         with self.assertRaises(ValueError) as err:
@@ -1918,67 +1908,69 @@
         self.assertText('The * identifier can only be used in a SELECT clause.', str(err.exception))
 
         # Param "*" provided with other values.
         with self.assertRaises(ValueError) as err:
             self.connector.validate.sanitize_columns_clause('* , id')
         self.assertText('The * identifier can only be used in a SELECT clause.', str(err.exception))
 
-        # Mistmatching quotes - double then single.
-        identifier = """\"id'"""
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_columns_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier "id\'',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - single then double.
-        identifier = """'id\""""
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_columns_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier \'id"',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - backtick then single.
-        identifier = "`id'"
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_columns_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier `id\'',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - single then backtick.
-        identifier = "'id`"
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_columns_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier \'id`',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - double then backtick.
-        identifier = '"id`'
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_columns_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier "id`',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - backtick then double.
-        identifier = '`id"'
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_columns_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier `id"',
-            str(err.exception),
-        )
+        # # For now, we are no longer testing this.
+        # # While uncommon, there might be legitimate cases where a string starts/ends with one quote.
+        # # Mistmatching quotes - double then single.
+        # identifier = """\"id'"""
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_columns_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier "id\'',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - single then double.
+        # identifier = """'id\""""
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_columns_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier \'id"',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - backtick then single.
+        # identifier = "`id'"
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_columns_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier `id\'',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - single then backtick.
+        # identifier = "'id`"
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_columns_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier \'id`',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - double then backtick.
+        # identifier = '"id`'
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_columns_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier "id`',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - backtick then double.
+        # identifier = '`id"'
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_columns_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier `id"',
+        #     str(err.exception),
+        # )
 
     # def test__sanitize_values_clause__success(self):
     #     """
     #     Test sanitizing a VALUES clause, in cases when it should succeed.
     #
     #     For the most part, we test that the library gracefully handles any of
     #     the "standard" database quote types (', ", and `), and then properly
@@ -1988,600 +1980,600 @@
     #         TypeError('Invalid _columns_clause_format_str variable. Is None.')
     #
     #     with self.subTest('Values as str - Without quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause('id')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(' id ')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES id')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause('values id')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES (id)')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause('values (id)')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause('id, name')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(' id ,  name ')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES id, name')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause('values id, name')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES (id, name)')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause('values (id, name)')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause('id, name, code')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(' id ,  name ,  code ')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES id, name, code')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause('values id, name, code')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES (id, name, code)')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause('values (id, name, code)')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #     with self.subTest('Values as triple str - Without quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause("""id""")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(""" id """)
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause("""VALUES id""")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause("""values id""")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause("""VALUES (id)""")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause("""values (id)""")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause("""id, name""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(""" id , name """)
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause("""VALUES id, name""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause("""values id, name""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause("""VALUES (id, name)""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause("""values (id, name)""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause("""id, name, code""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(""" id , name , code """)
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause("""VALUES id, name, code""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause("""values id, name, code""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause("""VALUES (id, name, code)""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause("""values (id, name, code)""")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #     with self.subTest('Values as list - Without quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(['id'])
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause([' id '])
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(['id', 'name'])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause([' id ', ' name '])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(['id', 'name', 'code'])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause([' id ', ' name ', ' code '])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                     self._quote_str_literal_format.format(' code '),
     #                 ),
+    #                 result,
     #             )
     #
     #     with self.subTest('Values as tuple - Without quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(('id',))
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause((' id ',))
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(('id', 'name'))
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause((' id ', ' name '))
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(('id', 'name', 'code'))
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause((' id ', ' name ', ' code '))
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                     self._quote_str_literal_format.format(' code '),
     #                 ),
+    #                 result,
     #             )
     #
     #     with self.subTest('Values as str - With single quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause("'id'")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(" ' id ' ")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')), result)
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause("VALUES 'id'")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause("values 'id'")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause("VALUES ('id')")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause("values ('id')")
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause("'id', 'name'")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(" ' id ' , ' name ' ")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause("VALUES 'id', 'name',")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause("values 'id', 'name'")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause("VALUES ('id', 'name')")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause("values ('id', 'name')")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause("'id', 'name', 'code'")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(" ' id ' , ' name ' , ' code ' ")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                     self._quote_str_literal_format.format(' code '),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause("VALUES 'id', 'name', 'code'")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause("values 'id', 'name', 'code'")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause("VALUES ('id', 'name', 'code')")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause("values ('id', 'name', 'code')")
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #     # with self.subTest('Values as list - With single quotes'):
     #     #
     #     #     with self.subTest('Single val provided'):
     #     #         # Base value.
     #     #         print('\n\n\n\n\n\n\n\n\n\n\n\n\n')
     #     #         # All of these tokenize to the same thing? Okay then...
     #     #         # TODO: Figure out how to tokenize this as expected.
     #     #         result = self.connector.validate.sanitize_values_clause('id')
     #     #         result = self.connector.validate.sanitize_values_clause("id")
     #     #         result = self.connector.validate.sanitize_values_clause("'id'")
     #     #         result = self.connector.validate.sanitize_values_clause(["'id'"])
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format("'id'")))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format("'id'")))
     #     #
     #     #         # With extra whitespace.
     #     #         result = self.connector.validate.sanitize_values_clause([" ' id ' "])
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(" ' id ' ")))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(" ' id ' ")))
     #     #
     #     #     with self.subTest('Two vals provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(["'id'", "'name'"])
     #     #         self.assertText(
     #     #             result,
     #     #             '\nVALUES ({0}, {1})'.format(
@@ -2624,19 +2616,19 @@
     #     #         )
     #
     #     # with self.subTest('Values as tuple - With single quotes'):
     #     #
     #     #     with self.subTest('Single val provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(("'id'",))
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format("'id'")))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format("'id'")))
     #     #
     #     #         # With extra whitespace.
     #     #         result = self.connector.validate.sanitize_values_clause((" ' id ' ",))
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(" ' id ' ")))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(" ' id ' ")))
     #     #
     #     #     with self.subTest('Two vals provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(("'id'", "'name'"))
     #     #         self.assertText(
     #     #             result,
     #     #             '\nVALUES ({0}, {1})'.format(
@@ -2679,297 +2671,297 @@
     #     #         )
     #
     #     with self.subTest('Values as str - With double quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause('"id"')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(' " id " ')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' id ')), result)
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES "id"')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause('values "id"')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES ("id")')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause('values ("id")')
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('id')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause('"id", "name"')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(' " id " , " name " ')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES "id", "name"')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause('values "id", "name"')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES ("id", "name")')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause('values ("id", "name")')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause('"id", "name", "code"')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause(' " id " , " name " , " code " ')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format(' id '),
     #                     self._quote_str_literal_format.format(' name '),
     #                     self._quote_str_literal_format.format(' code '),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, no parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES "id", "name", "code"')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, no parens.
     #             result = self.connector.validate.sanitize_values_clause('values "id", "name", "code"')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - upper, with parens.
     #             result = self.connector.validate.sanitize_values_clause('VALUES ("id", "name", "code")')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With full statement - lower, with parens.
     #             result = self.connector.validate.sanitize_values_clause('values ("id", "name", "code")')
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('id'),
     #                     self._quote_str_literal_format.format('name'),
     #                     self._quote_str_literal_format.format('code'),
     #                 ),
+    #                 result,
     #             )
     #
     #     with self.subTest('Values as list - With double quotes'):
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(['"id"'])
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('"id"')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('"id"')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause([' " id " '])
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' " id " ')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' " id " ')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(['"id"', '"name"'])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('"id"'),
     #                     self._quote_str_literal_format.format('"name"'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause([' " id " ', ' " name " '])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format(' " id " '),
     #                     self._quote_str_literal_format.format(' " name " '),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(['"id"', '"name"', '"code"'])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('"id"'),
     #                     self._quote_str_literal_format.format('"name"'),
     #                     self._quote_str_literal_format.format('"code"'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause([' " id " ', ' " name " ', ' " code " '])
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format(' " id " '),
     #                     self._quote_str_literal_format.format(' " name " '),
     #                     self._quote_str_literal_format.format(' " code " '),
     #                 ),
+    #                 result,
     #             )
     #
     #     with self.subTest('Values as tuple - With double quotes'):
     #
     #         with self.subTest('Single val provided'):
     #             # Base value.
     #             result = self.connector.validate.sanitize_values_clause(('"id"',))
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('"id"')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('"id"')), result)
     #
     #             # With extra whitespace.
     #             result = self.connector.validate.sanitize_values_clause((' " id " ',))
-    #             self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' " id " ')))
+    #             self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' " id " ')), result)
     #
     #         with self.subTest('Two vals provided'):
     #             # Base value.
-    #             result = self.connector.validate.sanitize_values_clause(('"id"', '"name"'))
-    #             self.assertText(
-    #                 result, '\nVALUES ({0}, {1})'.format(
+    #             result = self.connector.validate.sanitize_values_clause(('"id"', '"name"'), result)
+    #             self.assertText( '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format('"id"'),
     #                     self._quote_str_literal_format.format('"name"'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
-    #             result = self.connector.validate.sanitize_values_clause((' " id " ', ' " name " '))
-    #             self.assertText(
-    #                 result, '\nVALUES ({0}, {1})'.format(
+    #             result = self.connector.validate.sanitize_values_clause((' " id " ', ' " name " '), result)
+    #             self.assertText( '\nVALUES ({0}, {1})'.format(
     #                     self._quote_str_literal_format.format(' " id " '),
     #                     self._quote_str_literal_format.format(' " name " '),
     #                 ),
+    #                 result,
     #             )
     #
     #         with self.subTest('Three vals provided'):
     #             # Base value.
-    #             result = self.connector.validate.sanitize_values_clause(('"id"', '"name"', '"code"'))
+    #             result = self.connector.validate.sanitize_values_clause(('"id"', '"name"', '"code"'), result)
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format('"id"'),
     #                     self._quote_str_literal_format.format('"name"'),
     #                     self._quote_str_literal_format.format('"code"'),
     #                 ),
+    #                 result,
     #             )
     #
     #             # With extra whitespace.
-    #             result = self.connector.validate.sanitize_values_clause((' " id " ', ' " name " ', ' " code " '))
+    #             result = self.connector.validate.sanitize_values_clause((' " id " ', ' " name " ', ' " code " '), result)
     #             self.assertText(
-    #                 result,
     #                 '\nVALUES ({0}, {1}, {2})'.format(
     #                     self._quote_str_literal_format.format(' " id " '),
     #                     self._quote_str_literal_format.format(' " name " '),
     #                     self._quote_str_literal_format.format(' " code " '),
     #                 ),
+    #                 result,
     #             )
     #
     #     # with self.subTest('Values as str - With backtick quotes'):
     #     #
     #     #     with self.subTest('Single val provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause('`id`')
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #         # With extra whitespace.
     #     #         result = self.connector.validate.sanitize_values_clause(' ` id ` ')
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('` id `')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('` id `')))
     #     #
     #     #         # With full statement - upper, no parens.
     #     #         result = self.connector.validate.sanitize_values_clause('VALUES `id`')
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #         # With full statement - lower, no parens.
     #     #         result = self.connector.validate.sanitize_values_clause('values `id`')
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #         # With full statement - upper, no parens.
     #     #         result = self.connector.validate.sanitize_values_clause('VALUES `id`')
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #         # With full statement - lower, no parens.
     #     #         result = self.connector.validate.sanitize_values_clause('values `id`')
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #     with self.subTest('Two vals provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause('`id`, `name`')
     #     #         self.assertText(
     #     #             result,
     #     #             '\nVALUES ({0}, {1})'.format(
@@ -3096,19 +3088,19 @@
     #     #         )
     #
     #     # with self.subTest('Values as list - With backtick quotes'):
     #     #
     #     #     with self.subTest('Single val provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(['`id`'])
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #         # With extra whitespace.
     #     #         result = self.connector.validate.sanitize_values_clause([' ` id ` '])
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('` id `')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('` id `')))
     #     #
     #     #     with self.subTest('Two vals provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(['`id`', '`name`'])
     #     #         self.assertText(
     #     #             result,
     #     #             '\nVALUES ({0}, {1})'.format(
@@ -3151,19 +3143,19 @@
     #     #         )
     #
     #     # with self.subTest('Values as tuple - With backtick quotes'):
     #     #
     #     #     with self.subTest('Single val provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(('`id`',))
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format('`id`')))
     #     #
     #     #         # With extra whitespace.
     #     #         result = self.connector.validate.sanitize_values_clause((' ` id ` ',))
-    #     #         self.assertText(result, '\nVALUES ({0})'.format(self._quote_str_literal_format.format(' ` id ` ')))
+    #     #         self.assertText('\nVALUES ({0})'.format(self._quote_str_literal_format.format(' ` id ` ')))
     #     #
     #     #     with self.subTest('Two vals provided'):
     #     #         # Base value.
     #     #         result = self.connector.validate.sanitize_values_clause(('`id`', '`name`'))
     #     #         self.assertText(
     #     #             result,
     #     #             '\nVALUES ({0}, {1})'.format(
@@ -3204,19 +3196,19 @@
     #     #                 self._quote_str_literal_format.format(' ` code ` '),
     #     #             ),
     #     #         )
     #
     #     with self.subTest('Values as non-standard types'):
     #         result = self.connector.validate.sanitize_values_clause((1, True))
     #         self.assertText(
-    #             result,
     #             '\nVALUES ({0}, {1})'.format(
     #                 1,
     #                 True,
     #             ),
+    #             result,
     #         )
     #
     #     # # Mistmatching quotes - double then single.
     #     # identifier = """\"id'"""
     #     # result = self.connector.validate.sanitize_values_clause(identifier)
     #     # self.assertText(
     #     #     'Found mismatching quotes for identifier "id\'',
@@ -3314,641 +3306,630 @@
         converts it to the actual type/format as expected by the given database.
         """
         if self._quote_columns_format is None:
             TypeError('Invalid _columns_clause_format_str variable. Is None.')
 
         # None provided. Defaults back to empty string.
         result = self.connector.validate.sanitize_order_by_clause(None)
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (single-quote str).
         result = self.connector.validate.sanitize_order_by_clause('')
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (double-quote str).
         result = self.connector.validate.sanitize_order_by_clause("")
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (triple double-quote str).
         result = self.connector.validate.sanitize_order_by_clause("""""")
-        self.assertText(result, '')
+        self.assertText('', result)
 
         with self.subTest('Values as str - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause('id')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause(' id ')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - upper.
             result = self.connector.validate.sanitize_order_by_clause('ORDER BY id')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - lower.
             result = self.connector.validate.sanitize_order_by_clause('order by id')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause('id, name')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name')
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause(' id ,  name ')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause('id, name, code')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause(' id ,  name ,  code ')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as triple str - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause("""id""")
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause(""" id """)
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - upper.
             result = self.connector.validate.sanitize_order_by_clause("""ORDER BY id""")
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - lower.
             result = self.connector.validate.sanitize_order_by_clause("""order by id""")
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause("""id, name""")
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause(""" id ,  name """)
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause("""id, name, code""")
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause(""" id ,  name ,  code """)
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(['id'])
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause([' id '])
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(['id', 'name'])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause([' id ', ' name '])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(['id', 'name', 'code'])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause([' id ', ' name ', ' code '])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - Without quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(('id',))
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause((' id ',))
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(('id', 'name'))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause((' id ', ' name '))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(('id', 'name', 'code'))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
             # With extra whitespace.
             result = self.connector.validate.sanitize_order_by_clause((' id ', ' name ', ' code '))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause("'id'")
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - upper.
             result = self.connector.validate.sanitize_order_by_clause("ORDER BY 'id'")
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - lower.
             result = self.connector.validate.sanitize_order_by_clause("order by 'id'")
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause("'id', 'name'")
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause("'id', 'name', 'code'")
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code')
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(["'id'"])
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(["'id'", "'name'"])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(["'id'", "'name'", "'code'"])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With single quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(("'id'",))
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(("'id'", "'name'"))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(("'id'", "'name'", "'code'"))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause('"id"')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - upper.
             result = self.connector.validate.sanitize_order_by_clause('ORDER BY "id"')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - lower.
             result = self.connector.validate.sanitize_order_by_clause('order by "id"')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause('"id", "name"')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause('"id", "name", code')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(['"id"'])
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(['"id"', '"name"'])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(['"id"', '"name"', '"code"'])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With double quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(('"id"',))
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(('"id"', '"name"'))
             self.assertText(
                 result, '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(('"id"', '"name"', '"code"'))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as str - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause('`id`')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - upper.
             result = self.connector.validate.sanitize_order_by_clause('ORDER BY `id`')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
             # With full statement - lower.
             result = self.connector.validate.sanitize_order_by_clause('order by `id`')
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause('`id`, `name`')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause('`id`, `name`, `code`')
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as list - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(['`id`'])
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(['`id`', '`name`'])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(['`id`', '`name`', '`code`'])
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as tuple - With backtick quotes'):
             # Single val provided.
             result = self.connector.validate.sanitize_order_by_clause(('`id`',))
-            self.assertText(result, '\nORDER BY {0}'.format(self._quote_order_by_format.format('id')))
+            self.assertText('\nORDER BY {0}'.format(self._quote_order_by_format.format('id')), result)
 
             # Two vals provided.
             result = self.connector.validate.sanitize_order_by_clause(('`id`', '`name`'))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                 ),
+                result,
             )
 
             # Three vals provided.
             result = self.connector.validate.sanitize_order_by_clause(('`id`', '`name`', '`code`'))
             self.assertText(
-                result,
                 '\nORDER BY {0}, {1}, {2}'.format(
                     self._quote_order_by_format.format('id'),
                     self._quote_order_by_format.format('name'),
                     self._quote_order_by_format.format('code'),
                 ),
+                result,
             )
 
         with self.subTest('Values as non-standard types'):
             # TODO: Should these fail? These probably should fail.
             #  I think only literal column names should work.
             result = self.connector.validate.sanitize_order_by_clause((1, True))
-            self.assertText(
-                result,
-                '\nORDER BY {0}, {1}'.format(
-                    self._quote_order_by_format.format(1),
-                    self._quote_order_by_format.format(True),
-                ),
-            )
+            self.assertText('\nORDER BY {0}, {1}'.format(1, True), result)
 
     def test__sanitize_order_by_clause__failure(self):
         """
         Test sanitizing an ORDER BY clause, in cases when it should fail.
         """
-        # "ORDER BY" provided without any additional values.
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause('ORDER BY')
-        self.assertText('Invalid ORDER BY clause.', str(err.exception))
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause('   ORDER BY   ')
-        self.assertText('Invalid ORDER BY clause.', str(err.exception))
-
         # Param "*" provided.
         with self.assertRaises(ValueError) as err:
             self.connector.validate.sanitize_order_by_clause('*')
         self.assertText('The * identifier can only be used in a SELECT clause.', str(err.exception))
 
         # Param "*" provided with other values.
         with self.assertRaises(ValueError) as err:
             self.connector.validate.sanitize_order_by_clause('* , id')
         self.assertText('The * identifier can only be used in a SELECT clause.', str(err.exception))
 
-        # Mistmatching quotes - double then single.
-        identifier = """\"id'"""
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier "id\'',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - single then double.
-        identifier = """'id\""""
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier \'id"',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - backtick then single.
-        identifier = "`id'"
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier `id\'',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - single then backtick.
-        identifier = "'id`"
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier \'id`',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - double then backtick.
-        identifier = '"id`'
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier "id`',
-            str(err.exception),
-        )
-
-        # Mistmatching quotes - backtick then double.
-        identifier = '`id"'
-        with self.assertRaises(ValueError) as err:
-            self.connector.validate.sanitize_order_by_clause(identifier)
-        self.assertText(
-            'Found mismatching quotes for identifier `id"',
-            str(err.exception),
-        )
+        # # For now, we are no longer testing this.
+        # # While uncommon, there might be legitimate cases where a string starts/ends with one quote.
+        # # Mistmatching quotes - double then single.
+        # identifier = """\"id'"""
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_order_by_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier "id\'',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - single then double.
+        # identifier = """'id\""""
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_order_by_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier \'id"',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - backtick then single.
+        # identifier = "`id'"
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_order_by_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier `id\'',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - single then backtick.
+        # identifier = "'id`"
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_order_by_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier \'id`',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - double then backtick.
+        # identifier = '"id`'
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_order_by_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier "id`',
+        #     str(err.exception),
+        # )
+        #
+        # # Mistmatching quotes - backtick then double.
+        # identifier = '`id"'
+        # with self.assertRaises(ValueError) as err:
+        #     self.connector.validate.sanitize_order_by_clause(identifier)
+        # self.assertText(
+        #     'Found mismatching quotes for identifier `id"',
+        #     str(err.exception),
+        # )
 
     def test__sanitize_limit_clause__success(self):
         """
         Test sanitizing a LIMIT clause, in cases when it should succeed.
         """
         # None provided. Defaults back to empty string.
         result = self.connector.validate.sanitize_limit_clause(None)
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (single-quote str).
         result = self.connector.validate.sanitize_limit_clause('')
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (double-quote str).
         result = self.connector.validate.sanitize_limit_clause("")
-        self.assertText(result, '')
+        self.assertText('', result)
 
         # Empty string provided (triple double-quote str).
         result = self.connector.validate.sanitize_limit_clause("""""")
-        self.assertText(result, '')
+        self.assertText('', result)
 
         with self.subTest('Limit of 1 (lowest acceptable limit)'):
             # As int.
             result = self.connector.validate.sanitize_limit_clause(1)
-            self.assertText(result, ' LIMIT 1')
+            self.assertText(' LIMIT 1', result)
 
             # As str.
             result = self.connector.validate.sanitize_limit_clause('1')
-            self.assertText(result, ' LIMIT 1')
+            self.assertText(' LIMIT 1', result)
 
             # As full str (upper).
             result = self.connector.validate.sanitize_limit_clause('LIMIT 1')
-            self.assertText(result, ' LIMIT 1')
+            self.assertText(' LIMIT 1', result)
 
             # As full str (lower).
             result = self.connector.validate.sanitize_limit_clause('limit 1')
-            self.assertText(result, ' LIMIT 1')
+            self.assertText(' LIMIT 1', result)
 
         with self.subTest('Limit of 2'):
             # As int.
             result = self.connector.validate.sanitize_limit_clause(2)
-            self.assertText(result, ' LIMIT 2')
+            self.assertText(' LIMIT 2', result)
 
             # As str.
             result = self.connector.validate.sanitize_limit_clause('2')
-            self.assertText(result, ' LIMIT 2')
+            self.assertText(' LIMIT 2', result)
 
             # As full str (upper).
             result = self.connector.validate.sanitize_limit_clause('LIMIT 2')
-            self.assertText(result, ' LIMIT 2')
+            self.assertText(' LIMIT 2', result)
 
             # As full str (lower).
             result = self.connector.validate.sanitize_limit_clause('limit 2')
-            self.assertText(result, ' LIMIT 2')
+            self.assertText(' LIMIT 2', result)
 
         with self.subTest('Limit of 100'):
             # As int.
             result = self.connector.validate.sanitize_limit_clause(100)
-            self.assertText(result, ' LIMIT 100')
+            self.assertText(' LIMIT 100', result)
 
             # As str.
             result = self.connector.validate.sanitize_limit_clause('100')
-            self.assertText(result, ' LIMIT 100')
+            self.assertText(' LIMIT 100', result)
 
             # As full str (upper).
             result = self.connector.validate.sanitize_limit_clause('LIMIT 100')
-            self.assertText(result, ' LIMIT 100')
+            self.assertText(' LIMIT 100', result)
 
             # As full str (lower).
             result = self.connector.validate.sanitize_limit_clause('limit 100')
-            self.assertText(result, ' LIMIT 100')
+            self.assertText(' LIMIT 100', result)
 
     def test__sanitize_limit_clause__failure(self):
         """
         Test sanitizing a LIMIT clause, in cases when it should fail.
         """
         # Zero provided.
         with self.assertRaises(ValueError) as err:
```

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/constants.py` & `py-dbcn-0.3.2/tests/connectors/mysql/constants.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/expected_display_output.py` & `py-dbcn-0.3.2/tests/connectors/mysql/expected_display_output.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_core.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_database.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_display.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_query.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_records.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_tables.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_utils.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/mysql/test_validate.py` & `py-dbcn-0.3.2/tests/connectors/mysql/test_validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/constants.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/constants.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/expected_display_output.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/expected_display_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -123,247 +123,247 @@
 
 # region Record Display Output
 
 EXPECTED__RECORD__SELECT__PT_1 = """
 +----+------+-------------+
 | id | name | description |
 +----+------+-------------+
-| 1  | tn   | td          |
+| 1  | 'tn' | 'td'        |
 +----+------+-------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_2 = """
-+----+------+-------------+
-| id | name | description |
-+----+------+-------------+
-| 1  | tn   | td          |
-| 2  | t n  | t d         |
-+----+------+-------------+
-""".strip()
-
-
-EXPECTED__RECORD__SELECT__PT_3 = """
-+----+------+-------------+
-| id | name | description |
-+----+------+-------------+
-| 1  | tn   | td          |
-| 2  | t n  | t d         |
-| 3  | te n | te d        |
-+----+------+-------------+
-""".strip()
-
-
-EXPECTED__RECORD__SELECT__PT_4 = """
 +----+-------+-------------+
 | id | name  | description |
 +----+-------+-------------+
-| 1  | tn    | td          |
-| 2  | t n   | t d         |
-| 3  | te n  | te d        |
-| 4  | tes n | tes d       |
+| 1  | 'tn'  | 'td'        |
+| 2  | 't n' | 't d'       |
 +----+-------+-------------+
 """.strip()
 
 
-EXPECTED__RECORD__SELECT__PT_5 = """
+EXPECTED__RECORD__SELECT__PT_3 = """
 +----+--------+-------------+
 | id | name   | description |
 +----+--------+-------------+
-| 1  | tn     | td          |
-| 2  | t n    | t d         |
-| 3  | te n   | te d        |
-| 4  | tes n  | tes d       |
-| 5  | test n | test d      |
+| 1  | 'tn'   | 'td'        |
+| 2  | 't n'  | 't d'       |
+| 3  | 'te n' | 'te d'      |
 +----+--------+-------------+
 """.strip()
 
 
-EXPECTED__RECORD__SELECT__PT_6 = """
+EXPECTED__RECORD__SELECT__PT_4 = """
 +----+---------+-------------+
 | id | name    | description |
 +----+---------+-------------+
-| 1  | tn      | td          |
-| 2  | t n     | t d         |
-| 3  | te n    | te d        |
-| 4  | tes n   | tes d       |
-| 5  | test n  | test d      |
-| 6  | test na | test de     |
+| 1  | 'tn'    | 'td'        |
+| 2  | 't n'   | 't d'       |
+| 3  | 'te n'  | 'te d'      |
+| 4  | 'tes n' | 'tes d'     |
 +----+---------+-------------+
 """.strip()
 
 
-EXPECTED__RECORD__SELECT__PT_7 = """
+EXPECTED__RECORD__SELECT__PT_5 = """
 +----+----------+-------------+
 | id | name     | description |
 +----+----------+-------------+
-| 1  | tn       | td          |
-| 2  | t n      | t d         |
-| 3  | te n     | te d        |
-| 4  | tes n    | tes d       |
-| 5  | test n   | test d      |
-| 6  | test na  | test de     |
-| 7  | test nam | test des    |
+| 1  | 'tn'     | 'td'        |
+| 2  | 't n'    | 't d'       |
+| 3  | 'te n'   | 'te d'      |
+| 4  | 'tes n'  | 'tes d'     |
+| 5  | 'test n' | 'test d'    |
 +----+----------+-------------+
 """.strip()
 
 
-EXPECTED__RECORD__SELECT__PT_8 = """
+EXPECTED__RECORD__SELECT__PT_6 = """
 +----+-----------+-------------+
 | id | name      | description |
 +----+-----------+-------------+
-| 1  | tn        | td          |
-| 2  | t n       | t d         |
-| 3  | te n      | te d        |
-| 4  | tes n     | tes d       |
-| 5  | test n    | test d      |
-| 6  | test na   | test de     |
-| 7  | test nam  | test des    |
-| 8  | test name | test desc   |
+| 1  | 'tn'      | 'td'        |
+| 2  | 't n'     | 't d'       |
+| 3  | 'te n'    | 'te d'      |
+| 4  | 'tes n'   | 'tes d'     |
+| 5  | 'test n'  | 'test d'    |
+| 6  | 'test na' | 'test de'   |
 +----+-----------+-------------+
 """.strip()
 
 
+EXPECTED__RECORD__SELECT__PT_7 = """
++----+------------+-------------+
+| id | name       | description |
++----+------------+-------------+
+| 1  | 'tn'       | 'td'        |
+| 2  | 't n'      | 't d'       |
+| 3  | 'te n'     | 'te d'      |
+| 4  | 'tes n'    | 'tes d'     |
+| 5  | 'test n'   | 'test d'    |
+| 6  | 'test na'  | 'test de'   |
+| 7  | 'test nam' | 'test des'  |
++----+------------+-------------+
+""".strip()
+
+
+EXPECTED__RECORD__SELECT__PT_8 = """
++----+-------------+-------------+
+| id | name        | description |
++----+-------------+-------------+
+| 1  | 'tn'        | 'td'        |
+| 2  | 't n'       | 't d'       |
+| 3  | 'te n'      | 'te d'      |
+| 4  | 'tes n'     | 'tes d'     |
+| 5  | 'test n'    | 'test d'    |
+| 6  | 'test na'   | 'test de'   |
+| 7  | 'test nam'  | 'test des'  |
+| 8  | 'test name' | 'test desc' |
++----+-------------+-------------+
+""".strip()
+
+
 EXPECTED__RECORD__SELECT__PT_9 = """
-+----+-----------+-------------+
-| id | name      | description |
-+----+-----------+-------------+
-| 1  | tn        | td          |
-| 2  | t n       | t d         |
-| 3  | te n      | te d        |
-| 4  | tes n     | tes d       |
-| 5  | test n    | test d      |
-| 6  | test na   | test de     |
-| 7  | test nam  | test des    |
-| 8  | test name | test desc   |
-| 9  | test name | test descr  |
-+----+-----------+-------------+
++----+-------------+--------------+
+| id | name        | description  |
++----+-------------+--------------+
+| 1  | 'tn'        | 'td'         |
+| 2  | 't n'       | 't d'        |
+| 3  | 'te n'      | 'te d'       |
+| 4  | 'tes n'     | 'tes d'      |
+| 5  | 'test n'    | 'test d'     |
+| 6  | 'test na'   | 'test de'    |
+| 7  | 'test nam'  | 'test des'   |
+| 8  | 'test name' | 'test desc'  |
+| 9  | 'test name' | 'test descr' |
++----+-------------+--------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_10 = """
-+----+-----------+-------------+
-| id | name      | description |
-+----+-----------+-------------+
-| 1  | tn        | td          |
-| 2  | t n       | t d         |
-| 3  | te n      | te d        |
-| 4  | tes n     | tes d       |
-| 5  | test n    | test d      |
-| 6  | test na   | test de     |
-| 7  | test nam  | test des    |
-| 8  | test name | test desc   |
-| 9  | test name | test descr  |
-| 10 | test name | test descri |
-+----+-----------+-------------+
++----+-------------+---------------+
+| id | name        | description   |
++----+-------------+---------------+
+| 1  | 'tn'        | 'td'          |
+| 2  | 't n'       | 't d'         |
+| 3  | 'te n'      | 'te d'        |
+| 4  | 'tes n'     | 'tes d'       |
+| 5  | 'test n'    | 'test d'      |
+| 6  | 'test na'   | 'test de'     |
+| 7  | 'test nam'  | 'test des'    |
+| 8  | 'test name' | 'test desc'   |
+| 9  | 'test name' | 'test descr'  |
+| 10 | 'test name' | 'test descri' |
++----+-------------+---------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_11 = """
-+-----+-----------+--------------+
-| id  | name      | description  |
-+-----+-----------+--------------+
-| 1   | tn        | td           |
-| 2   | t n       | t d          |
-| 3   | te n      | te d         |
-| 4   | tes n     | tes d        |
-| 5   | test n    | test d       |
-| 6   | test na   | test de      |
-| 7   | test nam  | test des     |
-| 8   | test name | test desc    |
-| 9   | test name | test descr   |
-| 10  | test name | test descri  |
-| 101 | test name | test descrip |
-+-----+-----------+--------------+
++-----+-------------+----------------+
+| id  | name        | description    |
++-----+-------------+----------------+
+| 1   | 'tn'        | 'td'           |
+| 2   | 't n'       | 't d'          |
+| 3   | 'te n'      | 'te d'         |
+| 4   | 'tes n'     | 'tes d'        |
+| 5   | 'test n'    | 'test d'       |
+| 6   | 'test na'   | 'test de'      |
+| 7   | 'test nam'  | 'test des'     |
+| 8   | 'test name' | 'test desc'    |
+| 9   | 'test name' | 'test descr'   |
+| 10  | 'test name' | 'test descri'  |
+| 101 | 'test name' | 'test descrip' |
++-----+-------------+----------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_12 = """
-+------+-----------+---------------+
-| id   | name      | description   |
-+------+-----------+---------------+
-| 1    | tn        | td            |
-| 2    | t n       | t d           |
-| 3    | te n      | te d          |
-| 4    | tes n     | tes d         |
-| 5    | test n    | test d        |
-| 6    | test na   | test de       |
-| 7    | test nam  | test des      |
-| 8    | test name | test desc     |
-| 9    | test name | test descr    |
-| 10   | test name | test descri   |
-| 101  | test name | test descrip  |
-| 1010 | test name | test descript |
-+------+-----------+---------------+
++------+-------------+-----------------+
+| id   | name        | description     |
++------+-------------+-----------------+
+| 1    | 'tn'        | 'td'            |
+| 2    | 't n'       | 't d'           |
+| 3    | 'te n'      | 'te d'          |
+| 4    | 'tes n'     | 'tes d'         |
+| 5    | 'test n'    | 'test d'        |
+| 6    | 'test na'   | 'test de'       |
+| 7    | 'test nam'  | 'test des'      |
+| 8    | 'test name' | 'test desc'     |
+| 9    | 'test name' | 'test descr'    |
+| 10   | 'test name' | 'test descri'   |
+| 101  | 'test name' | 'test descrip'  |
+| 1010 | 'test name' | 'test descript' |
++------+-------------+-----------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_13 = """
-+-------+-----------+----------------+
-| id    | name      | description    |
-+-------+-----------+----------------+
-| 1     | tn        | td             |
-| 2     | t n       | t d            |
-| 3     | te n      | te d           |
-| 4     | tes n     | tes d          |
-| 5     | test n    | test d         |
-| 6     | test na   | test de        |
-| 7     | test nam  | test des       |
-| 8     | test name | test desc      |
-| 9     | test name | test descr     |
-| 10    | test name | test descri    |
-| 101   | test name | test descrip   |
-| 1010  | test name | test descript  |
-| 10101 | test name | test descripti |
-+-------+-----------+----------------+
++-------+-------------+------------------+
+| id    | name        | description      |
++-------+-------------+------------------+
+| 1     | 'tn'        | 'td'             |
+| 2     | 't n'       | 't d'            |
+| 3     | 'te n'      | 'te d'           |
+| 4     | 'tes n'     | 'tes d'          |
+| 5     | 'test n'    | 'test d'         |
+| 6     | 'test na'   | 'test de'        |
+| 7     | 'test nam'  | 'test des'       |
+| 8     | 'test name' | 'test desc'      |
+| 9     | 'test name' | 'test descr'     |
+| 10    | 'test name' | 'test descri'    |
+| 101   | 'test name' | 'test descrip'   |
+| 1010  | 'test name' | 'test descript'  |
+| 10101 | 'test name' | 'test descripti' |
++-------+-------------+------------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_14 = """
-+--------+-----------+-----------------+
-| id     | name      | description     |
-+--------+-----------+-----------------+
-| 1      | tn        | td              |
-| 2      | t n       | t d             |
-| 3      | te n      | te d            |
-| 4      | tes n     | tes d           |
-| 5      | test n    | test d          |
-| 6      | test na   | test de         |
-| 7      | test nam  | test des        |
-| 8      | test name | test desc       |
-| 9      | test name | test descr      |
-| 10     | test name | test descri     |
-| 101    | test name | test descrip    |
-| 1010   | test name | test descript   |
-| 10101  | test name | test descripti  |
-| 101010 | test name | test descriptio |
-+--------+-----------+-----------------+
++--------+-------------+-------------------+
+| id     | name        | description       |
++--------+-------------+-------------------+
+| 1      | 'tn'        | 'td'              |
+| 2      | 't n'       | 't d'             |
+| 3      | 'te n'      | 'te d'            |
+| 4      | 'tes n'     | 'tes d'           |
+| 5      | 'test n'    | 'test d'          |
+| 6      | 'test na'   | 'test de'         |
+| 7      | 'test nam'  | 'test des'        |
+| 8      | 'test name' | 'test desc'       |
+| 9      | 'test name' | 'test descr'      |
+| 10     | 'test name' | 'test descri'     |
+| 101    | 'test name' | 'test descrip'    |
+| 1010   | 'test name' | 'test descript'   |
+| 10101  | 'test name' | 'test descripti'  |
+| 101010 | 'test name' | 'test descriptio' |
++--------+-------------+-------------------+
 """.strip()
 
 
 EXPECTED__RECORD__SELECT__PT_15 = """
-+---------+-----------+------------------+
-| id      | name      | description      |
-+---------+-----------+------------------+
-| 1       | tn        | td               |
-| 2       | t n       | t d              |
-| 3       | te n      | te d             |
-| 4       | tes n     | tes d            |
-| 5       | test n    | test d           |
-| 6       | test na   | test de          |
-| 7       | test nam  | test des         |
-| 8       | test name | test desc        |
-| 9       | test name | test descr       |
-| 10      | test name | test descri      |
-| 101     | test name | test descrip     |
-| 1010    | test name | test descript    |
-| 10101   | test name | test descripti   |
-| 101010  | test name | test descriptio  |
-| 1010101 | test name | test description |
-+---------+-----------+------------------+
++---------+-------------+--------------------+
+| id      | name        | description        |
++---------+-------------+--------------------+
+| 1       | 'tn'        | 'td'               |
+| 2       | 't n'       | 't d'              |
+| 3       | 'te n'      | 'te d'             |
+| 4       | 'tes n'     | 'tes d'            |
+| 5       | 'test n'    | 'test d'           |
+| 6       | 'test na'   | 'test de'          |
+| 7       | 'test nam'  | 'test des'         |
+| 8       | 'test name' | 'test desc'        |
+| 9       | 'test name' | 'test descr'       |
+| 10      | 'test name' | 'test descri'      |
+| 101     | 'test name' | 'test descrip'     |
+| 1010    | 'test name' | 'test descript'    |
+| 10101   | 'test name' | 'test descripti'   |
+| 101010  | 'test name' | 'test descriptio'  |
+| 1010101 | 'test name' | 'test description' |
++---------+-------------+--------------------+
 """.strip()
 
 
 EXPECTED__RECORD__LIMITED_SELECT__BASIC__ALL = """
 +----+-------------------+-------------+
 | id | name              | description |
 +----+-------------------+-------------+
```

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_core.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_core.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_database.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_database.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_display.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_display.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_query.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_query.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_records.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_records.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_tables.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_tables.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_utils.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/postgresql/test_validate.py` & `py-dbcn-0.3.2/tests/connectors/postgresql/test_validate.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/sqlite/test_utils.py` & `py-dbcn-0.3.2/tests/connectors/sqlite/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-dbcn-0.3.1/tests/connectors/sqlite/test_validate.py` & `py-dbcn-0.3.2/tests/connectors/sqlite/test_validate.py`

 * *Files identical despite different names*

