# Comparing `tmp/abmatrix-0.1.7.tar.gz` & `tmp/abmatrix-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.1.7.tar", last modified: Sun Jun  4 05:48:00 2023, max compression
+gzip compressed data, was "abmatrix-0.2.0.tar", last modified: Sun Jun  4 15:35:52 2023, max compression
```

## Comparing `abmatrix-0.1.7.tar` & `abmatrix-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 popgendad   (501) staff       (20)        0 2023-06-04 05:48:00.221908 abmatrix-0.1.7/
--rw-r--r--   0 popgendad   (501) staff       (20)      449 2023-06-04 05:48:00.221962 abmatrix-0.1.7/PKG-INFO
--rw-r--r--   0 popgendad   (501) staff       (20)       61 2023-06-03 05:37:23.000000 abmatrix-0.1.7/README.md
-drwxr-xr-x   0 popgendad   (501) staff       (20)        0 2023-06-04 05:48:00.221048 abmatrix-0.1.7/abmatrix/
--rw-r--r--   0 popgendad   (501) staff       (20)        0 2023-06-04 05:46:24.000000 abmatrix-0.1.7/abmatrix/__init__.py
--rw-r--r--   0 popgendad   (501) staff       (20)     3706 2023-06-03 22:03:29.000000 abmatrix-0.1.7/abmatrix/abmatrix.py
-drwxr-xr-x   0 popgendad   (501) staff       (20)        0 2023-06-04 05:48:00.221798 abmatrix-0.1.7/abmatrix.egg-info/
--rw-r--r--   0 popgendad   (501) staff       (20)      449 2023-06-04 05:48:00.000000 abmatrix-0.1.7/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 popgendad   (501) staff       (20)      204 2023-06-04 05:48:00.000000 abmatrix-0.1.7/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 popgendad   (501) staff       (20)        1 2023-06-04 05:48:00.000000 abmatrix-0.1.7/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 popgendad   (501) staff       (20)        9 2023-06-04 05:48:00.000000 abmatrix-0.1.7/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 popgendad   (501) staff       (20)      506 2023-06-04 05:47:48.000000 abmatrix-0.1.7/pyproject.toml
--rw-r--r--   0 popgendad   (501) staff       (20)       94 2023-06-04 05:48:00.222151 abmatrix-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:52.335849 abmatrix-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 15:35:52.335849 abmatrix-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 15:35:42.000000 abmatrix-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:52.335849 abmatrix-0.2.0/abmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:42.000000 abmatrix-0.2.0/abmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-04 15:35:42.000000 abmatrix-0.2.0/abmatrix/abmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 15:35:52.335849 abmatrix-0.2.0/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 15:35:52.000000 abmatrix-0.2.0/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 15:35:42.000000 abmatrix-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 15:35:52.339849 abmatrix-0.2.0/setup.cfg
```

