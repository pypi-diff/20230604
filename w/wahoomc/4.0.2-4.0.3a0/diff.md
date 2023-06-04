# Comparing `tmp/wahoomc-4.0.2.tar.gz` & `tmp/wahoomc-4.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wahoomc-4.0.2.tar", last modified: Sat May  6 08:02:52 2023, max compression
+gzip compressed data, was "wahoomc-4.0.3a0.tar", last modified: Sun Jun  4 19:25:45 2023, max compression
```

## Comparing `wahoomc-4.0.2.tar` & `wahoomc-4.0.3a0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.507640 wahoomc-4.0.2/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4401 2023-05-06 08:02:52.507756 wahoomc-4.0.2/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3862 2023-05-05 19:23:35.000000 wahoomc-4.0.2/README.md
--rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.2/pyproject.toml
--rw-r--r--   0 bkreusc  (1890165452) 58041779      827 2023-05-06 08:02:52.508151 wahoomc-4.0.2/setup.cfg
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.494531 wahoomc-4.0.2/tests/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.2/tests/test_cli.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-05-05 19:23:35.000000 wahoomc-4.0.2/tests/test_constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     5494 2023-05-05 19:23:35.000000 wahoomc-4.0.2/tests/test_constants_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-05-05 19:23:35.000000 wahoomc-4.0.2/tests/test_downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-05-05 19:23:35.000000 wahoomc-4.0.2/tests/test_generated_files.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     9487 2023-05-05 19:23:35.000000 wahoomc-4.0.2/tests/test_geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     7214 2023-05-05 19:23:35.000000 wahoomc-4.0.2/tests/test_osm_maps.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.2/tests/test_setup.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.497635 wahoomc-4.0.2/wahoomc/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.2/wahoomc/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1590 2023-05-06 08:00:24.000000 wahoomc-4.0.2/wahoomc/constants.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/constants_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    12209 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/downloader.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     5720 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/file_directory_functions.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    21372 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/geofabrik.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4635 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/geofabrik_json.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.498572 wahoomc-4.0.2/wahoomc/init/
--rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.2/wahoomc/init/__init__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.2/wahoomc/init/__main__.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    18039 2023-05-06 07:59:43.000000 wahoomc-4.0.2/wahoomc/input.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779     3668 2023-05-06 07:59:43.000000 wahoomc-4.0.2/wahoomc/main.py
--rw-r--r--   0 bkreusc  (1890165452) 58041779    40391 2023-05-06 07:59:43.000000 wahoomc-4.0.2/wahoomc/osm_maps_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.499673 wahoomc-4.0.2/wahoomc/resources/
--rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/resources/sea.osm
--rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/resources/shape2osm.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.500108 wahoomc-4.0.2/wahoomc/resources/tag_wahoo_adjusted/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     9575 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.2/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.501157 wahoomc-4.0.2/wahoomc/resources/tag_wahoo_initial/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779     2304 2023-05-05 19:21:07.000000 wahoomc-4.0.2/wahoomc/resources/tags-to-keep.json
--rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.2/wahoomc/resources/tunnel-transform.xml
--rw-r--r--   0 bkreusc  (1890165452) 58041779    10562 2023-05-05 19:23:35.000000 wahoomc-4.0.2/wahoomc/setup_functions.py
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.506882 wahoomc-4.0.2/wahoomc/tooling_win/
--rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/tooling_win/7za.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/tooling_win/7za.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.2/wahoomc/tooling_win/7zxa.dll
--rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.2/wahoomc/tooling_win/lzma.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.2/wahoomc/tooling_win/osmconvert.exe
--rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.2/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
-drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-05-06 08:02:52.498298 wahoomc-4.0.2/wahoomc.egg-info/
--rw-r--r--   0 bkreusc  (1890165452) 58041779     4401 2023-05-06 08:02:52.000000 wahoomc-4.0.2/wahoomc.egg-info/PKG-INFO
--rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-05-06 08:02:52.000000 wahoomc-4.0.2/wahoomc.egg-info/SOURCES.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-05-06 08:02:52.000000 wahoomc-4.0.2/wahoomc.egg-info/dependency_links.txt
--rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-05-06 08:02:52.000000 wahoomc-4.0.2/wahoomc.egg-info/top_level.txt
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.374887 wahoomc-4.0.3a0/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-06-04 19:25:45.375048 wahoomc-4.0.3a0/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3862 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/README.md
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      103 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/pyproject.toml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      829 2023-06-04 19:25:45.376099 wahoomc-4.0.3a0/setup.cfg
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.351466 wahoomc-4.0.3a0/tests/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      812 2022-10-06 21:14:05.000000 wahoomc-4.0.3a0/tests/test_cli.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6758 2023-06-04 19:22:17.000000 wahoomc-4.0.3a0/tests/test_constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5494 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_constants_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7030 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10238 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_generated_files.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     9487 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     7214 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/tests/test_osm_maps.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3514 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/tests/test_setup.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.355392 wahoomc-4.0.3a0/wahoomc/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      131 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/wahoomc/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1592 2023-06-04 19:25:01.000000 wahoomc-4.0.3a0/wahoomc/constants.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4597 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/constants_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    12209 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/downloader.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     5720 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/file_directory_functions.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    21372 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/geofabrik.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4635 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/geofabrik_json.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.356645 wahoomc-4.0.3a0/wahoomc/init/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        0 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/wahoomc/init/__init__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      137 2023-03-27 20:10:10.000000 wahoomc-4.0.3a0/wahoomc/init/__main__.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    18039 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/input.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     3668 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/main.py
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    39982 2023-06-04 19:22:20.000000 wahoomc-4.0.3a0/wahoomc/osm_maps_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.358095 wahoomc-4.0.3a0/wahoomc/resources/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      824 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/resources/sea.osm
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    15766 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/resources/shape2osm.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.358660 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     9834 2023-06-04 19:22:17.000000 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    41694 2022-10-09 22:58:21.000000 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.359686 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_initial/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     6354 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     2360 2023-06-04 19:22:17.000000 wahoomc-4.0.3a0/wahoomc/resources/tags-to-keep.json
+-rw-r--r--   0 bkreusc  (1890165452) 58041779      511 2023-03-27 20:10:11.000000 wahoomc-4.0.3a0/wahoomc/resources/tunnel-transform.xml
+-rw-r--r--   0 bkreusc  (1890165452) 58041779    10562 2023-05-15 21:32:03.000000 wahoomc-4.0.3a0/wahoomc/setup_functions.py
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.374011 wahoomc-4.0.3a0/wahoomc/tooling_win/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   269312 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/7za.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   739840 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/7za.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   158720 2022-05-21 18:01:35.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/7zxa.dll
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   108544 2022-05-21 18:01:36.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/lzma.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   299998 2022-11-29 06:53:00.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert.exe
+-rw-r--r--   0 bkreusc  (1890165452) 58041779   311997 2022-11-29 06:53:00.000000 wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert64-0.8.8p.exe
+drwxr-xr-x   0 bkreusc  (1890165452) 58041779        0 2023-06-04 19:25:45.356275 wahoomc-4.0.3a0/wahoomc.egg-info/
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     4403 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/PKG-INFO
+-rw-r--r--   0 bkreusc  (1890165452) 58041779     1183 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/SOURCES.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        1 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/dependency_links.txt
+-rw-r--r--   0 bkreusc  (1890165452) 58041779        8 2023-06-04 19:25:45.000000 wahoomc-4.0.3a0/wahoomc.egg-info/top_level.txt
```

### Comparing `wahoomc-4.0.2/PKG-INFO` & `wahoomc-4.0.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.2
+Version: 4.0.3a0
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.2 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.3a0 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
```

### Comparing `wahoomc-4.0.2/README.md` & `wahoomc-4.0.3a0/README.md`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/setup.cfg` & `wahoomc-4.0.3a0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wahoomc
-version = 4.0.2
+version = 4.0.3a0
 author = Benjamin Kreuscher
 author_email = benni.kreuscher@gmail.com
 description = Create maps for your Wahoo bike computer based on latest OSM maps
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/treee111/wahooMapsCreator
 project_urls =
```

