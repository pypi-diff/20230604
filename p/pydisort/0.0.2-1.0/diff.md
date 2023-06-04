# Comparing `tmp/pydisort-0.0.2.tar.gz` & `tmp/pydisort-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydisort-0.0.2.tar", last modified: Fri Jun  2 21:54:27 2023, max compression
+gzip compressed data, was "pydisort-1.0.tar", last modified: Sun Jun  4 01:29:02 2023, max compression
```

## Comparing `pydisort-0.0.2.tar` & `pydisort-1.0.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-02 21:54:27.784177 pydisort-0.0.2/
--rw-r--r--   0 zyhu       (502) staff       (20)     1074 2023-04-11 04:11:16.000000 pydisort-0.0.2/LICENSE
--rw-r--r--   0 zyhu       (502) staff       (20)      453 2023-06-02 21:54:27.783604 pydisort-0.0.2/PKG-INFO
--rw-r--r--   0 zyhu       (502) staff       (20)       76 2023-04-11 04:12:00.000000 pydisort-0.0.2/README.md
--rw-r--r--   0 zyhu       (502) staff       (20)      364 2023-06-02 21:53:22.000000 pydisort-0.0.2/pyproject.toml
--rw-r--r--   0 zyhu       (502) staff       (20)       38 2023-06-02 21:54:27.784343 pydisort-0.0.2/setup.cfg
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-02 21:54:27.778094 pydisort-0.0.2/src/
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-02 21:54:27.780427 pydisort-0.0.2/src/pydisort/
--rw-r--r--   0 zyhu       (502) staff       (20)        0 2023-04-11 04:11:16.000000 pydisort-0.0.2/src/pydisort/__init__.py
--rw-r--r--   0 zyhu       (502) staff       (20)        0 2023-04-11 04:11:16.000000 pydisort-0.0.2/src/pydisort/main.py
-drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-02 21:54:27.783034 pydisort-0.0.2/src/pydisort.egg-info/
--rw-r--r--   0 zyhu       (502) staff       (20)      453 2023-06-02 21:54:27.000000 pydisort-0.0.2/src/pydisort.egg-info/PKG-INFO
--rw-r--r--   0 zyhu       (502) staff       (20)      222 2023-06-02 21:54:27.000000 pydisort-0.0.2/src/pydisort.egg-info/SOURCES.txt
--rw-r--r--   0 zyhu       (502) staff       (20)        1 2023-06-02 21:54:27.000000 pydisort-0.0.2/src/pydisort.egg-info/dependency_links.txt
--rw-r--r--   0 zyhu       (502) staff       (20)        9 2023-06-02 21:54:27.000000 pydisort-0.0.2/src/pydisort.egg-info/top_level.txt
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 01:29:02.951361 pydisort-1.0/
+-rw-r--r--   0 zyhu       (502) staff       (20)       50 2023-06-04 01:29:02.950839 pydisort-1.0/PKG-INFO
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 01:29:02.943333 pydisort-1.0/pydisort/
+-rw-r--r--   0 zyhu       (502) staff       (20)       24 2023-06-04 01:28:16.000000 pydisort-1.0/pydisort/__init__.py
+-rwxr-xr-x   0 zyhu       (502) staff       (20)   542488 2023-06-04 00:45:04.000000 pydisort-1.0/pydisort/pydisort.cpython-311-darwin.so
+drwxr-xr-x   0 zyhu       (502) staff       (20)        0 2023-06-04 01:29:02.949862 pydisort-1.0/pydisort.egg-info/
+-rw-r--r--   0 zyhu       (502) staff       (20)       50 2023-06-04 01:29:02.000000 pydisort-1.0/pydisort.egg-info/PKG-INFO
+-rw-r--r--   0 zyhu       (502) staff       (20)      197 2023-06-04 01:29:02.000000 pydisort-1.0/pydisort.egg-info/SOURCES.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)        1 2023-06-04 01:29:02.000000 pydisort-1.0/pydisort.egg-info/dependency_links.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)        9 2023-06-04 01:29:02.000000 pydisort-1.0/pydisort.egg-info/top_level.txt
+-rw-r--r--   0 zyhu       (502) staff       (20)       38 2023-06-04 01:29:02.951541 pydisort-1.0/setup.cfg
+-rw-r--r--   0 zyhu       (502) staff       (20)      191 2023-06-04 01:28:41.000000 pydisort-1.0/setup.py
```

