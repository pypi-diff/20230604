# Comparing `tmp/abmatrix-0.1.4.tar.gz` & `tmp/abmatrix-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abmatrix-0.1.4.tar", last modified: Sat Jun  3 22:34:58 2023, max compression
+gzip compressed data, was "abmatrix-0.1.5.tar", last modified: Sun Jun  4 02:14:26 2023, max compression
```

## Comparing `abmatrix-0.1.4.tar` & `abmatrix-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.785984 abmatrix-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:34:58.785984 abmatrix-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-03 22:34:49.000000 abmatrix-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-03 22:34:49.000000 abmatrix-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 22:34:58.785984 abmatrix-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.781984 abmatrix-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.781984 abmatrix-0.1.4/src/abmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:49.000000 abmatrix-0.1.4/src/abmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-03 22:34:49.000000 abmatrix-0.1.4/src/abmatrix/abmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 22:34:58.785984 abmatrix-0.1.4/src/abmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 22:34:58.000000 abmatrix-0.1.4/src/abmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:14:26.597377 abmatrix-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 02:14:26.597377 abmatrix-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-04 02:14:13.000000 abmatrix-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 02:14:26.597377 abmatrix-0.1.5/abmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 02:14:26.000000 abmatrix-0.1.5/abmatrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 02:14:13.000000 abmatrix-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 02:14:26.597377 abmatrix-0.1.5/setup.cfg
```

