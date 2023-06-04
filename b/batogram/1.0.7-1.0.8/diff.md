# Comparing `tmp/batogram-1.0.7.tar.gz` & `tmp/batogram-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batogram-1.0.7.tar", last modified: Mon May  8 12:53:54 2023, max compression
+gzip compressed data, was "batogram-1.0.8.tar", last modified: Sun Jun  4 17:12:13 2023, max compression
```

## Comparing `batogram-1.0.7.tar` & `batogram-1.0.8.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.808996 batogram-1.0.7/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.0.7/LICENSE
--rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.0.7/MANIFEST.in
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6425 2023-05-08 12:53:54.808996 batogram-1.0.7/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4478 2023-05-08 11:32:46.000000 batogram-1.0.7/README.md
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.802996 batogram-1.0.7/batogram/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-05-08 12:45:47.000000 batogram-1.0.7/batogram/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/__main__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/about.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4634 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/amplitudegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6212 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/appsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/appsettingsmodal.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.804996 batogram-1.0.7/batogram/assets/
--rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/3669170_home_ic_icon.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-left-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-left-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-right-circle-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/arrow-right-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/batogram.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/download-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/drag-move-2-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/expand-left-right-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/expand-up-down-fill.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/fullscreen-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/home-4-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/assets/zoom-in-line.png
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7542 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/audiofileservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/breadcrumbservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/buttonframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/chunky_spectrogram.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.807996 batogram-1.0.7/batogram/colour_maps/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L01.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L03.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L05.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L06.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L07.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L08.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L09.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L16.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L17.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L18.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L19.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/CET-L20.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/black-body-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/inferno-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colour_maps/kindlmann-table-byte-1024.csv
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/colourmap.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1605 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/common.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1762 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/constants.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.807996 batogram-1.0.7/batogram/external/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/external/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/external/guano.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/external/tooltip.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/fileinfoframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2638 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/frames.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5241 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/graphsettings.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/historianservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    30878 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/layouts.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1134 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/modalwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    28313 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/morebncframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    12442 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/moreframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/morerenderingframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6055 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/morescaleframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     4596 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/profilegraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/readoutframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    59357 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/rendering.py
--rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35194 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/rootwindow.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/runner.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.807996 batogram-1.0.7/batogram/samples/
--rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/samples/__init__.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    18969 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/spectrogramgraphframe.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    15546 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/spectrogrammouseservice.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/validatingwidgets.py
--rw-r--r--   0 jmears    (1000) jmears    (1000)    13442 2023-05-08 11:30:20.000000 batogram-1.0.7/batogram/wavfileparser.py
-drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-05-08 12:53:54.802996 batogram-1.0.7/batogram.egg-info/
--rw-r--r--   0 jmears    (1000) jmears    (1000)     6425 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/PKG-INFO
--rw-r--r--   0 jmears    (1000) jmears    (1000)     2262 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/SOURCES.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/dependency_links.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/entry_points.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/requires.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-05-08 12:53:54.000000 batogram-1.0.7/batogram.egg-info/top_level.txt
--rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-05-08 12:46:12.000000 batogram-1.0.7/pyproject.toml
--rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-05-08 12:53:54.808996 batogram-1.0.7/setup.cfg
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.864102 batogram-1.0.8/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1053 2023-05-08 11:30:20.000000 batogram-1.0.8/LICENSE
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      118 2023-05-08 11:30:20.000000 batogram-1.0.8/MANIFEST.in
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:12:13.864102 batogram-1.0.8/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4611 2023-06-04 17:11:53.000000 batogram-1.0.8/README.md
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.804101 batogram-1.0.8/batogram/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      310 2023-06-04 17:06:48.000000 batogram-1.0.8/batogram/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      535 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/__main__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2189 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/about.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4648 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/amplitudegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6212 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/appsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    10133 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/appsettingsmodal.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.816102 batogram-1.0.8/batogram/assets/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      232 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/3669170_home_ic_icon.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      407 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-left-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      230 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-left-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      425 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-right-circle-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      224 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/arrow-right-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1373 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/batogram.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      263 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/download-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      362 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/drag-move-2-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      222 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/expand-left-right-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      214 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/expand-up-down-fill.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      171 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/fullscreen-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      337 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/home-4-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      452 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/assets/zoom-in-line.png
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7542 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/audiofileservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3159 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/breadcrumbservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     7261 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/buttonframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5245 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/chunky_spectrogram.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.845102 batogram-1.0.8/batogram/colour_maps/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2727 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L01.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2280 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L03.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2343 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L05.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2618 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L06.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2679 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L07.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2726 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L08.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2663 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L09.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2612 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L16.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2933 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L17.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2857 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L18.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2961 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L19.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2705 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/CET-L20.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30096 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/black-body-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29916 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    30107 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/inferno-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    29566 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colour_maps/kindlmann-table-byte-1024.csv
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3627 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/colourmap.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1658 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/common.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1817 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/constants.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.854102 batogram-1.0.8/batogram/external/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/external/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    19291 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/external/guano.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4666 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/external/tooltip.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2063 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/fileinfoframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2968 2023-05-17 18:30:45.000000 batogram-1.0.8/batogram/frames.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5588 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/graphsettings.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2096 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/historianservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    31653 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/layouts.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    31047 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/markers.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1134 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/modalwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    28313 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/morebncframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    12440 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/moreframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     5140 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/morerenderingframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6851 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/morescaleframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     4610 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/profilegraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     3518 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/readoutframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    59357 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/rendering.py
+-rwxr-xr-x   0 jmears    (1000) jmears    (1000)    35194 2023-06-04 16:22:36.000000 batogram-1.0.8/batogram/rootwindow.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)      493 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/runner.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.863103 batogram-1.0.8/batogram/samples/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        0 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/samples/__init__.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    21200 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/spectrogramgraphframe.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    16042 2023-06-04 16:54:05.000000 batogram-1.0.8/batogram/spectrogrammouseservice.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    17001 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/validatingwidgets.py
+-rw-r--r--   0 jmears    (1000) jmears    (1000)    13442 2023-05-08 11:30:20.000000 batogram-1.0.8/batogram/wavfileparser.py
+drwxr-xr-x   0 jmears    (1000) jmears    (1000)        0 2023-06-04 17:12:13.808102 batogram-1.0.8/batogram.egg-info/
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     6558 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/PKG-INFO
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     2282 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/SOURCES.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        1 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/dependency_links.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       49 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/entry_points.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       58 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/requires.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)        9 2023-06-04 17:12:13.000000 batogram-1.0.8/batogram.egg-info/top_level.txt
+-rw-r--r--   0 jmears    (1000) jmears    (1000)     1518 2023-06-04 17:07:09.000000 batogram-1.0.8/pyproject.toml
+-rw-r--r--   0 jmears    (1000) jmears    (1000)       38 2023-06-04 17:12:13.865102 batogram-1.0.8/setup.cfg
```

### Comparing `batogram-1.0.7/LICENSE` & `batogram-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/PKG-INFO` & `batogram-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.7
+Version: 1.0.8
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -42,15 +42,17 @@
 Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
