# Comparing `tmp/SimpleSQLite-1.3.0.tar.gz` & `tmp/SimpleSQLite-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SimpleSQLite-1.3.0.tar", last modified: Sun Jun 20 11:07:25 2021, max compression
+gzip compressed data, was "SimpleSQLite-1.3.1.tar", last modified: Sun Jun  4 07:01:56 2023, max compression
```

## Comparing `SimpleSQLite-1.3.0.tar` & `SimpleSQLite-1.3.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.115994 SimpleSQLite-1.3.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)    13969 2021-06-20 11:07:25.115994 SimpleSQLite-1.3.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    12189 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/SimpleSQLite.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)    13969 2021-06-20 11:07:25.000000 SimpleSQLite-1.3.0/SimpleSQLite.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1110 2021-06-20 11:07:25.000000 SimpleSQLite-1.3.0/SimpleSQLite.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2021-06-20 11:07:25.000000 SimpleSQLite-1.3.0/SimpleSQLite.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      264 2021-06-20 11:07:25.000000 SimpleSQLite-1.3.0/SimpleSQLite.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       13 2021-06-20 11:07:25.000000 SimpleSQLite-1.3.0/SimpleSQLite.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)      177 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/docs/pages/introduction/summary.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1268 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      130 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       98 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2021-06-20 11:07:25.115994 SimpleSQLite-1.3.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     3039 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/simplesqlite/
--rw-r--r--   0 toor      (1000) toor      (1000)      590 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1025 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_common.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4870 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_func.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/simplesqlite/_logger/
--rw-r--r--   0 toor      (1000) toor      (1000)       55 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_logger/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      888 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_logger/_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1071 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_logger/_null_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6421 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_sanitizer.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4280 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/_validator.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3529 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/converter.py
--rw-r--r--   0 toor      (1000) toor      (1000)    58899 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/core.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1381 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8879 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/model.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/py.typed
--rw-r--r--   0 toor      (1000) toor      (1000)    13682 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/query.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2560 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/simplesqlite/sqlquery.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.105994 SimpleSQLite-1.3.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      266 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/_common.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-20 11:07:25.115994 SimpleSQLite-1.3.0/test/data/
--rw-r--r--   0 toor      (1000) toor      (1000)    71819 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/data/python - Wiktionary.html
--rw-r--r--   0 toor      (1000) toor      (1000)     1902 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/fixture.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3123 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_convertor.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1271 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_from_file.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4169 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_func.py
--rw-r--r--   0 toor      (1000) toor      (1000)      561 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_logger.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1145 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_orm.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1837 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_pandas.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12907 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_query.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9922 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_sanitizer.py
--rw-r--r--   0 toor      (1000) toor      (1000)    42408 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_simplesqlite.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2927 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_sqlquery.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7876 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/test/test_validator.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1591 2021-06-20 11:07:02.000000 SimpleSQLite-1.3.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)    14377 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    12565 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)    14377 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1110 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      287 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       13 2023-06-04 07:01:56.000000 SimpleSQLite-1.3.1/SimpleSQLite.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/docs/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/docs/pages/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/docs/pages/introduction/
+-rw-r--r--   0 toor      (1000) toor      (1000)      177 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/docs/pages/introduction/summary.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1336 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/requirements/docs_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      130 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      121 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3079 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/simplesqlite/
+-rw-r--r--   0 toor      (1000) toor      (1000)      590 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1025 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_common.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4870 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_func.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.913954 SimpleSQLite-1.3.1/simplesqlite/_logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)       55 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      888 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_logger/_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1071 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_logger/_null_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6522 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_sanitizer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4280 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/_validator.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3529 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/converter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    58899 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/core.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1381 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8879 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/model.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/py.typed
+-rw-r--r--   0 toor      (1000) toor      (1000)    13682 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/query.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2560 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/simplesqlite/sqlquery.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      266 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/_common.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-04 07:01:56.923955 SimpleSQLite-1.3.1/test/data/
+-rw-r--r--   0 toor      (1000) toor      (1000)    71819 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/data/python - Wiktionary.html
+-rw-r--r--   0 toor      (1000) toor      (1000)     1902 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/fixture.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3123 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_convertor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1317 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_from_file.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4169 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_func.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      561 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_logger.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_orm.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1837 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_pandas.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12906 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_query.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10549 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_sanitizer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    42407 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_simplesqlite.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2927 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_sqlquery.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7876 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/test/test_validator.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1498 2023-06-04 07:00:43.000000 SimpleSQLite-1.3.1/tox.ini
```

### Comparing `SimpleSQLite-1.3.0/LICENSE` & `SimpleSQLite-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/PKG-INFO` & `SimpleSQLite-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: SimpleSQLite
-Version: 1.3.0
+Version: 1.3.1
 Summary: SimpleSQLite is a Python library to simplify SQLite database operations: table creation, data insertion and get data as other data formats. Simple ORM functionality for SQLite.
 Home-page: https://github.com/thombashi/SimpleSQLite
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://SimpleSQLite.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/SimpleSQLite
 Project-URL: Tracker, https://github.com/thombashi/SimpleSQLite/issues