### Comparing `wahoomc-4.0.2/tests/test_cli.py` & `wahoomc-4.0.3a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_constants.py` & `wahoomc-4.0.3a0/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_constants_geofabrik.py` & `wahoomc-4.0.3a0/tests/test_constants_geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_downloader.py` & `wahoomc-4.0.3a0/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_generated_files.py` & `wahoomc-4.0.3a0/tests/test_generated_files.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_geofabrik.py` & `wahoomc-4.0.3a0/tests/test_geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_osm_maps.py` & `wahoomc-4.0.3a0/tests/test_osm_maps.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/tests/test_setup.py` & `wahoomc-4.0.3a0/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/constants.py` & `wahoomc-4.0.3a0/wahoomc/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 # Python Package - wahooMapsCreator directory
 WAHOO_MC_DIR = os.path.dirname(__file__)
 RESOURCES_DIR = os.path.join(WAHOO_MC_DIR, 'resources')
 TOOLING_WIN_DIR = os.path.join(WAHOO_MC_DIR, 'tooling_win')
 # location of repo / python installation - not used
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir))
-VERSION = '4.0.2'
+VERSION = '4.0.3a0'
 
 
 block_download = ['dach', 'alps', 'britain-and-ireland', 'south-africa-and-lesotho',
                   'us-midwest', 'us-northeast', 'us-pacific', 'us-south', 'us-west']
 
 # Special_regions like (former) colonies where the map of the wanted region is not present in the map of the parent country.
 # example Guadeloupe, it's Geofabrik parent country is France but Guadeloupe is not located within the region covered by the map of France.
