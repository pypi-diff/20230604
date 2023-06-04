# Comparing `tmp/inegm.staff-0.2.1.tar.gz` & `tmp/inegm.staff-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inegm.staff-0.2.1.tar", last modified: Sun Jun  4 09:43:47 2023, max compression
+gzip compressed data, was "inegm.staff-0.2.2.tar", last modified: Sun Jun  4 09:50:33 2023, max compression
```

## Comparing `inegm.staff-0.2.1.tar` & `inegm.staff-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/inegm.staff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/staff/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/staff/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/patterns/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/patterns/pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/pitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/tests/test_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/tests/test_pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.075904 inegm.staff-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 09:50:33.075904 inegm.staff-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:50:33.075904 inegm.staff-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/inegm.staff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 09:50:33.000000 inegm.staff-0.2.2/src/inegm.staff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/staff/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/src/staff/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/patterns/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/patterns/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/src/staff/pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:50:33.071903 inegm.staff-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/tests/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-04 09:49:56.000000 inegm.staff-0.2.2/tests/test_pitch.py
```

### Comparing `inegm.staff-0.2.1/LICENSE` & `inegm.staff-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/pyproject.toml` & `inegm.staff-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/src/staff/duration.py` & `inegm.staff-0.2.2/src/staff/duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/src/staff/patterns/duration.py` & `inegm.staff-0.2.2/src/staff/patterns/duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/src/staff/patterns/pattern.py` & `inegm.staff-0.2.2/src/staff/patterns/pattern.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/src/staff/pitch.py` & `inegm.staff-0.2.2/src/staff/pitch.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/tests/test_duration.py` & `inegm.staff-0.2.2/tests/test_duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.1/tests/test_pitch.py` & `inegm.staff-0.2.2/tests/test_pitch.py`

 * *Files identical despite different names*