-Project-URL: Changes, https://github.com/thombashi/SimpleSQLite/releases
+Project-URL: Changlog, https://github.com/thombashi/SimpleSQLite/releases
 Keywords: SQLite,CSV,Google Sheets,JSON
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
@@ -56,22 +56,22 @@
     :target: https://pypi.org/project/SimpleSQLite
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/SimpleSQLite/actions/workflows/lint_and_test.yml/badge.svg
     :target: https://github.com/thombashi/SimpleSQLite/actions/workflows/lint_and_test.yml
     :alt: CI status of Linux/macOS/Windows
 
+.. image:: https://github.com/thombashi/SimpleSQLite/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/SimpleSQLite/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 .. image:: https://coveralls.io/repos/github/thombashi/SimpleSQLite/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/SimpleSQLite?branch=master
     :alt: Test coverage
 
-.. image:: https://img.shields.io/github/stars/thombashi/SimpleSQLite.svg?style=social&label=Star
-    :target: https://github.com/thombashi/SimpleSQLite
-    :alt: GitHub stars
-
 Features
 --------
 - Automated SQLite table creation from data
 - Support various data types of record(s) insertion into a table:
     - ``dict``
     - ``namedtuple``
     - ``list``
@@ -86,16 +86,16 @@
     - `tabledata.TableData <https://github.com/thombashi/tabledata>`__ instance
 - Simple object-relational mapping (ORM) functionality
 
 Examples
 ==========
 Create a table
 ----------------
-Create a table from data matrix
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Create a table from a data matrix
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 :Sample Code:
     .. code-block:: python
 
         from simplesqlite import SimpleSQLite
 
 
         table_name = "sample_table"
@@ -169,17 +169,17 @@
         for record in result.fetchall():
             print(record)
 
 :Output:
     .. code-block::
 
         ['attr_a', 'attr_b', 'attr_c']
-        (1, 4.0, u'a')
-        (2, 2.1, u'bb')
-        (3, 120.9, u'ccc')
+        (1, 4.0, 'a')
+        (2, 2.1, 'bb')
+        (3, 120.9, 'ccc')
 
 Create a table from pandas.DataFrame
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 :Sample Code:
     .. code-block:: python
 
         from simplesqlite import SimpleSQLite
@@ -422,15 +422,19 @@
 
 Related Project
 =================
 - `sqlitebiter <https://github.com/thombashi/sqlitebiter>`__: CLI tool to convert CSV/Excel/HTML/JSON/LTSV/Markdown/TSV/Google-Sheets SQLite database by using SimpleSQLite
 
 Sponsors
 ====================================
-.. image:: https://avatars0.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
    :alt: Charles Becker (chasbecker)
+.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: onetime: Arturi0
+.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: onetime: Dmitry Belyaev (b4tman)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
 
-
-
```

### Comparing `SimpleSQLite-1.3.0/README.rst` & `SimpleSQLite-1.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,22 @@
     :target: https://pypi.org/project/SimpleSQLite
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/SimpleSQLite/actions/workflows/lint_and_test.yml/badge.svg
     :target: https://github.com/thombashi/SimpleSQLite/actions/workflows/lint_and_test.yml
     :alt: CI status of Linux/macOS/Windows
 
+.. image:: https://github.com/thombashi/SimpleSQLite/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/SimpleSQLite/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 .. image:: https://coveralls.io/repos/github/thombashi/SimpleSQLite/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/SimpleSQLite?branch=master
     :alt: Test coverage
 
