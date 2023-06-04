# Comparing `tmp/fetch-lyrics-from-genius-0.1.1.tar.gz` & `tmp/fetch-lyrics-from-genius-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetch-lyrics-from-genius-0.1.1.tar", last modified: Sun Jun  4 20:07:35 2023, max compression
+gzip compressed data, was "fetch-lyrics-from-genius-0.1.2.tar", last modified: Sun Jun  4 20:11:03 2023, max compression
```

## Comparing `fetch-lyrics-from-genius-0.1.1.tar` & `fetch-lyrics-from-genius-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:07:35.325181 fetch-lyrics-from-genius-0.1.1/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-03-25 11:31:07.000000 fetch-lyrics-from-genius-0.1.1/LICENSE
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      200 2023-06-04 20:07:35.324925 fetch-lyrics-from-genius-0.1.1/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      103 2023-03-25 11:31:07.000000 fetch-lyrics-from-genius-0.1.1/README.md
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:07:35.319846 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:01:49.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius/__init__.py
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)     5526 2023-03-26 02:02:49.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius/fetch_lyrics.py
-drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:07:35.324438 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      200 2023-06-04 20:07:35.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/PKG-INFO
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      394 2023-06-04 20:07:35.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-04 20:07:35.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       88 2023-06-04 20:07:35.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/entry_points.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       43 2023-06-04 20:07:35.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/requires.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       25 2023-06-04 20:07:35.000000 fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius.egg-info/top_level.txt
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-04 20:07:35.325242 fetch-lyrics-from-genius-0.1.1/setup.cfg
--rw-r--r--   0 andrew.beveridge   (503) staff       (20)      528 2023-06-04 20:06:35.000000 fetch-lyrics-from-genius-0.1.1/setup.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:11:03.713787 fetch-lyrics-from-genius-0.1.2/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     1069 2023-03-25 11:31:07.000000 fetch-lyrics-from-genius-0.1.2/LICENSE
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      344 2023-06-04 20:11:03.713442 fetch-lyrics-from-genius-0.1.2/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      103 2023-03-25 11:31:07.000000 fetch-lyrics-from-genius-0.1.2/README.md
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:11:03.708704 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:01:49.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius/__init__.py
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)     5526 2023-03-26 02:02:49.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius/fetch_lyrics.py
+drwxr-xr-x   0 andrew.beveridge   (503) staff       (20)        0 2023-06-04 20:11:03.712955 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      344 2023-06-04 20:11:03.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      394 2023-06-04 20:11:03.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)        1 2023-06-04 20:11:03.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       88 2023-06-04 20:11:03.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/entry_points.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       43 2023-06-04 20:11:03.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/requires.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       25 2023-06-04 20:11:03.000000 fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius.egg-info/top_level.txt
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)       38 2023-06-04 20:11:03.713848 fetch-lyrics-from-genius-0.1.2/setup.cfg
+-rw-r--r--   0 andrew.beveridge   (503) staff       (20)      817 2023-06-04 20:10:21.000000 fetch-lyrics-from-genius-0.1.2/setup.py
```

### Comparing `fetch-lyrics-from-genius-0.1.1/LICENSE` & `fetch-lyrics-from-genius-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fetch-lyrics-from-genius-0.1.1/fetch_lyrics_from_genius/fetch_lyrics.py` & `fetch-lyrics-from-genius-0.1.2/fetch_lyrics_from_genius/fetch_lyrics.py`

 * *Files identical despite different names*

