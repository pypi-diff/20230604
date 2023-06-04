# Comparing `tmp/batogram-1.0.8.tar.gz` & `tmp/batogram-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batogram-1.0.8.tar", last modified: Sun Jun  4 17:12:13 2023, max compression
+gzip compressed data, was "batogram-1.0.9.tar", last modified: Sun Jun  4 17:50:27 2023, max compression
```

## Comparing `batogram-1.0.8.tar` & `batogram-1.0.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.864102 batogram-1.0.8/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.0.8/LICENSE
--rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.0.8/MANIFEST.in
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:12:13.864102 batogram-1.0.8/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4611 2023-06-04 17:11:53.000000 batogram-1.0.8/README.md
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.804101 batogram-1.0.8/batogram/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-06-04 17:06:48.000000 batogram-1.0.8/batogram/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/__main__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/about.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4648 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/amplitudegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6212 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/appsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/appsettingsmodal.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.816102 batogram-1.0.8/batogram/assets/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/3669170_home_ic_icon.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-left-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-left-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-right-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-right-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/batogram.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/download-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/drag-move-2-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/expand-left-right-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/expand-up-down-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/fullscreen-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/home-4-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/zoom-in-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7542 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/audiofileservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/breadcrumbservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/buttonframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/chunky_spectrogram.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.845102 batogram-1.0.8/batogram/colour_maps/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L01.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L03.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L05.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L06.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L07.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L08.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L09.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L16.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L17.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L18.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L19.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L20.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/black-body-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/inferno-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colourmap.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1658 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/common.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1817 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/constants.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.854102 batogram-1.0.8/batogram/external/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/external/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/external/guano.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/external/tooltip.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/fileinfoframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2968 2023-05-17 18:30:45.000000 batogram-1.0.8/batogram/frames.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5588 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/graphsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/historianservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    31653 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/layouts.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    31047 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/markers.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1134 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/modalwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    28313 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/morebncframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    12440 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/moreframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/morerenderingframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6851 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/morescaleframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4610 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/profilegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/readoutframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    59357 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/rendering.py
--rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35194 2023-06-04 16:22:36.000000 batogram-1.0.8/batogram/rootwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/runner.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.863103 batogram-1.0.8/batogram/samples/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/samples/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    21200 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/spectrogramgraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    16042 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/spectrogrammouseservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/validatingwidgets.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    13442 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/wavfileparser.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.808102 batogram-1.0.8/batogram.egg-info/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2282 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/SOURCES.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/dependency_links.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/entry_points.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/requires.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/top_level.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-06-04 17:07:09.000000 batogram-1.0.8/pyproject.toml
--rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-06-04 17:12:13.865102 batogram-1.0.8/setup.cfg
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.974586 batogram-1.0.9/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.0.9/LICENSE
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.0.9/MANIFEST.in
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:50:27.974586 batogram-1.0.9/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4611 2023-06-04 17:11:53.000000 batogram-1.0.9/README.md
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.920585 batogram-1.0.9/batogram/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-06-04 17:50:01.000000 batogram-1.0.9/batogram/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/__main__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/about.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4673 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/amplitudegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6212 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/appsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/appsettingsmodal.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.931585 batogram-1.0.9/batogram/assets/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/3669170_home_ic_icon.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-left-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-left-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-right-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/arrow-right-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/batogram.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/download-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/drag-move-2-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/expand-left-right-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/expand-up-down-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/fullscreen-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/home-4-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/assets/zoom-in-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7549 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/audiofileservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/breadcrumbservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/buttonframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/chunky_spectrogram.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.954586 batogram-1.0.9/batogram/colour_maps/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L01.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L03.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L05.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L06.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L07.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L08.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L09.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L16.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L17.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L18.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L19.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/CET-L20.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/black-body-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/inferno-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colour_maps/kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/colourmap.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1658 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/common.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1817 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/constants.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.964586 batogram-1.0.9/batogram/external/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/external/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/external/guano.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/external/tooltip.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/fileinfoframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2968 2023-05-17 18:30:45.000000 batogram-1.0.9/batogram/frames.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5588 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/graphsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/historianservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    31653 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/layouts.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    31047 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/markers.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1134 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/modalwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    28313 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/morebncframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    12440 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/moreframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/morerenderingframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6851 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/morescaleframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4635 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/profilegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/readoutframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    59357 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/rendering.py
+-rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35201 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/rootwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/runner.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.973586 batogram-1.0.9/batogram/samples/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.9/batogram/samples/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    21200 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/spectrogramgraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    16042 2023-06-04 16:54:05.000000 batogram-1.0.9/batogram/spectrogrammouseservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    17007 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/validatingwidgets.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    13442 2023-06-04 17:45:35.000000 batogram-1.0.9/batogram/wavfileparser.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:50:27.924585 batogram-1.0.9/batogram.egg-info/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2282 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/SOURCES.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/dependency_links.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/entry_points.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/requires.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-06-04 17:50:27.000000 batogram-1.0.9/batogram.egg-info/top_level.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-06-04 17:49:38.000000 batogram-1.0.9/pyproject.toml
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-06-04 17:50:27.974586 batogram-1.0.9/setup.cfg
```

### Comparing `batogram-1.0.8/LICENSE` & `batogram-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/PKG-INFO` & `batogram-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.8
+Version: 1.0.9
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `batogram-1.0.8/README.md` & `batogram-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/__main__.py` & `batogram-1.0.9/batogram/__main__.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/about.py` & `batogram-1.0.9/batogram/about.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/amplitudegraphframe.py` & `batogram-1.0.9/batogram/amplitudegraphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
+from typing import Tuple
 
 from .constants import MAIN_AMPLITUDE_COMPLETER_EVENT, AXIS_FONT_HEIGHT
 from . import layouts
 from .audiofileservice import AudioFileService, RawDataReader
 from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
 from .rendering import AmplitudePipelineRequest
@@ -80,15 +81,15 @@
                                   self._pipeline_error_handler)
         else:
             # No data, so we can complete drawing the graph right away:
             graph_completer()
 
     @staticmethod
     def _get_pipeline_request(data, data_area, time_range: AxisRange, frequency_range: AxisRange,
-                              amplitude_range: AxisRange, screen_factors: tuple[float, float], rdr: RawDataReader):
+                              amplitude_range: AxisRange, screen_factors: Tuple[float, float], rdr: RawDataReader):
 
         request = AmplitudePipelineRequest(data_area, data, time_range, frequency_range,
                                            amplitude_range, screen_factors, rdr)
         return request
 
     def _do_completer(self, _):
         # A bit of a hack because tkinter doesn't seem to allow data to be attached to an event:
```

