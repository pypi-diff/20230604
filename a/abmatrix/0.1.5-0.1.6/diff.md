# Comparing `tmp/abmatrix-0.1.5.tar.gz` & `tmp/abmatrix-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.1.5.tar", last modified: Sun Jun  4 02:14:26 2023, max compression
+gzip compressed data, was "abmatrix-0.1.6.tar", last modified: Sun Jun  4 05:30:06 2023, max compression
```

## Comparing `abmatrix-0.1.5.tar` & `abmatrix-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:14:26.597377 abmatrix-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 02:14:26.597377 abmatrix-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 02:14:13.000000 abmatrix-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:14:26.597377 abmatrix-0.1.5/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 02:14:13.000000 abmatrix-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:14:26.597377 abmatrix-0.1.5/setup.cfg
+drwxr-xr-x   0 popgendad   (501) staff       (20)        0 2023-06-04 05:30:06.248230 abmatrix-0.1.6/
+-rw-r--r--   0 popgendad   (501) staff       (20)      449 2023-06-04 05:30:06.248291 abmatrix-0.1.6/PKG-INFO
+-rw-r--r--   0 popgendad   (501) staff       (20)       61 2023-06-03 05:37:23.000000 abmatrix-0.1.6/README.md
+drwxr-xr-x   0 popgendad   (501) staff       (20)        0 2023-06-04 05:30:06.247804 abmatrix-0.1.6/abmatrix.egg-info/
+-rw-r--r--   0 popgendad   (501) staff       (20)      449 2023-06-04 05:30:06.000000 abmatrix-0.1.6/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 popgendad   (501) staff       (20)      209 2023-06-04 05:30:06.000000 abmatrix-0.1.6/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 popgendad   (501) staff       (20)        1 2023-06-04 05:30:06.000000 abmatrix-0.1.6/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 popgendad   (501) staff       (20)       11 2023-06-04 05:30:06.000000 abmatrix-0.1.6/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 popgendad   (501) staff       (20)        1 2023-06-04 05:30:06.000000 abmatrix-0.1.6/abmatrix.egg-info/zip-safe
+-rw-r--r--   0 popgendad   (501) staff       (20)      506 2023-06-04 05:21:08.000000 abmatrix-0.1.6/pyproject.toml
+-rw-r--r--   0 popgendad   (501) staff       (20)      120 2023-06-04 05:30:06.248514 abmatrix-0.1.6/setup.cfg
+drwxr-xr-x   0 popgendad   (501) staff       (20)        0 2023-06-04 05:30:06.247917 abmatrix-0.1.6/tests/
+-rw-r--r--   0 popgendad   (501) staff       (20)     2750 2023-06-03 22:03:29.000000 abmatrix-0.1.6/tests/pulltraits.py
```