-.. image:: https://img.shields.io/github/stars/thombashi/SimpleSQLite.svg?style=social&label=Star
-    :target: https://github.com/thombashi/SimpleSQLite
-    :alt: GitHub stars
-
 Features
 --------
 - Automated SQLite table creation from data
 - Support various data types of record(s) insertion into a table:
     - ``dict``
     - ``namedtuple``
     - ``list``
@@ -48,16 +48,16 @@
     - `tabledata.TableData <https://github.com/thombashi/tabledata>`__ instance
 - Simple object-relational mapping (ORM) functionality
 
 Examples
 ==========
 Create a table
 ----------------
-Create a table from data matrix
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Create a table from a data matrix
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 :Sample Code:
     .. code-block:: python
 
         from simplesqlite import SimpleSQLite
 
 
         table_name = "sample_table"
@@ -131,17 +131,17 @@
         for record in result.fetchall():
             print(record)
 
 :Output:
     .. code-block::
 
         ['attr_a', 'attr_b', 'attr_c']
-        (1, 4.0, u'a')
-        (2, 2.1, u'bb')
-        (3, 120.9, u'ccc')
+        (1, 4.0, 'a')
+        (2, 2.1, 'bb')
+        (3, 120.9, 'ccc')
 
 Create a table from pandas.DataFrame
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 :Sample Code:
     .. code-block:: python
 
         from simplesqlite import SimpleSQLite
@@ -384,13 +384,19 @@
 
 Related Project
 =================
 - `sqlitebiter <https://github.com/thombashi/sqlitebiter>`__: CLI tool to convert CSV/Excel/HTML/JSON/LTSV/Markdown/TSV/Google-Sheets SQLite database by using SimpleSQLite
 
 Sponsors
 ====================================
-.. image:: https://avatars0.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
    :alt: Charles Becker (chasbecker)
+.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: onetime: Arturi0
+.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: onetime: Dmitry Belyaev (b4tman)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
```

### Comparing `SimpleSQLite-1.3.0/SimpleSQLite.egg-info/PKG-INFO` & `SimpleSQLite-1.3.1/SimpleSQLite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: SimpleSQLite
-Version: 1.3.0
+Version: 1.3.1
 Summary: SimpleSQLite is a Python library to simplify SQLite database operations: table creation, data insertion and get data as other data formats. Simple ORM functionality for SQLite.
 Home-page: https://github.com/thombashi/SimpleSQLite
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Documentation, https://SimpleSQLite.rtfd.io/
 Project-URL: Source, https://github.com/thombashi/SimpleSQLite
 Project-URL: Tracker, https://github.com/thombashi/SimpleSQLite/issues
-Project-URL: Changes, https://github.com/thombashi/SimpleSQLite/releases
+Project-URL: Changlog, https://github.com/thombashi/SimpleSQLite/releases
 Keywords: SQLite,CSV,Google Sheets,JSON
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
@@ -56,22 +56,22 @@
     :target: https://pypi.org/project/SimpleSQLite
     :alt: Supported Python implementations
 
 .. image:: https://github.com/thombashi/SimpleSQLite/actions/workflows/lint_and_test.yml/badge.svg
     :target: https://github.com/thombashi/SimpleSQLite/actions/workflows/lint_and_test.yml
     :alt: CI status of Linux/macOS/Windows
 
+.. image:: https://github.com/thombashi/SimpleSQLite/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/SimpleSQLite/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
 .. image:: https://coveralls.io/repos/github/thombashi/SimpleSQLite/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/SimpleSQLite?branch=master
     :alt: Test coverage
 
-.. image:: https://img.shields.io/github/stars/thombashi/SimpleSQLite.svg?style=social&label=Star
-    :target: https://github.com/thombashi/SimpleSQLite
-    :alt: GitHub stars
-
 Features
 --------
 - Automated SQLite table creation from data
 - Support various data types of record(s) insertion into a table:
     - ``dict``
     - ``namedtuple``
     - ``list``
@@ -86,16 +86,16 @@
     - `tabledata.TableData <https://github.com/thombashi/tabledata>`__ instance
 - Simple object-relational mapping (ORM) functionality
 
 Examples
 ==========
 Create a table
 ----------------