### Comparing `batogram-1.0.8/batogram/appsettings.py` & `batogram-1.0.9/batogram/appsettings.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/appsettingsmodal.py` & `batogram-1.0.9/batogram/appsettingsmodal.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/assets/batogram.png` & `batogram-1.0.9/batogram/assets/batogram.png`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/audiofileservice.py` & `batogram-1.0.9/batogram/audiofileservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 import time
-from typing import Optional
+from typing import Optional, Tuple
 
 import numpy as np
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from numpy import ndarray
 from .common import AxisRange
@@ -35,15 +35,15 @@
 class RawDataReader(ABC):
     """An abstraction for reading raw data."""
 
     def __init__(self):
         pass
 
     @abstractmethod
-    def read_raw_data(self, index_range: tuple[int, int]) -> ndarray:
+    def read_raw_data(self, index_range: Tuple[int, int]) -> ndarray:
         """Read raw file data for the half open range provided."""
         raise NotImplementedError()
 
 
 class AudioFileService(RawDataReader):
     """A service that allows the application to read raw data from a data file."""
 
@@ -172,15 +172,15 @@
             channels=self._channels,
             bytes_per_value=self._bytes_per_value
         )
 
     def get_guano_data(self):
         return self._guano_data
 
-    def read_raw_data(self, index_range: tuple[int, int]) -> tuple[ndarray, int]:
+    def read_raw_data(self, index_range: Tuple[int, int]) -> Tuple[ndarray, int]:
         """
         Read raw file data for the half open range provided.
         Truncate the data to the actual range available from the file.
         """
 
         # Sanitize the range requested:
         start, end = index_range
