# Comparing `tmp/whisper_autosrt-0.1.0.tar.gz` & `tmp/whisper_autosrt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper_autosrt-0.1.0.tar", last modified: Sat Jun  3 21:39:00 2023, max compression
+gzip compressed data, was "whisper_autosrt-0.1.1.tar", last modified: Sun Jun  4 14:03:41 2023, max compression
```

## Comparing `whisper_autosrt-0.1.0.tar` & `whisper_autosrt-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 21:39:00.463532 whisper_autosrt-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1956 2023-06-03 21:39:00.464281 whisper_autosrt-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.0/README.md
--rw-rw-rw-   0        0        0      147 2023-06-03 21:39:00.467278 whisper_autosrt-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:39:00.429568 whisper_autosrt-0.1.0/whisper_autosrt/
--rw-rw-rw-   0        0        0    82496 2023-06-03 21:38:51.000000 whisper_autosrt-0.1.0/whisper_autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:39:00.462034 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-06-03 21:39:00.000000 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-03 21:39:00.000000 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 21:39:00.000000 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-03 21:39:00.000000 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-06-03 21:39:00.000000 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-03 21:39:00.000000 whisper_autosrt-0.1.0/whisper_autosrt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 14:03:40.998343 whisper_autosrt-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 whisper_autosrt-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1956 2023-06-04 14:03:40.999093 whisper_autosrt-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4700 2023-05-27 16:57:41.000000 whisper_autosrt-0.1.1/README.md
+-rw-rw-rw-   0        0        0      147 2023-06-04 14:03:41.001340 whisper_autosrt-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2023-06-02 17:36:46.000000 whisper_autosrt-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:03:40.960876 whisper_autosrt-0.1.1/whisper_autosrt/
+-rw-rw-rw-   0        0        0    82619 2023-06-04 12:34:43.000000 whisper_autosrt-0.1.1/whisper_autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 14:03:40.996844 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/
+-rw-rw-rw-   0        0        0     1956 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 14:03:40.000000 whisper_autosrt-0.1.1/whisper_autosrt.egg-info/top_level.txt
```

### Comparing `whisper_autosrt-0.1.0/LICENSE` & `whisper_autosrt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.0/PKG-INFO` & `whisper_autosrt-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper_autosrt
-Version: 0.1.0
+Version: 0.1.1
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `whisper_autosrt-0.1.0/README.md` & `whisper_autosrt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.0/setup.py` & `whisper_autosrt-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `whisper_autosrt-0.1.0/whisper_autosrt/__init__.py` & `whisper_autosrt-0.1.1/whisper_autosrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import warnings
 warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 from faster_whisper import WhisperModel
 import ctypes
 import shutil
 
 
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 #marker='█'
 
 
 #======================================================== ffmpeg_progress_yield ========================================================#
 
 
 import re
@@ -755,14 +755,15 @@
         self.list_codes.append("bn")
         self.list_codes.append("bho")
         self.list_codes.append("bs")
         self.list_codes.append("bg")
         self.list_codes.append("ca")
         self.list_codes.append("ceb")
         self.list_codes.append("ny")
+        self.list_codes.append("zh")
         self.list_codes.append("zh-CN")
         self.list_codes.append("zh-TW")
         self.list_codes.append("co")
         self.list_codes.append("hr")
         self.list_codes.append("cs")
         self.list_codes.append("da")
         self.list_codes.append("dv")
@@ -889,14 +890,15 @@
         self.list_names.append("Bengali")
         self.list_names.append("Bhojpuri")
         self.list_names.append("Bosnian")
         self.list_names.append("Bulgarian")
         self.list_names.append("Catalan")
         self.list_names.append("Cebuano")
         self.list_names.append("Chichewa")
+        self.list_names.append("Chinese")
         self.list_names.append("Chinese (Simplified)")
         self.list_names.append("Chinese (Traditional)")
         self.list_names.append("Corsican")
         self.list_names.append("Croatian")
         self.list_names.append("Czech")
         self.list_names.append("Danish")
         self.list_names.append("Dhivehi")
@@ -1026,14 +1028,15 @@
                         'bn': 'Bengali',
                         'bho': 'Bhojpuri',
                         'bs': 'Bosnian',
                         'bg': 'Bulgarian',
                         'ca': 'Catalan',
                         'ceb': 'Cebuano',
                         'ny': 'Chichewa',
+                        'zh': 'Chinese',
                         'zh-CN': 'Chinese (Simplified)',
                         'zh-TW': 'Chinese (Traditional)',
                         'co': 'Corsican',
                         'hr': 'Croatian',
                         'cs': 'Czech',
                         'da': 'Danish',
                         'dv': 'Dhivehi',
```

### Comparing `whisper_autosrt-0.1.0/whisper_autosrt.egg-info/PKG-INFO` & `whisper_autosrt-0.1.1/whisper_autosrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-autosrt
-Version: 0.1.0
+Version: 0.1.1
 Summary: a command line utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/whisper_autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