+* Graphical markers allow time and frequency ranges to be conveniently read.
 * Handling of multichannel data files, including stereo.
+* Ability to correct for microphone frequency response.
 * Basic side by side comparison of two spectrograms.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
 * Runs on Windows, Linux and macOS (experimental) operating systems.
 
 Installation
 ------------
```

### Comparing `batogram-1.0.7/README.md` & `batogram-1.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
+* Graphical markers allow time and frequency ranges to be conveniently read.
 * Handling of multichannel data files, including stereo.
+* Ability to correct for microphone frequency response.
 * Basic side by side comparison of two spectrograms.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
 * Runs on Windows, Linux and macOS (experimental) operating systems.
 
 Installation
 ------------
```

### Comparing `batogram-1.0.7/batogram/__main__.py` & `batogram-1.0.8/batogram/__main__.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/about.py` & `batogram-1.0.8/batogram/about.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/amplitudegraphframe.py` & `batogram-1.0.8/batogram/amplitudegraphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 
-from .constants import MAIN_AMPLITUDE_COMPLETER_EVENT, FONT_SIZE
+from .constants import MAIN_AMPLITUDE_COMPLETER_EVENT, AXIS_FONT_HEIGHT
 from . import layouts
 from .audiofileservice import AudioFileService, RawDataReader
 from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
 from .rendering import AmplitudePipelineRequest
 
 AMPLITUDE_HEIGHT = 60
@@ -57,15 +57,15 @@
         afs: AudioFileService = self._dc.get_afs()
 
         # Allow the canvas to catch up with any pending resizes so that get the right
         # size below:
         self.update_idletasks()
 
         width, height = self._canvas.winfo_width(), self._canvas.winfo_height()
-        layout = layouts.AmplitudeLayout(FONT_SIZE, width, height, is_reference=self._is_reference)
+        layout = layouts.AmplitudeLayout(AXIS_FONT_HEIGHT, width, height, is_reference=self._is_reference)
         # Draw the graph axes here in the UI thread, as that is fast and provides responsiveness to the user:
         graph_completer, data_area = layout.draw(self._canvas, time_range, amplitude_range, self._settings.show_grid)
 
         if afs and self._pipeline:
             # Kick off the pipeline which will create a spectrogram in another thread,
             # and complete by generating an event that will finish drawing the graph in
             # this thread.
```

### Comparing `batogram-1.0.7/batogram/appsettings.py` & `batogram-1.0.8/batogram/appsettings.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/appsettingsmodal.py` & `batogram-1.0.8/batogram/appsettingsmodal.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/assets/batogram.png` & `batogram-1.0.8/batogram/assets/batogram.png`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/audiofileservice.py` & `batogram-1.0.8/batogram/audiofileservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/breadcrumbservice.py` & `batogram-1.0.8/batogram/breadcrumbservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/buttonframe.py` & `batogram-1.0.8/batogram/buttonframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/chunky_spectrogram.py` & `batogram-1.0.8/batogram/chunky_spectrogram.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L01.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L01.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L03.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L03.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L05.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L05.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L06.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L06.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L07.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L07.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L08.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L08.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L09.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L09.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L16.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L16.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L17.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L17.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L18.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L18.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L19.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L19.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/CET-L20.csv` & `batogram-1.0.8/batogram/colour_maps/CET-L20.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/black-body-table-byte-1024.csv` & `batogram-1.0.8/batogram/colour_maps/black-body-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv` & `batogram-1.0.8/batogram/colour_maps/extended-kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/inferno-table-byte-1024.csv` & `batogram-1.0.8/batogram/colour_maps/inferno-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colour_maps/kindlmann-table-byte-1024.csv` & `batogram-1.0.8/batogram/colour_maps/kindlmann-table-byte-1024.csv`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/colourmap.py` & `batogram-1.0.8/batogram/colourmap.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/common.py` & `batogram-1.0.8/batogram/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from dataclasses import dataclass
 from typing import Tuple, TypeVar
 
 AreaTuple = Tuple[int, int, int, int]