```

### Comparing `batogram-1.0.8/batogram/breadcrumbservice.py` & `batogram-1.0.9/batogram/breadcrumbservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/buttonframe.py` & `batogram-1.0.9/batogram/buttonframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/chunky_spectrogram.py` & `batogram-1.0.9/batogram/chunky_spectrogram.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L01.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L01.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L03.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L03.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L05.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L05.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L06.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L06.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L07.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L07.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L08.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L08.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L09.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L09.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L16.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L16.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L17.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L17.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L18.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L18.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L19.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L19.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/CET-L20.csv` & `batogram-1.0.9/batogram/colour_maps/CET-L20.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/black-body-table-byte-1024.csv` & `batogram-1.0.9/batogram/colour_maps/black-body-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv` & `batogram-1.0.9/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/inferno-table-byte-1024.csv` & `batogram-1.0.9/batogram/colour_maps/inferno-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colour_maps/kindlmann-table-byte-1024.csv` & `batogram-1.0.9/batogram/colour_maps/kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/colourmap.py` & `batogram-1.0.9/batogram/colourmap.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/common.py` & `batogram-1.0.9/batogram/common.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/constants.py` & `batogram-1.0.9/batogram/constants.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/external/guano.py` & `batogram-1.0.9/batogram/external/guano.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/external/tooltip.py` & `batogram-1.0.9/batogram/external/tooltip.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/fileinfoframe.py` & `batogram-1.0.9/batogram/fileinfoframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/frames.py` & `batogram-1.0.9/batogram/frames.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/graphsettings.py` & `batogram-1.0.9/batogram/graphsettings.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/historianservice.py` & `batogram-1.0.9/batogram/historianservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/layouts.py` & `batogram-1.0.9/batogram/layouts.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/markers.py` & `batogram-1.0.9/batogram/markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             upper_clipped = True
         if upper <= lower:
             upper = lower + 1
 
         return (lower, band_pixel_width[1], upper, band_pixel_width[0]), (lower_clipped, upper_clipped)
 
     def draw_text_impl(self, canvas: "SpectrogramCanvas", band_rect: AreaTuple,
-                       text: list[str], is_clipped: Tuple[bool, bool]) -> List[int]:
+                       text: List[str], is_clipped: Tuple[bool, bool]) -> List[int]:
         l, t, r, b = band_rect
         text_id = None
         if len(text) > 0 and not is_clipped[0] and not is_clipped[1]:
             text_id = None
             min_space_for_text = 60
             if r - l > min_space_for_text:
                 # Annotation. +2 to get the text inside the band. Me neither.
```

### Comparing `batogram-1.0.8/batogram/modalwindow.py` & `batogram-1.0.9/batogram/modalwindow.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/morebncframe.py` & `batogram-1.0.9/batogram/morebncframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
 class ScaleCanvas(tk.Canvas):
     """A canvas the displays the colour scale for a spectrogram."""
 
     def __init__(self, parent):
         super().__init__(parent, bg="black", height=15, width=CANVAS_WIDTH)
 
-    def set_scale_pixels(self, prange: Optional[tuple[int, int]]):
+    def set_scale_pixels(self, prange: Optional[Tuple[int, int]]):
         """Draw a colour mapped scale."""
         width, height = self.winfo_width(), self.winfo_height()
 
         self.clear()
         if prange is not None:
             xmin, xmax = prange
             if xmin < xmax:
@@ -194,33 +194,33 @@
     def __init__(self, canvas: "HistogramCanvas", line: "BnCLine", which: int, tag_name: str):
         self._line = line
         self._canvas = canvas
         self._tag_name = tag_name
         self._which = which  # Which dragger are we? Maybe a subclass would be cleaner, but hey ho.
         self._rectangle: Optional[int] = None  # The rectangle drawn on the canvas, if any.
         # _pos is the position we were originally drawn at:
