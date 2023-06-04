# Comparing `tmp/adb-enhanced-2.5.8.tar.gz` & `tmp/adb-enhanced-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb-enhanced-2.5.8.tar", last modified: Wed Dec 23 13:42:18 2020, max compression
+gzip compressed data, was "adb-enhanced-2.5.9.tar", last modified: Mon Feb  1 07:58:56 2021, max compression
```

## Comparing `adb-enhanced-2.5.8.tar` & `adb-enhanced-2.5.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ashishb    (501) staff       (20)        0 2020-12-23 13:42:18.486712 adb-enhanced-2.5.8/
--rw-r--r--   0 ashishb    (501) staff       (20)      184 2020-03-31 08:15:34.000000 adb-enhanced-2.5.8/MANIFEST.in
--rw-r--r--   0 ashishb    (501) staff       (20)    13462 2020-12-23 13:42:18.487040 adb-enhanced-2.5.8/PKG-INFO
--rw-r--r--   0 ashishb    (501) staff       (20)     9778 2020-11-17 07:49:52.000000 adb-enhanced-2.5.8/README.md
-drwxr-xr-x   0 ashishb    (501) staff       (20)        0 2020-12-23 13:42:18.419807 adb-enhanced-2.5.8/adb_enhanced.egg-info/
--rw-r--r--   0 ashishb    (501) staff       (20)    13462 2020-12-23 13:42:18.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/PKG-INFO
--rw-r--r--   0 ashishb    (501) staff       (20)      453 2020-12-23 13:42:18.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/SOURCES.txt
--rw-r--r--   0 ashishb    (501) staff       (20)        1 2020-12-23 13:42:18.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/dependency_links.txt
--rw-r--r--   0 ashishb    (501) staff       (20)       41 2020-12-23 13:42:18.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/entry_points.txt
--rw-r--r--   0 ashishb    (501) staff       (20)       14 2020-12-23 13:42:18.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/requires.txt
--rw-r--r--   0 ashishb    (501) staff       (20)        5 2020-12-23 13:42:18.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/top_level.txt
--rw-r--r--   0 ashishb    (501) staff       (20)        1 2018-08-18 04:46:52.000000 adb-enhanced-2.5.8/adb_enhanced.egg-info/zip-safe
-drwxr-xr-x   0 ashishb    (501) staff       (20)        0 2020-12-23 13:42:18.486399 adb-enhanced-2.5.8/adbe/
--rw-r--r--   0 ashishb    (501) staff       (20)       23 2020-03-31 08:15:34.000000 adb-enhanced-2.5.8/adbe/__init__.py
--rw-r--r--   0 ashishb    (501) staff       (20)  8113580 2020-03-31 08:15:34.000000 adb-enhanced-2.5.8/adbe/abe.jar
--rwxr-xr-x   0 ashishb    (501) staff       (20)    62296 2020-12-23 13:39:30.000000 adb-enhanced-2.5.8/adbe/adb_enhanced.py
--rw-r--r--   0 ashishb    (501) staff       (20)     7848 2020-10-03 02:43:06.000000 adb-enhanced-2.5.8/adbe/adb_helper.py
--rw-r--r--   0 ashishb    (501) staff       (20)   352064 2020-03-31 08:15:34.000000 adb-enhanced-2.5.8/adbe/apksigner.jar
--rw-r--r--   0 ashishb    (501) staff       (20)      942 2020-05-08 05:36:08.000000 adb-enhanced-2.5.8/adbe/asyncio_helper.py
--rwxr-xr-x   0 ashishb    (501) staff       (20)    15931 2020-12-23 13:09:03.000000 adb-enhanced-2.5.8/adbe/main.py
--rw-r--r--   0 ashishb    (501) staff       (20)     1008 2020-05-08 04:36:06.000000 adb-enhanced-2.5.8/adbe/output_helper.py
--rw-r--r--   0 ashishb    (501) staff       (20)        5 2020-12-23 13:42:05.000000 adb-enhanced-2.5.8/adbe/version.txt
--rw-r--r--   0 ashishb    (501) staff       (20)       79 2020-12-23 13:42:18.487701 adb-enhanced-2.5.8/setup.cfg
--rw-r--r--   0 ashishb    (501) staff       (20)     1623 2020-11-17 07:46:20.000000 adb-enhanced-2.5.8/setup.py
+drwxr-xr-x   0 ashishb    (501) staff       (20)        0 2021-02-01 07:58:56.226172 adb-enhanced-2.5.9/
+-rw-r--r--   0 ashishb    (501) staff       (20)      184 2020-03-31 08:15:34.000000 adb-enhanced-2.5.9/MANIFEST.in
+-rw-r--r--   0 ashishb    (501) staff       (20)    15306 2021-02-01 07:58:56.226716 adb-enhanced-2.5.9/PKG-INFO
+-rw-r--r--   0 ashishb    (501) staff       (20)    10865 2021-01-31 08:23:44.000000 adb-enhanced-2.5.9/README.md
+drwxr-xr-x   0 ashishb    (501) staff       (20)        0 2021-02-01 07:58:56.128562 adb-enhanced-2.5.9/adb_enhanced.egg-info/
+-rw-r--r--   0 ashishb    (501) staff       (20)    15306 2021-02-01 07:58:55.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/PKG-INFO
+-rw-r--r--   0 ashishb    (501) staff       (20)      453 2021-02-01 07:58:55.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/SOURCES.txt
+-rw-r--r--   0 ashishb    (501) staff       (20)        1 2021-02-01 07:58:55.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/dependency_links.txt
+-rw-r--r--   0 ashishb    (501) staff       (20)       41 2021-02-01 07:58:55.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/entry_points.txt
+-rw-r--r--   0 ashishb    (501) staff       (20)       14 2021-02-01 07:58:55.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/requires.txt
+-rw-r--r--   0 ashishb    (501) staff       (20)        5 2021-02-01 07:58:55.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/top_level.txt
+-rw-r--r--   0 ashishb    (501) staff       (20)        1 2018-08-18 04:46:52.000000 adb-enhanced-2.5.9/adb_enhanced.egg-info/zip-safe
+drwxr-xr-x   0 ashishb    (501) staff       (20)        0 2021-02-01 07:58:56.225556 adb-enhanced-2.5.9/adbe/
+-rw-r--r--   0 ashishb    (501) staff       (20)       23 2020-03-31 08:15:34.000000 adb-enhanced-2.5.9/adbe/__init__.py
+-rw-r--r--   0 ashishb    (501) staff       (20)  8113580 2020-03-31 08:15:34.000000 adb-enhanced-2.5.9/adbe/abe.jar
+-rwxr-xr-x   0 ashishb    (501) staff       (20)    72408 2021-02-01 07:57:20.000000 adb-enhanced-2.5.9/adbe/adb_enhanced.py
+-rw-r--r--   0 ashishb    (501) staff       (20)     7848 2020-10-03 02:43:06.000000 adb-enhanced-2.5.9/adbe/adb_helper.py
+-rw-r--r--   0 ashishb    (501) staff       (20)   352064 2020-03-31 08:15:34.000000 adb-enhanced-2.5.9/adbe/apksigner.jar
+-rw-r--r--   0 ashishb    (501) staff       (20)      942 2020-05-08 05:36:08.000000 adb-enhanced-2.5.9/adbe/asyncio_helper.py
+-rwxr-xr-x   0 ashishb    (501) staff       (20)    17344 2021-02-01 07:52:56.000000 adb-enhanced-2.5.9/adbe/main.py
+-rw-r--r--   0 ashishb    (501) staff       (20)     1008 2020-05-08 04:36:06.000000 adb-enhanced-2.5.9/adbe/output_helper.py
+-rw-r--r--   0 ashishb    (501) staff       (20)        5 2021-02-01 07:58:40.000000 adb-enhanced-2.5.9/adbe/version.txt
+-rw-r--r--   0 ashishb    (501) staff       (20)       79 2021-02-01 07:58:56.227591 adb-enhanced-2.5.9/setup.cfg
+-rw-r--r--   0 ashishb    (501) staff       (20)     1623 2021-01-06 09:38:13.000000 adb-enhanced-2.5.9/setup.py
```

### Comparing `adb-enhanced-2.5.8/PKG-INFO` & `adb-enhanced-2.5.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: adb-enhanced
-Version: 2.5.8
+Version: 2.5.9
 Summary: Swiss-army knife for Android testing and development
 Home-page: https://github.com/ashishb/adb-enhanced
 Author: Ashish Bhatia
 Author-email: ashishb@ashishb.net
 License: Apache
 Description: ADB Enhanced |Downloads| |PyPI version|
         =======================================
         
