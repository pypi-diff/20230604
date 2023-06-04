# Comparing `tmp/bluepy3-1.6.1.tar.gz` & `tmp/bluepy3-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.6.1.tar", last modified: Wed May 24 14:50:04 2023, max compression
+gzip compressed data, was "bluepy3-1.6.2.tar", last modified: Sun Jun  4 08:20:43 2023, max compression
```

## Comparing `bluepy3-1.6.1.tar` & `bluepy3-1.6.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-05-24 14:50:04.151330 bluepy3-1.6.1/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.1/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-05-24 14:50:04.151408 bluepy3-1.6.1/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3454 2023-04-29 09:30:37.000000 bluepy3-1.6.1/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-05-24 14:50:04.150602 bluepy3-1.6.1/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-04-29 09:33:24.000000 bluepy3-1.6.1/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-05-19 05:34:25.000000 bluepy3-1.6.1/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9750 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.1/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-05-24 14:50:04.151220 bluepy3-1.6.1/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-05-24 14:50:04.000000 bluepy3-1.6.1/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-05-24 14:50:04.000000 bluepy3-1.6.1/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-05-24 14:50:04.000000 bluepy3-1.6.1/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-05-24 14:50:04.000000 bluepy3-1.6.1/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-05-24 14:50:04.000000 bluepy3-1.6.1/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-05-24 14:50:04.151607 bluepy3-1.6.1/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3425 2023-05-24 14:49:20.000000 bluepy3-1.6.1/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 08:20:43.102784 bluepy3-1.6.2/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.2/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 08:20:43.102864 bluepy3-1.6.2/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.6.2/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 08:20:43.102011 bluepy3-1.6.2/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-04-29 09:33:24.000000 bluepy3-1.6.2/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-05-19 05:34:25.000000 bluepy3-1.6.2/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/config.5.66.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-05-28 05:30:47.000000 bluepy3-1.6.2/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.2/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 08:20:43.102672 bluepy3-1.6.2/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      521 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-06-04 08:20:43.000000 bluepy3-1.6.2/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-06-04 08:20:43.103080 bluepy3-1.6.2/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3424 2023-06-04 08:20:15.000000 bluepy3-1.6.2/setup.py
```

### Comparing `bluepy3-1.6.1/LICENSE` & `bluepy3-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/PKG-INFO` & `bluepy3-1.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -29,16 +29,15 @@
 
 ###### Note: If you are reading this on [PyPi](https://pypi.org/project/bluepy3/) then note that the formatting below looks terrible. Visit the project's homepage to read the correctly formatted [README.md](https://github.com/Mausy5043/bluepy3#readme) file. 
 
 ## Requirements
 
 Please be aware that this is not a beginners tool. Some experience with Linux CLI, Python3 and BT/BLE is expected.
 
-The package requires Python 3 v3.7 or higher to be installed. It has been extensively tested on a 
-Raspberry Pi 3 Model B+ (aarch64) with Debian GNU Linux 11 kernel 6.1.19-v8+.
+The package has been extensively tested on a Raspberry Pi 3 Model B+ (aarch64) with Debian GNU Linux 11 kernel 6.* and Python 3.9.*. It requires Python v3.7 or higher to be installed.
 
 The code needs an executable `bluepy3-helper` which is compiled from C source automatically 
 if you use the recommended pip installation method (see below). Otherwise,
 you can rebuild it using the Makefile in the `bluepy3` directory.
 
 The `bluepy3` package comes installed with lists of compatible UUIDs in `uuids.json`. 
 If, for whatever reason, you want to rebuild those lists, then the Python3 modules