-        self._pos: Optional[tuple[int, int]] = None
+        self._pos: Optional[Tuple[int, int]] = None
         # _moved is the position have been moved to, updated during a drag:
-        self._moved: Optional[tuple[int, int]] = None
+        self._moved: Optional[Tuple[int, int]] = None
 
         self._start_event: Optional[Any] = None  # If this is non None, we know we are currently dragging.
         self._width: Optional[int] = None
         self._height: Optional[int] = None
-        self._allowed_x_range: Optional[tuple[int, int]] = None
+        self._allowed_x_range: Optional[Tuple[int, int]] = None
 
         canvas.tag_bind(self._tag_name, "<Enter>", lambda event: self.mouse_enters_dragger(event))
         canvas.tag_bind(self._tag_name, "<Leave>", lambda event: self.mouse_leaves_dragger(event))
         canvas.tag_bind(self._tag_name, "<Button-1>", lambda event: self._on_click(event))
         canvas.tag_bind(self._tag_name, "<B1-Motion>", lambda event: self._on_move(event))
         canvas.tag_bind(self._tag_name, "<ButtonRelease-1>", lambda event: self._on_release(event))
 
-    def get_pos(self) -> tuple[int, int]:
+    def get_pos(self) -> Tuple[int, int]:
         return self._pos
 
-    def show(self, pos: tuple[int, int]):
+    def show(self, pos: Tuple[int, int]):
         self._width, self._height = self._canvas.winfo_width(), self._canvas.winfo_height()
         # Get rid of any dragger we have previously drawn:
         self._canvas.delete(self._tag_name)
         self._pos = pos
         self._rectangle = self._canvas.create_rectangle(*self._to_rect(*pos, self.HALF_SIZE),
                                                         fill=self._COLOUR, activefill=self._ACTIVE_COLOUR,
                                                         tags=[self._tag_name])
@@ -319,20 +319,20 @@
 
         # The line always has a dragger at each end. We will show and hide them as required by the mode:
         self._min_dragger: Dragger = Dragger(self._histogram_canvas, self, self.MIN_DRAGGER, "min")
         self._max_dragger: Dragger = Dragger(self._histogram_canvas, self, self.MAX_DRAGGER, "max")
         self._draggers: List[Dragger] = [self._min_dragger, self._max_dragger]
 
         self._line: Optional[int] = None       # The line object in the canvas.
-        self._prange: Optional[tuple[int, int]] = None     # The x pixel range spanned by the line.
+        self._prange: Optional[Tuple[int, int]] = None     # The x pixel range spanned by the line.
 
         self._width: Optional[int] = None      # Cache the canvas size for convenience.
         self._height: Optional[int] = None
 
-    def show(self, prange: tuple[int, int], with_draggers: bool):
+    def show(self, prange: Tuple[int, int], with_draggers: bool):
         """
         Draw or remove the BnC line, with or without draggers according to mode.
         """
 
         # Cache the canvas size for convenience:
         self._width, self._height = self._histogram_canvas.winfo_width(), self._histogram_canvas.winfo_height()
         self._draw_all(*prange, with_draggers)
@@ -344,15 +344,15 @@
         # Draw draggers if required:
         if with_draggers:
             # This has the effect of redraing them if there are already drawn:
             self._show_draggers()
         else:
             self._hide_draggers()
 
-    def _draw_line(self, prange: tuple[int, int]):
+    def _draw_line(self, prange: Tuple[int, int]):
         pmin, pmax = prange
         # Delete any existing line:
         if self._line is not None:
             self._histogram_canvas.delete(self._line)
         coords = [pmin, 0, pmin, self._height - 1, pmax - 1, 0, pmax - 1, self._height - 1]
         self._line = self._histogram_canvas.create_line(*coords, fill=self._BNC_LINE_COLOUR, dash=(3, 5),
                                                         tags=self._LINE_TAG)
