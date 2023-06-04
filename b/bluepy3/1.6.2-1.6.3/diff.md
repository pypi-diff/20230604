# Comparing `tmp/bluepy3-1.6.2.tar.gz` & `tmp/bluepy3-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.6.2.tar", last modified: Sun Jun  4 08:20:43 2023, max compression
+gzip compressed data, was "bluepy3-1.6.3.tar", last modified: Sun Jun  4 09:14:23 2023, max compression
```

## Comparing `bluepy3-1.6.2.tar` & `bluepy3-1.6.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 08:20:43.102784 bluepy3-1.6.2/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.2/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 08:20:43.102864 bluepy3-1.6.2/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.6.2/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 08:20:43.102011 bluepy3-1.6.2/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-04-29 09:33:24.000000 bluepy3-1.6.2/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-05-19 05:34:25.000000 bluepy3-1.6.2/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-05-28 05:30:47.000000 bluepy3-1.6.2/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 08:20:43.102672 bluepy3-1.6.2/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-06-04 08:20:43.103080 bluepy3-1.6.2/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3424 2023-06-04 08:20:15.000000 bluepy3-1.6.2/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 09:14:23.539191 bluepy3-1.6.3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.3/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 09:14:23.539261 bluepy3-1.6.3/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.6.3/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 09:14:23.538346 bluepy3-1.6.3/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-06-04 08:43:37.000000 bluepy3-1.6.3/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.66.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 09:14:23.539071 bluepy3-1.6.3/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      521 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-06-04 09:14:23.539488 bluepy3-1.6.3/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3424 2023-06-04 09:14:02.000000 bluepy3-1.6.3/setup.py
```

### Comparing `bluepy3-1.6.2/LICENSE` & `bluepy3-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/PKG-INFO` & `bluepy3-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.6.2/README.md` & `bluepy3-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/Makefile` & `bluepy3-1.6.3/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/blescan.py` & `bluepy3-1.6.3/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/bluepy3-helper.c` & `bluepy3-1.6.3/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/btle.py` & `bluepy3-1.6.3/bluepy3/btle.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/config.5.47.h` & `bluepy3-1.6.3/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/config.5.50.h` & `bluepy3-1.6.3/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/config.5.60.h` & `bluepy3-1.6.3/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/config.5.66.h` & `bluepy3-1.6.3/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/get_services.py` & `bluepy3-1.6.3/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/scan_fuzz.py` & `bluepy3-1.6.3/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/sensortag.py` & `bluepy3-1.6.3/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/thingy52.py` & `bluepy3-1.6.3/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3/uuids.json` & `bluepy3-1.6.3/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.6.3/bluepy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.6.2/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.6.3/bluepy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.2/setup.py` & `bluepy3-1.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
 # VERSION = "1.5.1"   # latest version for testing
-VERSION = "1.6.2"  # latest version for production
+VERSION = "1.6.3"  # latest version for production
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
```