-        |LintPython2| |LintPython3| |InstallAdbeTest|
+        |LintPython2| |LintPython3|
         
-        |AdbeUnitTestsPython3| |AdbeInstallTestsPython3|
-        |AdbeUnitTestsPython3Scheduled|
+        |InstallAdbeTest| |AdbeInstallTestsPython3| |AdbeUnitTestsPython3|
+        
+        |AdbeUnitTestsPython3-Api16| |AdbeUnitTestsPython3-Api21|
+        |AdbeUnitTestsPython3-Api22| |AdbeUnitTestsPython3-Api23|
+        |AdbeUnitTestsPython3-Api24| |AdbeUnitTestsPython3-Api25|
+        |AdbeUnitTestsPython3-Api26| |AdbeUnitTestsPython3-Api27|
+        |AdbeUnitTestsPython3-Api28| |AdbeUnitTestsPython3-Api29|
         
         .. figure:: docs/logo.png
            :alt: Logo
         
            Logo
         
         ADB-Enhanced is a Swiss-army knife for Android testing and development.
@@ -69,14 +74,16 @@
         
            ``adbe dont-keep-activities on``
         
         -  Take a screenshot ``adbe screenshot ~/Downloads/screenshot1.png``
         
         -  Take a video ``adbe screenrecord video.mp4 # Press ^C when finished``
         
+        -  Turn Wireless Debug mode on ``adbe enable wireless debugging``
+        
         Permissions
         ~~~~~~~~~~~
         
         -  Grant storage-related runtime permissions
         
            ``adbe permissions grant com.example storage``
         
@@ -195,15 +202,15 @@
            ::
         
               $ adbe app backup com.google.android.youtube backup.tar
         
         Usage
         ~~~~~
         
-        ::
+        .. code:: bash
         
            adbe [options] rotate (landscape | portrait | left | right)
            adbe [options] gfx (on | off | lines)
            adbe [options] overdraw (on | off | deut)
            adbe [options] layout (on | off)
            adbe [options] airplane (on | off)
            adbe [options] battery level <percentage>
@@ -226,14 +233,15 @@
            adbe [options] stay-awake-while-charging (on | off)
            adbe [options] input-text <text>
            adbe [options] press back
            adbe [options] open-url <url>
            adbe [options] permission-groups list all
            adbe [options] permissions list (all | dangerous)
            adbe [options] permissions (grant | revoke) <app_name> (calendar | camera | contacts | location | microphone | phone | sensors | sms | storage)
+           adbe [options] notifications list
            adbe [options] apps list (all | system | third-party | debug | backup-enabled)
            adbe [options] standby-bucket get <app_name>
            adbe [options] standby-bucket set <app_name> (active | working_set | frequent | rare)
            adbe [options] restrict-background (true | false) <app_name>
            adbe [options] ls [-a] [-l] [-R|-r] <file_path>
            adbe [options] rm [-f] [-R|-r] <file_path>
            adbe [options] mv [-f] <src_path> <dest_path>
@@ -247,21 +255,24 @@
            adbe [options] force-stop <app_name>
            adbe [options] clear-data <app_name>
            adbe [options] app info <app_name>
            adbe [options] app path <app_name>
            adbe [options] app signature <app_name>
            adbe [options] app backup <app_name> [<backup_tar_file_path>]
            adbe [options] install <file_path>