@@ -409,15 +409,15 @@
         # Redraw everything so that we end up with the correct depth order, so that the mouse
         # cursor changes correctly:
         self._draw_all(*self._prange, True)
 
         # Tell the canvas about the change:
         self._histogram_canvas.on_bnc_interactive_change((min_x, max_x))
 
-    def get_allowed_range(self, which_asking: int) -> tuple[int, int]:
+    def get_allowed_range(self, which_asking: int) -> Tuple[int, int]:
         """A dragger calls this method to get the range of x values which we will
         allow it to have."""
         min_spacing = 5
         prange = 1, self._width - 1
         if which_asking == BnCLine.MIN_DRAGGER:
             # This dragger must be to the left of the max dragger:
             x_pos, _ = self._max_dragger.get_pos()
@@ -479,15 +479,15 @@
         self.bind('<Button-4>', self._on_wheel_up)
         self.bind('<Button-5>', self._on_wheel_down)
         # For Windows:
         self.bind("<MouseWheel>", self._on_wheel)
 
         self._reset_histogram()
 
-    def on_bnc_interactive_change(self, prange: tuple[int, int]):
+    def on_bnc_interactive_change(self, prange: Tuple[int, int]):
         # Scale the pixels to values:
         vrange: Optional[Tuple[float, float]] = self._pixels_to_values(prange)
         if vrange is not None:
             self._parent.on_bnc_interactive_change(vrange)
 
     def show_histogram(self, data: np.ndarray):
         """Called from the rendering pipeline to display the histogram,
@@ -544,15 +544,15 @@
         self._bin_edges = None
         self._auto_vrange = None
 
     def on_bnc_settings_changed(self):
         # Convert the value range provided to a pixel range. Pixels
         # correspond to bin edges:
         vrange = self._settings.bnc_manual_min, self._settings.bnc_manual_max
-        prange: Optional[tuple[int, int]] = self._values_to_pixels(vrange)
+        prange: Optional[Tuple[int, int]] = self._values_to_pixels(vrange)
         interactive_mode: bool = self._settings.bnc_adjust_type == BNC_INTERACTIVE_MODE
         self._is_interactive_mode = interactive_mode
         if prange is not None:
             self._bnc_line.show(prange, interactive_mode)
 
     def hide_bnc_line(self):
         self._is_interactive_mode = False
@@ -573,15 +573,15 @@
     def _on_wheel(self, event):
         if self._is_interactive_mode:
             if event.delta > 0:
                 self._bnc_line.on_wheel_move(self._WHEEL_DELTA)
             else:
                 self._bnc_line.on_wheel_move(-self._WHEEL_DELTA)
 
-    def _values_to_pixels(self, vrange: tuple[float, float]) -> Optional[Tuple[int, int]]:
+    def _values_to_pixels(self, vrange: Tuple[float, float]) -> Optional[Tuple[int, int]]:
         prange: Optional[Tuple[int, int]] = None
         if self._bin_edges is not None:
             vmin, vmax = vrange
             # Scale vmin and vmax to bin numbers (which correspond to the x coordinate).
             # We choose the bin whose centre is closest to the value - that means,
             # add half a bin width and then floor.
             bin_count = len(self._bin_edges) - 1  # n bins have n+1 boundaries.
@@ -630,15 +630,15 @@
         self._scale_canvas = ScaleCanvas(self)
         self._histogram_canvas = HistogramCanvas(self, parent, self._scale_canvas, settings)
         self._histogram_canvas.grid(row=0, column=0, sticky="NSEW", padx=pad, pady=(pad, 0))
         self._scale_canvas.grid(row=1, column=0, sticky="NSEW", padx=pad, pady=(0, pad))
         self.rowconfigure(0, weight=1)
         self.rowconfigure(1, weight=0)
 
-    def on_bnc_interactive_change(self, vrange: tuple[float, float]):
+    def on_bnc_interactive_change(self, vrange: Tuple[float, float]):
         """Respond to a manual change to BnC from the histogram: dragging or mouse wheel."""
         self._settings.bnc_manual_min, self._settings.bnc_manual_max = vrange
         # Tell whomever it may concern that new settings values are available,
         # limiting it to a spectrogram redraw only to limit general flicker:
         self._settings.on_user_applied_settings(draw_scope=DrawableFrame.DRAW_SPECTROGRAM)
 
     def show_histogram(self, data: np.ndarray):
```

### Comparing `batogram-1.0.8/batogram/moreframe.py` & `batogram-1.0.9/batogram/moreframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/morerenderingframe.py` & `batogram-1.0.9/batogram/morerenderingframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/morescaleframe.py` & `batogram-1.0.9/batogram/morescaleframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/profilegraphframe.py` & `batogram-1.0.9/batogram/profilegraphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
+from typing import Tuple
 
 from .constants import MAIN_PROFILE_COMPLETER_EVENT, AXIS_FONT_HEIGHT
 from . import layouts
 from .audiofileservice import RawDataReader
 from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
 from .rendering import ProfilePipelineRequest
@@ -78,15 +79,15 @@
                                   lambda: self.event_generate(MAIN_PROFILE_COMPLETER_EVENT),
                                   self._pipeline_error_handler)
         else:
             # No data, so we can complete drawing the graph right away:
             graph_completer()
 
     @staticmethod
-    def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range, screen_factors: tuple[float, float], rdr: RawDataReader):
+    def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range, screen_factors: Tuple[float, float], rdr: RawDataReader):
         request = ProfilePipelineRequest(is_reference, data_area, data, time_range, frequency_range, screen_factors, rdr)
         return request
 
     def _do_completer(self, _):
         # A bit of a hack because tkinter doesn't seem to allow data to be attached to an event:
         completer = self._completer
         if completer:
```

### Comparing `batogram-1.0.8/batogram/readoutframe.py` & `batogram-1.0.9/batogram/readoutframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/rendering.py` & `batogram-1.0.9/batogram/rendering.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         # Subclasses whose calculation depends on any settings MUST implement this
         # so that caching properly.
         return None
 
 
 class SpectrogramPipelineRequest(RenderingRequest):
     def __init__(self, is_reference: bool, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
-                 frequency_range: AxisRange, screen_factors: tuple[float, float],
+                 frequency_range: AxisRange, screen_factors: Tuple[float, float],
                  raw_data_reader: RawDataReader):
         super().__init__(data_area, file_data)
         self.axis_time_range: AxisRange = time_range
         self.axis_frequency_range: AxisRange = frequency_range
         self.raw_data_reader = raw_data_reader
         self.screen_factors = screen_factors
         self.is_reference = is_reference
@@ -293,15 +293,15 @@
     actual_freq_axis_max: float
     actual_fft_samples: int
     actual_fft_overlap_percent: float
     actual_fft_overlap_samples: int
     step_count: int
 
     def __init__(self, settings: GraphSettings, axis_time_range: AxisRange, axis_frequency_range: AxisRange,
-                 file_data: AudioFileService.RenderingData, screen_factors: tuple[float, float],
+                 file_data: AudioFileService.RenderingData, screen_factors: Tuple[float, float],
                  canvas_width: int, canvas_height: int):
         """
             Do all the scale and offset calculations we will need to render a spectrogram.
 
             Note: we choose t=0 axis time to be the middle of the first sfft segment. This
             avoids the complication of the first segment offset being more than subsequent ones
             if we chose t=0 to be the left of the first segment. This results in possible negative
