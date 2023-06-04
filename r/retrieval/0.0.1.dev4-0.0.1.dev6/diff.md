# Comparing `tmp/retrieval-0.0.1.dev4.tar.gz` & `tmp/retrieval-0.0.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retrieval-0.0.1.dev4.tar", last modified: Wed Oct 12 17:41:05 2022, max compression
+gzip compressed data, was "retrieval-0.0.1.dev6.tar", last modified: Sun Jun  4 21:06:32 2023, max compression
```

## Comparing `retrieval-0.0.1.dev4.tar` & `retrieval-0.0.1.dev6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-10-12 17:41:05.067742 retrieval-0.0.1.dev4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2022-09-27 22:08:38.000000 retrieval-0.0.1.dev4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      502 2022-10-12 17:41:05.063742 retrieval-0.0.1.dev4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      194 2022-10-12 17:34:58.000000 retrieval-0.0.1.dev4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-10-12 17:41:05.063742 retrieval-0.0.1.dev4/retrieval.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      502 2022-10-12 17:41:05.000000 retrieval-0.0.1.dev4/retrieval.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2022-10-12 17:41:05.000000 retrieval-0.0.1.dev4/retrieval.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-10-12 17:41:05.000000 retrieval-0.0.1.dev4/retrieval.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2022-10-12 17:41:05.000000 retrieval-0.0.1.dev4/retrieval.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-10-12 17:41:05.000000 retrieval-0.0.1.dev4/retrieval.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2022-10-12 17:41:05.067742 retrieval-0.0.1.dev4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      855 2022-10-12 17:40:48.000000 retrieval-0.0.1.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:32.088511 retrieval-0.0.1.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 21:06:17.000000 retrieval-0.0.1.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-04 21:06:32.088511 retrieval-0.0.1.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-04 21:06:17.000000 retrieval-0.0.1.dev6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 21:06:32.088511 retrieval-0.0.1.dev6/retrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-04 21:06:32.000000 retrieval-0.0.1.dev6/retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-04 21:06:32.000000 retrieval-0.0.1.dev6/retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:06:32.000000 retrieval-0.0.1.dev6/retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-04 21:06:32.000000 retrieval-0.0.1.dev6/retrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 21:06:32.000000 retrieval-0.0.1.dev6/retrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 21:06:32.088511 retrieval-0.0.1.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-04 21:06:17.000000 retrieval-0.0.1.dev6/setup.py
```

### Comparing `retrieval-0.0.1.dev4/LICENSE` & `retrieval-0.0.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `retrieval-0.0.1.dev4/setup.py` & `retrieval-0.0.1.dev6/setup.py`

 * *Files identical despite different names*

