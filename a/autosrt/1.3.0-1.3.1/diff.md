# Comparing `tmp/autosrt-1.3.0.tar.gz` & `tmp/autosrt-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.0.tar", last modified: Sat Jun  3 21:10:09 2023, max compression
+gzip compressed data, was "autosrt-1.3.1.tar", last modified: Sun Jun  4 13:27:47 2023, max compression
```

## Comparing `autosrt-1.3.0.tar` & `autosrt-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.605443 autosrt-1.3.0/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.0/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-03 21:10:09.606190 autosrt-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.504491 autosrt-1.3.0/autosrt/
--rw-rw-rw-   0        0        0    15502 2023-06-03 21:05:35.000000 autosrt-1.3.0/autosrt/__init__.py
--rw-rw-rw-   0        0        0    55404 2023-06-03 21:09:04.000000 autosrt-1.3.0/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.585212 autosrt-1.3.0/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-06-03 21:10:09.000000 autosrt-1.3.0/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-03 21:10:08.000000 autosrt-1.3.0/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-03 21:10:09.609938 autosrt-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:10:09.601693 autosrt-1.3.0/test/
--rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.0/test/test1.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.0/test/test2.py
--rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.0/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.0/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.943765 autosrt-1.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-04 13:27:47.944515 autosrt-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.835138 autosrt-1.3.1/autosrt/
+-rw-rw-rw-   0        0        0    15502 2023-06-03 21:05:35.000000 autosrt-1.3.1/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    55527 2023-06-04 11:41:51.000000 autosrt-1.3.1/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.878584 autosrt-1.3.1/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-04 13:27:47.948264 autosrt-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.942268 autosrt-1.3.1/test/
+-rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.1/test/test1.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.1/test/test2.py
+-rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.1/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.1/test/test4.py
```

### Comparing `autosrt-1.3.0/LICENSE` & `autosrt-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/PKG-INFO` & `autosrt-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.0
+Version: 1.3.1
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.0/README.md` & `autosrt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/autosrt/__init__.py` & `autosrt-1.3.1/autosrt/__init__.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/autosrt/autosrt.py` & `autosrt-1.3.1/autosrt/autosrt.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 except ImportError:
     JSONDecodeError = ValueError
 from progressbar import ProgressBar, Percentage, Bar, ETA
 import pysrt
 import six
 import shlex
 
-VERSION = "1.3.0"
+VERSION = "1.3.1"
 
 
 #======================================================== ffmpeg_progress_yield ========================================================#
 
 
 import re
 #import subprocess
@@ -420,14 +420,15 @@
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
@@ -554,14 +555,15 @@
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
@@ -691,14 +693,15 @@
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

### Comparing `autosrt-1.3.0/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.1/autosrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.0
+Version: 1.3.1
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.0/setup.py` & `autosrt-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/test/test1.py` & `autosrt-1.3.1/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/test/test2.py` & `autosrt-1.3.1/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/test/test3.py` & `autosrt-1.3.1/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.0/test/test4.py` & `autosrt-1.3.1/test/test4.py`

 * *Files identical despite different names*