@@ -449,15 +449,15 @@
 
         pixels_per_hz: float = canvas_height / (freq_axis_max - freq_axis_min)
         self.freq_dilated_pixels: int = int(
             pixels_per_hz * (self.actual_freq_axis_max - self.actual_freq_axis_min) + 0.5)
         self.freq_offset_pixels: int = int((freq_axis_min - self.actual_freq_axis_min) * pixels_per_hz + 0.5)
 
     @staticmethod
-    def _calculate_auto_fft_samples(sample_rate: int, screen_factors: tuple[float, float]) -> int:
+    def _calculate_auto_fft_samples(sample_rate: int, screen_factors: Tuple[float, float]) -> int:
         """Select a number of FFT samples that roughly results in square image elements on the screen."""
 
         # Overlapping of windows increases the resultant sample rate:
         # overlap_ratio = 100.0 / (100.0 - fft_overlap_percent)
 
         # It seems to work best if we ignore overlapping - which doesn't actually increase
         # time resolution, just smooths over time:
@@ -549,15 +549,15 @@
         self._spectrogram_step = spectrogram_step
         self._data_reader_step = data_reader_step
         self._zoom_step = SpectrogramZoomStep(settings)
         self._bnc_step = SpectrogramBNCStep(settings)
         self._apply_colour_map_step = SpectrogramApplyColourMapStep(settings)
 
         # Remember info about the last histogram data, so we know if there is any change to it:
-        self._last_histogram_data_details: tuple[int, int] | None = None
+        self._last_histogram_data_details: Tuple[int, int] | None = None
 
     def get_completion_data(self):
         return self._completion_data
 
     def get_graph_parameters(self) -> Optional[GraphParams]:
         return self._graph_params
 
@@ -980,15 +980,15 @@
         outputdata = colourmap.instance.map(inputdata)
         return outputdata
 
 
 class AmplitudePipelineRequest(RenderingRequest):
     def __init__(self, data_area, file_data: AudioFileService.RenderingData, time_range: AxisRange,
                  frequency_range: AxisRange,
-                 amplitude_range: AxisRange, screen_factors: tuple[float, float], rdr: RawDataReader):
+                 amplitude_range: AxisRange, screen_factors: Tuple[float, float], rdr: RawDataReader):
         super().__init__(data_area, file_data)
         self.time_range: AxisRange = time_range
         self.amplitude_range: AxisRange = amplitude_range
         self.frequency_range = frequency_range
         self.raw_data_reader = rdr
         self.screen_factors = screen_factors
```

### Comparing `batogram-1.0.8/batogram/rootwindow.py` & `batogram-1.0.9/batogram/rootwindow.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import sys
 import tkinter as tk
 import tkinter.filedialog
 import tkinter.messagebox
 
 from itertools import chain
 from timeit import default_timer as timer
-from typing import NamedTuple, Optional
+from typing import NamedTuple, Optional, Tuple
 from . import audiofileservice as af, appsettings, colourmap
 from .amplitudegraphframe import AmplitudeGraphFrame
 from .appsettings import COLOUR_MAPS
 from .appsettingsmodal import AppSettingsWindow
 from .audiofileservice import AudioFileService
 from .breadcrumbservice import BreadcrumbService, Breadcrumb
 from .buttonframe import ButtonFrame
@@ -342,15 +342,15 @@
         existing_centre = (t1 + t2) / 2
         new_half_span = (new_t2 - new_t1) / 2
         # Scale the half span by ratio of canvas widths so the on-screen scaling is the same:
         new_half_span *= this_canvas_width / other_canvas_width
         centred_time_range = AxisRange(existing_centre - new_half_span, existing_centre + new_half_span)
         self.on_rescale_handler(centred_time_range, frequency_range, add_breadcrumb=True)
 
-    def get_screen_factors(self) -> tuple[float, float]:
+    def get_screen_factors(self) -> Tuple[float, float]:
         # Calculate the screen aspect factor based on the spectrogram graph,
         # that will be used in adaptive window length calculations.
         return self._spectrogram_frame.calculate_screen_factors()
 
     def on_left_key(self, event):
         self._spectrogram_frame.tview(tk.SCROLL, -1, tk.UNITS)
```

### Comparing `batogram-1.0.8/batogram/spectrogramgraphframe.py` & `batogram-1.0.9/batogram/spectrogramgraphframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         else:
             self._canvas.config(cursor="")
 
         self._canvas.set_cursor_mode(mode)
 
     @staticmethod
     def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range,
