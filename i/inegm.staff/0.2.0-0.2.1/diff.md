# Comparing `tmp/inegm.staff-0.2.0.tar.gz` & `tmp/inegm.staff-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inegm.staff-0.2.0.tar", last modified: Sun Jun  4 09:25:55 2023, max compression
+gzip compressed data, was "inegm.staff-0.2.1.tar", last modified: Sun Jun  4 09:43:47 2023, max compression
```

## Comparing `inegm.staff-0.2.0.tar` & `inegm.staff-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-06-04 09:25:55.512174 inegm.staff-0.2.0/
--rw-r--r--   0 daedalus   (501) staff       (20)     1068 2023-05-14 11:40:58.000000 inegm.staff-0.2.0/LICENSE
--rw-r--r--   0 daedalus   (501) staff       (20)      433 2023-06-04 09:25:55.512053 inegm.staff-0.2.0/PKG-INFO
--rw-r--r--   0 daedalus   (501) staff       (20)       72 2023-06-04 08:55:11.000000 inegm.staff-0.2.0/README.md
--rw-r--r--   0 daedalus   (501) staff       (20)      823 2023-06-04 09:25:32.000000 inegm.staff-0.2.0/pyproject.toml
--rw-r--r--   0 daedalus   (501) staff       (20)        0 2023-05-14 11:39:32.000000 inegm.staff-0.2.0/requirements.txt
--rw-r--r--   0 daedalus   (501) staff       (20)       38 2023-06-04 09:25:55.512207 inegm.staff-0.2.0/setup.cfg
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-06-04 09:25:55.509657 inegm.staff-0.2.0/src/
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-06-04 09:25:55.510723 inegm.staff-0.2.0/src/inegm.staff.egg-info/
--rw-r--r--   0 daedalus   (501) staff       (20)      433 2023-06-04 09:25:55.000000 inegm.staff-0.2.0/src/inegm.staff.egg-info/PKG-INFO
--rw-r--r--   0 daedalus   (501) staff       (20)      490 2023-06-04 09:25:55.000000 inegm.staff-0.2.0/src/inegm.staff.egg-info/SOURCES.txt
--rw-r--r--   0 daedalus   (501) staff       (20)        1 2023-06-04 09:25:55.000000 inegm.staff-0.2.0/src/inegm.staff.egg-info/dependency_links.txt
--rw-r--r--   0 daedalus   (501) staff       (20)       46 2023-06-04 09:25:55.000000 inegm.staff-0.2.0/src/inegm.staff.egg-info/entry_points.txt
--rw-r--r--   0 daedalus   (501) staff       (20)        6 2023-06-04 09:25:55.000000 inegm.staff-0.2.0/src/inegm.staff.egg-info/top_level.txt
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-06-04 09:25:55.511258 inegm.staff-0.2.0/src/staff/
--rw-r--r--   0 daedalus   (501) staff       (20)      217 2023-06-04 09:22:08.000000 inegm.staff-0.2.0/src/staff/__init__.py
--rw-r--r--   0 daedalus   (501) staff       (20)       32 2023-05-14 12:09:22.000000 inegm.staff-0.2.0/src/staff/__main__.py
--rw-r--r--   0 daedalus   (501) staff       (20)     8912 2023-06-04 08:34:45.000000 inegm.staff-0.2.0/src/staff/duration.py
--rw-r--r--   0 daedalus   (501) staff       (20)      335 2023-05-31 19:20:53.000000 inegm.staff-0.2.0/src/staff/numerical.py
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-06-04 09:25:55.511615 inegm.staff-0.2.0/src/staff/patterns/
--rw-r--r--   0 daedalus   (501) staff       (20)       76 2023-05-31 19:35:43.000000 inegm.staff-0.2.0/src/staff/patterns/__init__.py
--rw-r--r--   0 daedalus   (501) staff       (20)     4142 2023-05-31 19:44:58.000000 inegm.staff-0.2.0/src/staff/patterns/duration.py
--rw-r--r--   0 daedalus   (501) staff       (20)      821 2023-05-31 19:36:23.000000 inegm.staff-0.2.0/src/staff/patterns/pattern.py
--rw-r--r--   0 daedalus   (501) staff       (20)    15313 2023-06-03 19:21:09.000000 inegm.staff-0.2.0/src/staff/pitch.py
-drwxr-xr-x   0 daedalus   (501) staff       (20)        0 2023-06-04 09:25:55.511876 inegm.staff-0.2.0/tests/
--rw-r--r--   0 daedalus   (501) staff       (20)     2388 2023-05-27 14:41:12.000000 inegm.staff-0.2.0/tests/test_duration.py
--rw-r--r--   0 daedalus   (501) staff       (20)     4928 2023-06-04 08:37:56.000000 inegm.staff-0.2.0/tests/test_pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/inegm.staff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-04 09:43:47.000000 inegm.staff-0.2.1/src/inegm.staff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/staff/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/src/staff/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/patterns/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/patterns/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/src/staff/pitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:43:47.193930 inegm.staff-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/tests/test_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-04 09:43:10.000000 inegm.staff-0.2.1/tests/test_pitch.py
```

### Comparing `inegm.staff-0.2.0/LICENSE` & `inegm.staff-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/pyproject.toml` & `inegm.staff-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/src/staff/duration.py` & `inegm.staff-0.2.1/src/staff/duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/src/staff/patterns/duration.py` & `inegm.staff-0.2.1/src/staff/patterns/duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/src/staff/patterns/pattern.py` & `inegm.staff-0.2.1/src/staff/patterns/pattern.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/src/staff/pitch.py` & `inegm.staff-0.2.1/src/staff/pitch.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/tests/test_duration.py` & `inegm.staff-0.2.1/tests/test_duration.py`

 * *Files identical despite different names*

### Comparing `inegm.staff-0.2.0/tests/test_pitch.py` & `inegm.staff-0.2.1/tests/test_pitch.py`

 * *Files identical despite different names*