-Create a table from data matrix
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Create a table from a data matrix
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 :Sample Code:
     .. code-block:: python
 
         from simplesqlite import SimpleSQLite
 
 
         table_name = "sample_table"
@@ -169,17 +169,17 @@
         for record in result.fetchall():
             print(record)
 
 :Output:
     .. code-block::
 
         ['attr_a', 'attr_b', 'attr_c']
-        (1, 4.0, u'a')
-        (2, 2.1, u'bb')
-        (3, 120.9, u'ccc')
+        (1, 4.0, 'a')
+        (2, 2.1, 'bb')
+        (3, 120.9, 'ccc')
 
 Create a table from pandas.DataFrame
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 :Sample Code:
     .. code-block:: python
 
         from simplesqlite import SimpleSQLite
@@ -422,15 +422,19 @@
 
 Related Project
 =================
 - `sqlitebiter <https://github.com/thombashi/sqlitebiter>`__: CLI tool to convert CSV/Excel/HTML/JSON/LTSV/Markdown/TSV/Google-Sheets SQLite database by using SimpleSQLite
 
 Sponsors
 ====================================
-.. image:: https://avatars0.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
+.. image:: https://avatars.githubusercontent.com/u/44389260?s=48&u=6da7176e51ae2654bcfd22564772ef8a3bb22318&v=4
    :target: https://github.com/chasbecker
    :alt: Charles Becker (chasbecker)
+.. image:: https://avatars.githubusercontent.com/u/46711571?s=48&u=57687c0e02d5d6e8eeaf9177f7b7af4c9f275eb5&v=4
+   :target: https://github.com/Arturi0
+   :alt: onetime: Arturi0
+.. image:: https://avatars.githubusercontent.com/u/3658062?s=48&v=4
+   :target: https://github.com/b4tman
+   :alt: onetime: Dmitry Belyaev (b4tman)
 
 `Become a sponsor <https://github.com/sponsors/thombashi>`__
 
