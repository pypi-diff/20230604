# Comparing `tmp/podval-1.0.tar.gz` & `tmp/podval-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\podval-1.0.tar", last modified: Sun Jun  4 17:23:22 2023, max compression
+gzip compressed data, was "dist\podval-2.0.tar", last modified: Sun Jun  4 19:52:17 2023, max compression
```

## Comparing `podval-1.0.tar` & `podval-2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:23:22.000000 podval-1.0/
--rw-rw-rw-   0        0        0      188 2023-06-04 17:23:22.000000 podval-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 17:23:22.000000 podval-1.0/podval/
--rw-rw-rw-   0        0        0    23935 2023-06-04 17:19:38.000000 podval-1.0/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:23:22.000000 podval-1.0/podval.egg-info/
--rw-rw-rw-   0        0        0      188 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-1.0/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:23:22.000000 podval-1.0/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-04 17:21:18.000000 podval-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:52:17.000000 podval-2.0/
+-rw-rw-rw-   0        0        0      188 2023-06-04 19:52:17.000000 podval-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 19:52:17.000000 podval-2.0/podval/
+-rw-rw-rw-   0        0        0   111373 2023-06-04 19:49:44.000000 podval-2.0/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:52:17.000000 podval-2.0/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-04 19:52:17.000000 podval-2.0/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-04 19:52:17.000000 podval-2.0/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 19:52:17.000000 podval-2.0/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-2.0/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-04 19:52:17.000000 podval-2.0/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 19:52:17.000000 podval-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-04 19:51:49.000000 podval-2.0/setup.py
```

