# Comparing `tmp/whg-lotr-sdk-0.1.tar.gz` & `tmp/whg-lotr-sdk-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\whg-lotr-sdk-0.1.tar", last modified: Sun Jun  4 20:21:00 2023, max compression
+gzip compressed data, was "dist\whg-lotr-sdk-0.2.tar", last modified: Sun Jun  4 20:24:59 2023, max compression
```

## Comparing `whg-lotr-sdk-0.1.tar` & `whg-lotr-sdk-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/
--rw-rw-rw-   0        0        0      225 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/
-drwxrwxrwx   0        0        0        0 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/handlers/
--rw-rw-rw-   0        0        0        0 2023-06-04 18:35:30.000000 whg-lotr-sdk-0.1/sdk/handlers/__init__.py
--rw-rw-rw-   0        0        0     2492 2023-06-04 19:45:57.000000 whg-lotr-sdk-0.1/sdk/handlers/base_handler.py
--rw-rw-rw-   0        0        0     1030 2023-06-04 20:18:26.000000 whg-lotr-sdk-0.1/sdk/handlers/movie_handler.py
--rw-rw-rw-   0        0        0     1209 2023-06-04 20:19:49.000000 whg-lotr-sdk-0.1/sdk/handlers/quote_handler.py
-drwxrwxrwx   0        0        0        0 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/whg_lotr_sdk.egg-info/
--rw-rw-rw-   0        0        0      225 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/whg_lotr_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/whg_lotr_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/whg_lotr_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/whg_lotr_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/sdk/whg_lotr_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 20:21:00.000000 whg-lotr-sdk-0.1/setup.cfg
--rw-rw-rw-   0        0        0      337 2023-06-04 20:16:35.000000 whg-lotr-sdk-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/
+-rw-rw-rw-   0        0        0      225 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/sdk/
+drwxrwxrwx   0        0        0        0 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/sdk/handlers/
+-rw-rw-rw-   0        0        0        0 2023-06-04 18:35:30.000000 whg-lotr-sdk-0.2/sdk/handlers/__init__.py
+-rw-rw-rw-   0        0        0     2492 2023-06-04 19:45:57.000000 whg-lotr-sdk-0.2/sdk/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1030 2023-06-04 20:18:26.000000 whg-lotr-sdk-0.2/sdk/handlers/movie_handler.py
+-rw-rw-rw-   0        0        0     1209 2023-06-04 20:19:49.000000 whg-lotr-sdk-0.2/sdk/handlers/quote_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/sdk/whg_lotr_sdk.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-06-04 20:24:58.000000 whg-lotr-sdk-0.2/sdk/whg_lotr_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/sdk/whg_lotr_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 20:24:58.000000 whg-lotr-sdk-0.2/sdk/whg_lotr_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 20:24:58.000000 whg-lotr-sdk-0.2/sdk/whg_lotr_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-04 20:24:58.000000 whg-lotr-sdk-0.2/sdk/whg_lotr_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 20:24:59.000000 whg-lotr-sdk-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      339 2023-06-04 20:24:46.000000 whg-lotr-sdk-0.2/setup.py
```

### Comparing `whg-lotr-sdk-0.1/sdk/handlers/base_handler.py` & `whg-lotr-sdk-0.2/sdk/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `whg-lotr-sdk-0.1/sdk/handlers/movie_handler.py` & `whg-lotr-sdk-0.2/sdk/handlers/movie_handler.py`

 * *Files identical despite different names*

### Comparing `whg-lotr-sdk-0.1/sdk/handlers/quote_handler.py` & `whg-lotr-sdk-0.2/sdk/handlers/quote_handler.py`

 * *Files identical despite different names*

