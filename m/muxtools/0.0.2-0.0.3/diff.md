# Comparing `tmp/muxtools-0.0.2.tar.gz` & `tmp/muxtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxtools-0.0.2.tar", last modified: Sun Jun  4 11:10:42 2023, max compression
+gzip compressed data, was "muxtools-0.0.3.tar", last modified: Sun Jun  4 11:22:49 2023, max compression
```

## Comparing `muxtools-0.0.2.tar` & `muxtools-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.264687 muxtools-0.0.2/
--rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1115 2023-06-04 11:10:42.264687 muxtools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.230345 muxtools-0.0.2/muxtools/
--rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.248352 muxtools-0.0.2/muxtools/audio/
--rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.2/muxtools/audio/__init__.py
--rw-rw-rw-   0        0        0    11068 2023-06-03 01:30:34.000000 muxtools-0.0.2/muxtools/audio/audioutils.py
--rw-rw-rw-   0        0        0    14858 2023-06-04 10:23:26.000000 muxtools-0.0.2/muxtools/audio/encoders.py
--rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.2/muxtools/audio/extractors.py
--rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.2/muxtools/audio/memecoders.py
--rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.2/muxtools/audio/tools.py
--rw-rw-rw-   0        0        0     7680 2023-06-01 16:53:16.000000 muxtools-0.0.2/muxtools/cli.py
--rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.2/muxtools/functions.py
--rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/main.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.250352 muxtools-0.0.2/muxtools/misc/
--rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.2/muxtools/misc/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/misc/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.254352 muxtools-0.0.2/muxtools/muxing/
--rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/muxing/__init__.py
--rw-rw-rw-   0        0        0     4386 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/muxing/mux.py
--rw-rw-rw-   0        0        0     4403 2023-06-03 01:13:02.000000 muxtools-0.0.2/muxtools/muxing/muxfiles.py
--rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/muxing/tmdb.py
--rw-rw-rw-   0        0        0     6836 2023-06-04 10:19:37.000000 muxtools-0.0.2/muxtools/muxing/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.257354 muxtools-0.0.2/muxtools/subtitle/
--rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/subtitle/__init__.py
--rw-rw-rw-   0        0        0     1621 2023-06-04 10:32:35.000000 muxtools-0.0.2/muxtools/subtitle/font.py
--rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/subtitle/styles.py
--rw-rw-rw-   0        0        0    19594 2023-06-04 10:24:58.000000 muxtools-0.0.2/muxtools/subtitle/sub.py
--rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/subtitle/subutils.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.263687 muxtools-0.0.2/muxtools/utils/
--rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/convert.py
--rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.2/muxtools/utils/download.py
--rw-rw-rw-   0        0        0     1449 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/env.py
--rw-rw-rw-   0        0        0     5357 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/files.py
--rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/format.py
--rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/glob.py
--rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/utils/log.py
--rw-rw-rw-   0        0        0     8163 2023-06-01 18:49:53.000000 muxtools-0.0.2/muxtools/utils/parsing.py
--rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.2/muxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.244351 muxtools-0.0.2/muxtools.egg-info/
--rw-rw-rw-   0        0        0     1115 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1054 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1335 2023-06-04 11:10:17.000000 muxtools-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 11:10:42.264687 muxtools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.110119 muxtools-0.0.3/
+-rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1115 2023-06-04 11:22:49.110119 muxtools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.077110 muxtools-0.0.3/muxtools/
+-rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.095115 muxtools-0.0.3/muxtools/audio/
+-rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.3/muxtools/audio/__init__.py
+-rw-rw-rw-   0        0        0    11068 2023-06-03 01:30:34.000000 muxtools-0.0.3/muxtools/audio/audioutils.py
+-rw-rw-rw-   0        0        0    14858 2023-06-04 10:23:26.000000 muxtools-0.0.3/muxtools/audio/encoders.py
+-rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.3/muxtools/audio/extractors.py
+-rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.3/muxtools/audio/memecoders.py
+-rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.3/muxtools/audio/tools.py
+-rw-rw-rw-   0        0        0     7680 2023-06-01 16:53:16.000000 muxtools-0.0.3/muxtools/cli.py
+-rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.3/muxtools/functions.py
+-rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.096115 muxtools-0.0.3/muxtools/misc/
+-rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.3/muxtools/misc/__init__.py
+-rw-rw-rw-   0        0        0     7572 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/misc/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.099116 muxtools-0.0.3/muxtools/muxing/
+-rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/muxing/__init__.py
+-rw-rw-rw-   0        0        0     4386 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/muxing/mux.py
+-rw-rw-rw-   0        0        0     4403 2023-06-03 01:13:02.000000 muxtools-0.0.3/muxtools/muxing/muxfiles.py
+-rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/muxing/tmdb.py
+-rw-rw-rw-   0        0        0     6836 2023-06-04 10:19:37.000000 muxtools-0.0.3/muxtools/muxing/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.102116 muxtools-0.0.3/muxtools/subtitle/
+-rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/subtitle/__init__.py
+-rw-rw-rw-   0        0        0     1621 2023-06-04 10:32:35.000000 muxtools-0.0.3/muxtools/subtitle/font.py
+-rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/subtitle/styles.py
+-rw-rw-rw-   0        0        0    19594 2023-06-04 10:24:58.000000 muxtools-0.0.3/muxtools/subtitle/sub.py
+-rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/subtitle/subutils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.109120 muxtools-0.0.3/muxtools/utils/
+-rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/convert.py
+-rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.3/muxtools/utils/download.py
+-rw-rw-rw-   0        0        0     1449 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/env.py
+-rw-rw-rw-   0        0        0     5357 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/files.py
+-rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/format.py
+-rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.3/muxtools/utils/glob.py
+-rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.3/muxtools/utils/log.py
+-rw-rw-rw-   0        0        0     8153 2023-06-04 11:20:52.000000 muxtools-0.0.3/muxtools/utils/parsing.py
+-rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.3/muxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:22:49.091114 muxtools-0.0.3/muxtools.egg-info/
+-rw-rw-rw-   0        0        0     1115 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-04 11:22:49.000000 muxtools-0.0.3/muxtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1335 2023-06-04 11:22:12.000000 muxtools-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:22:49.110119 muxtools-0.0.3/setup.cfg
```

### Comparing `muxtools-0.0.2/LICENSE` & `muxtools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/PKG-INFO` & `muxtools-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.2/muxtools/__init__.py` & `muxtools-0.0.3/muxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/audio/audioutils.py` & `muxtools-0.0.3/muxtools/audio/audioutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/audio/encoders.py` & `muxtools-0.0.3/muxtools/audio/encoders.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/audio/extractors.py` & `muxtools-0.0.3/muxtools/audio/extractors.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/audio/memecoders.py` & `muxtools-0.0.3/muxtools/audio/memecoders.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/audio/tools.py` & `muxtools-0.0.3/muxtools/audio/tools.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/cli.py` & `muxtools-0.0.3/muxtools/cli.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/functions.py` & `muxtools-0.0.3/muxtools/functions.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/main.py` & `muxtools-0.0.3/muxtools/main.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/misc/chapters.py` & `muxtools-0.0.3/muxtools/misc/chapters.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/muxing/mux.py` & `muxtools-0.0.3/muxtools/muxing/mux.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/muxing/muxfiles.py` & `muxtools-0.0.3/muxtools/muxing/muxfiles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/muxing/tmdb.py` & `muxtools-0.0.3/muxtools/muxing/tmdb.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/muxing/tracks.py` & `muxtools-0.0.3/muxtools/muxing/tracks.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/subtitle/font.py` & `muxtools-0.0.3/muxtools/subtitle/font.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/subtitle/styles.py` & `muxtools-0.0.3/muxtools/subtitle/styles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/subtitle/sub.py` & `muxtools-0.0.3/muxtools/subtitle/sub.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/subtitle/subutils.py` & `muxtools-0.0.3/muxtools/subtitle/subutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/convert.py` & `muxtools-0.0.3/muxtools/utils/convert.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/download.py` & `muxtools-0.0.3/muxtools/utils/download.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/env.py` & `muxtools-0.0.3/muxtools/utils/env.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/files.py` & `muxtools-0.0.3/muxtools/utils/files.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/format.py` & `muxtools-0.0.3/muxtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/glob.py` & `muxtools-0.0.3/muxtools/utils/glob.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/log.py` & `muxtools-0.0.3/muxtools/utils/log.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools/utils/parsing.py` & `muxtools-0.0.3/muxtools/utils/parsing.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import subprocess
 from pathlib import Path
 from fractions import Fraction
 from pyparsebluray import mpls
 from .types import Chapter, PathLike, AudioInfo, AudioStats, AudioFrame, TrackType
 from .files import ensure_path_exists