-           adbe [options] uninstall <app_name>
+           adbe [options] uninstall [--first-user] <app_name>
+           adbe [options] enable wireless debugging
+           adbe [options] disable wireless debugging
            adbe [options] screen (on | off | toggle)
+           adbe [options] alarm (all | top | pending | history)
         
         Options
         ~~~~~~~
         
-        ::
+        .. code:: bash
         
            -e, --emulator          directs the command to the only running emulator
            -d, --device            directs the command to the only connected "USB" device
            -s, --serial SERIAL     directs the command to the device or emulator with the given serial number or qualifier.
                                    Overrides ANDROID_SERIAL environment variable.
            -l                      For long list format, only valid for "ls" command
            -R                      For recursive directory listing, only valid for "ls" and "rm" command
@@ -310,16 +321,25 @@
         .. |Downloads| image:: http://pepy.tech/badge/adb-enhanced
            :target: http://pepy.tech/project/adb-enhanced
         .. |PyPI version| image:: https://badge.fury.io/py/adb-enhanced.svg
            :target: https://badge.fury.io/py/adb-enhanced
         .. |LintPython2| image:: https://github.com/ashishb/adb-enhanced/workflows/LintPython2/badge.svg
         .. |LintPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/LintPython3/badge.svg
         .. |InstallAdbeTest| image:: https://github.com/ashishb/adb-enhanced/workflows/InstallAdbeTest/badge.svg
-        .. |AdbeUnitTestsPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3/badge.svg
         .. |AdbeInstallTestsPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeInstallTestsPython3/badge.svg
-        .. |AdbeUnitTestsPython3Scheduled| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3Scheduled/badge.svg
+        .. |AdbeUnitTestsPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3/badge.svg
+        .. |AdbeUnitTestsPython3-Api16| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api16/badge.svg
+        .. |AdbeUnitTestsPython3-Api21| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api21/badge.svg
+        .. |AdbeUnitTestsPython3-Api22| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api22/badge.svg
+        .. |AdbeUnitTestsPython3-Api23| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api23/badge.svg
+        .. |AdbeUnitTestsPython3-Api24| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api24/badge.svg
+        .. |AdbeUnitTestsPython3-Api25| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api25/badge.svg
+        .. |AdbeUnitTestsPython3-Api26| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api26/badge.svg
+        .. |AdbeUnitTestsPython3-Api27| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api27/badge.svg
+        .. |AdbeUnitTestsPython3-Api28| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api28/badge.svg
+        .. |AdbeUnitTestsPython3-Api29| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api29/badge.svg
         
 Keywords: Android ADB developer
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.4
 Description-Content-Type: text/x-rst
```

### Comparing `adb-enhanced-2.5.8/adb_enhanced.egg-info/PKG-INFO` & `adb-enhanced-2.5.9/adb_enhanced.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: adb-enhanced
-Version: 2.5.8
+Version: 2.5.9
 Summary: Swiss-army knife for Android testing and development
 Home-page: https://github.com/ashishb/adb-enhanced
 Author: Ashish Bhatia
 Author-email: ashishb@ashishb.net
 License: Apache
 Description: ADB Enhanced |Downloads| |PyPI version|
         =======================================
         
-        |LintPython2| |LintPython3| |InstallAdbeTest|
+        |LintPython2| |LintPython3|
         
-        |AdbeUnitTestsPython3| |AdbeInstallTestsPython3|
-        |AdbeUnitTestsPython3Scheduled|
+        |InstallAdbeTest| |AdbeInstallTestsPython3| |AdbeUnitTestsPython3|
+        
+        |AdbeUnitTestsPython3-Api16| |AdbeUnitTestsPython3-Api21|
+        |AdbeUnitTestsPython3-Api22| |AdbeUnitTestsPython3-Api23|
+        |AdbeUnitTestsPython3-Api24| |AdbeUnitTestsPython3-Api25|
+        |AdbeUnitTestsPython3-Api26| |AdbeUnitTestsPython3-Api27|
+        |AdbeUnitTestsPython3-Api28| |AdbeUnitTestsPython3-Api29|
         
         .. figure:: docs/logo.png
            :alt: Logo
         
            Logo
         
         ADB-Enhanced is a Swiss-army knife for Android testing and development.
@@ -69,14 +74,16 @@
         
            ``adbe dont-keep-activities on``
         
         -  Take a screenshot ``adbe screenshot ~/Downloads/screenshot1.png``
         
         -  Take a video ``adbe screenrecord video.mp4 # Press ^C when finished``
         
+        -  Turn Wireless Debug mode on ``adbe enable wireless debugging``
+        
         Permissions
         ~~~~~~~~~~~
         
         -  Grant storage-related runtime permissions
         
            ``adbe permissions grant com.example storage``
         
@@ -195,15 +202,15 @@
            ::
         
               $ adbe app backup com.google.android.youtube backup.tar
         
         Usage
         ~~~~~
         
-        ::
+        .. code:: bash
         
            adbe [options] rotate (landscape | portrait | left | right)
            adbe [options] gfx (on | off | lines)
            adbe [options] overdraw (on | off | deut)
            adbe [options] layout (on | off)
            adbe [options] airplane (on | off)
            adbe [options] battery level <percentage>
@@ -226,14 +233,15 @@
            adbe [options] stay-awake-while-charging (on | off)
            adbe [options] input-text <text>
            adbe [options] press back
            adbe [options] open-url <url>
            adbe [options] permission-groups list all
            adbe [options] permissions list (all | dangerous)
            adbe [options] permissions (grant | revoke) <app_name> (calendar | camera | contacts | location | microphone | phone | sensors | sms | storage)