@@ -79,29 +78,31 @@
 BD Address: B8:27:EB:90:4F:F5  ACL MTU: 1021:8  SCO MTU: 64:1
 UP RUNNING
 RX bytes:15332515 acl:452626 sco:0 events:333729 errors:0
 TX bytes:7376962 acl:438075 sco:0 commands:72113 errors:0
 ```
 Use `hciconfig [hci0] up` to activate the BT device if the above returns an error.
 
+Although Python v3.7 will still work, official support for v3.7 is dropped as of JUN2023 since that is EOL. It is advised to upgrade your Python installation to v3.9 or above.
+
 ## Documentation
 
-Documentation can be built from the sources in the docs/ directory using Sphinx.
+Documentation can be built from the sources in the `docs/` directory using Sphinx.
 
 ## License  
 
 See [LICENSE](LICENSE)
 
 ## Acknowledgements
 
 This work builds on previous work by [Ian Harvey](https://github.com/IanHarvey/bluepy) and uses code 
 by the [BleuZ project](http://www.bluez.org/) (not a https site) and the more 
 up-to-date [BleuZ on GitHub](https://github.com/bluez/bluez)
 
-Original source code and documentation can be found at:   
+Original source code and excellent documentation can be found at:   
   https://github.com/IanHarvey/bluepy   
   http://ianharvey.github.io/bluepy-doc/
 
 MIT License
 
 Copyright (c) 2023 Maurice (mausy5043) Hendrix
```

### Comparing `bluepy3-1.6.1/README.md` & `bluepy3-1.6.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 ###### Note: If you are reading this on [PyPi](https://pypi.org/project/bluepy3/) then note that the formatting below looks terrible. Visit the project's homepage to read the correctly formatted [README.md](https://github.com/Mausy5043/bluepy3#readme) file. 
 
 ## Requirements
 
 Please be aware that this is not a beginners tool. Some experience with Linux CLI, Python3 and BT/BLE is expected.
 
-The package requires Python 3 v3.7 or higher to be installed. It has been extensively tested on a 
-Raspberry Pi 3 Model B+ (aarch64) with Debian GNU Linux 11 kernel 6.1.19-v8+.
+The package has been extensively tested on a Raspberry Pi 3 Model B+ (aarch64) with Debian GNU Linux 11 kernel 6.* and Python 3.9.*. It requires Python v3.7 or higher to be installed.
 
 The code needs an executable `bluepy3-helper` which is compiled from C source automatically 
 if you use the recommended pip installation method (see below). Otherwise,
 you can rebuild it using the Makefile in the `bluepy3` directory.
 
 The `bluepy3` package comes installed with lists of compatible UUIDs in `uuids.json`. 
 If, for whatever reason, you want to rebuild those lists, then the Python3 modules
@@ -59,24 +58,26 @@
 BD Address: B8:27:EB:90:4F:F5  ACL MTU: 1021:8  SCO MTU: 64:1
 UP RUNNING
 RX bytes:15332515 acl:452626 sco:0 events:333729 errors:0
 TX bytes:7376962 acl:438075 sco:0 commands:72113 errors:0
 ```
 Use `hciconfig [hci0] up` to activate the BT device if the above returns an error.
 
+Although Python v3.7 will still work, official support for v3.7 is dropped as of JUN2023 since that is EOL. It is advised to upgrade your Python installation to v3.9 or above.
+
 ## Documentation
 
-Documentation can be built from the sources in the docs/ directory using Sphinx.
+Documentation can be built from the sources in the `docs/` directory using Sphinx.
 
 ## License  
 
 See [LICENSE](LICENSE)
 
 ## Acknowledgements
 
 This work builds on previous work by [Ian Harvey](https://github.com/IanHarvey/bluepy) and uses code 
 by the [BleuZ project](http://www.bluez.org/) (not a https site) and the more 
 up-to-date [BleuZ on GitHub](https://github.com/bluez/bluez)
 
-Original source code and documentation can be found at:   
+Original source code and excellent documentation can be found at:   
   https://github.com/IanHarvey/bluepy   
   http://ianharvey.github.io/bluepy-doc/
```

