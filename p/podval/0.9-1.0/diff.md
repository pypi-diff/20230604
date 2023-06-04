# Comparing `tmp/podval-0.9.tar.gz` & `tmp/podval-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podval-0.9.tar", last modified: Sat Jun  3 22:49:19 2023, max compression
+gzip compressed data, was "dist\podval-1.0.tar", last modified: Sun Jun  4 17:23:22 2023, max compression
```

## Comparing `podval-0.9.tar` & `podval-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 22:49:19.352454 podval-0.9/
--rw-rw-rw-   0        0        0       86 2023-06-03 22:49:19.352454 podval-0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-03 22:49:19.341412 podval-0.9/podval/
--rw-rw-rw-   0        0        0       36 2023-06-03 22:31:36.000000 podval-0.9/podval/podval.py
-drwxrwxrwx   0        0        0        0 2023-06-03 22:49:19.349452 podval-0.9/podval.egg-info/
--rw-rw-rw-   0        0        0       86 2023-06-03 22:49:19.000000 podval-0.9/podval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-03 22:49:19.000000 podval-0.9/podval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 22:49:19.000000 podval-0.9/podval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-0.9/podval.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-03 22:49:19.000000 podval-0.9/podval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 22:49:19.352454 podval-0.9/setup.cfg
--rw-rw-rw-   0        0        0      173 2023-06-03 22:49:06.000000 podval-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:23:22.000000 podval-1.0/
+-rw-rw-rw-   0        0        0      188 2023-06-04 17:23:22.000000 podval-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 17:23:22.000000 podval-1.0/podval/
+-rw-rw-rw-   0        0        0    23935 2023-06-04 17:19:38.000000 podval-1.0/podval/podval.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:23:22.000000 podval-1.0/podval.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-03 21:34:23.000000 podval-1.0/podval.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-04 17:23:21.000000 podval-1.0/podval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:23:22.000000 podval-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-04 17:21:18.000000 podval-1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