-                              screen_factors: tuple[float, float],
+                              screen_factors: Tuple[float, float],
                               raw_data_reader: RawDataReader):
         request = SpectrogramPipelineRequest(is_reference, data_area, data, time_range, frequency_range, screen_factors,
                                              raw_data_reader)
         return request
 
     def _do_completer(self, _):
         # A bit of a hack because tkinter doesn't seem to allow data to be attached to an event:
@@ -473,15 +473,15 @@
 
         # print("set {} {}".format(start, end))
         self._scroller_f.set(start, end)
 
     def get_canvas_size(self):
         return self._canvas.winfo_width(), self._canvas.winfo_height()
 
-    def calculate_screen_factors(self) -> tuple[float, float]:
+    def calculate_screen_factors(self) -> Tuple[float, float]:
         """
         Calculate:
          * the screen aspect factor in s/Hz that will be used for adaptive window
             length calculations,
          * The number of x pixels per second that will be used for adaptive
             overlap calculations.
         """
```

### Comparing `batogram-1.0.8/batogram/spectrogrammouseservice.py` & `batogram-1.0.9/batogram/spectrogrammouseservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/batogram/validatingwidgets.py` & `batogram-1.0.9/batogram/validatingwidgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from abc import ABC, abstractmethod
-from typing import Any, Tuple, List, Callable
+from typing import Any, Tuple, List, Callable, Dict
 
 import numpy as np
 import tkinter as tk
 import re
 
 
 class AbstractValidatingWidgetMixin(ABC):
@@ -332,17 +332,17 @@
 
     def value_to_native(self, value):
         return str(value)
 
 
 class ValidatingMapOptionMenu(ValidatingOptionMenu):
     def __init__(self, parent: tk.Widget, controlling_frame: tk.Widget, container: tk.Widget,
-                 dictionary: dict[Any, str], value_validator=None):
+                 dictionary: Dict[Any, str], value_validator=None):
         self._dictionary = dictionary
-        keys: list[Any] = [k for k in dictionary.keys()]
+        keys: List[Any] = [k for k in dictionary.keys()]
         keys.sort()
         values = [dictionary[k] for k in keys]
         super().__init__(parent, controlling_frame, container, tuple(values), value_validator)
 
     def native_to_value(self, native):
         # Only good for short lists:
         for k, v in self._dictionary.items():
```

### Comparing `batogram-1.0.8/batogram/wavfileparser.py` & `batogram-1.0.9/batogram/wavfileparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         # to seek to the end of data chunk now to not confused the caller:
         self._f.seek(self._start_of_data + data_byte_count)
 
         return WavFileParser.Data(actual_sample_count=actual_sample_count,
                                   data_range=(min_value, max_value),
                                   data_byte_count=data_byte_count)
 
-    def read_data(self, index_range: tuple[int, int]) -> tuple[Optional[np.ndarray], int]:
+    def read_data(self, index_range: Tuple[int, int]) -> Tuple[Optional[np.ndarray], int]:
         """Read the request range of data (half open), and return the data and actual count read."""
 
         dt = None
         if self._fmt_header.bits_per_sample == 8:
             dt = np.dtype(np.uint8)
         elif self._fmt_header.bits_per_sample == 16:
             dt = np.dtype(np.int16)
```

### Comparing `batogram-1.0.8/batogram.egg-info/PKG-INFO` & `batogram-1.0.9/batogram.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.8
+Version: 1.0.9
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `batogram-1.0.8/batogram.egg-info/SOURCES.txt` & `batogram-1.0.9/batogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `batogram-1.0.8/pyproject.toml` & `batogram-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "batogram"
-version = "1.0.8"   # Set this to the version number during release, and revert to 0.0.0 between releases.
+version = "1.0.9"   # Set this to the version number during release, and revert to 0.0.0 between releases.
 authors = [
     {name = "John Mears", email = "john+batogram@themears.co.uk"},
 ]
 description = "Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["bat", "spectrogram", "chiropterology", "fourier", "ultrasonic", "ultrasound", "echo", "GUANO"]
```