### Comparing `bluepy3-1.6.1/bluepy3/Makefile` & `bluepy3-1.6.2/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/blescan.py` & `bluepy3-1.6.2/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/bluepy3-helper.c` & `bluepy3-1.6.2/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/btle.py` & `bluepy3-1.6.2/bluepy3/btle.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/config.5.47.h` & `bluepy3-1.6.2/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/config.5.50.h` & `bluepy3-1.6.2/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/config.5.60.h` & `bluepy3-1.6.2/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/config.5.66.h` & `bluepy3-1.6.2/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/get_services.py` & `bluepy3-1.6.2/bluepy3/get_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 Note that the original tables from which the UUIDs were gathered nolonger exist.
 Therefore, the archived webpages are used from archive.com
 """
 
 import errno
 import os
 import tempfile
-
 import requests
 from bs4 import BeautifulSoup
 
 # fmt: off
 URL_CHARACTERISTICS = "https://web.archive.org/web/20170201044907/" \
                       "https://www.bluetooth.com/specifications/gatt/characteristics"
 URL_DECLARATIONS = "https://web.archive.org/web/20170502191915/" \
```

### Comparing `bluepy3-1.6.1/bluepy3/scan_fuzz.py` & `bluepy3-1.6.2/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/sensortag.py` & `bluepy3-1.6.2/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/thingy52.py` & `bluepy3-1.6.2/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3/uuids.json` & `bluepy3-1.6.2/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.6.2/bluepy3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.1
+Version: 1.6.2
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -29,16 +29,15 @@
 
 ###### Note: If you are reading this on [PyPi](https://pypi.org/project/bluepy3/) then note that the formatting below looks terrible. Visit the project's homepage to read the correctly formatted [README.md](https://github.com/Mausy5043/bluepy3#readme) file. 
 
 ## Requirements
 
 Please be aware that this is not a beginners tool. Some experience with Linux CLI, Python3 and BT/BLE is expected.
 
-The package requires Python 3 v3.7 or higher to be installed. It has been extensively tested on a 
-Raspberry Pi 3 Model B+ (aarch64) with Debian GNU Linux 11 kernel 6.1.19-v8+.
+The package has been extensively tested on a Raspberry Pi 3 Model B+ (aarch64) with Debian GNU Linux 11 kernel 6.* and Python 3.9.*. It requires Python v3.7 or higher to be installed.
 
 The code needs an executable `bluepy3-helper` which is compiled from C source automatically 
 if you use the recommended pip installation method (see below). Otherwise,
 you can rebuild it using the Makefile in the `bluepy3` directory.
 
 The `bluepy3` package comes installed with lists of compatible UUIDs in `uuids.json`. 
 If, for whatever reason, you want to rebuild those lists, then the Python3 modules
@@ -79,29 +78,31 @@
 BD Address: B8:27:EB:90:4F:F5  ACL MTU: 1021:8  SCO MTU: 64:1
 UP RUNNING
 RX bytes:15332515 acl:452626 sco:0 events:333729 errors:0
 TX bytes:7376962 acl:438075 sco:0 commands:72113 errors:0
 ```
 Use `hciconfig [hci0] up` to activate the BT device if the above returns an error.
 
+Although Python v3.7 will still work, official support for v3.7 is dropped as of JUN2023 since that is EOL. It is advised to upgrade your Python installation to v3.9 or above.
+
 ## Documentation
 
-Documentation can be built from the sources in the docs/ directory using Sphinx.
+Documentation can be built from the sources in the `docs/` directory using Sphinx.
 
 ## License  
 
 See [LICENSE](LICENSE)
 
 ## Acknowledgements
 
 This work builds on previous work by [Ian Harvey](https://github.com/IanHarvey/bluepy) and uses code 
 by the [BleuZ project](http://www.bluez.org/) (not a https site) and the more 
 up-to-date [BleuZ on GitHub](https://github.com/bluez/bluez)
 
-Original source code and documentation can be found at:   
+Original source code and excellent documentation can be found at:   
   https://github.com/IanHarvey/bluepy   
   http://ianharvey.github.io/bluepy-doc/
 
 MIT License
 
 Copyright (c) 2023 Maurice (mausy5043) Hendrix
```

### Comparing `bluepy3-1.6.1/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.6.2/bluepy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.1/setup.py` & `bluepy3-1.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
 # VERSION = "1.5.1"   # latest version for testing
-VERSION = "1.6.1"   # latest version for production
+VERSION = "1.6.2"  # latest version for production
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
```