+RangeTuple = Tuple[int, int]
+
+FontName = "helvetica"
 
 
 @dataclass
 class AxisRange:
     min: float
     max: float
```

### Comparing `batogram-1.0.7/batogram/constants.py` & `batogram-1.0.8/batogram/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 PROGRAM_NAME = "Batogram"
 DATA_CHANGE_MAIN_EVENT = "<<OnDataChangeMain>>"  # Underlying data has change: for example, a file opened or closed.
 DATA_CHANGE_REF_EVENT = "<<OnDataChangeRef>>"  # Underlying data has change: for example, a file opened or closed.
 MAIN_SPECTROGAM_COMPLETER_EVENT = "<<MainSpectrogramCompleter>>"
 MAIN_AMPLITUDE_COMPLETER_EVENT = "<<MainAmplitudeCompleter>>"
 MAIN_PROFILE_COMPLETER_EVENT = "<<MainProfileCompleter>>"
-FONT_SIZE = 12
 ZOOM_ORDER = 2  # This will move into settings. 0-2 is a useful range.
 COLOUR_MAPS_PATH = "colour_maps"
 ASSETS_PATH = "assets"
+AXIS_FONT_NAME = "helvetica"
+AXIS_FONT_HEIGHT = 12           # Pixels
 
 # Limit how far they can zoom in:
 MIN_F_RANGE: float = 500
 MIN_T_RANGE: float = 0.001
```

### Comparing `batogram-1.0.7/batogram/external/guano.py` & `batogram-1.0.8/batogram/external/guano.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/external/tooltip.py` & `batogram-1.0.8/batogram/external/tooltip.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/fileinfoframe.py` & `batogram-1.0.8/batogram/fileinfoframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/frames.py` & `batogram-1.0.8/batogram/frames.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,17 +50,24 @@
         super().__init__(parent)
         self._completer = None
         self._my_root = root
         self._pipeline = pipeline
         self._dc = data_context
         self._settings: "GraphSettings" = settings
         self._layout = None
+        self._after_id = None
 
     def _on_canvas_change(self, _):
-        self.draw()
+        # Don't directly draw here, it results in very laggy window resizing on Windows. Perhaps
+        # there is contention between tkinter and the rendering threads?
+
+        if self._after_id:
+            self.after_cancel(self._after_id)
+        lag_ms = 500
+        self._after_id = self.after(lag_ms, self.draw)
 
     @staticmethod
     def _pipeline_error_handler(e):
         tk.messagebox.showerror(PROGRAM_NAME, "Error encountered in processing pipeline: {}".format(e))
         raise e
 
     def reset_draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
```

### Comparing `batogram-1.0.7/batogram/graphsettings.py` & `batogram-1.0.8/batogram/graphsettings.py`

 * *Files 9% similar despite different names*

```diff
@@ -75,14 +75,16 @@
     colour_mapping_path: str
     colour_mapping_steps: int
     do_histogram_normalization: bool
     bnc_adjust_type: int
     bnc_background_threshold_percent: float
     bnc_manual_min: float  # bnc manual min and max are percentages of the data range.
     bnc_manual_max: float
+    show_time_markers: bool
+    show_frequency_markers: bool
 
     def __init__(self,
                  on_app_modified_settings: Callable[[int], NoReturn],
                  on_user_applied_settings: Callable[[int], NoReturn],
                  show_profile=True):
         self.time_range = AxisRange(0, 1)
         self.zero_based_time = True
@@ -95,20 +97,26 @@
         self.fft_overlap = DEFAULT_FFT_OVERLAP_PERCENT
         self.window_type = DEFAULT_WINDOW_TYPE
         self.zoom_interpolation = DEFAULT_INTERPOLATION
         self.do_histogram_normalization = False
         self.bnc_adjust_type = BNC_ADAPTIVE_MODE
         self.bnc_background_threshold_percent = 80.0
         self.bnc_manual_min, self.bnc_manual_max = 0.0, 1.0
+        self.show_time_markers = False
+        self.show_frequency_markers = False
 
     def on_app_modified_settings(self, draw_scope: int = DrawableFrame.DRAW_ALL) -> NoReturn:
         """Signal to the settings UI that the underlying settings values have changed."""
         self._on_app_modified_settings(draw_scope)
 
     def on_user_applied_settings(self, draw_scope: int = DrawableFrame.DRAW_ALL) -> NoReturn:
         """Signal to the application that the underlying settings values have changed."""
         self._on_user_applied_settings(draw_scope)
 
     def on_open_new_file(self):
         # Always start with auto BnC, so that the manual range
         # gets initialized to something sensible:
         self.bnc_adjust_type = BNC_ADAPTIVE_MODE
+        # Always start with markers disabled: any existing marker positions may be outside
+        # the range of view:
+        self.show_time_markers = False
+        self.show_frequency_markers = False
```

### Comparing `batogram-1.0.7/batogram/historianservice.py` & `batogram-1.0.8/batogram/historianservice.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/layouts.py` & `batogram-1.0.8/batogram/layouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import numpy as np
 
 from typing import Optional, Tuple, List
 from PIL import ImageTk, Image, ImageOps
 
 from . import colourmap
 from .common import AxisRange
+from .constants import AXIS_FONT_NAME
 
 AXIS_BG_COLOUR = "#404040"
 AXIS_FG_COLOUR = "white"
 GRID_COLOUR = "#404040"
 
 
 class Layout:
@@ -253,15 +254,15 @@
 
     def __init__(self, orientation: int, font_height: int, title: str, canvas_width: int,
                  canvas_height: int, units: List[AxisUnit], hide_text: bool = False):
         super().__init__(font_height, canvas_width, canvas_height)
         self._orientation = orientation
         self._title = title
         self._hide_text = hide_text
