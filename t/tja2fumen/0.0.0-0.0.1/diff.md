# Comparing `tmp/tja2fumen-0.0.0.tar.gz` & `tmp/tja2fumen-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.0.0.tar", last modified: Sun Jun  4 18:49:02 2023, max compression
+gzip compressed data, was "tja2fumen-0.0.1.tar", last modified: Sun Jun  4 19:27:41 2023, max compression
```

## Comparing `tja2fumen-0.0.0.tar` & `tja2fumen-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 18:49:02.120049 tja2fumen-0.0.0/
--rw-rw-rw-   0        0        0     1083 2023-06-04 16:36:23.000000 tja2fumen-0.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3502 2023-06-04 18:49:02.119030 tja2fumen-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1781 2023-06-03 15:07:27.000000 tja2fumen-0.0.0/README.md
--rw-rw-rw-   0        0        0      720 2023-06-04 18:48:15.000000 tja2fumen-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 18:49:02.120049 tja2fumen-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       96 2023-06-04 15:18:33.000000 tja2fumen-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:49:02.077821 tja2fumen-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 18:49:02.091458 tja2fumen-0.0.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     1178 2023-06-04 16:30:47.000000 tja2fumen-0.0.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-06-04 16:25:40.000000 tja2fumen-0.0.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    11608 2023-06-04 18:47:43.000000 tja2fumen-0.0.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    20666 2023-06-04 16:25:40.000000 tja2fumen-0.0.0/src/tja2fumen/parsers.py
--rw-rw-rw-   0        0        0    13964 2023-06-04 18:47:43.000000 tja2fumen-0.0.0/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2851 2023-06-04 16:25:40.000000 tja2fumen-0.0.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-06-04 18:49:02.118041 tja2fumen-0.0.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     3502 2023-06-04 18:49:02.000000 tja2fumen-0.0.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-06-04 18:49:02.000000 tja2fumen-0.0.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 18:49:02.000000 tja2fumen-0.0.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-04 18:49:02.000000 tja2fumen-0.0.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-06-04 18:49:02.000000 tja2fumen-0.0.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 18:49:02.000000 tja2fumen-0.0.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.963748 tja2fumen-0.0.1/
+-rw-rw-rw-   0        0        0     1083 2023-06-04 16:36:23.000000 tja2fumen-0.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4390 2023-06-04 19:27:41.962749 tja2fumen-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-06-04 19:27:00.000000 tja2fumen-0.0.1/README.md
+-rw-rw-rw-   0        0        0      720 2023-06-04 19:27:19.000000 tja2fumen-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 19:27:41.963748 tja2fumen-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       96 2023-06-04 15:18:33.000000 tja2fumen-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.922466 tja2fumen-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.937436 tja2fumen-0.0.1/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1178 2023-06-04 16:30:47.000000 tja2fumen-0.0.1/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-06-04 16:25:40.000000 tja2fumen-0.0.1/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    11608 2023-06-04 18:47:43.000000 tja2fumen-0.0.1/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    20666 2023-06-04 16:25:40.000000 tja2fumen-0.0.1/src/tja2fumen/parsers.py
+-rw-rw-rw-   0        0        0    13964 2023-06-04 18:47:43.000000 tja2fumen-0.0.1/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2851 2023-06-04 16:25:40.000000 tja2fumen-0.0.1/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:27:41.960375 tja2fumen-0.0.1/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4390 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 19:27:41.000000 tja2fumen-0.0.1/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.0.0/LICENSE.txt` & `tja2fumen-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/PKG-INFO` & `tja2fumen-0.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.0.0
+Version: 0.0.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,27 +30,52 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 License-File: LICENSE.txt
 
 # tja2fumen
 