+           adbe [options] notifications list
            adbe [options] apps list (all | system | third-party | debug | backup-enabled)
            adbe [options] standby-bucket get <app_name>
            adbe [options] standby-bucket set <app_name> (active | working_set | frequent | rare)
            adbe [options] restrict-background (true | false) <app_name>
            adbe [options] ls [-a] [-l] [-R|-r] <file_path>
            adbe [options] rm [-f] [-R|-r] <file_path>
            adbe [options] mv [-f] <src_path> <dest_path>
@@ -247,21 +255,24 @@
            adbe [options] force-stop <app_name>
            adbe [options] clear-data <app_name>
            adbe [options] app info <app_name>
            adbe [options] app path <app_name>
            adbe [options] app signature <app_name>
            adbe [options] app backup <app_name> [<backup_tar_file_path>]
            adbe [options] install <file_path>
-           adbe [options] uninstall <app_name>
+           adbe [options] uninstall [--first-user] <app_name>
+           adbe [options] enable wireless debugging
+           adbe [options] disable wireless debugging
            adbe [options] screen (on | off | toggle)
+           adbe [options] alarm (all | top | pending | history)
         
         Options
         ~~~~~~~
         
-        ::
+        .. code:: bash
         
            -e, --emulator          directs the command to the only running emulator
            -d, --device            directs the command to the only connected "USB" device
            -s, --serial SERIAL     directs the command to the device or emulator with the given serial number or qualifier.
                                    Overrides ANDROID_SERIAL environment variable.
            -l                      For long list format, only valid for "ls" command
            -R                      For recursive directory listing, only valid for "ls" and "rm" command
@@ -310,16 +321,25 @@
         .. |Downloads| image:: http://pepy.tech/badge/adb-enhanced
            :target: http://pepy.tech/project/adb-enhanced
         .. |PyPI version| image:: https://badge.fury.io/py/adb-enhanced.svg
            :target: https://badge.fury.io/py/adb-enhanced
         .. |LintPython2| image:: https://github.com/ashishb/adb-enhanced/workflows/LintPython2/badge.svg
         .. |LintPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/LintPython3/badge.svg
         .. |InstallAdbeTest| image:: https://github.com/ashishb/adb-enhanced/workflows/InstallAdbeTest/badge.svg
-        .. |AdbeUnitTestsPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3/badge.svg
         .. |AdbeInstallTestsPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeInstallTestsPython3/badge.svg
-        .. |AdbeUnitTestsPython3Scheduled| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3Scheduled/badge.svg
+        .. |AdbeUnitTestsPython3| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3/badge.svg
+        .. |AdbeUnitTestsPython3-Api16| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api16/badge.svg
+        .. |AdbeUnitTestsPython3-Api21| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api21/badge.svg
+        .. |AdbeUnitTestsPython3-Api22| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api22/badge.svg
+        .. |AdbeUnitTestsPython3-Api23| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api23/badge.svg
+        .. |AdbeUnitTestsPython3-Api24| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api24/badge.svg
+        .. |AdbeUnitTestsPython3-Api25| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api25/badge.svg
+        .. |AdbeUnitTestsPython3-Api26| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api26/badge.svg
+        .. |AdbeUnitTestsPython3-Api27| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api27/badge.svg
+        .. |AdbeUnitTestsPython3-Api28| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api28/badge.svg
+        .. |AdbeUnitTestsPython3-Api29| image:: https://github.com/ashishb/adb-enhanced/workflows/AdbeUnitTestsPython3-Api29/badge.svg
         
 Keywords: Android ADB developer
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.4
 Description-Content-Type: text/x-rst
```

### Comparing `adb-enhanced-2.5.8/adbe/abe.jar` & `adb-enhanced-2.5.9/adbe/abe.jar`

 * *Files identical despite different names*

### Comparing `adb-enhanced-2.5.8/adbe/adb_enhanced.py` & `adb-enhanced-2.5.9/adbe/adb_enhanced.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 import tempfile
 import threading
 import time
 import os
 import random
 from urllib.parse import urlparse
+from enum import Enum
 import psutil
 
 # asyncio was introduced in version 3.5
 if sys.version_info >= (3, 5):
     try:
         import asyncio_helper
         _ASYNCIO_AVAILABLE = True
@@ -23,25 +24,32 @@
 else:
     _ASYNCIO_AVAILABLE = False
 
 try:
     # This fails when the code is executed directly and not as a part of python package installation,
     # I definitely need a better way to handle this.
     from adbe.adb_helper import (get_adb_shell_property, execute_adb_command2,
-            execute_adb_shell_command, execute_adb_shell_command2,
-            execute_file_related_adb_shell_command, get_package,
-            root_required_to_access_file, get_device_android_api_version, toggle_screen)
-    from adbe.output_helper import print_message, print_error, print_error_and_exit, print_verbose
+                                 execute_adb_shell_command, execute_adb_shell_command2,
+                                 execute_file_related_adb_shell_command, get_package,
+                                 root_required_to_access_file,
+                                 get_device_android_api_version, toggle_screen)
+    from adbe.output_helper import (print_message, print_error, print_error_and_exit,
+                                    print_verbose)
 except ImportError:
     # This works when the code is executed directly.
+    # noinspection PyUnresolvedReferences
     from adb_helper import (get_adb_shell_property, execute_adb_command2,
-            execute_adb_shell_command, execute_adb_shell_command2,
-            execute_file_related_adb_shell_command, get_package,
-            root_required_to_access_file, get_device_android_api_version, toggle_screen)
-    from output_helper import print_message, print_error, print_error_and_exit, print_verbose
+                            execute_adb_shell_command, execute_adb_shell_command2,
+                            execute_file_related_adb_shell_command, get_package,
+                            root_required_to_access_file,
+                            get_device_android_api_version, toggle_screen)
+
+    # noinspection PyUnresolvedReferences
+    from output_helper import (print_message, print_error, print_error_and_exit,
+                               print_verbose)
 
 
 _KEYCODE_BACK = 4
 _MIN_API_FOR_RUNTIME_PERMISSIONS = 23
 
 # Value to be return as 'on' to the user
 _USER_PRINT_VALUE_ON = 'on'