-
-
```

### Comparing `SimpleSQLite-1.3.0/SimpleSQLite.egg-info/SOURCES.txt` & `SimpleSQLite-1.3.1/SimpleSQLite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/pyproject.toml` & `SimpleSQLite-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
+target-version = ['py36', 'py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.isort]
 known_third_party = [
     'dataproperty',
     'logbook',
     'mbstrdecoder',
     'pandas',
```

### Comparing `SimpleSQLite-1.3.0/setup.py` & `SimpleSQLite-1.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-#!/usr/bin/env python
-
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "SimpleSQLite"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -56,15 +54,15 @@
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Documentation": f"https://{MODULE_NAME:s}.rtfd.io/",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
-        "Changes": f"{REPOSITORY_URL:s}/releases",
+        "Changlog": f"{REPOSITORY_URL:s}/releases",
     },
     python_requires=">=3.6",
     install_requires=install_requires,
     tests_require=tests_requires,
     extras_require={"logging": ["loguru>=0.4.1,<1"], "test": tests_requires},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -75,14 +73,15 @@
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Database",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `SimpleSQLite-1.3.0/simplesqlite/__init__.py` & `SimpleSQLite-1.3.1/simplesqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/_common.py` & `SimpleSQLite-1.3.1/simplesqlite/_common.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/_func.py` & `SimpleSQLite-1.3.1/simplesqlite/_func.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/_logger/_logger.py` & `SimpleSQLite-1.3.1/simplesqlite/_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/_logger/_null_logger.py` & `SimpleSQLite-1.3.1/simplesqlite/_logger/_null_logger.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/_sanitizer.py` & `SimpleSQLite-1.3.1/simplesqlite/_sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import List, Optional, Sequence, cast
 
 import dataproperty
 import pathvalidate as pv
 import typepy
 from dataproperty.typing import TypeHint
 from pathvalidate.error import ErrorReason, ValidationError
+from pathvalidate.handler import raise_error
 from tabledata import (
     DataError,
     InvalidHeaderNameError,
     InvalidTableNameError,
     TableData,
     convert_idx_to_alphabet,
 )
@@ -22,15 +23,14 @@
 from ._validator import validate_sqlite_attr_name, validate_sqlite_table_name
 from .converter import RecordConvertor
 from .error import NameValidationError
 from .query import Attr, AttrList
 
 
 class SQLiteTableDataSanitizer(AbstractTableDataNormalizer):
-
     __RENAME_TEMPLATE = "rename_{:s}"
 
     @property
     def _type_hints(self) -> Optional[List[TypeHint]]:
         if self.__is_type_inference:
             return self._tabledata.dp_extractor.column_type_hints
 
@@ -68,15 +68,17 @@
             self.__upper_headers.append(header)
 
         self.__dup_col_handler = dup_col_handler
         self.__is_type_inference = is_type_inference
 
     def _preprocess_table_name(self) -> str:
         try:
-            new_name = str(pv.sanitize_filename(self._tabledata.table_name, replacement_text="_"))
+            new_name = pv.sanitize_filename(
+                self._tabledata.table_name, replacement_text="_", null_value_handler=raise_error
+            )
         except TypeError:
             raise NameValidationError(
                 f"table name must be a string: actual='{self._tabledata.table_name}'"
             )
 
         new_name = pv.replace_unprintable_char(new_name, replacement_text="")
         new_name = pv.replace_symbol(
```

### Comparing `SimpleSQLite-1.3.0/simplesqlite/_validator.py` & `SimpleSQLite-1.3.1/simplesqlite/_validator.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/converter.py` & `SimpleSQLite-1.3.1/simplesqlite/converter.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/core.py` & `SimpleSQLite-1.3.1/simplesqlite/core.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/error.py` & `SimpleSQLite-1.3.1/simplesqlite/error.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/model.py` & `SimpleSQLite-1.3.1/simplesqlite/model.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/query.py` & `SimpleSQLite-1.3.1/simplesqlite/query.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/simplesqlite/sqlquery.py` & `SimpleSQLite-1.3.1/simplesqlite/sqlquery.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/data/python - Wiktionary.html` & `SimpleSQLite-1.3.1/test/data/python - Wiktionary.html`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/fixture.py` & `SimpleSQLite-1.3.1/test/fixture.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_convertor.py` & `SimpleSQLite-1.3.1/test/test_convertor.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_from_file.py` & `SimpleSQLite-1.3.1/test/test_from_file.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 
 import pytest
 
 from simplesqlite import SimpleSQLite, SQLiteTableDataSanitizer
 
 
 class Test_SimpleSQLite_create_table_from_tabledata:
-    @pytest.mark.parametrize(["filename"], [["python - Wiktionary.html"]])
+    @pytest.mark.parametrize(
+        ["filename"],
+        [
+            ["python - Wiktionary.html"],
+        ],
+    )
     def test_smoke(self, tmpdir, filename):
         try:
             import pytablereader as ptr
         except ImportError:
             pytest.skip("requires pytablereader")
 
         p = tmpdir.join("tmp.db")
```

### Comparing `SimpleSQLite-1.3.0/test/test_func.py` & `SimpleSQLite-1.3.1/test/test_func.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_logger.py` & `SimpleSQLite-1.3.1/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_orm.py` & `SimpleSQLite-1.3.1/test/test_orm.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_pandas.py` & `SimpleSQLite-1.3.1/test/test_pandas.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_query.py` & `SimpleSQLite-1.3.1/test/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     )
     def test_exception(self, value, expected):
         with pytest.raises(expected):
             assert f"{Table(value)}"
 
 
 class Test_Attr:
-
     RESERVED_KEYWORDS = [
         "ADD",
         "ALL",
         "ALTER",
         "AND",
         "AS",
         "AUTOINCREMENT",
```

### Comparing `SimpleSQLite-1.3.0/test/test_sanitizer.py` & `SimpleSQLite-1.3.1/test/test_sanitizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,18 +142,28 @@
 
     @pytest.mark.parametrize(
         ["table_name", "headers", "records", "type_hints", "expecte_col_types", "expecte_data"],
         [
             [
                 "w/ type inference",
                 ["a", "b_c"],
-                [[1, 2], [3, 4]],
+                [
+                    [1, 2],
+                    [3, 4],
+                ],
                 [String],
                 ["STRING", "INTEGER"],
-                TableData("w_type_inference", ["a", "b_c"], [["1", 2], ["3", 4]]),
+                TableData(
+                    "w_type_inference",
+                    ["a", "b_c"],
+                    [
+                        ["1", 2],
+                        ["3", 4],
+                    ],
+                ),
             ]
         ],
     )
     def test_normal_type_hints(
         self, table_name, headers, records, type_hints, expecte_col_types, expecte_data
     ):
         new_tabledata = SQLiteTableDataSanitizer(
@@ -176,26 +186,46 @@
             "expecte_col_types",
             "expecte_data",
         ],
         [
             [
                 "w/ type inference",
                 ["a", "b_c"],
-                [["1", "2"], ["3", "4"]],
+                [
+                    ["1", "2"],
+                    ["3", "4"],
+                ],
                 True,
                 ["INTEGER", "INTEGER"],
-                TableData("w_type_inference", ["a", "b_c"], [[1, 2], [3, 4]]),
+                TableData(
+                    "w_type_inference",
+                    ["a", "b_c"],
+                    [
+                        [1, 2],
+                        [3, 4],
+                    ],
+                ),
             ],
             [
                 "w/o type inference",
                 ["a", "b_c"],
-                [["1", "2"], ["3", "4"]],
+                [
+                    ["1", "2"],
+                    ["3", "4"],
+                ],
                 False,
                 ["STRING", "STRING"],
-                TableData("w_o_type_inference", ["a", "b_c"], [["1", "2"], ["3", "4"]]),
+                TableData(
+                    "w_o_type_inference",
+                    ["a", "b_c"],
+                    [
+                        ["1", "2"],
+                        ["3", "4"],
+                    ],
+                ),
             ],
         ],
     )
     def test_normal_type_inference(
         self, table_name, headers, records, is_type_inference, expecte_col_types, expecte_data
     ):
         new_tabledata = SQLiteTableDataSanitizer(
```

### Comparing `SimpleSQLite-1.3.0/test/test_simplesqlite.py` & `SimpleSQLite-1.3.1/test/test_simplesqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1236,15 +1236,14 @@
         con.close()
 
     def test_null(self, con_null):
         con_null.close()
 
 
 class Test_SimpleSQLite_create_index:
-
     CHARS = [
         "/",
         ":",
         "*",
         "?",
         '"',
         "<",
```

### Comparing `SimpleSQLite-1.3.0/test/test_sqlquery.py` & `SimpleSQLite-1.3.1/test/test_sqlquery.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/test/test_validator.py` & `SimpleSQLite-1.3.1/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `SimpleSQLite-1.3.0/tox.ini` & `SimpleSQLite-1.3.1/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,80 @@
 [tox]
 envlist =
-    py{36,37,38,39,310}
+    py{36,37,38,39,310,311}
     pypy3
     build
-    clean
     cov
     docs
     lint
     fmt
     readme
 
 [testenv]
-deps =
-    .[test]
+passenv = *
+extras =
+    test
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
     twine
     wheel
 commands =
     python setup.py sdist bdist_wheel
     twine check dist/*.whl dist/*.tar.gz
     python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.2
+    cleanpy>=0.4
 commands =
-    cleanpy --force --all --exclude-envs .
+    cleanpy --all --exclude-envs .
 
 [testenv:cov]
+extras =
+    test
 deps =
-    .[test]
-    coverage[toml]
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:docs]
-basepython = python3.8
 deps =
     -r{toxinidir}/requirements/docs_requirements.txt
 commands =
     python setup.py build_sphinx --source-dir=docs/ --build-dir=docs/_build --all-files
 
 [testenv:fmt]
-basepython = python3.8
 skip_install = true
 deps =
-    autoflake
-    black
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports --exclude ".pytype" .
     isort .
     black setup.py test sample simplesqlite
 
 [testenv:lint]
-basepython = python3.8
 skip_install = true
 deps =
-    codespell
-    mypy>=0.902
-    pylama
+    codespell>=2
+    mypy>=1
+    pylama>=8.4.1
 commands =
     python setup.py check
     mypy simplesqlite
     codespell simplesqlite docs/pages sample test -q2 --check-filenames --ignore-words-list te -x "test/data/python - Wiktionary.html"
     pylama setup.py test sample simplesqlite
 
 [testenv:readme]
 changedir = docs
 skip_install = true
 deps =
     path
-    readmemaker>=1.0.0
+    readmemaker>=1.1.0
 commands =
     python make_readme.py
```