-        self._font_name = "helvetica"
+        self._font_name = AXIS_FONT_NAME
         self._layout()
         self._min_pixel = None
         self._max_pixel = None
         self._axis_range: Optional[AxisRange] = None
         self._units: List[AxisUnit] = sorted(units, key=lambda u: u.limit)  # Ascending.
         self._units_to_use: Optional[AxisUnit] = None
 
@@ -362,15 +363,15 @@
         """Decide what units to use based on the axis range."""
 
         if len(self._units) == 1:
             return self._units[0]
         else:
             abs_max: float = max(abs(axis_range.min), abs(axis_range.max))
             # The possible units are already sorted in ascending order.
-            u = self._units[0]      # Avoid a warning.
+            u = self._units[0]  # Avoid a warning.
             for u in self._units:
                 if abs_max < u.limit:
                     return u
             return u
 
     _preferred_ms_per_100pixels = [1.0, 2.0, 5.0, 10.0, 20.0, 50.0, 100.0, 200.0, 500.0, 1000.0, 2000.0, 5000.0]
 
@@ -389,17 +390,17 @@
         current_range = self._axis_range
         centre = (current_range.min + current_range.max) / 2
         span = current_range.max - current_range.min
         pixel_span = self._max_pixel - self._min_pixel
 
         # Calculate the current scaling, that we went to round up or down to preferred:
         ms_per_100pixels = span * 100.0 * 1000.0 / pixel_span
-        new_ms_per_100pixels = ms_per_100pixels     # Default - no change.
+        new_ms_per_100pixels = ms_per_100pixels  # Default - no change.
 
-        nudge_factor = 1.05     # Slight fudge in case the current range is a preferred range.
+        nudge_factor = 1.05  # Slight fudge in case the current range is a preferred range.
         if sign > 0:
             # We want to increase and round the range:
             nudged_ms_per_100pixels = ms_per_100pixels * nudge_factor
             for preferred in self._preferred_ms_per_100pixels:
                 if nudged_ms_per_100pixels < preferred:
                     new_ms_per_100pixels = preferred
                     break
@@ -428,16 +429,19 @@
     """This Layout knows how to lay out and raw a spectrogram."""
 
     _x_axis_unit = [AxisUnit(scaler=1.0, units="s"),  # Default
                     AxisUnit(limit=0.5, scaler=1E-3, units="ms")
                     ]
     _y_axis_unit = [AxisUnit(scaler=1000.0, units="kHz")]
 
-    def __init__(self, font_height, canvas_width, canvas_height):
+    def __init__(self, font_height, canvas_width, canvas_height,
+                 time_marker_pair: Optional["TimeMarkerPair"], frequency_marker_pair: Optional["FrequencyMarkerPair"]):
         super().__init__(font_height, canvas_width, canvas_height)
+        self._time_marker_pair: Optional["TimeMarkerPair"] = time_marker_pair
+        self._frequency_marker_pair: Optional["FrequencyMarkerPair"] = frequency_marker_pair
         self._x_axis = AxisLayout(AxisLayout.ORIENT_HORIZONTAL, font_height, "time", canvas_width,
                                   canvas_height, self._x_axis_unit)
         self._y_axis = AxisLayout(AxisLayout.ORIENT_VERTICAL, font_height, "frequency", canvas_width,
                                   canvas_height, self._y_axis_unit, hide_text=False)
         self._layout()
 
     def _layout(self):