@@ -357,41 +365,56 @@
     if return_code != 0 or not result:
         return False
     result = result.strip()
     return result.find(app_name) != -1
 
 
 def handle_list_devices():
+    device_serials = _get_device_serials()
+
+    if not device_serials:
+        print_error_and_exit('No attached Android device found')
+
+    for device_serial in device_serials:
+        _print_device_info(device_serial)
+
+
+def _get_device_serials() -> [str]:
     cmd = 'devices -l'
     return_code, stdout, stderr = execute_adb_command2(cmd)
     if return_code != 0:
         print_error_and_exit('Failed to execute command %s, error: %s ' % (cmd, stderr))
 
+    device_serials = []
     # Skip the first line, it says "List of devices attached"
     device_infos = stdout.split('\n')[1:]
 
     if len(device_infos) == 0 or (
             len(device_infos) == 1 and len(device_infos[0]) == 0):
-        print_error_and_exit('No attached Android device found')
-    elif len(device_infos) == 1:
-        _print_device_info()
-    else:
-        for device_info in device_infos:
-            if not device_info:
-                continue
-            device_serial = device_info.split()[0]
-            if 'unauthorized' in device_info:
-                device_info = ' '.join(device_info.split()[1:])
-                print_error(
-                    ('Unlock Device "%s" and give USB debugging access to ' +
-                     'this PC/Laptop by unlocking and reconnecting ' +
-                     'the device. More info about this device: "%s"\n') % (
-                         device_serial, device_info))
-            else:
-                _print_device_info(device_serial)
+        return []
+
+    if len(device_infos) == 1:
+        device_serial = device_infos[0].split(" ")[0]
+        device_serials.append(device_serial)
+        return device_serials
+
+    for device_info in device_infos:
+        if not device_info:
+            continue
+        device_serial = device_info.split()[0]
+        if 'unauthorized' in device_info:
+            device_info = ' '.join(device_info.split()[1:])
+            print_error(
+                ('Unlock Device "%s" and give USB debugging access to ' +
+                 'this PC/Laptop by unlocking and reconnecting ' +
+                 'the device. More info about this device: "%s"\n') % (
+                     device_serial, device_info))
+        else:
+            device_serials.append(device_serial)
+    return device_serials
 
 
 def _print_device_info(device_serial=None):
     manufacturer = get_adb_shell_property('ro.product.manufacturer', device_serial=device_serial)
     model = get_adb_shell_property('ro.product.model', device_serial=device_serial)
     # This worked on 4.4.3 API 19 Moto E
     display_name = get_adb_shell_property('ro.product.display', device_serial=device_serial)
@@ -697,15 +720,18 @@
 def get_show_taps_state():
     cmd = 'get system show_touches'
     return_code, stdout, _ = execute_adb_shell_settings_command2(cmd)
     if return_code != 0:
         print_error('Failed to get current state of "show user taps" setting')
         return _USER_PRINT_VALUE_UNKNOWN
 
-    if int(stdout.strip()) == 1:
+    stdout = stdout.strip()
+    if stdout == 'null':
+        return _USER_PRINT_VALUE_OFF
+    if int(stdout) == 1:
         return _USER_PRINT_VALUE_ON
     return _USER_PRINT_VALUE_OFF
 
 
 def toggle_show_taps(turn_on):
     if turn_on:
         value = 1
@@ -917,18 +943,32 @@
     if result:
         for line in result.split('\n'):
             _, package_name = line.split(':', 2)
             packages.append(package_name)
     return packages
 
 
+# "dumpsys package" is more accurate than "pm list packages" but that means the results of
+# list_all_apps are now different from list_system_apps, list_non_system_apps, and
+# list_debug_apps
+# For now, we can live with this discrepancy but in the longer run we want to fix those
+# other functions as well
+# https://stackoverflow.com/questions/63416599/adb-shell-pm-list-packages-missing-some-packages
 def list_all_apps():
-    cmd = 'pm list packages'
-    packages = _get_all_packages(cmd)
-    print('\n'.join(packages))
+    # https://developer.android.com/studio/command-line/dumpsys
+    cmd = 'dumpsys package'
+    pattern_packages = re.compile('Package \\[(.*?)\\]')
+    return_code, result, _ = execute_adb_shell_command2(cmd)
+    if return_code != 0:
+        print_error_and_exit('Command "%s" failed, something is wrong' % cmd)
+        return
+    all_apps = re.findall(pattern_packages, result)
+    # Get the unique results
+    all_apps = sorted(list(dict.fromkeys(all_apps)))
+    print_message('\n'.join(all_apps))
 
 
 def list_system_apps():
     cmd = 'pm list packages -s'
     packages = _get_all_packages(cmd)
     print('\n'.join(packages))
 
@@ -1465,18 +1505,33 @@
     print_verbose('Installing %s' % file_path)
     # -r: replace existing application
     return_code, _, stderr = execute_adb_command2('install -r %s' % file_path)
     if return_code != 0:
         print_error('Failed to install %s, stderr: %s' % (file_path, stderr))
 
 
-@ensure_package_exists
-def perform_uninstall(app_name):
+@ensure_package_exists2
+def perform_uninstall(app_name, first_user):
     print_verbose('Uninstalling %s' % app_name)
-    return_code, _, stderr = execute_adb_command2('uninstall %s' % app_name)
+    cmd = ""
+    if first_user:
+        # For system apps, that cannot uninstalled,
+        # this command uninstalls them for user 0 without doing a system uninstall
+        # since that would fail.
+        # https://www.xda-developers.com/uninstall-carrier-oem-bloatware-without-root-access/
+        cmd = "--user 0"
+    return_code, _, stderr = execute_adb_shell_command2('pm uninstall %s %s' % (cmd, app_name))
+    if return_code == 0:
+        return
+
+    if not cmd:
+        print_message("Uninstall failed, trying to uninstall for user 0...")
+        cmd = "--user 0"
+        return_code, _, stderr = execute_adb_shell_command2('pm uninstall %s %s' % (cmd, app_name))
+
     if return_code != 0:
         print_error('Failed to uninstall %s, stderr: %s' % (app_name, stderr))
 
 
 def _get_window_size():
     adb_cmd = 'shell wm size'
     _, result, _ = execute_adb_command2(adb_cmd)
