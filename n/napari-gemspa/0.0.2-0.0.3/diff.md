# Comparing `tmp/napari-gemspa-0.0.2.tar.gz` & `tmp/napari-gemspa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-gemspa-0.0.2.tar", last modified: Sat Jun  3 23:48:14 2023, max compression
+gzip compressed data, was "napari-gemspa-0.0.3.tar", last modified: Sun Jun  4 00:07:09 2023, max compression
```

## Comparing `napari-gemspa-0.0.2.tar` & `napari-gemspa-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.881116 napari-gemspa-0.0.2/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1512 2023-04-13 14:56:39.000000 napari-gemspa-0.0.2/LICENSE
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       96 2023-04-02 00:08:59.000000 napari-gemspa-0.0.2/MANIFEST.in
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     9798 2023-06-03 23:48:14.881227 napari-gemspa-0.0.2/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8524 2023-06-03 23:42:01.000000 napari-gemspa-0.0.2/README.md
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      130 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/pyproject.toml
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1761 2023-06-03 23:48:14.881777 napari-gemspa-0.0.2/setup.cfg
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.874477 napari-gemspa-0.0.2/src/
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.876077 napari-gemspa-0.0.2/src/_tests/
--rw-------   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/_tests/__init__.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1777 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/_tests/run_napari.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     3224 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/_tests/test_gemspa_locate_worker.py
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.880060 napari-gemspa-0.0.2/src/napari_gemspa/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      320 2023-05-29 19:40:41.000000 napari-gemspa-0.0.2/src/napari_gemspa/__init__.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    25898 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_analyze_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    19439 2023-06-03 18:51:07.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_data_views.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8770 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_file_import_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     6596 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_filter_links_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     6021 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_link_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     8503 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_locate_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)    10201 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_plugin.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     7789 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_widget.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     2582 2023-05-22 18:46:47.000000 napari-gemspa-0.0.2/src/napari_gemspa/_reader.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1764 2023-05-24 21:55:19.000000 napari-gemspa-0.0.2/src/napari_gemspa/_utils.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     3553 2023-06-03 16:24:39.000000 napari-gemspa-0.0.2/src/napari_gemspa/_writer.py
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     1352 2023-05-29 19:40:41.000000 napari-gemspa-0.0.2/src/napari_gemspa/napari.yaml
-drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 23:48:14.881000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/
--rw-r--r--   0 sarahkeegan   (501) staff       (20)     9798 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/PKG-INFO
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      873 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/SOURCES.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)        1 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/dependency_links.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       60 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/entry_points.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)      137 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/requires.txt
--rw-r--r--   0 sarahkeegan   (501) staff       (20)       21 2023-06-03 23:48:14.000000 napari-gemspa-0.0.2/src/napari_gemspa.egg-info/top_level.txt
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.946341 napari-gemspa-0.0.3/
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1512 2023-04-13 14:56:39.000000 napari-gemspa-0.0.3/LICENSE
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)       96 2023-04-02 00:08:59.000000 napari-gemspa-0.0.3/MANIFEST.in
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    11015 2023-06-04 00:07:09.946491 napari-gemspa-0.0.3/PKG-INFO
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     9741 2023-06-04 00:05:29.000000 napari-gemspa-0.0.3/README.md
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      130 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/pyproject.toml
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1761 2023-06-04 00:07:09.946987 napari-gemspa-0.0.3/setup.cfg
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.939971 napari-gemspa-0.0.3/src/
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.941502 napari-gemspa-0.0.3/src/_tests/
+-rw-------   0 sarahkeegan   (501) staff       (20)        0 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/_tests/__init__.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1777 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/_tests/run_napari.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     3224 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/_tests/test_gemspa_locate_worker.py
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.945159 napari-gemspa-0.0.3/src/napari_gemspa/
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      320 2023-05-29 19:40:41.000000 napari-gemspa-0.0.3/src/napari_gemspa/__init__.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    25898 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_analyze_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    19439 2023-06-03 18:51:07.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_data_views.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     8770 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_file_import_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     6596 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_filter_links_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     6021 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_link_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     8503 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_locate_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    10201 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_plugin.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     7789 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_widget.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     2582 2023-05-22 18:46:47.000000 napari-gemspa-0.0.3/src/napari_gemspa/_reader.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1764 2023-05-24 21:55:19.000000 napari-gemspa-0.0.3/src/napari_gemspa/_utils.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     3553 2023-06-03 16:24:39.000000 napari-gemspa-0.0.3/src/napari_gemspa/_writer.py
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)     1352 2023-05-29 19:40:41.000000 napari-gemspa-0.0.3/src/napari_gemspa/napari.yaml
+drwxr-xr-x   0 sarahkeegan   (501) staff       (20)        0 2023-06-04 00:07:09.946182 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)    11015 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/PKG-INFO
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      873 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/SOURCES.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)        1 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/dependency_links.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)       60 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/entry_points.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)      137 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/requires.txt
+-rw-r--r--   0 sarahkeegan   (501) staff       (20)       21 2023-06-04 00:07:09.000000 napari-gemspa-0.0.3/src/napari_gemspa.egg-info/top_level.txt
```

### Comparing `napari-gemspa-0.0.2/LICENSE` & `napari-gemspa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/setup.cfg` & `napari-gemspa-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-gemspa
-version = 0.0.2
+version = 0.0.3
 description = A plugin for analysis of single particle tracking experiments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/liamholtlab/napari-gemspa
 author = Sarah Keegan
 author_email = sarah.keegan@nyulangone.org
 license = BSD-3-Clause
```

### Comparing `napari-gemspa-0.0.2/src/_tests/run_napari.py` & `napari-gemspa-0.0.3/src/_tests/run_napari.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/_tests/test_gemspa_locate_worker.py` & `napari-gemspa-0.0.3/src/_tests/test_gemspa_locate_worker.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_analyze_widget.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_analyze_widget.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_data_views.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_data_views.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_file_import_widget.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_file_import_widget.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_filter_links_widget.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_filter_links_widget.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_link_widget.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_link_widget.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_locate_widget.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_locate_widget.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_plugin.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_plugin.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_gemspa_widget.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_gemspa_widget.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_reader.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_utils.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/_writer.py` & `napari-gemspa-0.0.3/src/napari_gemspa/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa/napari.yaml` & `napari-gemspa-0.0.3/src/napari_gemspa/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-gemspa-0.0.2/src/napari_gemspa.egg-info/SOURCES.txt` & `napari-gemspa-0.0.3/src/napari_gemspa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