@@ -459,15 +463,15 @@
         (2) The image and things overlaying it (such as the grid) are drawn later when the image
             has been calculated. A capture is returned that the caller can use later to do this.
         """
 
         # We draw things in a specific order so that some things appear on top of others.
 
         # First blank out the entire canvas to avoid leftovers being visible when resizing:
-        Layout._create_rectangle(canvas, 0, 0, self._canvas_width, self._canvas_height, 'black')
+        canvas.delete('all')
 
         # Fill the margins and the bit of dead space in the bottom left:
         (t, l, r, b) = self._dead_space
         Layout._create_rectangle(canvas, t, l, r, b, AXIS_BG_COLOUR)
 
         Layout._create_rectangle(canvas, *self._get_right_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._get_top_margin(), AXIS_BG_COLOUR)
@@ -496,14 +500,28 @@
             elif image is not None:
                 self._draw_graph_image(canvas, self._data_area, image)
 
             if show_grid:
                 self._draw_x_grid(canvas, x_ticks, self._data_area)
                 self._draw_y_grid(canvas, y_ticks, self._data_area)
 
+            if self._time_marker_pair is not None:
+                al, at, ar, ab = self._get_top_margin()
+                al += self._y_axis_width
+                ar -= self._margin
+                marker_rect = al, at, ar, ab
+                self._time_marker_pair.draw(marker_rect, self._data_area, self._margin, self._x_axis.get_axis_range())
+
+            if self._frequency_marker_pair is not None:
+                al, at, ar, ab = self._get_right_margin()
+                ab -= self._x_axis_height
+                at += self._margin
+                marker_rect = al, at, ar, ab
+                self._frequency_marker_pair.draw(marker_rect, self._data_area, self._margin, self._y_axis.get_axis_range())
+
         return draw_completer, self._data_area
 
     def canvas_to_data_area(self, p_canvas):
         """Finded the zoomed data value corresponding to the canvas point provided."""
 
         t_canvas, f_canvas = p_canvas
         if self._x_axis and self._y_axis:
@@ -550,15 +568,15 @@
 
         width = canvas.winfo_width()
         height = canvas.winfo_height()
 
         # We draw things in a specific order so that some things appear on top of others.
 
         # First blank out the entire canvas to avoid leftovers being visible when resizing:
-        Layout._create_rectangle(canvas, 0, 0, width, height, 'black')
+        canvas.delete('all')
 
         # Fill the margins:
         Layout._create_rectangle(canvas, *self._get_right_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._get_left_margin(self._y_axis_width), AXIS_BG_COLOUR)
 
         xaxis_x, xaxis_extent = self._y_axis_width - 1, width - self._y_axis_width - self._margin
         x_ticks, _ = self._x_axis.calculate_ticks(x_range, 1, xaxis_extent)
@@ -574,17 +592,14 @@
             if not is_memory_limit_hit:
 
                 # Draw the actual data:
                 line_colour = "#00FFFF"
                 if line_segments is not None:
                     self._draw_graph_line_segments(canvas, self._data_area, line_segments, line_colour)
 
-                if show_grid:
-                    self._draw_x_grid(canvas, x_ticks, self._data_area)
-
         return draw_followup, self._data_area
 
 
 class ProfileLayout(GraphLayout):
     """This Layout knows how to lay out and raw a profile graph."""
 
     _x_axis_unit = [AxisUnit()]
@@ -620,15 +635,15 @@
 
         width = canvas.winfo_width()
         height = canvas.winfo_height()
 
         # We draw things in a specific order so that some things appear on top of others.
 
         # First blank out the entire canvas to avoid leftovers being visible when resizing:
-        Layout._create_rectangle(canvas, 0, 0, width, height, 'black')
+        canvas.delete('all')
 
         # Fill the margins:
         Layout._create_rectangle(canvas, *self._get_top_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._get_right_margin(), AXIS_BG_COLOUR)
         Layout._create_rectangle(canvas, *self._dead_space, AXIS_BG_COLOUR)
 
         # Draw the axes:
```

### Comparing `batogram-1.0.7/batogram/modalwindow.py` & `batogram-1.0.8/batogram/modalwindow.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/morebncframe.py` & `batogram-1.0.8/batogram/morebncframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/moreframe.py` & `batogram-1.0.8/batogram/moreframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         super().__init__(parent)
         self._settings = settings
 
         self._guano_frame = GuanoFrame(self, pad)
         self.add(self._guano_frame, text="GUANO Metadata")
 
         self._axis_frame = ScaleFrame(self, button_frame, settings, pad)
-        self.add(self._axis_frame, text="Scaling")
+        self.add(self._axis_frame, text="Scale")
 
         self._bnc_frame = BrightnessContrastFrame(self, button_frame, settings, pad)
         self.add(self._bnc_frame, text="Brightness/Contrast")
         self._histogram_interface = self._bnc_frame.get_histogram_interface()
 
         self._processing_frame = RenderingFrame(self, button_frame, settings, pad)
         self.add(self._processing_frame, text="Rendering")
```

### Comparing `batogram-1.0.7/batogram/morerenderingframe.py` & `batogram-1.0.8/batogram/morerenderingframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/morescaleframe.py` & `batogram-1.0.8/batogram/morescaleframe.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,37 +74,47 @@
                                                                    message="The maximum frequency must be greater than the minimum.")
 
         self._f_max = DoubleValidatingEntry(self, controlling_frame, self, width=width,
                                             decimal_places=self._FREQUENCY_DPS,
                                             scaler=self._FREQUENCY_SCALER, value_validator=f_max_validator)
         self._f_max.grid(row=2, column=2, padx=pad)
 
-        self._show_grid_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Show grid")
-        self._show_grid_checkbutton.grid(row=1, column=4, padx=pad, sticky="W")
+        self._show_time_markers_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Show markers")
+        self._show_time_markers_checkbutton.grid(row=1, column=4, padx=pad, sticky="W")
+
+        self._show_frequency_markers_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Show markers")
+        self._show_frequency_markers_checkbutton.grid(row=2, column=4, padx=pad, sticky="W")
 
         self._zero_based_time_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Zero based time")
         self._zero_based_time_checkbutton.grid(row=1, column=5, padx=pad, sticky="W")
 
+        self._show_grid_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, "Show grid")
+        self._show_grid_checkbutton.grid(row=3, column=1, padx=pad, sticky="W")
+
         self._show_profile_checkbutton = ValidatingCheckbutton(self, controlling_frame, self, text="Show profile")
-        self._show_profile_checkbutton.grid(row=2, column=4, padx=pad, sticky="W")
+        self._show_profile_checkbutton.grid(row=3, column=2, padx=pad, sticky="W")
 
         self.copy_settings_to_widgets()
 
     def copy_settings_to_widgets(self):
         # Update the entry values from settings:
         self._t_max.set_value(self._settings.time_range.max)
         self._t_min.set_value(self._settings.time_range.min)
         self._f_max.set_value(self._settings.frequency_range.max)
         self._f_min.set_value(self._settings.frequency_range.min)
         self._show_grid_checkbutton.set_value(self._settings.show_grid)
         self._zero_based_time_checkbutton.set_value(self._settings.zero_based_time)
         self._show_profile_checkbutton.set_value(self._settings.show_profile)
+        self._show_time_markers_checkbutton.set_value(self._settings.show_time_markers)
+        self._show_frequency_markers_checkbutton.set_value(self._settings.show_frequency_markers)
 
     def copy_widgets_to_settings(self):
         # Update the settings values from the UI:
         self._settings.time_range.max = self._t_max.get_value()
         self._settings.time_range.min = self._t_min.get_value()
         self._settings.frequency_range.max = self._f_max.get_value()
         self._settings.frequency_range.min = self._f_min.get_value()
         self._settings.show_grid = self._show_grid_checkbutton.get_value()
         self._settings.zero_based_time = self._zero_based_time_checkbutton.get_value()
         self._settings.show_profile = self._show_profile_checkbutton.get_value()
+        self._settings.show_time_markers = self._show_time_markers_checkbutton.get_value()
+        self._settings.show_frequency_markers = self._show_frequency_markers_checkbutton.get_value()
```

### Comparing `batogram-1.0.7/batogram/profilegraphframe.py` & `batogram-1.0.8/batogram/profilegraphframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 
-from .constants import MAIN_PROFILE_COMPLETER_EVENT, FONT_SIZE
+from .constants import MAIN_PROFILE_COMPLETER_EVENT, AXIS_FONT_HEIGHT
 from . import layouts
 from .audiofileservice import RawDataReader
 from .common import AxisRange
 from .frames import GraphFrame, DrawableFrame
 from .rendering import ProfilePipelineRequest
 
 PROFILE_WIDTH = 90
@@ -59,15 +59,15 @@
         af_data = self._dc.get_afs_data()
 
         # Allow the canvas to catch up with any pending resizes so that we get the right
         # size below:
         self.update_idletasks()
 
         width, height = self._canvas.winfo_width(), self._canvas.winfo_height()
-        layout = layouts.ProfileLayout(FONT_SIZE, width, height)
+        layout = layouts.ProfileLayout(AXIS_FONT_HEIGHT, width, height)
         # Draw the graph axes here in the UI thread, as that is fast and provides responsiveness to the user:
         graph_completer, data_area = layout.draw(self._canvas, profile_range, frequency_range,
                                                  self._settings.show_grid, self._settings.zero_based_time)
         if af_data and self._pipeline:
             # Kick off the pipeline which will create a graph in another thread,
             # and complete by generating an event that will finish drawing the grph:
             self._completer = graph_completer
```

### Comparing `batogram-1.0.7/batogram/readoutframe.py` & `batogram-1.0.8/batogram/readoutframe.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/rendering.py` & `batogram-1.0.8/batogram/rendering.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/rootwindow.py` & `batogram-1.0.8/batogram/rootwindow.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/spectrogramgraphframe.py` & `batogram-1.0.8/batogram/spectrogramgraphframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import tkinter as tk
 from typing import Tuple, Optional
 
-from .constants import MAIN_SPECTROGAM_COMPLETER_EVENT, FONT_SIZE, MIN_F_RANGE, MIN_T_RANGE
+from .constants import MAIN_SPECTROGAM_COMPLETER_EVENT, AXIS_FONT_HEIGHT, MIN_F_RANGE, MIN_T_RANGE, \
+    AXIS_FONT_HEIGHT
 from . import layouts
 from .audiofileservice import RawDataReader, AudioFileService
-from .common import AxisRange
+from .common import AxisRange, clip_to_range
 from .frames import GraphFrame, DrawableFrame
+from .markers import TimeMarkerPair, FrequencyMarkerPair
 from .spectrogrammouseservice import SpectrogramMouseService, CursorMode
 from .rendering import SpectrogramPipelineRequest
 from .moreframe import HistogramInterface
 
 
 class SpectrogramCanvas(tk.Canvas):
     """A Canvas containing a spectrogram."""
@@ -41,14 +43,17 @@
 
     def set_cursor_mode(self, mode):
         self._mouse_service.set_cursor_mode(mode)
 
     def notify_draw_complete(self):
         self._mouse_service.notify_draw_complete()
 
+    def preempt_mouse(self, preempt: bool):
+        self._mouse_service.preempt_mouse(preempt)
+
 
 class SpectrogramGraphFrame(GraphFrame):
     """A graph frame containing a spectrogram."""
 
     def __init__(self, parent: "PanelFrame", root, pipeline, data_context, settings, initial_cursor_mode, is_reference):
         super().__init__(parent, root, pipeline, data_context, settings)
 
@@ -63,14 +68,20 @@
 
         # Scrollers are (individually) optional:
         self._scroller_t = None
         self._scroller_f = None
 
         self._parent = parent
 
+        # Optional time marker pair, depends whether the user has enabled time markers or not:
+        self._time_marker_pair: Optional[TimeMarkerPair] = None
+        self._frequency_marker_pair: Optional[FrequencyMarkerPair] = None
+        # self._time_marker_pair: Optional[TimeMarkerPair] = TimeMarkerPair(self._canvas, self, 0.2, 0.4)
+        # self._frequency_marker_pair: Optional[FrequencyMarkerPair] = FrequencyMarkerPair(self._canvas, self, 20000, 50000)
+
         self.bind("<Configure>", self._on_canvas_change)
         self.bind(MAIN_SPECTROGAM_COMPLETER_EVENT, self._do_completer)
 
     def set_histogram_interface(self, interface: HistogramInterface):
         self._histogram_interface = interface
 
     def set_scroller_t(self, time_scroller):
@@ -106,42 +117,49 @@
             cmd, f, = args
             self._scroll_move_frequency(float(f))
         elif cmd == tk.SCROLL:
             cmd, delta, size, = args
             self._scroll_delta_frequency(delta, size)
 
     def draw(self, draw_scope: int = DrawableFrame.DRAW_ALL):
+        # print("SpectrogramGraphFrame.draw()")
         super().draw(draw_scope)
 
         if not draw_scope & DrawableFrame.DRAW_SPECTROGRAM:
             return
 
         time_range, frequency_range = self._dc.time_range, self._dc.frequency_range
         afs_data = self._dc.get_afs_data()
 
         # Allow the canvas to catch up with any pending resizes so that we get the right
-        # size below:        self._parent = parent
+        # size below:
         self.update_idletasks()
 
+        self._show_hide_markers(time_range, frequency_range)
+
         width, height = self.get_canvas_size()
-        self._layout = layouts.SpectrogramLayout(FONT_SIZE, width, height)
+        self._layout = layouts.SpectrogramLayout(AXIS_FONT_HEIGHT, width, height,
+                                                 self._time_marker_pair, self._frequency_marker_pair)
+
         # Draw the graph axes here in the UI thread, as that is fast and provides responsiveness to the user:
-        graph_completer, data_area = self._layout.draw(self._canvas, time_range, frequency_range, self._settings.show_grid,
+        graph_completer, data_area = self._layout.draw(self._canvas, time_range, frequency_range,
+                                                       self._settings.show_grid,
                                                        self._settings.zero_based_time)
 
         if afs_data:
             self._update_time_scroller(time_range, afs_data.time_range)
             self._update_frequency_scroller(frequency_range, afs_data.frequency_range)
             if self._pipeline:
                 # Kick off the pipeline which will create a spectrogram in another thread,
                 # and complete by generating an event that will finish drawing the graph in
                 # this thread.
                 self._completer = graph_completer
                 screen_factors = self._parent.get_screen_factors()
-                request = self._get_pipeline_request(self._is_reference, afs_data, data_area, time_range, frequency_range, screen_factors,
+                request = self._get_pipeline_request(self._is_reference, afs_data, data_area, time_range,
+                                                     frequency_range, screen_factors,
                                                      self._dc.get_afs())
                 self._pipeline.submit(request,
                                       lambda: self.event_generate(MAIN_SPECTROGAM_COMPLETER_EVENT),
                                       self._pipeline_error_handler)
         else:
             # No data, make the sliders full length:
             self._update_time_scroller(AxisRange(0, 1), AxisRange(0, 1))
@@ -150,32 +168,55 @@
             # No data, so clear the histogram:
             self._histogram_interface.hide_histogram()
 
             # No data, so we can complete drawing the graph right away:
             graph_completer()
 
         # Allow the screen update to happen:
-        self.update()
+        self.update_idletasks()
 
         self._canvas.notify_draw_complete()
 
+    def _show_hide_markers(self, time_range: AxisRange, frequency_range: AxisRange):
+        """Create or destory markers depending on the settings."""
+
+        if self._settings.show_time_markers:
+            if self._time_marker_pair is None:
+                # Create a marker pair that is visible in the current time scale:
+                delta = time_range.max - time_range.min
+                self._time_marker_pair = TimeMarkerPair(self._canvas, self,
+                                                        time_range.min + delta / 3, time_range.max - delta / 3)
+        else:
+            self._time_marker_pair = None
+
+        if self._settings.show_frequency_markers:
+            if self._frequency_marker_pair is None:
+                # Create a marker pair that is visible in the current frequency scale:
+                delta = frequency_range.max - frequency_range.min
+                self._frequency_marker_pair = FrequencyMarkerPair(self._canvas, self,
+                                                                  frequency_range.min + delta / 3, frequency_range.max - delta / 3)
+        else:
+            self._frequency_marker_pair = None
+
     def set_cursor_mode(self, mode):
         if mode == CursorMode.CURSOR_ZOOM:
             self._canvas.config(cursor="cross")
         elif mode == CursorMode.CURSOR_PAN:
             self._canvas.config(cursor="fleur")
         else:
             self._canvas.config(cursor="")
 
         self._canvas.set_cursor_mode(mode)
 
     @staticmethod
-    def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range, screen_factors: tuple[float, float],
+    def _get_pipeline_request(is_reference: bool, data, data_area, time_range, frequency_range,
+                              screen_factors: tuple[float, float],
                               raw_data_reader: RawDataReader):
-        request = SpectrogramPipelineRequest(is_reference, data_area, data, time_range, frequency_range, screen_factors, raw_data_reader)
+        request = SpectrogramPipelineRequest(is_reference, data_area, data, time_range, frequency_range, screen_factors,
+                                             raw_data_reader)
         return request
 
     def _do_completer(self, _):
         # A bit of a hack because tkinter doesn't seem to allow data to be attached to an event:
         completer = self._completer
         if completer:
             memory_limit_hit, request, image, histogram, auto_vrange = self._pipeline.get_completion_data()  # Can be None.
@@ -243,31 +284,32 @@
         """
 
         # If a position is provided, we apply an offset so that that position
         # becomes the centre of the axis ranges:
         if position:
             position_t_v, position_f_v = self._layout.canvas_to_axis(position)
             time_range, frequency_range = self._layout.get_data_ranges()