@@ -1533,14 +1588,73 @@
 
 
 def _is_emulator():
     qemu = get_adb_shell_property('ro.kernel.qemu')
     return qemu is not None and qemu.strip() == '1'
 
 
+def enable_wireless_debug():
+    code, result, stderr = execute_adb_shell_command2("ip address")
+    if code != 0:
+        print_error_and_exit('Failed to switch device to wireless debug mode, stderr: '
+                             '%s' % stderr)
+
+    # Check, that phone connected to wlan
+    matching = re.findall(r"inet ([\d]{1,3}\.[\d]{1,3}\.[\d]{1,3}\.[\d]{1,3}).*wlan0$",
+            result, re.MULTILINE)
+    if matching is None or not matching:
+        print_error_and_exit('Failed to switch device to wireless debug mode')
+
+    ip = matching[0]
+
+    code, _, stderr = execute_adb_command2("tcpip 5555")
+    if code != 0:
+        print_error_and_exit('Failed to switch device %s to wireless debug mode, '
+                             'stderr: %s' % (ip, stderr))
+
+    code, _, stderr = execute_adb_command2("connect %s" % ip)
+    if code != 0:
+        print_error_and_exit('Cannot enable wireless debugging. Error: %s' % stderr)
+        return False
+    print_message('Connected via IP now you can disconnect the cable\nIP: %s' % ip)
+    return True
+
+
+def disable_wireless_debug():
+    device_serials = _get_device_serials()
+
+    if not device_serials:
+        print_error_and_exit('No connected device found')
+        return
+
+    ip_list = []
+    for device_serial in device_serials:
+        ips = re.findall(r"([\d]{1,3}\.[\d]{1,3}\.[\d]{1,3}\.[\d]{1,3}:[\d]{1,5})", device_serial, 0)
+        if not ips:
+            print_verbose('Not a IP connect device, serial: %s' % device_serial)
+            continue
+        if len(ips) > 1:
+            print_error('Malformed device IP: %s' % device_serial)
+        print_verbose('Found an IP connected ADB session: %s' % ips[0])
+        ip_list.append(ips[0])
+
+    result = True
+
+    for ip in ip_list:
+        code, _, stderr = execute_adb_command2('disconnect %s' % ip)
+        if code != 0:
+            print_error('Failed to disconnect %s: %s' % (ip, stderr))
+            result = False
+        else:
+            print_message('Disconnected %s' % ip)
+
+    if not result:
+        print_error_and_exit('')
+
+
 def switch_screen(switch_type):
     if switch_type == SCREEN_TOGGLE:
         c, o, e = toggle_screen()
 
         if c != 0:
             print_error_and_exit("Something gone wrong on "
                                  "screen control operation. Error: %s" % e)
@@ -1567,19 +1681,19 @@
 def print_notifications():
     # Noredact is neeed on >= Android 6.0 to see title and text
     code, output, err = execute_adb_shell_command2("dumpsys notification --noredact")
     if code != 0:
         print_error_and_exit("Something gone wrong on "
                              "fetching notification info. Error: %s" % err)
     notification_records = re.findall(r"\s*NotificationRecord\(.*", output, re.MULTILINE)
-    for i in range(0, len(notification_records)):
-        output_for_this_notification = output.split(notification_records[i])[1]
+    for i, notification_record in enumerate(notification_records):
+        output_for_this_notification = output.split(notification_record)[1]
         if i + 1 < len(notification_records):
             output_for_this_notification = output_for_this_notification.split(notification_records[i+1])[0]
-        notification_package = re.findall(r"pkg=(\S*)", notification_records[i])[0]
+        notification_package = re.findall(r"pkg=(\S*)", notification_record)[0]
         titles = re.findall("android.title=(.*)", output_for_this_notification)
         if len(titles) > 0:
             notification_title = titles[0]
         else:
             notification_title = None
         texts = re.findall("android.text=(.*)", output_for_this_notification)
         if len(texts) > 0:
@@ -1598,7 +1712,158 @@
         if notification_title:
             print_message('Title: %s' % notification_title)
         if notification_text and notification_text != 'null':
             print_message('Text: %s' % notification_text)
         for action in notification_actions:
             print_message('Action: %s' % action)
         print_message('')