-This repo a new attempt to write a tja2fumen chart converter to replace/complement the existing [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter. 
+`tja2fumen` is a tool for Taiko no Tatsujin games that allows you to convert TJA files (`.tja`) to fumen files (`.bin`).
 
-### Goals
+This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako. 
 
-- Fix desyncronization issues due to BPMCHANGE commands. (See: https://github.com/Fluto/TakoTako/issues/16)
-- Provide open source code, as opposed to distributing only a closed-source binary.
-- Provide a highly-documented reference for parsing both the TJA and Fumen file formats.
-- Stick to "pure Python", i.e. no external dependencies if possible.
-- Provide support for Windows/Linux/macOS via [`PyInstaller`](https://pyinstaller.org/en/stable/) or something similar.
+## Goals
 
-### Usage
+- Act as a drop-in replacement for `tja2bin.exe` in TakoTako.
+- Fix https://github.com/Fluto/TakoTako/issues/16. (The original `tjabin.exe` doesn't properly handle `#BPMCHANGE` commands.)
+- Provide open source code to act as a reference for parsing and writing both the TJA and Fumen file formats.
+- Stick to the Python stdlib, i.e. no external dependencies if possible.
 
-The converter is in a messy/experimental state, and is not yet fit for use due to lack of support for important TJA commands.
+## Usage
 
-### Attribution
+### Option 1: Standalone Python installation
+
+If you're familiar with Python, you can install `tja2fumen` by running:
+
+```
+pip install tja2fumen
+```
+
+Then, you can convert a TJA file by running:
+
+```
+tja2fumen file.tja
+```
+
+### Option 2: Using with TakoTako
+
+> **Note**: Before adding `tja2fumen` to TakoTako, you may want to back up the original `tja2bin.exe` file, to make sure you can switch back to the old converter if necessary. The easiest way to do this is by renaming the existing file to `tja2bin.exe.bak`.
+
+To use this converter with TakoTako, head to the [Releases](https://github.com/vivaria/tja2fumen/releases) page, and download the `tja2fumen.exe` file attached to the release. Then, rename `tja2fumen.exe` to `tja2bin.exe`, and place the file in the TakoTako plugin folder.
+
+TakoTako's plugin folder is inside of the BepInEx folder, which will typically look something like:
+
+```
+C:\XboxGames\T Tablet\Content\BepInEx\plugins\com.fluto.takotako
+```
+
+## Attribution
 
 - The fumen-parsing code in this project is based off of a modified copy of the [`readFumen()`](https://github.com/KatieFrogs/fumen-tools/blob/6ff3a2f7f53687f3dd49c5c57fcfc5ccbe3e5a10/fumen2osu/fumen2osu.py#L7-L152) function from the [`fumen2osu.py`](https://github.com/KatieFrogs/fumen-tools/blob/main/fumen2osu/fumen2osu.py) found in @KatieFrogs' [`fumen-tools`](https://github.com/KatieFrogs/fumen-tools) project.
 - The TJA-parsing code in this project is a Python translation of the [`parseTJA.js`](https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js) file from @WHMHammer's [`tja-tools`](https://github.com/WHMHammer/tja-tools).
 
 > **Note**: To be explicily clear, neither @KatieFrogs nor @WHMHammer have endorsed this project, are affiliated with this project, or have made any direct contributions to this project. I have just modified their existing work.
```

### Comparing `tja2fumen-0.0.0/pyproject.toml` & `tja2fumen-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.0.0"
+version = "0.0.1"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.0.0/src/tja2fumen/__init__.py` & `tja2fumen-0.0.1/src/tja2fumen/__init__.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/src/tja2fumen/constants.py` & `tja2fumen-0.0.1/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/src/tja2fumen/converters.py` & `tja2fumen-0.0.1/src/tja2fumen/converters.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/src/tja2fumen/parsers.py` & `tja2fumen-0.0.1/src/tja2fumen/parsers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/src/tja2fumen/utils.py` & `tja2fumen-0.0.1/src/tja2fumen/utils.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/src/tja2fumen/writers.py` & `tja2fumen-0.0.1/src/tja2fumen/writers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.0.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.0.1/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.0.0
+Version: 0.0.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -30,27 +30,52 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: build
 License-File: LICENSE.txt
 
 # tja2fumen
 
-This repo a new attempt to write a tja2fumen chart converter to replace/complement the existing [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter. 
+`tja2fumen` is a tool for Taiko no Tatsujin games that allows you to convert TJA files (`.tja`) to fumen files (`.bin`).
 
-### Goals
+This project attempts to replace/complement the existing closed-source [tja2bin.exe](https://github.com/Fluto/TakoTako/blob/c269bcab60530877a16c2a473c84796b94d0a5ce/README.md?plain=1#L181) converter packaged alongside TakoTako. 
 
-- Fix desyncronization issues due to BPMCHANGE commands. (See: https://github.com/Fluto/TakoTako/issues/16)
-- Provide open source code, as opposed to distributing only a closed-source binary.
-- Provide a highly-documented reference for parsing both the TJA and Fumen file formats.
-- Stick to "pure Python", i.e. no external dependencies if possible.
-- Provide support for Windows/Linux/macOS via [`PyInstaller`](https://pyinstaller.org/en/stable/) or something similar.
+## Goals
 
-### Usage
+- Act as a drop-in replacement for `tja2bin.exe` in TakoTako.
+- Fix https://github.com/Fluto/TakoTako/issues/16. (The original `tjabin.exe` doesn't properly handle `#BPMCHANGE` commands.)
+- Provide open source code to act as a reference for parsing and writing both the TJA and Fumen file formats.
+- Stick to the Python stdlib, i.e. no external dependencies if possible.
 
-The converter is in a messy/experimental state, and is not yet fit for use due to lack of support for important TJA commands.
+## Usage
 
-### Attribution
+### Option 1: Standalone Python installation
+
+If you're familiar with Python, you can install `tja2fumen` by running:
+
+```
+pip install tja2fumen
+```
+
+Then, you can convert a TJA file by running:
+
+```
+tja2fumen file.tja
+```
+
+### Option 2: Using with TakoTako
+
+> **Note**: Before adding `tja2fumen` to TakoTako, you may want to back up the original `tja2bin.exe` file, to make sure you can switch back to the old converter if necessary. The easiest way to do this is by renaming the existing file to `tja2bin.exe.bak`.
+
+To use this converter with TakoTako, head to the [Releases](https://github.com/vivaria/tja2fumen/releases) page, and download the `tja2fumen.exe` file attached to the release. Then, rename `tja2fumen.exe` to `tja2bin.exe`, and place the file in the TakoTako plugin folder.
+
+TakoTako's plugin folder is inside of the BepInEx folder, which will typically look something like:
+
+```
+C:\XboxGames\T Tablet\Content\BepInEx\plugins\com.fluto.takotako
+```
+
+## Attribution
 
 - The fumen-parsing code in this project is based off of a modified copy of the [`readFumen()`](https://github.com/KatieFrogs/fumen-tools/blob/6ff3a2f7f53687f3dd49c5c57fcfc5ccbe3e5a10/fumen2osu/fumen2osu.py#L7-L152) function from the [`fumen2osu.py`](https://github.com/KatieFrogs/fumen-tools/blob/main/fumen2osu/fumen2osu.py) found in @KatieFrogs' [`fumen-tools`](https://github.com/KatieFrogs/fumen-tools) project.
 - The TJA-parsing code in this project is a Python translation of the [`parseTJA.js`](https://github.com/WHMHammer/tja-tools/blob/master/src/js/parseTJA.js) file from @WHMHammer's [`tja-tools`](https://github.com/WHMHammer/tja-tools).
 
 > **Note**: To be explicily clear, neither @KatieFrogs nor @WHMHammer have endorsed this project, are affiliated with this project, or have made any direct contributions to this project. I have just modified their existing work.
```