-            centre_t_v, centre_f_v = (time_range.min + time_range.max) / 2, (frequency_range.min + frequency_range.max) / 2
+            centre_t_v, centre_f_v = (time_range.min + time_range.max) / 2, (
+                    frequency_range.min + frequency_range.max) / 2
             offset_t_v, offset_f_v = centre_t_v - position_t_v, centre_f_v - position_f_v
-            axis_ranges = AxisRange(time_range.min - offset_t_v, time_range.max - offset_t_v),\
+            axis_ranges = AxisRange(time_range.min - offset_t_v, time_range.max - offset_t_v), \
                 AxisRange(frequency_range.min - offset_f_v, frequency_range.max - offset_f_v)
         else:
             axis_ranges = self._layout.get_data_ranges()
 
         # We need to zoom the axis ranges in or out relative to the centres of their ranges:
         time_range, frequency_range = axis_ranges
 
         (l, r), (b, t) = time_range.get_tuple(), frequency_range.get_tuple()
 
         if t - b < MIN_F_RANGE or r - l < MIN_T_RANGE:
             # Allow them to zoom back out again, to avoid getting stuck.
             if factor < 1.0:
                 print("Ignoring insane zoom in.")
-                return False    # Insane zoom requested, ignore it.
+                return False  # Insane zoom requested, ignore it.
 
         # Offset to the centre of the axis ranges:
         centre_t_v, centre_f_v = (l + r) / 2, (t + b) / 2
         l, t, r, b = l - centre_t_v, t - centre_f_v, r - centre_t_v, b - centre_f_v
         # Apply the zoom:
         l, t, r, b = l * factor, t * factor, r * factor, b * factor
         # Reverse the offset we applied:
```

### Comparing `batogram-1.0.7/batogram/spectrogrammouseservice.py` & `batogram-1.0.8/batogram/spectrogrammouseservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         self._line = None
         self._line1 = None
         self._line2 = None
         self._last_wheel_time = timer()
         self._canvas_height: Optional[int] = None
         self._canvas_width: Optional[int] = None
         self._last_drag_mode: Optional[DragMode] = None
+        self._preempted: bool = False
 
         # Left mouse button:
         canvas.bind('<ButtonPress-1>', self._on_button1_press)
         canvas.bind('<Shift-ButtonPress-1>', self._on_button1_press)
         canvas.bind('<ButtonRelease-1>', self._on_button1_release)
         canvas.bind('<Shift-ButtonRelease-1>', self._on_shift_button1_release)
         canvas.bind('<B1-Motion>', self._on_button1_move)
@@ -97,40 +98,56 @@
         # Any mouse motion:
         canvas.bind('<Motion>', self._on_move)
         canvas.bind('<Leave>', self._on_leave)
 
         # Mouse wheel:
         self._bind_wheel()
 
+    def preempt_mouse(self, preempt: bool):
+        """Call this to take mouse control from this service, and to return it."""
+        self._preempted = preempt
+
     def _on_button1_press(self, event):
         # print("1+")