+
+
+# Alarm Enum
+class AlarmEnum(Enum):
+    TOP = 't'
+    PENDING = 'p'
+    HISTORY = 'h'
+    ALL = 'a'
+
+
+def print_history_alarms(output_dump_alarm, padding):
+    print("App Alarm history")
+
+    pattern_pending_alarm = \
+        re.compile(r'(?<=App Alarm history:)'
+                   r'.*?(?=Past-due non-wakeup alarms)',
+                   re.DOTALL)
+    alarm_to_parse = re.sub(r' +', ' ',
+                            re.search(pattern_pending_alarm, output_dump_alarm).
+                            group(0)).split("\n")[1:-1]
+
+    for line in alarm_to_parse:
+        package_name = line[0:line.find(",")]
+        # +1 to escape ',' before user id
+        fields = line[line.find(",") + 1:].split(":")
+        user_id = fields[0]
+        print("%sPackage name: %s" % (padding, package_name))
+        print("%sUser ID: %s" % (padding * 2, user_id))
+        # History might be missing for new alarms
+        if len(fields) >= 2:
+            history = fields[1]
+            print("%shistory: %s" % (padding * 2, history))
+
+
+def print_top_alarms(output_dump_alarm, padding):
+    print("Top Alarms:")
+    pattern_top_alarm = re.compile(r'(?<=Top Alarms:\n).*?(?=Alarm Stats:)',
+                                   re.DOTALL)
+    alarm_to_parse = re.sub(
+        r' +', ' ',
+        re.search(pattern_top_alarm, output_dump_alarm).group(0)).split("\n")
+    temp_dict = {}
+    for i, alarm_i in enumerate(alarm_to_parse):
+        if re.match(r"^\+", alarm_i):
+            temp_dict[alarm_i] = alarm_to_parse[i + 1]
+            i += 1
+
+    for key, value in temp_dict.items():
+        # key example: +2m19s468ms running, 0 wakeups, 708 alarms: 1000:android
+        # value example: *alarm*:com.android.server.action.NETWORK_STATS_POLL
+        temp = key.split(',')
+        running_time = temp[0].split(" ")[0]
+        nb_woke_up = temp[1].strip().split(" ")[0]
+        nb_alarms = temp[2].strip().split(" ")[0]
+        uid = temp[2].strip().split(":")[1].strip()
+        package_name = temp[2].strip().split(":")[2].strip()
+        action = value.split(":")[1]
+        print("%sPackage name: %s" % (padding, package_name))
+        print("%sAction: %s" % (padding * 2, action))
+        print("%sRunning time: %s" % (padding * 2, running_time))
+        print("%sNumber of device woke up: %s" % (padding * 2, nb_woke_up))
+        print("%sNumber of alarms: %s" % (padding * 2, nb_alarms))
+        print("%sUser ID: %s" % (padding * 2, uid))
+
+
+def print_pending_alarms(output_dump_alarm, padding):
+    print("Pending Alarms:")
+    pattern_pending_alarm = \
+        re.compile(
+            r'(?<=Pending alarm batches:)'
+            r'.*?(?=(Pending user blocked background alarms|Past-due non-wakeup alarms))',
+            re.DOTALL)
+    alarm_to_parse = re.sub(
+        r' +', ' ',
+        re.search(pattern_pending_alarm, output_dump_alarm).group(0)).split("\n")[1:-1]
+    for line in alarm_to_parse:
+        line = line.strip()
+        if not line.startswith("Batch"):
+            continue
+
+        pattern_batch_info = re.compile(r'(?<=Batch\{).*?(?=\}:)',
+                                        re.DOTALL)
+        info = re.search(pattern_batch_info, line).group(0).split(" ")
+        print("%sID: %s" % (padding, info[0]))
+        print("%sNumber of alarms: %s" % (padding * 2, info[1].split("=")[1]))
+        print_verbose("%sStart: %s" % (padding * 2, info[2].split("=")[1]))
+        print_verbose("%sEnd: %s" % (padding * 2, info[3].split("=")[1]))
+        if "flgs" in line:
+            # TO-DO: translate the flags
+            print_verbose("%sflag: %s" % (padding * 2, info[4].split("=")[1]))
+
+        if line.startswith("RTC") or line.startswith("RTC_WAKEUP") or \
+                line.startswith("ELAPSED") or line.startswith("ELAPSED_WAKEUP"):
+            pattern_between_brackets = re.compile(r'(?<=\{).*?(?=\})',
+                                                  re.DOTALL)
+            info = re.search(pattern_between_brackets, line).group(0).split(" ")
+            print("%sAlarm #%s:" % (padding * 2, line.split("#")[1].split(":")[0]))
+            print_verbose("%sType: %s" % (padding * 2, line.split("#")[0]))
+            print_verbose("%sID: %s" % (padding * 2, info[0]))
+            print_verbose("%sType: %s" % (padding * 2, info[2]))
+            print_verbose("%sWhen: %s" % (padding * 2, info[4]))
+            print("%sPackage: %s" % (padding * 2, info[5]))
+
+
+def alarm_manager(param):
+    cmd = "dumpsys alarm"
+    api_version = get_device_android_api_version()
+    err_msg_api = "Your Android version (API 28 and bellow) does not support " \
+                  "listing pending alarm"
+
+    c, o, e = execute_adb_shell_command2(cmd)
+    if c != 0:
+        print_error_and_exit("Something gone wrong on "
+                             "dumping alarms. Error: %s" % e)
+        return
+
+    if not isinstance(param, AlarmEnum):
+        print_error("Not supported parameter")
+        return
+
+    run_all = 0
+    padding = ""
+    if param == AlarmEnum.ALL:
+        run_all = 1
+        padding = "\t"
+
+    if param == AlarmEnum.TOP or run_all == 1:
+        print_top_alarms(o, padding)
+
+    if param == AlarmEnum.PENDING or run_all == 1:
+        if api_version > 28:
+            print_pending_alarms(o, padding)
+        else:
+            print_error(err_msg_api)
+
+    if param == AlarmEnum.HISTORY or run_all == 1:
+        if api_version > 28:
+            print_history_alarms(o, padding)
+        else:
+            print_error(err_msg_api)
+
+
+# This permissions group seems to have been removed in API 29 and beyond.
+# https://github.com/ashishb/adb-enhanced/runs/1799363523?check_suite_focus=true
+def is_permission_group_unavailable_after_api_29(permission_group):
+    return permission_group in [
+        'android.permission-group.CONTACTS',
+        'android.permission-group.MICROPHONE',
+        'android.permission-group.LOCATION',
+        'android.permission-group.SMS',
+    ]
```

### Comparing `adb-enhanced-2.5.8/adbe/adb_helper.py` & `adb-enhanced-2.5.9/adbe/adb_helper.py`

 * *Files identical despite different names*

### Comparing `adb-enhanced-2.5.8/adbe/apksigner.jar` & `adb-enhanced-2.5.9/adbe/apksigner.jar`

 * *Files identical despite different names*

### Comparing `adb-enhanced-2.5.8/adbe/asyncio_helper.py` & `adb-enhanced-2.5.9/adbe/asyncio_helper.py`

 * *Files identical despite different names*

### Comparing `adb-enhanced-2.5.8/adbe/main.py` & `adb-enhanced-2.5.9/adbe/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 
 import docopt
 
 
 # This is required only for Python 2
 # pylint: disable=import-error