```

### Comparing `wahoomc-4.0.2/wahoomc/constants_functions.py` & `wahoomc-4.0.3a0/wahoomc/constants_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/downloader.py` & `wahoomc-4.0.3a0/wahoomc/downloader.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/file_directory_functions.py` & `wahoomc-4.0.3a0/wahoomc/file_directory_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/geofabrik.py` & `wahoomc-4.0.3a0/wahoomc/geofabrik.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/geofabrik_json.py` & `wahoomc-4.0.3a0/wahoomc/geofabrik_json.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/input.py` & `wahoomc-4.0.3a0/wahoomc/input.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/main.py` & `wahoomc-4.0.3a0/wahoomc/main.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/osm_maps_functions.py` & `wahoomc-4.0.3a0/wahoomc/osm_maps_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,38 +36,32 @@
 
 
 def run_subprocess_and_log_output(cmd, error_message, cwd=""):
     """
     run given cmd-subprocess and issue error message if wished
     """
     if not cwd:
-        process = subprocess.Popen(
-            cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        process = subprocess.run(
+            cmd, capture_output=True, text=True, encoding="utf-8", check=True)
+
     else:
-        process = subprocess.Popen(  # pylint: disable=consider-using-with
-            cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd)
+        process = subprocess.run(  # pylint: disable=consider-using-with
+            cmd, capture_output=True, cwd=cwd, text=True, encoding="utf-8", check=True)
 
-    if error_message and process.wait() != 0:  # 0 means success
-        for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
-            # print(line.rstrip())
-            try:
-                log.error('subprocess:%r', line.decode("utf-8").strip())
-            except UnicodeDecodeError:
-                log.error('subprocess:%r', line.decode("latin-1").strip())
+    if error_message and process.returncode != 0:  # 0 means success
+        log.error('subprocess error output:')
+        if process.stderr:
+            log.error(process.stderr)
 
         log.error(error_message)
         sys.exit()
 
-    else:
-        for line in iter(process.stdout.readline, b''):  # b'\n'-separated lines
-            # print(line.rstrip())
-            try:
-                log.debug('subprocess:%r', line.decode("utf-8").strip())
-            except UnicodeDecodeError:
-                log.debug('subprocess:%r', line.decode("latin-1").strip())
+    elif process.stdout:
+        log.debug('subprocess debug output:')
+        log.debug(process.stdout)
 
 
 def get_timestamp_last_changed(file_path):
     """
     returns the timestamp of the last-changed datetime of the given file
     """
     chg_time = os.path.getmtime(file_path)
```

### Comparing `wahoomc-4.0.2/wahoomc/resources/sea.osm` & `wahoomc-4.0.3a0/wahoomc/resources/sea.osm`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/resources/shape2osm.py` & `wahoomc-4.0.3a0/wahoomc/resources/shape2osm.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml` & `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml`

 * *Files 1% similar despite different names*

#### Comparing `wahoomc-4.0.2/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml` & `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo-poi.xml`

```diff
@@ -1,27 +1,31 @@
 <?xml version="1.0" encoding="utf-8"?>
 <tag-mapping xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://mapsforge.org/tag-mapping" default-zoom-appear="16" profile-name="default-profile" xsi:schemaLocation="http://mapsforge.org/tag-mapping https://raw.githubusercontent.com/mapsforge/mapsforge/master/resources/tag-mapping.xsd">
   <!-- ************* POIS *************** -->
   <pois>
     <osm-tag key="amenity" value="fuel" zoom-appear="14"/>
     <osm-tag key="amenity" value="cafe" zoom-appear="14"/>
     <osm-tag key="amenity" value="drinking_water" zoom-appear="14"/>
+    <osm-tag key="amenity" value="shelter" zoom-appear="10"/>
     <osm-tag key="shop" value="bakery" zoom-appear="14"/>
     <osm-tag key="shop" value="bicycle" zoom-appear="14"/>
     <osm-tag key="railway" value="station" zoom-appear="13"/>
     <osm-tag key="railway" value="stop" zoom-appear="13"/>
+    <osm-tag key="tourism" value="alpine_hut" zoom-appear="10"/>
   </pois>
   <ways>
     <osm-tag key="amenity" label-position="true" value="fuel" zoom-appear="14"/>
     <osm-tag key="amenity" label-position="true" value="cafe" zoom-appear="14"/>
     <osm-tag key="amenity" label-position="true" value="drinking_water" zoom-appear="14"/>
+    <osm-tag key="amenity" value="shelter" zoom-appear="10"/>
     <osm-tag key="shop" label-position="true" value="bakery" zoom-appear="14"/>
     <osm-tag key="shop" label-position="true" value="bicycle" zoom-appear="14"/>
     <osm-tag key="railway" label-position="true" value="station" zoom-appear="13"/>
     <osm-tag key="railway" label-position="true" value="stop" zoom-appear="13"/>
+    <osm-tag key="tourism" value="alpine_hut" zoom-appear="10"/>
   </ways>
   <ways>
     <osm-tag key="contour_ext" value="elevation_minor" zoom-appear="12" force-polygon-line="true"/>
     <osm-tag key="contour_ext" value="elevation_medium" zoom-appear="12" force-polygon-line="true"/>
     <osm-tag key="contour_ext" value="elevation_major" zoom-appear="12" force-polygon-line="true"/>
     <osm-tag key="ele" value="100" zoom-appear="14"/>
     <osm-tag key="ele" value="200" zoom-appear="14"/>
```

### Comparing `wahoomc-4.0.2/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml` & `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_adjusted/tag-wahoo.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml` & `wahoomc-4.0.3a0/wahoomc/resources/tag_wahoo_initial/tag-wahoo_original.xml`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/resources/tags-to-keep.json` & `wahoomc-4.0.3a0/wahoomc/resources/tags-to-keep.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'TAGS_TO_KEEP_UNIVERSAL'": "{'amenity': {insert: [(3, 'shelter')]}, 'tourism': 'alpine_hut'}"}*

```diff
@@ -18,15 +18,16 @@
         ]
     },
     "TAGS_TO_KEEP_UNIVERSAL": {
         "access": "",
         "amenity": [
             "fuel",
             "cafe",
-            "drinking_water"
+            "drinking_water",
+            "shelter"
         ],
         "area": "yes",
         "bicycle": "",
         "bridge": "",
         "foot": [
             "ft_yes",
             "foot_designated"
@@ -89,14 +90,15 @@
             "stop"
         ],
         "shop": [
             "bakery",
             "bicycle"
         ],
         "surface": "",
+        "tourism": "alpine_hut",
         "tracktype": "",
         "tunnel": "",
         "waterway": [
             "canal",
             "drain",
             "river",
             "riverbank",
```

### Comparing `wahoomc-4.0.2/wahoomc/setup_functions.py` & `wahoomc-4.0.3a0/wahoomc/setup_functions.py`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/tooling_win/7za.dll` & `wahoomc-4.0.3a0/wahoomc/tooling_win/7za.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/tooling_win/7za.exe` & `wahoomc-4.0.3a0/wahoomc/tooling_win/7za.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/tooling_win/7zxa.dll` & `wahoomc-4.0.3a0/wahoomc/tooling_win/7zxa.dll`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/tooling_win/lzma.exe` & `wahoomc-4.0.3a0/wahoomc/tooling_win/lzma.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/tooling_win/osmconvert.exe` & `wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc/tooling_win/osmconvert64-0.8.8p.exe` & `wahoomc-4.0.3a0/wahoomc/tooling_win/osmconvert64-0.8.8p.exe`

 * *Files identical despite different names*

### Comparing `wahoomc-4.0.2/wahoomc.egg-info/PKG-INFO` & `wahoomc-4.0.3a0/wahoomc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wahoomc
-Version: 4.0.2
+Version: 4.0.3a0
 Summary: Create maps for your Wahoo bike computer based on latest OSM maps
 Home-page: https://github.com/treee111/wahooMapsCreator
 Author: Benjamin Kreuscher
 Author-email: benni.kreuscher@gmail.com
 Project-URL: Bug Tracker, https://github.com/treee111/wahooMapsCreator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wahoomc Version: 4.0.2 Summary: Create maps for
+Metadata-Version: 2.1 Name: wahoomc Version: 4.0.3a0 Summary: Create maps for
 your Wahoo bike computer based on latest OSM maps Home-page: https://
 github.com/treee111/wahooMapsCreator Author: Benjamin Kreuscher Author-email:
 benni.kreuscher@gmail.com Project-URL: Bug Tracker, https://github.com/
 treee111/wahooMapsCreator/issues Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.10 Description-Content-Type:
 text/markdown
```

### Comparing `wahoomc-4.0.2/wahoomc.egg-info/SOURCES.txt` & `wahoomc-4.0.3a0/wahoomc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