-from .log import error, warn, debug
+from .log import error, warn, debug, info
 from .download import get_executable
 from .files import get_absolute_tracknum
 from .convert import (
     timedelta_from_formatted,
     timedelta_to_frame,
     frame_to_timedelta,
     mpls_timestamp_to_timedelta,
@@ -174,19 +174,19 @@
             if (plsmarks := playlist_mark.playlist_marks) is not None:
                 marks = plsmarks
             else:
                 raise error("There are no playlist marks in this file!", parse_chapters_bdmv)
 
         for i, playitem in enumerate(playlist.play_items):
             if (
-                playitem.clip_information_filename == src.file.stem
-                and playitem.clip_codec_identifier.lower() == src.file.suffix.lower().split(".")[1]
+                playitem.clip_information_filename == src.stem
+                and playitem.clip_codec_identifier.lower() == src.suffix.lower().split(".")[1]
             ):
                 if _print:
-                    print(f'Found chapters for "{src.file.name}" in "{f.name}":')
+                    info(f'Found chapters for "{src.name}" in "{f.name}":')
                 linked_marks = [mark for mark in marks if mark.ref_to_play_item_id == i]
                 try:
                     assert playitem.intime
                     offset = min(playitem.intime, linked_marks[0].mark_timestamp)
                 except IndexError:
                     continue
                 if (
```

### Comparing `muxtools-0.0.2/muxtools/utils/types.py` & `muxtools-0.0.3/muxtools/utils/types.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/muxtools.egg-info/PKG-INFO` & `muxtools-0.0.3/muxtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.2/muxtools.egg-info/SOURCES.txt` & `muxtools-0.0.3/muxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.2/pyproject.toml` & `muxtools-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "muxtools"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library for various muxing and automation tools for anything and everything fansubbing related"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "requests>=2.31.0",
     "fontcollector>=2.1.0",
```