+
 try:
     # First try local import for development
     from adbe import adb_enhanced
     from adbe import adb_helper
     from adbe.output_helper import print_error_and_exit, print_message, set_verbose
 # Python 3.6 onwards, this throws ModuleNotFoundError
 except (ImportError, ModuleNotFoundError):
@@ -44,15 +45,15 @@
     adbe [options] wifi (on | off)
     adbe [options] rtl (on | off)
     adbe [options] screenshot <filename.png>
     adbe [options] screenrecord <filename.mp4>
     adbe [options] dont-keep-activities (on | off)
     adbe [options] animations (on | off)
     adbe [options] show-taps (on | off)
-    adbe [options] stay-awake-while-charging (on | off) 
+    adbe [options] stay-awake-while-charging (on | off)
     adbe [options] input-text <text>
     adbe [options] press back
     adbe [options] open-url <url>
     adbe [options] permission-groups list all
     adbe [options] permissions list (all | dangerous)
     adbe [options] permissions (grant | revoke) <app_name> (calendar | camera | contacts | location | microphone | phone | sensors | sms | storage)
     adbe [options] notifications list
@@ -73,16 +74,19 @@
     adbe [options] force-stop <app_name>
     adbe [options] clear-data <app_name>
     adbe [options] app info <app_name>
     adbe [options] app path <app_name>
     adbe [options] app signature <app_name>
     adbe [options] app backup <app_name> [<backup_tar_file_path>]
     adbe [options] install <file_path>
-    adbe [options] uninstall <app_name>
+    adbe [options] uninstall [--first-user] <app_name>
+    adbe [options] enable wireless debugging
+    adbe [options] disable wireless debugging
     adbe [options] screen (on | off | toggle)
+    adbe [options] alarm (all | top | pending | history)
 
 Options:
     -e, --emulator          directs the command to the only running emulator
     -d, --device            directs the command to the only connected "USB" device
     -s, --serial SERIAL     directs the command to the device or emulator with the given serial number or qualifier.
                             Overrides ANDROID_SERIAL environment variable.
     -l                      For long list format, only valid for "ls" command
@@ -92,14 +96,15 @@
     -v, --verbose           Verbose mode
 
 """
 
 """
 List of things which this tool will do in the future
 
+* adbe [options] (enable | disable) wireless debugging - disabled since it is not working
 * adbe b[ack]g[round-]c[ellular-]d[ata] [on|off] $app_name # This might not be needed at all after mobile-data saver mode
 * adbe app-standby $app_name
 * adbe rtl (on | off)  # adb shell settings put global debug.force_rtl 1 does not seem to work
 * adb shell input keyevent KEYCODE_POWER can do the toggle
 * adbe press up
 * adbe set_app_name [-f] $app_name
 * adbe reset_app_name
@@ -243,16 +248,23 @@
     elif args['permission-groups'] and args['list'] and args['all']:
         adb_enhanced.list_permission_groups()
     elif args['permissions'] and args['list']:
         adb_enhanced.list_permissions(args['dangerous'])
     elif args['permissions']:
         app_name = args['<app_name>']
         permission_group = adb_enhanced.get_permission_group(args)
+
         permissions = adb_enhanced.get_permissions_in_permission_group(permission_group)
-        if not permissions:
+        if not permissions and \
+                adb_enhanced.is_permission_group_unavailable_after_api_29(permission_group) and \
+                adb_enhanced.get_device_android_api_version() >= 29:
+            print_error_and_exit('Android has made contacts group empty on API 29 and beyond, '
+                                 'your device version is %d' %
+                                 adb_enhanced.get_device_android_api_version())
+        elif not permissions:
             print_error_and_exit('No permissions found in permissions group: %s' % permission_group)
         adb_enhanced.grant_or_revoke_runtime_permissions(
             app_name, args['grant'], permissions)
 
     elif args['notifications'] and args['list']:
         adb_enhanced.print_notifications()
 
@@ -335,15 +347,34 @@
     elif args['screen'] and args['toggle']:
         adb_enhanced.switch_screen(adb_enhanced.SCREEN_TOGGLE)
 
     elif args['install']:
         file_path = args['<file_path>']
         adb_enhanced.perform_install(file_path)
     elif args['uninstall']:
-        adb_enhanced.perform_uninstall(args['<app_name>'])
+        adb_enhanced.perform_uninstall(args['<app_name>'], args['--first-user'])
+
+    elif args['enable']:
+        if args['wireless'] and args['debugging']:
+            adb_enhanced.enable_wireless_debug()
+
+    elif args['disable']:
+        if args['wireless'] and args['debugging']:
+            adb_enhanced.disable_wireless_debug()
+
+    # alarm
+    elif args['alarm'] and args['all']:
+        adb_enhanced.alarm_manager(adb_enhanced.AlarmEnum.ALL)
+    elif args['alarm'] and args['history']:
+        adb_enhanced.alarm_manager(adb_enhanced.AlarmEnum.HISTORY)
+    elif args['alarm'] and args['pending']:
+        adb_enhanced.alarm_manager(adb_enhanced.AlarmEnum.PENDING)
+    elif args['alarm'] and args['top']:
+        adb_enhanced.alarm_manager(adb_enhanced.AlarmEnum.TOP)
+
     else:
         print_error_and_exit('Not implemented: "%s"' % ' '.join(sys.argv))
 
 
 def print_state_change_info(state_name, old_state, new_state):
     if old_state != new_state:
         print_message('\"%s\" state changed from "%s" -> "%s"' % (state_name, old_state, new_state))
```

### Comparing `adb-enhanced-2.5.8/adbe/output_helper.py` & `adb-enhanced-2.5.9/adbe/output_helper.py`

 * *Files identical despite different names*

### Comparing `adb-enhanced-2.5.8/setup.py` & `adb-enhanced-2.5.9/setup.py`

 * *Files identical despite different names*