+        if self._preempted:
+            return
+
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
             self._on_zoom_press(event)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_press(event)
 
     def _on_button1_move(self, event):
+        # print("SpectrogramMouseService._on_button1_move")
+        if self._preempted:
+            return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
             self._on_zoom_move(event, is_shift=False)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_move(event, is_shift=False)
 
     def _on_shift_button1_move(self, event):
+        if self._preempted:
+            return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
             self._on_zoom_move(event, is_shift=True)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_move(event, is_shift=True)
 
     def _on_button1_release(self, event):
+        if self._preempted:
+            return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
             self._on_zoom_release(event, is_shift=False)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_release(event, is_shift=False)
 
     def _on_shift_button1_release(self, event):
+        if self._preempted:
+            return
         if self._cursor_mode == CursorMode.CURSOR_ZOOM:
             self._on_zoom_release(event, is_shift=True)
         elif self._cursor_mode == CursorMode.CURSOR_PAN:
             self._on_pan_release(event, is_shift=True)
 
     def _on_button2_press(self, event):
         # print("2+")
```

### Comparing `batogram-1.0.7/batogram/validatingwidgets.py` & `batogram-1.0.8/batogram/validatingwidgets.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram/wavfileparser.py` & `batogram-1.0.8/batogram/wavfileparser.py`

 * *Files identical despite different names*

### Comparing `batogram-1.0.7/batogram.egg-info/PKG-INFO` & `batogram-1.0.8/batogram.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batogram
-Version: 1.0.7
+Version: 1.0.8
 Summary: Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls.
 Author-email: John Mears <john+batogram@themears.co.uk>
 License: Copyright (c) 2023 John Mears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -42,15 +42,17 @@
 Batogram is an open source application for viewing bat call spectrograms.
 
 Some capabilities and features: 
 * Rendering of spectrograms from .wav files.
 * Auto selection of many parameters for simple operation.
 * Efficient rendering with graceful handling of larger data files.
 * Pan and scale using the mouse, keys or by manual selection.
+* Graphical markers allow time and frequency ranges to be conveniently read.
 * Handling of multichannel data files, including stereo.
+* Ability to correct for microphone frequency response.
 * Basic side by side comparison of two spectrograms.
 * Display of GUANO metadata, including the ability to click to open the location in Google Maps.
 * Runs on Windows, Linux and macOS (experimental) operating systems.
 
 Installation
 ------------
```

### Comparing `batogram-1.0.7/batogram.egg-info/SOURCES.txt` & `batogram-1.0.8/batogram.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 batogram/common.py
 batogram/constants.py
 batogram/fileinfoframe.py
 batogram/frames.py
 batogram/graphsettings.py
 batogram/historianservice.py
 batogram/layouts.py
+batogram/markers.py
 batogram/modalwindow.py
 batogram/morebncframe.py
 batogram/moreframe.py
 batogram/morerenderingframe.py
 batogram/morescaleframe.py
 batogram/profilegraphframe.py
 batogram/readoutframe.py
```

### Comparing `batogram-1.0.7/pyproject.toml` & `batogram-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "batogram"
-version = "1.0.7"   # Set this to the version number during release, and revert to 0.0.0 between releases.
+version = "1.0.8"   # Set this to the version number during release, and revert to 0.0.0 between releases.
 authors = [
     {name = "John Mears", email = "john+batogram@themears.co.uk"},
 ]
 description = "Batogram is a GUI program for rendering spectrograms from full spectrum recordings of bat calls."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["bat", "spectrogram", "chiropterology", "fourier", "ultrasonic", "ultrasound", "echo", "GUANO"]
```

