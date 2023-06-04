# Comparing `tmp/helloworld_deshrit-0.0.1.tar.gz` & `tmp/helloworld_deshrit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helloworld_deshrit-0.0.1.tar", last modified: Sun Jun  4 13:32:29 2023, max compression
+gzip compressed data, was "helloworld_deshrit-0.0.2.tar", last modified: Sun Jun  4 14:23:39 2023, max compression
```

## Comparing `helloworld_deshrit-0.0.1.tar` & `helloworld_deshrit-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 13:32:29.371957 helloworld_deshrit-0.0.1/
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      121 2023-06-04 13:32:29.371957 helloworld_deshrit-0.0.1/PKG-INFO
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       38 2023-06-04 13:32:29.371957 helloworld_deshrit-0.0.1/setup.cfg
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      203 2023-06-04 13:18:14.000000 helloworld_deshrit-0.0.1/setup.py
-drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 13:32:29.363957 helloworld_deshrit-0.0.1/src/
-drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 13:32:29.367957 helloworld_deshrit-0.0.1/src/helloworld_deshrit.egg-info/
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      121 2023-06-04 13:32:29.000000 helloworld_deshrit-0.0.1/src/helloworld_deshrit.egg-info/PKG-INFO
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      240 2023-06-04 13:32:29.000000 helloworld_deshrit-0.0.1/src/helloworld_deshrit.egg-info/SOURCES.txt
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)        1 2023-06-04 13:32:29.000000 helloworld_deshrit-0.0.1/src/helloworld_deshrit.egg-info/dependency_links.txt
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       11 2023-06-04 13:32:29.000000 helloworld_deshrit-0.0.1/src/helloworld_deshrit.egg-info/top_level.txt
-drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 13:32:29.371957 helloworld_deshrit-0.0.1/src/hw_deshrit/
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 13:25:16.000000 helloworld_deshrit-0.0.1/src/hw_deshrit/__init__.py
--rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       56 2023-06-04 13:13:58.000000 helloworld_deshrit-0.0.1/src/hw_deshrit/hw.py
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 14:23:39.210129 helloworld_deshrit-0.0.2/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      172 2023-06-04 14:23:39.210129 helloworld_deshrit-0.0.2/PKG-INFO
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       38 2023-06-04 14:23:39.210129 helloworld_deshrit-0.0.2/setup.cfg
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      264 2023-06-04 14:23:15.000000 helloworld_deshrit-0.0.2/setup.py
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 14:23:39.210129 helloworld_deshrit-0.0.2/src/
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 14:23:39.210129 helloworld_deshrit-0.0.2/src/helloworld_deshrit.egg-info/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      172 2023-06-04 14:23:39.000000 helloworld_deshrit-0.0.2/src/helloworld_deshrit.egg-info/PKG-INFO
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)      240 2023-06-04 14:23:39.000000 helloworld_deshrit-0.0.2/src/helloworld_deshrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)        1 2023-06-04 14:23:39.000000 helloworld_deshrit-0.0.2/src/helloworld_deshrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       11 2023-06-04 14:23:39.000000 helloworld_deshrit-0.0.2/src/helloworld_deshrit.egg-info/top_level.txt
+drwxrwxr-x   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 14:23:39.210129 helloworld_deshrit-0.0.2/src/hw_deshrit/
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)        0 2023-06-04 13:25:16.000000 helloworld_deshrit-0.0.2/src/hw_deshrit/__init__.py
+-rw-rw-r--   0 deshrit   (1000) deshrit   (1000)       56 2023-06-04 13:13:58.000000 helloworld_deshrit-0.0.2/src/hw_deshrit/hw.py
```

