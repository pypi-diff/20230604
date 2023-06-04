# Comparing `tmp/pyFIS-1.8.1.tar.gz` & `tmp/pyFIS-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFIS-1.8.1.tar", last modified: Sat Feb  5 22:04:51 2022, max compression
+gzip compressed data, was "dist\pyFIS-1.9.0.tar", last modified: Fri Feb 18 16:39:03 2022, max compression
```

## Comparing `pyFIS-1.8.1.tar` & `pyFIS-1.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.877215 pyFIS-1.8.1/
--rw-r--r--   0 cato      (1000) cato      (1000)    35149 2020-10-03 17:00:08.000000 pyFIS-1.8.1/LICENSE
--rw-r--r--   0 cato      (1000) cato      (1000)      434 2022-02-05 22:04:51.877215 pyFIS-1.8.1/PKG-INFO
--rw-r--r--   0 cato      (1000) cato      (1000)     5365 2022-01-16 23:41:44.000000 pyFIS-1.8.1/README.md
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.863882 pyFIS-1.8.1/pyFIS.egg-info/
--rw-r--r--   0 cato      (1000) cato      (1000)      434 2022-02-05 22:04:51.000000 pyFIS-1.8.1/pyFIS.egg-info/PKG-INFO
--rw-r--r--   0 cato      (1000) cato      (1000)     1096 2022-02-05 22:04:51.000000 pyFIS-1.8.1/pyFIS.egg-info/SOURCES.txt
--rw-r--r--   0 cato      (1000) cato      (1000)        1 2022-02-05 22:04:51.000000 pyFIS-1.8.1/pyFIS.egg-info/dependency_links.txt
--rw-r--r--   0 cato      (1000) cato      (1000)        9 2022-02-05 22:04:51.000000 pyFIS-1.8.1/pyFIS.egg-info/requires.txt
--rw-r--r--   0 cato      (1000) cato      (1000)        6 2022-02-05 22:04:51.000000 pyFIS-1.8.1/pyFIS.egg-info/top_level.txt
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.867215 pyFIS-1.8.1/pyfis/
--rw-r--r--   0 cato      (1000) cato      (1000)      707 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/__init__.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.867215 pyFIS-1.8.1/pyfis/aegmis/
--rw-r--r--   0 cato      (1000) cato      (1000)      768 2022-01-15 19:58:30.000000 pyFIS-1.8.1/pyfis/aegmis/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)    17874 2022-01-16 23:33:26.000000 pyFIS-1.8.1/pyfis/aegmis/ecs_lcd.py
--rw-r--r--   0 cato      (1000) cato      (1000)     4834 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/aegmis/mis1_gcu.py
--rw-r--r--   0 cato      (1000) cato      (1000)     4381 2022-02-05 14:32:00.000000 pyFIS-1.8.1/pyfis/aegmis/mis2_gcu.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.867215 pyFIS-1.8.1/pyfis/ibis/
--rw-r--r--   0 cato      (1000) cato      (1000)      740 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/ibis/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)    22400 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/ibis/ibis_protocol.py
--rw-r--r--   0 cato      (1000) cato      (1000)     2071 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/ibis/ibis_serial.py
--rw-r--r--   0 cato      (1000) cato      (1000)     1771 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/ibis/ibis_tcp.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.870549 pyFIS-1.8.1/pyfis/krone/
--rw-r--r--   0 cato      (1000) cato      (1000)      809 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/krone/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)      791 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/krone/exceptions.py
--rw-r--r--   0 cato      (1000) cato      (1000)    10938 2022-02-05 21:58:17.000000 pyFIS-1.8.1/pyfis/krone/k8200.py
--rw-r--r--   0 cato      (1000) cato      (1000)     9738 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/krone/k9000_fbk.py
--rw-r--r--   0 cato      (1000) cato      (1000)     5829 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/krone/k9000_fbm.py
--rw-r--r--   0 cato      (1000) cato      (1000)     3107 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/krone/k9000_hlst.py
--rw-r--r--   0 cato      (1000) cato      (1000)     6340 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/krone/k9000_rs485.py
--rw-r--r--   0 cato      (1000) cato      (1000)     4670 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/krone/util.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.870549 pyFIS-1.8.1/pyfis/lawo/
--rw-r--r--   0 cato      (1000) cato      (1000)      736 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/lawo/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)    11672 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/lawo/lawo_font.py
--rw-r--r--   0 cato      (1000) cato      (1000)    12234 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/lawo/mono_protocol.py
--rw-r--r--   0 cato      (1000) cato      (1000)     1996 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/lawo/mono_serial.py
--rw-r--r--   0 cato      (1000) cato      (1000)     1063 2022-02-05 14:32:00.000000 pyFIS-1.8.1/pyfis/metadata.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.873882 pyFIS-1.8.1/pyfis/microsyst/
--rw-r--r--   0 cato      (1000) cato      (1000)      684 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/microsyst/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)    16803 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/microsyst/migra.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.873882 pyFIS-1.8.1/pyfis/omega/
--rw-r--r--   0 cato      (1000) cato      (1000)      696 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/omega/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)     3575 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/omega/rs485.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.877215 pyFIS-1.8.1/pyfis/splitflap_display/
--rw-r--r--   0 cato      (1000) cato      (1000)      801 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/splitflap_display/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)     6785 2020-10-03 17:00:08.000000 pyFIS-1.8.1/pyfis/splitflap_display/ascii_graphics.py
--rw-r--r--   0 cato      (1000) cato      (1000)    12322 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/splitflap_display/display.py
--rw-r--r--   0 cato      (1000) cato      (1000)    11038 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/splitflap_display/fields.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.877215 pyFIS-1.8.1/pyfis/utils/
--rw-r--r--   0 cato      (1000) cato      (1000)      676 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/utils/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)     5171 2022-02-05 21:58:44.000000 pyFIS-1.8.1/pyfis/utils/utils.py
-drwxr-xr-x   0 cato      (1000) cato      (1000)        0 2022-02-05 22:04:51.877215 pyFIS-1.8.1/pyfis/xatlabs/
--rw-r--r--   0 cato      (1000) cato      (1000)      751 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/xatlabs/__init__.py
--rw-r--r--   0 cato      (1000) cato      (1000)      701 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/xatlabs/exceptions.py
--rw-r--r--   0 cato      (1000) cato      (1000)     6761 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/xatlabs/rgb_dsa.py
--rw-r--r--   0 cato      (1000) cato      (1000)     3712 2022-01-15 19:57:09.000000 pyFIS-1.8.1/pyfis/xatlabs/splitflap.py
--rw-r--r--   0 cato      (1000) cato      (1000)       38 2022-02-05 22:04:51.877215 pyFIS-1.8.1/setup.cfg
--rw-r--r--   0 cato      (1000) cato      (1000)      463 2020-10-03 17:00:08.000000 pyFIS-1.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/
+-rw-rw-rw-   0        0        0      434 2022-02-18 16:39:03.000000 pyFIS-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5546 2022-02-18 16:38:58.000000 pyFIS-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyFIS.egg-info/
+-rw-rw-rw-   0        0        0      434 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyFIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1113 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyFIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyFIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyFIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyFIS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/
+-rw-rw-rw-   0        0        0      724 2020-08-13 19:35:11.000000 pyFIS-1.9.0/pyfis/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/aegmis/
+-rw-rw-rw-   0        0        0      787 2022-01-26 20:54:05.000000 pyFIS-1.9.0/pyfis/aegmis/__init__.py
+-rw-rw-rw-   0        0        0    18437 2022-02-18 16:38:58.000000 pyFIS-1.9.0/pyfis/aegmis/ecs_lcd.py
+-rw-rw-rw-   0        0        0     4968 2022-01-02 18:31:43.000000 pyFIS-1.9.0/pyfis/aegmis/mis1_gcu.py
+-rw-rw-rw-   0        0        0     4506 2022-01-26 20:54:05.000000 pyFIS-1.9.0/pyfis/aegmis/mis2_gcu.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/ibis/
+-rw-rw-rw-   0        0        0      758 2020-08-13 19:34:23.000000 pyFIS-1.9.0/pyfis/ibis/__init__.py
+-rw-rw-rw-   0        0        0    23067 2020-08-13 19:34:43.000000 pyFIS-1.9.0/pyfis/ibis/ibis_protocol.py
+-rw-rw-rw-   0        0        0     2139 2021-12-13 21:53:45.000000 pyFIS-1.9.0/pyfis/ibis/ibis_serial.py
+-rw-rw-rw-   0        0        0     1832 2020-08-13 19:34:40.000000 pyFIS-1.9.0/pyfis/ibis/ibis_tcp.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/krone/
+-rw-rw-rw-   0        0        0      867 2022-02-18 16:38:58.000000 pyFIS-1.9.0/pyfis/krone/__init__.py
+-rw-rw-rw-   0        0        0      817 2020-09-12 18:19:48.000000 pyFIS-1.9.0/pyfis/krone/exceptions.py
+-rw-rw-rw-   0        0        0    11263 2022-02-15 19:27:39.000000 pyFIS-1.9.0/pyfis/krone/k8200.py
+-rw-rw-rw-   0        0        0     2506 2022-02-18 16:38:58.000000 pyFIS-1.9.0/pyfis/krone/k8200_pst.py
+-rw-rw-rw-   0        0        0    10001 2020-09-24 22:06:53.000000 pyFIS-1.9.0/pyfis/krone/k9000_fbk.py
+-rw-rw-rw-   0        0        0     5999 2021-12-13 21:53:45.000000 pyFIS-1.9.0/pyfis/krone/k9000_fbm.py
+-rw-rw-rw-   0        0        0     3195 2020-09-12 21:37:44.000000 pyFIS-1.9.0/pyfis/krone/k9000_hlst.py
+-rw-rw-rw-   0        0        0     6520 2020-09-24 21:59:33.000000 pyFIS-1.9.0/pyfis/krone/k9000_rs485.py
+-rw-rw-rw-   0        0        0     4790 2020-09-08 00:06:03.000000 pyFIS-1.9.0/pyfis/krone/util.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/lawo/
+-rw-rw-rw-   0        0        0      754 2021-01-24 00:36:19.000000 pyFIS-1.9.0/pyfis/lawo/__init__.py
+-rw-rw-rw-   0        0        0    11962 2021-01-24 16:12:28.000000 pyFIS-1.9.0/pyfis/lawo/lawo_font.py
+-rw-rw-rw-   0        0        0    12612 2020-12-13 11:52:07.000000 pyFIS-1.9.0/pyfis/lawo/mono_protocol.py
+-rw-rw-rw-   0        0        0     2063 2021-12-13 21:53:45.000000 pyFIS-1.9.0/pyfis/lawo/mono_serial.py
+-rw-rw-rw-   0        0        0     1088 2022-02-18 16:38:58.000000 pyFIS-1.9.0/pyfis/metadata.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/microsyst/
+-rw-rw-rw-   0        0        0      702 2020-11-16 18:31:48.000000 pyFIS-1.9.0/pyfis/microsyst/__init__.py
+-rw-rw-rw-   0        0        0    17375 2020-11-30 16:32:55.000000 pyFIS-1.9.0/pyfis/microsyst/migra.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/omega/
+-rw-rw-rw-   0        0        0      714 2020-08-13 19:38:43.000000 pyFIS-1.9.0/pyfis/omega/__init__.py
+-rw-rw-rw-   0        0        0     3682 2021-12-13 21:53:45.000000 pyFIS-1.9.0/pyfis/omega/rs485.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/splitflap_display/
+-rw-rw-rw-   0        0        0      820 2020-08-13 19:39:34.000000 pyFIS-1.9.0/pyfis/splitflap_display/__init__.py
+-rw-rw-rw-   0        0        0     7000 2020-08-13 19:39:26.000000 pyFIS-1.9.0/pyfis/splitflap_display/ascii_graphics.py
+-rw-rw-rw-   0        0        0    12609 2020-10-06 19:32:29.000000 pyFIS-1.9.0/pyfis/splitflap_display/display.py
+-rw-rw-rw-   0        0        0    11321 2020-10-06 19:40:16.000000 pyFIS-1.9.0/pyfis/splitflap_display/fields.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/utils/
+-rw-rw-rw-   0        0        0      693 2021-12-13 21:46:39.000000 pyFIS-1.9.0/pyfis/utils/__init__.py
+-rw-rw-rw-   0        0        0     5313 2022-02-15 19:27:39.000000 pyFIS-1.9.0/pyfis/utils/utils.py
+drwxrwxrwx   0        0        0        0 2022-02-18 16:39:03.000000 pyFIS-1.9.0/pyfis/xatlabs/
+-rw-rw-rw-   0        0        0      770 2021-12-13 21:46:39.000000 pyFIS-1.9.0/pyfis/xatlabs/__init__.py
+-rw-rw-rw-   0        0        0      721 2021-12-13 21:46:39.000000 pyFIS-1.9.0/pyfis/xatlabs/exceptions.py
+-rw-rw-rw-   0        0        0     6969 2021-12-13 21:53:45.000000 pyFIS-1.9.0/pyfis/xatlabs/rgb_dsa.py
+-rw-rw-rw-   0        0        0     3825 2021-12-13 21:53:45.000000 pyFIS-1.9.0/pyfis/xatlabs/splitflap.py
+-rw-rw-rw-   0        0        0       42 2022-02-18 16:39:03.000000 pyFIS-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      481 2020-08-13 19:23:08.000000 pyFIS-1.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyFIS-1.8.1/README.md` & `pyFIS-1.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,99 +1,100 @@
-# What's this?
-pyFIS allows you to control various kinds of passenger information systems.
-
-# Supported devices
-This library currently supports the following devices:
-
-* Bus and train displays
-  * IBIS devices
-    * All standard telegrams as well as some manufacturer-specific variants
-    * Connection via serial or TCP
-  * LAWO's MONO system (still quite rough)
-    * Support for sending bitmaps to some LED displays
-    * Support for XY10 flipdot pixel control
-* Split-Flap displays
-  * KRONE / MAN System 9000/8200E "FBM" split-flap modules with ZiLOG microcontroller (in combination with the "FBUE" address board)
-  * KRONE / MAN System 9000/8200E "FBK" split-flap group controller boards
-  * KRONE / MAN System 9000/8200E "HLST" heater and light control boards
-  * KRONE System 8200 (doesn't require any modifications, can send commands to the integrated display controller)
-  * OMEGA split-flap units with RS-485 data protocol
-* Other displays
-  * AEG MIS LCD signs:
-    * Character-based displays with a Geavision Control Unit (GCU) using the MIS1 or MIS2 protocols
-    * Graphical displays using the ECS protocol
-  * microSYST migra industrial LED signs using TCP/IP
-  * My own very basic and generic split-flap interface protocol (you can use this to interface with any split-flap type display)
-  * My own protocol for controlling a single-line scrolling RGB text display
-* Other features
-  * Support for reading LAWO's font file format
-
-# The `SplitFlapDisplay` class
-The `SplitFlapDisplay` class is an abstraction level you can use to represent a display made up of multiple split-flap modules. It functions as a wrapper for the various display controller classes. Using this class, you can create various fields such as a `TextField`, which represents of one or more alphanumerical split-flap modules, or a `CustomMapField`, which represents split-flap modules with texts or symbols printed on the flaps. Of course, the mapping of position code to displayed value can be set according to the modules you have.
-
-It can even render the display layout as ASCII graphics in your terminal! For more details, take a look at [the example script](/splitflap_display_example.py).
-
-![ASCII rendering of display output](/images/ascii_render.png?raw=true)
-![Another ASCII rendering of display output](/images/ascii_render2.png?raw=true)
-
-# Hardware description
-Probably most relevant is the pinout of the various devices.
-Here's a short, incomplete summary.
-
-## KRONE / MAN system with ZiLOG microcontrollers
-This system has a ZiLOG microcontroller on every split-flap unit and separate address boards, where the units are usually plugged in. This enables easy swapping of units without having to change the address, since the address boards would be permanently mounted in the display's backplane.
-
-The address is set with DIP switches and transferred to the split-flap unit using a shift register.
-
-The split-flap units have a 10-pin connector exposing the FBM single interface:
-
-![FBM pin numbering](/images/krone_fbm_pin_numbering.jpg?raw=true)
-
-| Pin | Function                                        |
-|-----|-------------------------------------------------|
-| 1   | GND                                             |
-| 2   | 42V AC (Live)                                   |
-| 3   | VCC (9...12V DC)                                |
-| 4   | 42V AC (Neutral)                                |
-| 5   | 5V DC output for address logic                  |
-| 6   | Address shift register data                     |
-| 7   | Address shift register clock                    |
-| 8   | Tx / Data from unit (CMOS logic levels)         |
-| 9   | Rx / Data to unit (CMOS logic levels)           |
-| 10  | Address shift register strobe                   |
-
-However, this alone is rather impractical. Controlling these units in combination with the address boards is much easier. The address boards have a 20-pin connector which exposes the FBM bus interface:
-
-| Pin      | Function                                 |
-|----------|------------------------------------------|
-| 1...6    | 42V AC (Live)                            |
-| 7...12   | 42V AC (Neutral)                         |
-| 13,14,15  | VCC (9...12V DC)                        |
-| 16,18,20 | GND                                      |
-| 17       | Rx / Data to units (CMOS logic levels)   |
-| 19       | Tx / Data from units (CMOS logic levels) |
-
-If you don't have the address boards, you can order the remade version I created together with [Phalos Southpaw](http://www.phalos-werkstatt.de/), which is available [here](https://github.com/Mezgrman/Krone-FBUE)!
-
-# Reference photos
-In case you're not sure what kind of display you have, here are some pictures:
-
-![KRONE / MAN split-flap unit](/images/krone_zilog.jpg?raw=true)
-
-KRONE / MAN split-flap unit with ZiLOG microcontroller. There is also a variant with a THT microcontroller, which is also compatible.
-
-![FBUE address board](/images/krone_fbue.jpg?raw=true)
-
-KRONE / MAN "FBUE" address board for "FBM" split-flap units
-
-![KRONE / MAN FBK board](/images/krone_fbk.jpg?raw=true)
-
-KRONE / MAN "FBK" board for controlling groups of FBM+FBUE split-flap units
-
-![OMEGA split-flap unit](/images/omega_unit.jpg?raw=true)
-
-OMEGA split-flap unit with RS-485 and DC input, commonly found in SBB (Swiss train operator) displays
-
-
-
-# Installation
+# What's this?
+pyFIS allows you to control various kinds of passenger information systems.
+
+# Supported devices
+This library currently supports the following devices:
+
+* Bus and train displays
+  * IBIS devices
+    * All standard telegrams as well as some manufacturer-specific variants
+    * Connection via serial or TCP
+  * LAWO's MONO system (still quite rough)
+    * Support for sending bitmaps to some LED displays
+    * Support for XY10 flipdot pixel control
+* Split-Flap displays
+  * KRONE / MAN System 9000/8200E "FBM" split-flap modules with ZiLOG microcontroller (in combination with the "FBUE" address board)
+  * KRONE / MAN System 9000/8200E "FBK" split-flap group controller boards
+  * KRONE / MAN System 9000/8200E "HLST" heater and light control boards
+  * KRONE System 8200 (doesn't require any modifications, can send commands to the integrated display controller)
+  * KRONE System 8200 PST boards (the piggyback boards on each split-flap module)
+  * OMEGA split-flap units with RS-485 data protocol
+* Other displays
+  * AEG MIS LCD signs:
+    * Character-based displays with a Geavision Control Unit (GCU) using the MIS1 or MIS2 protocols
+    * Graphical displays using the ECS protocol
+  * microSYST migra industrial LED signs using TCP/IP
+  * My own very basic and generic split-flap interface protocol (you can use this to interface with any split-flap type display)
+  * My own protocol for controlling a single-line scrolling RGB text display
+* Other features
+  * Support for reading LAWO's font file format
+
+# The `SplitFlapDisplay` class
+The `SplitFlapDisplay` class is an abstraction level you can use to represent a display made up of multiple split-flap modules. It functions as a wrapper for the various display controller classes. Using this class, you can create various fields such as a `TextField`, which represents of one or more alphanumerical split-flap modules, or a `CustomMapField`, which represents split-flap modules with texts or symbols printed on the flaps. Of course, the mapping of position code to displayed value can be set according to the modules you have.
+
+It can even render the display layout as ASCII graphics in your terminal! For more details, take a look at [the example script](/splitflap_display_example.py).
+
+![ASCII rendering of display output](/images/ascii_render.png?raw=true)
+![Another ASCII rendering of display output](/images/ascii_render2.png?raw=true)
+
+# Hardware description
+Probably most relevant is the pinout of the various devices.
+Here's a short, incomplete summary.
+
+## KRONE / MAN system with ZiLOG microcontrollers
+This system has a ZiLOG microcontroller on every split-flap unit and separate address boards, where the units are usually plugged in. This enables easy swapping of units without having to change the address, since the address boards would be permanently mounted in the display's backplane.
+
+The address is set with DIP switches and transferred to the split-flap unit using a shift register.
+
+The split-flap units have a 10-pin connector exposing the FBM single interface:
+
+![FBM pin numbering](/images/krone_fbm_pin_numbering.jpg?raw=true)
+
+| Pin | Function                                        |
+|-----|-------------------------------------------------|
+| 1   | GND                                             |
+| 2   | 42V AC (Live)                                   |
+| 3   | VCC (9...12V DC)                                |
+| 4   | 42V AC (Neutral)                                |
+| 5   | 5V DC output for address logic                  |
+| 6   | Address shift register data                     |
+| 7   | Address shift register clock                    |
+| 8   | Tx / Data from unit (CMOS logic levels)         |
+| 9   | Rx / Data to unit (CMOS logic levels)           |
+| 10  | Address shift register strobe                   |
+
+However, this alone is rather impractical. Controlling these units in combination with the address boards is much easier. The address boards have a 20-pin connector which exposes the FBM bus interface:
+
+| Pin      | Function                                 |
+|----------|------------------------------------------|
+| 1...6    | 42V AC (Live)                            |
+| 7...12   | 42V AC (Neutral)                         |
+| 13,14,15  | VCC (9...12V DC)                        |
+| 16,18,20 | GND                                      |
+| 17       | Rx / Data to units (CMOS logic levels)   |
+| 19       | Tx / Data from units (CMOS logic levels) |
+
+If you don't have the address boards, you can order the remade version I created together with [Phalos Southpaw](http://www.phalos-werkstatt.de/), which is available [here](https://github.com/Mezgrman/Krone-FBUE)!
+
+# Reference photos
+In case you're not sure what kind of display you have, here are some pictures:
+
+![KRONE / MAN split-flap unit](/images/krone_zilog.jpg?raw=true)
+
+KRONE / MAN split-flap unit with ZiLOG microcontroller. There is also a variant with a THT microcontroller, which is also compatible.
+
+![FBUE address board](/images/krone_fbue.jpg?raw=true)
+
+KRONE / MAN "FBUE" address board for "FBM" split-flap units
+
+![KRONE / MAN FBK board](/images/krone_fbk.jpg?raw=true)
+
+KRONE / MAN "FBK" board for controlling groups of FBM+FBUE split-flap units
+
+![OMEGA split-flap unit](/images/omega_unit.jpg?raw=true)
+
+OMEGA split-flap unit with RS-485 and DC input, commonly found in SBB (Swiss train operator) displays
+
+
+
+# Installation
 `pip install pyfis`
```

### Comparing `pyFIS-1.8.1/pyFIS.egg-info/SOURCES.txt` & `pyFIS-1.9.0/pyFIS.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 pyFIS.egg-info/PKG-INFO
 pyFIS.egg-info/SOURCES.txt
 pyFIS.egg-info/dependency_links.txt
 pyFIS.egg-info/requires.txt
 pyFIS.egg-info/top_level.txt
@@ -15,14 +14,15 @@
 pyfis/ibis/__init__.py
 pyfis/ibis/ibis_protocol.py
 pyfis/ibis/ibis_serial.py
 pyfis/ibis/ibis_tcp.py
 pyfis/krone/__init__.py
 pyfis/krone/exceptions.py
 pyfis/krone/k8200.py
+pyfis/krone/k8200_pst.py
 pyfis/krone/k9000_fbk.py
 pyfis/krone/k9000_fbm.py
 pyfis/krone/k9000_hlst.py
 pyfis/krone/k9000_rs485.py
 pyfis/krone/util.py
 pyfis/lawo/__init__.py
 pyfis/lawo/lawo_font.py
```

### Comparing `pyFIS-1.8.1/pyfis/__init__.py` & `pyFIS-1.9.0/pyfis/microsyst/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-Copyright (C) 2016 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .metadata import version as __version__
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .migra import MigraTCP
```

### Comparing `pyFIS-1.8.1/pyfis/aegmis/__init__.py` & `pyFIS-1.9.0/pyfis/xatlabs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-"""
-Copyright (C) 2020-2022 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .ecs_lcd import ECSLCDisplay
-from .mis1_gcu import MIS1GCUDisplay
-from .mis2_gcu import MIS2GCUDisplay
+"""
+Copyright (C) 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .splitflap import xatLabsSplitFlapController
+from .rgb_dsa import xatLabsRGBDSAController
```

### Comparing `pyFIS-1.8.1/pyfis/aegmis/ecs_lcd.py` & `pyFIS-1.9.0/pyfis/aegmis/ecs_lcd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,524 +1,524 @@
-"""
-Copyright (C) 2022 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import datetime
-import socket
-import time
-
-from io import BytesIO
-from PIL import Image
-
-
-class ECSLCDisplay:
-    """
-    ERROR / STATUS CODES
-    """
-
-    CMD_STATUS_DICT = {
-        -1: "ERR_NO_RESPONSE",
-        0:  "ECS_LCD_OK",
-        1:  "ECS_LCD_EFONTSIZE",
-        2:  "ECS_LCD_CLIPPED",
-        3:  "ECS_LCD_ENOTFOUND",
-        4:  "ECS_LCD_EDEVICECMD",
-        5:  "ECS_LCD_ECHAR_ATTRIBUTE",
-        6:  "ECS_LCD_EINIT_DISPLAY",
-        7:  "ECS_LCD_EINIT_SECTOR",
-        8:  "ECS_LCD_ERANGE",
-        9:  "ECS_LCD_EOPTION_CONVERT",
-        10: "ECS_LCD_EOPTION_LEN",
-        11: "ECS_LCD_EOPTION",
-        12: "ECS_LCD_EMISOPTION",
-        13: "ECS_LCD_EHWDISPLAY",
-        14: "ECS_LCD_DISPLAY",
-        15: "ECS_LCD_ESECTOR",
-        16: "ECS_LCD_EPAGE",
-        17: "ECS_LCD_EPAGE_SEQ",
-        18: "ECS_LCD_ECOMMUNICATION",
-        19: "ECS_LCD_EBITMAP",
-        20: "ECS_LCD_ELINE",
-        21: "ECS_LCD_ESYNTAX",
-        22: "ECS_LCD_EDELTEXT",
-        23: "ECS_LCD_ENOPAGEACT",
-        24: "ECS_LCD_ESECTORNR",
-        25: "ECS_LCD_EPAGENR",
-        26: "ECS_LCD_ESECX",
-        27: "ECS_LCD_ESECY",
-        28: "ECS_LCD_EFONT_MISS",
-        29: "ECS_LCD_ESECLIN",
-        30: "ECS_LCD_ENOSECACT",
-        31: "ECS_LCD_EFEWPARS",
-        32: "ECS_LCD_EOPTION1",
-        33: "ECS_LCD_EOPTION2",
-        34: "ECS_LCD_EOPTION3",
-        35: "ECS_LCD_EOPTION4",
-        36: "ECS_LCD_EFONTNR",
-        37: "ECS_LCD_EFONTMISS",
-        38: "ECS_LCD_ESECTTYPE",
-        39: "ECS_LCD_EMUCHPARS",
-        40: "ECS_LCD_EDEC_MISS",
-        41: "ECS_LCD_COMMAND",
-        42: "ECS_LCD_ENOEND",
-        43: "ECS_LCD_EPREFIX",
-        44: "ECS_LCD_EPOSTFIX",
-        45: "ECS_LCD_EALIGN",
-        46: "ECS_LCD_EATTRIB",
-        47: "ECS_LCD_ECOLOR",
-        48: "ECS_LCD_ESAMECOLORS",
-        49: "ECS_LCD_ENOSPACE",
-        50: "ECS_LCD_ENOANZPAGE",
-        51: "ECS_LCD_EOUTOFRANGE",
-        52: "ECS_LCD_ENOPAGENOTIME",
-        53: "ECS_LCD_ECASE",
-        54: "ECS_LCD_EONOFF",
-        55: "ECS_LCD_EBIT",
-        56: "ECS_LCD_EVALUE",
-        57: "ECS_LCD_EALLOC",
-        58: "ECS_LCD_EFILE",
-        59: "ECS_LCD_EADRDOUBLE",
-        60: "ECS_LCD_EGMFC",
-        61: "ECS_LCD_EBLOCK",
-        62: "ECS_LCD_EFONT",
-        63: "ECS_LCD_EGLASTAB",
-        64: "ECS_LCD_EHWNOTSUPPORTED",
-        254: "ECS_LCD_ECONFIG",
-        255: "ECS_LCD_EGENERAL"
-    }
-
-    OP_STATUS_DICT = {
-        0: "OP_STAT_READY",
-        1: "OP_STAT_LAMP_FAULT",
-        2: "OP_STAT_LCD_FAULT",
-        3: "OP_STAT_LAMP_LCD_FAULT"
-    }
-
-
-    def __init__(self, host, port=7487, timeout=10.0, double_sided=True, debug=False):
-        self.host = host
-        self.port = port
-        self.timeout = timeout
-        self.double_sided = double_sided
-        self.debug = debug
-        self.socket = None
-        self.socket_rfile = None
-        self.socket_wfile = None
-        socket.setdefaulttimeout(timeout)
-        self._init_socket()
-        device_cfg = self.get_device_cfg()
-        self.width = device_cfg['xPixel']
-        if self.double_sided:
-            # Double-sided displays have the back side mapped below the front side
-            self.height = device_cfg['yPixel'] // 2
-        else:
-            self.height = device_cfg['yPixel']
-
-
-    """
-    SOCKET I/O
-    """
-
-    def _init_socket(self):
-        if self.socket is not None:
-            try:
-                self.socket.close()
-            except:
-                pass
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket.connect((self.host, self.port))
-        self.socket_rfile = self.socket.makefile('r')
-        self.socket_wfile = self.socket.makefile('w')
-
-    def write(self, data):
-        self.socket_wfile.write(data)
-        self.socket_wfile.flush()
-
-    def read_response(self):
-        try:
-            response = self.socket_rfile.readline()
-            if self.debug:
-                print("Received response: " + response.strip())
-            return response
-        except (socket.timeout, OSError):
-            self._init_socket()
-            return None
-
-    def parse_response(self):
-        response = self.read_response()
-        if response is None:
-            return {'status': -1, 'status_text': self.CMD_STATUS_DICT.get(-1, "UNKNOWN")}
-
-        # Stupid bug, some replies have a space before the equals sign
-        response = response.replace(" =", "=")
-
-        parts = response.split()
-        command = parts[0][:-1] # -1 to remove the trailing colon
-
-        resp_dict = {}
-        for part in parts[1:]:
-            subparts = part.split("=")
-            resp_dict[subparts[0]] = "=".join(subparts[1:])
-
-        for int_key in ('status', 'operative', 'xPixel', 'yPixel'):
-            if int_key in resp_dict:
-                resp_dict[int_key] = int(resp_dict[int_key])
-
-        if 'status' in resp_dict:
-            resp_dict['status_text'] = self.CMD_STATUS_DICT.get(resp_dict['status'], "UNKNOWN")
-        if 'operative' in resp_dict:
-            resp_dict['operative_text'] = self.OP_STATUS_DICT.get(resp_dict['operative'], "UNKNOWN")
-
-        if command == "ECS_LCD_GetTime":
-            if 'time' in resp_dict:
-                resp_dict['time'] = datetime.datetime.strptime(resp_dict['time'], "%H:%M:%S").time()
-            if 'date' in resp_dict:
-                resp_dict['date'] = datetime.datetime.strptime(resp_dict['date'], "%Y-%m-%d").date()
-            if 'time' in resp_dict and 'date' in resp_dict:
-                resp_dict['datetime'] = datetime.datetime.combine(resp_dict['date'], resp_dict['time'])
-        elif command == "ECS_LCD_GetResetTime":
-            if 'time' in resp_dict:
-                resp_dict['time'] = int(resp_dict['time'])
-
-        return resp_dict
-
-    def send_command(self, command, *args, **kwargs):
-        kwargs_list = []
-        for key, value in kwargs.items():
-            if value is None:
-                continue
-
-            if type(value) in (tuple, list):
-                value_str = " ".join(map(str, value))
-            elif type(value) in (bytes, bytearray):
-                value_str = " ".join(["{:02X}".format(b) for b in value])
-            else:
-                value_str = str(value)
-            kwargs_list.append("-" + key + " " + value_str)
-
-        args_str = " ".join(map(str, args))
-        kwargs_str = " ".join(kwargs_list)
-        command_str = command.strip()
-        if args_str:
-            command_str += " " + args_str
-        if kwargs_str:
-            command_str += " " + kwargs_str
-        command_str = command_str.strip() + "\r\n"
-        if self.debug:
-            print("Sending command:   " + command_str.strip())
-        self.write(command_str)
-        return self.parse_response()
-
-
-    """
-    COMMANDS
-    """
-
-    def define_normal_page(self, page):
-        """
-        Sets up a normal page with the given page ID.
-        Normal pages are exactly the same size as the display.
-        
-        page: page ID, 0...255
-        """
-        return self.send_command("ECS_LCD_DefineNormalPage", page=page)
-
-    def define_virtual_page(self, page, cols, rows):
-        """
-        Sets up a virtual page with the given page ID.
-        Virtual pages can be larger than the display size and support
-        vertical scrolling of rows.
-        
-        page: page ID, 0...255
-        cols: Page width in columns
-        rows: Page height in rows
-        """
-        return self.send_command("ECS_LCD_DefineVirtualPage", page=page, size=(cols, rows))
-
-    def delete_page(self, page):
-        """
-        Deletes the page with the given ID.
-        
-        page: page ID, 0...255
-        """
-        return self.send_command("ECS_LCD_DeletePage", page=page)
-
-    def select_page(self, page):
-        """
-        Selects the page with the given ID for editing.
-        
-        page: page ID, 0...255
-        """
-        return self.send_command("ECS_LCD_SelectPage", page=page)
-
-    def change_sector(self, sector, col, row, cols, rows, type, font=None, lines=None, bg_color=None):
-        """
-        Updates the currently selected sector on the currently
-        selected page with the given configuration.
-        
-        sector: sector ID, 0...255
-        col: sector origin column, 0...65024
-        row: sector origin row, 0...65024
-        cols: sector width in columns, 0...65024
-        rows: sector height in rows, 0...65024 (for virtual pages, only height 1 is valid)
-        type: sector type, text or graphic
-        font: font ID, 0...255 (only for sector type text)
-        lines: number of lines of text in the sector, 0...255 (only for sector type text)
-        bg_color: background color of the sector, 3-tuple, (0, 0, 0)...(255, 255, 255) (only for displays with RGB backlight)
-        """
-        return self.send_command("ECS_LCD_ChangeSector", sector=(sector, col, row, cols, rows), sectortype=type, font=font, lines=lines, bkcolor=bg_color)
-
-    def select_sector(self, sector):
-        """
-        Selects the sector with the given ID on the currently selected page for editing.
-        
-        sector: sector ID, 0...255
-        """
-        return self.send_command("ECS_LCD_SelectSector", sector=sector)
-
-    def chr_out_text(self, row, text, align, attribute, textcode=None):
-        """
-        Outputs text in the currently selected sector on the currently selected page.
-        
-        row: line index inside the current sector, 0...255
-        text: text to output
-        align: text alignment (left, center, right, flow) (flow: scroll text if it doesn't fit into the sector)
-        attribute: text display attribute (normal, blink, compblink, invers) (compblink: inverted and blinking)
-        textcode: index of pre-defined text for split-flap style control, 0...65535
-        """
-        text = "\"" + text.replace("\"", "") + "\""
-        return self.send_command("ECS_LCD_ChrOutText", row, text=text, align=align, textcode=textcode, attribute=attribute)
-
-    def put_image(self, col, row, image, filename=None):
-        """
-        Outputs the given image in the currently selected sector on the currently selected page.
-        
-        col: X position of the image in columns, 0...65024
-        row: Y position of the image in rows, 0...65024
-        image: image to output (path to image file, PIL Image object, or raw BMP image data)
-        filename: filename to save the image as on the display (max. 31 characters)
-        """
-        if isinstance(image, Image.Image):
-            bio = BytesIO()
-            image.convert('1')
-            image.save(bio, 'BMP')
-            bio.seek(0)
-            img_data = bio.read()
-        elif type(image) is str:
-            bio = BytesIO()
-            image = Image.open(image)
-            image.convert('1')
-            image.save(bio, 'BMP')
-            bio.seek(0)
-            img_data = bio.read()
-        else:
-            img_data = image
-        return self.send_command("ECS_LCD_PutImage", col, row, imagefilename=filename, image=img_data)
-
-    def insert_line(self, line):
-        """
-        Inserts a line of text into the currently selected sector,
-        below the line with the specified index.
-        The remaining lines will be shifted downwards.
-        
-        line: line ID, 0...255
-        """
-        return self.send_command("ECS_LCD_InsertLine", line=line)
-
-    def delete_line(self, line):
-        """
-        Deletes a line of text from the currently selected sector.
-        The remaining lines will be shifted upwards.
-        
-        line: line ID, 0...255
-        """
-        return self.send_command("ECS_LCD_DeleteLine", line=line)
-
-    def chr_clr_txt(self, line):
-        """
-        CLears a line of text in the currently selected sector.
-        
-        line: line ID, 0...255
-        """
-        return self.send_command("ECS_LCD_ChrClrTxt", line)
-
-    def clr_sector(self):
-        """
-        Deletes the contents of the currently selected sector.
-        """
-        return self.send_command("ECS_LCD_ClrSector")
-
-    def clr_page(self):
-        """
-        Deletes the contents of the currently selected page.
-        """
-        return self.send_command("ECS_LCD_ClrPage")
-
-    def show_page(self, page):
-        """
-        Displays the page with the given ID on the display.
-        
-        page: page ID, 0...255
-        """
-        return self.send_command("ECS_LCD_ShowPage", page=page)
-
-    def prog_page_sequence(self, page, duration):
-        """
-        Appends an entry to the current list of pages to show.
-        Each entry comprises the page ID to be shown and a duration.
-        
-        page: page ID, 0...255
-        duration: duration is milliseconds, 0...65024
-        """
-        return self.send_command("ECS_LCD_ProgPageSequence", page=page, time=duration)
-
-    def activate_page_sequence(self):
-        """
-        Activates the previously programmed page seqneuce.
-        """
-        return self.send_command("ECS_LCD_ActivatePageSequence")
-
-    def scroll_page(self, mode, lines=None, pause=None):
-        """
-        Scrolls the display contents up by the given amount of lines of text
-        with the given pause between lines.
-        
-        mode: scroll mode (off, line, cont)
-                off:  disable scrolling
-                line: scroll row by row
-                cont: scroll pixel by pixel
-        lines: the number of lines to scroll, 0...255
-        pause: the pause between lines in seconds, 0...255
-        """
-        return self.send_command("ECS_LCD_ScrollPage", scroll=mode, lines=lines, pausetime=pause)
-
-    def switch_background_light(self, state):
-        """
-        Turns the background light on or off.
-        
-        state: light state (on, off)
-        """
-        if type(state) in (bool, int):
-            state = 'on' if state else 'off'
-        return self.send_command("ECS_LCD_SwitchBackgroundLight", light=state)
-
-    def get_operative_status(self):
-        """
-        Get the operative status of the display.
-        """
-        return self.send_command("ECS_LCD_GetOperativeStatus")
-
-    def get_reset_time(self):
-        """
-        Get the number of seconds since the last reset.
-        """
-        return self.send_command("ECS_LCD_GetResetTime")
-
-    def get_time(self):
-        """
-        Get the system time.
-        """
-        return self.send_command("ECS_LCD_GetTime")
-
-    def get_software_version(self):
-        """
-        Get the software version.
-        """
-        return self.send_command("ECS_LCD_GetSoftwareVersion")
-
-    def get_device_cfg(self):
-        """
-        Get the device configuration.
-        """
-        return self.send_command("ECS_LCD_GetDeviceCfg")
-
-    def get_page_content(self, page):
-        """
-        Get the contents of the specified page.
-
-        page: page ID, 0...255
-        """
-        return self.send_command("ECS_LCD_GetPageContent", page=page)
-
-
-    """
-    CONVENIENCE FUNCTIONS
-    """
-
-    def display_text(self, page, text, font, align='center', attribute='normal'):
-        """
-        Displays a text on the given page.
-
-        page: page ID, 0...255
-        text: the text to display
-        font: font ID, 0...255
-        align: text alignment (left, center, right, flow)
-        attribute: text display attribute (normal, blink, compblink, invers) (compblink: inverted and blinking)
-        """
-        lines = text.splitlines()
-        self.define_normal_page(page)
-        self.select_page(page)
-        self.change_sector(0, 0, 0, self.width, self.height, 'text', font, lines=len(lines))
-        self.select_sector(0)
-        for i, row in enumerate(lines):
-            self.chr_out_text(i, row, align, attribute)
-
-        if self.double_sided:
-            self.change_sector(1, 0, self.height, self.width, self.height, 'text', font, lines=len(lines))
-            self.select_sector(1)
-            for i, row in enumerate(lines):
-                self.chr_out_text(i, row, align, attribute)
-        
-        self.show_page(page)
-
-    def display_image(self, page, image, halign='center', valign='middle'):
-        """
-        Displays an image on the given page.
-
-        page: page ID, 0...255
-        image: the image to display (PIL Image object or path to image)
-        halign: horizontal image alignment (left, center, right)
-        valign: vertical image alignment (top, middle, bottom)
-        """
-        if not isinstance(image, Image.Image):
-            image = Image.open(image)
-        width, height = image.size
-
-        if halign == 'center':
-            x = (self.width - width) // 2
-        elif halign == 'right':
-            x = self.width - width
-        else:
-            x = 0
-
-        if valign == 'middle':
-            y = (self.height - height) // 2
-        elif valign == 'bottom':
-            y = self.height - height
-        else:
-            y = 0
-
-        self.define_normal_page(page)
-        self.select_page(page)
-        self.change_sector(0, 0, 0, self.width, self.height, 'graphic')
-        self.select_sector(0)
-        self.put_image(x, y, image)
-
-        if self.double_sided:
-            self.change_sector(1, 0, self.height, self.width, self.height, 'graphic')
-            self.select_sector(1)
-            self.put_image(x, y, image)
-        
+"""
+Copyright (C) 2022 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import datetime
+import socket
+import time
+
+from io import BytesIO
+from PIL import Image
+
+
+class ECSLCDisplay:
+    """
+    ERROR / STATUS CODES
+    """
+
+    CMD_STATUS_DICT = {
+        -1: "ERR_NO_RESPONSE",
+        0:  "ECS_LCD_OK",
+        1:  "ECS_LCD_EFONTSIZE",
+        2:  "ECS_LCD_CLIPPED",
+        3:  "ECS_LCD_ENOTFOUND",
+        4:  "ECS_LCD_EDEVICECMD",
+        5:  "ECS_LCD_ECHAR_ATTRIBUTE",
+        6:  "ECS_LCD_EINIT_DISPLAY",
+        7:  "ECS_LCD_EINIT_SECTOR",
+        8:  "ECS_LCD_ERANGE",
+        9:  "ECS_LCD_EOPTION_CONVERT",
+        10: "ECS_LCD_EOPTION_LEN",
+        11: "ECS_LCD_EOPTION",
+        12: "ECS_LCD_EMISOPTION",
+        13: "ECS_LCD_EHWDISPLAY",
+        14: "ECS_LCD_DISPLAY",
+        15: "ECS_LCD_ESECTOR",
+        16: "ECS_LCD_EPAGE",
+        17: "ECS_LCD_EPAGE_SEQ",
+        18: "ECS_LCD_ECOMMUNICATION",
+        19: "ECS_LCD_EBITMAP",
+        20: "ECS_LCD_ELINE",
+        21: "ECS_LCD_ESYNTAX",
+        22: "ECS_LCD_EDELTEXT",
+        23: "ECS_LCD_ENOPAGEACT",
+        24: "ECS_LCD_ESECTORNR",
+        25: "ECS_LCD_EPAGENR",
+        26: "ECS_LCD_ESECX",
+        27: "ECS_LCD_ESECY",
+        28: "ECS_LCD_EFONT_MISS",
+        29: "ECS_LCD_ESECLIN",
+        30: "ECS_LCD_ENOSECACT",
+        31: "ECS_LCD_EFEWPARS",
+        32: "ECS_LCD_EOPTION1",
+        33: "ECS_LCD_EOPTION2",
+        34: "ECS_LCD_EOPTION3",
+        35: "ECS_LCD_EOPTION4",
+        36: "ECS_LCD_EFONTNR",
+        37: "ECS_LCD_EFONTMISS",
+        38: "ECS_LCD_ESECTTYPE",
+        39: "ECS_LCD_EMUCHPARS",
+        40: "ECS_LCD_EDEC_MISS",
+        41: "ECS_LCD_COMMAND",
+        42: "ECS_LCD_ENOEND",
+        43: "ECS_LCD_EPREFIX",
+        44: "ECS_LCD_EPOSTFIX",
+        45: "ECS_LCD_EALIGN",
+        46: "ECS_LCD_EATTRIB",
+        47: "ECS_LCD_ECOLOR",
+        48: "ECS_LCD_ESAMECOLORS",
+        49: "ECS_LCD_ENOSPACE",
+        50: "ECS_LCD_ENOANZPAGE",
+        51: "ECS_LCD_EOUTOFRANGE",
+        52: "ECS_LCD_ENOPAGENOTIME",
+        53: "ECS_LCD_ECASE",
+        54: "ECS_LCD_EONOFF",
+        55: "ECS_LCD_EBIT",
+        56: "ECS_LCD_EVALUE",
+        57: "ECS_LCD_EALLOC",
+        58: "ECS_LCD_EFILE",
+        59: "ECS_LCD_EADRDOUBLE",
+        60: "ECS_LCD_EGMFC",
+        61: "ECS_LCD_EBLOCK",
+        62: "ECS_LCD_EFONT",
+        63: "ECS_LCD_EGLASTAB",
+        64: "ECS_LCD_EHWNOTSUPPORTED",
+        254: "ECS_LCD_ECONFIG",
+        255: "ECS_LCD_EGENERAL"
+    }
+
+    OP_STATUS_DICT = {
+        0: "OP_STAT_READY",
+        1: "OP_STAT_LAMP_FAULT",
+        2: "OP_STAT_LCD_FAULT",
+        3: "OP_STAT_LAMP_LCD_FAULT"
+    }
+
+
+    def __init__(self, host, port=7487, timeout=10.0, double_sided=True, debug=False):
+        self.host = host
+        self.port = port
+        self.timeout = timeout
+        self.double_sided = double_sided
+        self.debug = debug
+        self.socket = None
+        self.socket_rfile = None
+        self.socket_wfile = None
+        socket.setdefaulttimeout(timeout)
+        self._init_socket()
+        device_cfg = self.get_device_cfg()
+        self.width = device_cfg['xPixel']
+        if self.double_sided:
+            # Double-sided displays have the back side mapped below the front side
+            self.height = device_cfg['yPixel'] // 2
+        else:
+            self.height = device_cfg['yPixel']
+
+
+    """
+    SOCKET I/O
+    """
+
+    def _init_socket(self):
+        if self.socket is not None:
+            try:
+                self.socket.close()
+            except:
+                pass
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.socket.connect((self.host, self.port))
+        self.socket_rfile = self.socket.makefile('r', encoding='latin-1')
+        self.socket_wfile = self.socket.makefile('w', encoding='latin-1')
+
+    def write(self, data):
+        self.socket_wfile.write(data)
+        self.socket_wfile.flush()
+
+    def read_response(self):
+        try:
+            response = self.socket_rfile.readline()
+            if self.debug:
+                print("Received response: " + response.strip())
+            return response
+        except (socket.timeout, OSError):
+            self._init_socket()
+            return None
+
+    def parse_response(self):
+        response = self.read_response()
+        if response is None:
+            return {'status': -1, 'status_text': self.CMD_STATUS_DICT.get(-1, "UNKNOWN")}
+
+        # Stupid bug, some replies have a space before the equals sign
+        response = response.replace(" =", "=")
+
+        parts = response.split()
+        command = parts[0][:-1] # -1 to remove the trailing colon
+
+        resp_dict = {}
+        for part in parts[1:]:
+            subparts = part.split("=")
+            resp_dict[subparts[0]] = "=".join(subparts[1:])
+
+        for int_key in ('status', 'operative', 'xPixel', 'yPixel'):
+            if int_key in resp_dict:
+                resp_dict[int_key] = int(resp_dict[int_key])
+
+        if 'status' in resp_dict:
+            resp_dict['status_text'] = self.CMD_STATUS_DICT.get(resp_dict['status'], "UNKNOWN")
+        if 'operative' in resp_dict:
+            resp_dict['operative_text'] = self.OP_STATUS_DICT.get(resp_dict['operative'], "UNKNOWN")
+
+        if command == "ECS_LCD_GetTime":
+            if 'time' in resp_dict:
+                resp_dict['time'] = datetime.datetime.strptime(resp_dict['time'], "%H:%M:%S").time()
+            if 'date' in resp_dict:
+                resp_dict['date'] = datetime.datetime.strptime(resp_dict['date'], "%Y-%m-%d").date()
+            if 'time' in resp_dict and 'date' in resp_dict:
+                resp_dict['datetime'] = datetime.datetime.combine(resp_dict['date'], resp_dict['time'])
+        elif command == "ECS_LCD_GetResetTime":
+            if 'time' in resp_dict:
+                resp_dict['time'] = int(resp_dict['time'])
+
+        return resp_dict
+
+    def send_command(self, command, *args, **kwargs):
+        kwargs_list = []
+        for key, value in kwargs.items():
+            if value is None:
+                continue
+
+            if type(value) in (tuple, list):
+                value_str = " ".join(map(str, value))
+            elif type(value) in (bytes, bytearray):
+                value_str = " ".join(["{:02X}".format(b) for b in value])
+            else:
+                value_str = str(value)
+            kwargs_list.append("-" + key + " " + value_str)
+
+        args_str = " ".join(map(str, args))
+        kwargs_str = " ".join(kwargs_list)
+        command_str = command.strip()
+        if args_str:
+            command_str += " " + args_str
+        if kwargs_str:
+            command_str += " " + kwargs_str
+        command_str = command_str.strip() + "\r\n"
+        if self.debug:
+            print("Sending command:   " + command_str.strip())
+        self.write(command_str)
+        return self.parse_response()
+
+
+    """
+    COMMANDS
+    """
+
+    def define_normal_page(self, page):
+        """
+        Sets up a normal page with the given page ID.
+        Normal pages are exactly the same size as the display.
+        
+        page: page ID, 0...255
+        """
+        return self.send_command("ECS_LCD_DefineNormalPage", page=page)
+
+    def define_virtual_page(self, page, cols, rows):
+        """
+        Sets up a virtual page with the given page ID.
+        Virtual pages can be larger than the display size and support
+        vertical scrolling of rows.
+        
+        page: page ID, 0...255
+        cols: Page width in columns
+        rows: Page height in rows
+        """
+        return self.send_command("ECS_LCD_DefineVirtualPage", page=page, size=(cols, rows))
+
+    def delete_page(self, page):
+        """
+        Deletes the page with the given ID.
+        
+        page: page ID, 0...255
+        """
+        return self.send_command("ECS_LCD_DeletePage", page=page)
+
+    def select_page(self, page):
+        """
+        Selects the page with the given ID for editing.
+        
+        page: page ID, 0...255
+        """
+        return self.send_command("ECS_LCD_SelectPage", page=page)
+
+    def change_sector(self, sector, col, row, cols, rows, type, font=None, lines=None, bg_color=None):
+        """
+        Updates the currently selected sector on the currently
+        selected page with the given configuration.
+        
+        sector: sector ID, 0...255
+        col: sector origin column, 0...65024
+        row: sector origin row, 0...65024
+        cols: sector width in columns, 0...65024
+        rows: sector height in rows, 0...65024 (for virtual pages, only height 1 is valid)
+        type: sector type, text or graphic
+        font: font ID, 0...255 (only for sector type text)
+        lines: number of lines of text in the sector, 0...255 (only for sector type text)
+        bg_color: background color of the sector, 3-tuple, (0, 0, 0)...(255, 255, 255) (only for displays with RGB backlight)
+        """
+        return self.send_command("ECS_LCD_ChangeSector", sector=(sector, col, row, cols, rows), sectortype=type, font=font, lines=lines, bkcolor=bg_color)
+
+    def select_sector(self, sector):
+        """
+        Selects the sector with the given ID on the currently selected page for editing.
+        
+        sector: sector ID, 0...255
+        """
+        return self.send_command("ECS_LCD_SelectSector", sector=sector)
+
+    def chr_out_text(self, row, text, align, attribute, textcode=None):
+        """
+        Outputs text in the currently selected sector on the currently selected page.
+        
+        row: line index inside the current sector, 0...255
+        text: text to output
+        align: text alignment (left, center, right, flow) (flow: scroll text if it doesn't fit into the sector)
+        attribute: text display attribute (normal, blink, compblink, invers) (compblink: inverted and blinking)
+        textcode: index of pre-defined text for split-flap style control, 0...65535
+        """
+        text = "\"" + text.replace("\"", "") + "\""
+        return self.send_command("ECS_LCD_ChrOutText", row, text=text, align=align, textcode=textcode, attribute=attribute)
+
+    def put_image(self, col, row, image, filename=None):
+        """
+        Outputs the given image in the currently selected sector on the currently selected page.
+        
+        col: X position of the image in columns, 0...65024
+        row: Y position of the image in rows, 0...65024
+        image: image to output (path to image file, PIL Image object, or raw BMP image data)
+        filename: filename to save the image as on the display (max. 31 characters)
+        """
+        if isinstance(image, Image.Image):
+            bio = BytesIO()
+            image.convert('1')
+            image.save(bio, 'BMP')
+            bio.seek(0)
+            img_data = bio.read()
+        elif type(image) is str:
+            bio = BytesIO()
+            image = Image.open(image)
+            image.convert('1')
+            image.save(bio, 'BMP')
+            bio.seek(0)
+            img_data = bio.read()
+        else:
+            img_data = image
+        return self.send_command("ECS_LCD_PutImage", col, row, imagefilename=filename, image=img_data)
+
+    def insert_line(self, line):
+        """
+        Inserts a line of text into the currently selected sector,
+        below the line with the specified index.
+        The remaining lines will be shifted downwards.
+        
+        line: line ID, 0...255
+        """
+        return self.send_command("ECS_LCD_InsertLine", line=line)
+
+    def delete_line(self, line):
+        """
+        Deletes a line of text from the currently selected sector.
+        The remaining lines will be shifted upwards.
+        
+        line: line ID, 0...255
+        """
+        return self.send_command("ECS_LCD_DeleteLine", line=line)
+
+    def chr_clr_txt(self, line):
+        """
+        CLears a line of text in the currently selected sector.
+        
+        line: line ID, 0...255
+        """
+        return self.send_command("ECS_LCD_ChrClrTxt", line)
+
+    def clr_sector(self):
+        """
+        Deletes the contents of the currently selected sector.
+        """
+        return self.send_command("ECS_LCD_ClrSector")
+
+    def clr_page(self):
+        """
+        Deletes the contents of the currently selected page.
+        """
+        return self.send_command("ECS_LCD_ClrPage")
+
+    def show_page(self, page):
+        """
+        Displays the page with the given ID on the display.
+        
+        page: page ID, 0...255
+        """
+        return self.send_command("ECS_LCD_ShowPage", page=page)
+
+    def prog_page_sequence(self, page, duration):
+        """
+        Appends an entry to the current list of pages to show.
+        Each entry comprises the page ID to be shown and a duration.
+        
+        page: page ID, 0...255
+        duration: duration is milliseconds, 0...65024
+        """
+        return self.send_command("ECS_LCD_ProgPageSequence", page=page, time=duration)
+
+    def activate_page_sequence(self):
+        """
+        Activates the previously programmed page seqneuce.
+        """
+        return self.send_command("ECS_LCD_ActivatePageSequence")
+
+    def scroll_page(self, mode, lines=None, pause=None):
+        """
+        Scrolls the display contents up by the given amount of lines of text
+        with the given pause between lines.
+        
+        mode: scroll mode (off, line, cont)
+                off:  disable scrolling
+                line: scroll row by row
+                cont: scroll pixel by pixel
+        lines: the number of lines to scroll, 0...255
+        pause: the pause between lines in seconds, 0...255
+        """
+        return self.send_command("ECS_LCD_ScrollPage", scroll=mode, lines=lines, pausetime=pause)
+
+    def switch_background_light(self, state):
+        """
+        Turns the background light on or off.
+        
+        state: light state (on, off)
+        """
+        if type(state) in (bool, int):
+            state = 'on' if state else 'off'
+        return self.send_command("ECS_LCD_SwitchBackgroundLight", light=state)
+
+    def get_operative_status(self):
+        """
+        Get the operative status of the display.
+        """
+        return self.send_command("ECS_LCD_GetOperativeStatus")
+
+    def get_reset_time(self):
+        """
+        Get the number of seconds since the last reset.
+        """
+        return self.send_command("ECS_LCD_GetResetTime")
+
+    def get_time(self):
+        """
+        Get the system time.
+        """
+        return self.send_command("ECS_LCD_GetTime")
+
+    def get_software_version(self):
+        """
+        Get the software version.
+        """
+        return self.send_command("ECS_LCD_GetSoftwareVersion")
+
+    def get_device_cfg(self):
+        """
+        Get the device configuration.
+        """
+        return self.send_command("ECS_LCD_GetDeviceCfg")
+
+    def get_page_content(self, page):
+        """
+        Get the contents of the specified page.
+
+        page: page ID, 0...255
+        """
+        return self.send_command("ECS_LCD_GetPageContent", page=page)
+
+
+    """
+    CONVENIENCE FUNCTIONS
+    """
+
+    def display_text(self, page, text, font, align='center', attribute='normal'):
+        """
+        Displays a text on the given page.
+
+        page: page ID, 0...255
+        text: the text to display
+        font: font ID, 0...255
+        align: text alignment (left, center, right, flow)
+        attribute: text display attribute (normal, blink, compblink, invers) (compblink: inverted and blinking)
+        """
+        lines = text.splitlines()
+        self.define_normal_page(page)
+        self.select_page(page)
+        self.change_sector(0, 0, 0, self.width, self.height, 'text', font, lines=len(lines))
+        self.select_sector(0)
+        for i, row in enumerate(lines):
+            self.chr_out_text(i, row, align, attribute)
+
+        if self.double_sided:
+            self.change_sector(1, 0, self.height, self.width, self.height, 'text', font, lines=len(lines))
+            self.select_sector(1)
+            for i, row in enumerate(lines):
+                self.chr_out_text(i, row, align, attribute)
+        
+        self.show_page(page)
+
+    def display_image(self, page, image, halign='center', valign='middle'):
+        """
+        Displays an image on the given page.
+
+        page: page ID, 0...255
+        image: the image to display (PIL Image object or path to image)
+        halign: horizontal image alignment (left, center, right)
+        valign: vertical image alignment (top, middle, bottom)
+        """
+        if not isinstance(image, Image.Image):
+            image = Image.open(image)
+        width, height = image.size
+
+        if halign == 'center':
+            x = (self.width - width) // 2
+        elif halign == 'right':
+            x = self.width - width
+        else:
+            x = 0
+
+        if valign == 'middle':
+            y = (self.height - height) // 2
+        elif valign == 'bottom':
+            y = self.height - height
+        else:
+            y = 0
+
+        self.define_normal_page(page)
+        self.select_page(page)
+        self.change_sector(0, 0, 0, self.width, self.height, 'graphic')
+        self.select_sector(0)
+        self.put_image(x, y, image)
+
+        if self.double_sided:
+            self.change_sector(1, 0, self.height, self.width, self.height, 'graphic')
+            self.select_sector(1)
+            self.put_image(x, y, image)
+        
         self.show_page(page)
```

### Comparing `pyFIS-1.8.1/pyfis/aegmis/mis1_gcu.py` & `pyFIS-1.9.0/pyfis/aegmis/mis1_gcu.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-"""
-Copyright (C) 2020-2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-import time
-
-from ..utils import debug_hex
-
-
-class MIS1GCUDisplay:
-    ALIGN_LEFT = 0x00
-    ALIGN_RIGHT = 0x01
-    ALIGN_CENTER = 0x02
-    ALIGN_SCROLL = 0x03 # apparently not supported
-    
-    ATTR_BLINK = 0x01
-    ATTR_INVERT = 0x02
-    ATTR_BLINK_INV = 0x08
-    
-    DATE_FORMAT_DISABLE = 0x00
-    DATE_FORMAT_DDMMYY = 0x01
-    DATE_FORMAT_MMDDYY = 0x02
-    DATE_FORMAT_YYMMDD = 0x03
-    
-    TIME_FORMAT_DISABLE = 0x00
-    TIME_FORMAT_24H = 0x01
-    TIME_FORMAT_12H_AM_PM = 0x02
-    TIME_FORMAT_12H = 0x03
-    
-    def __init__(self, port, address = 1, baudrate = 9600, exclusive = True, debug = False):
-        self.address = address
-        self.debug = debug
-        if isinstance(port, serial.Serial):
-            self.port = port
-        else:
-            self.port = serial.Serial(port, baudrate=baudrate, bytesize=8, parity="E", stopbits=1, exclusive=exclusive)
-
-    def checksum(self, data):
-        checksum = 0x00
-        for i, byte in enumerate(data):
-            checksum += byte
-        return (checksum % 256) | 0x80
-
-    def escape(self, data):
-        escaped = []
-        for byte in data:
-            if byte in (0x02, 0x03, 0x04, 0x05, 0x10):
-                escaped += [0x10, byte]
-            else:
-                escaped.append(byte)
-        return escaped
-    
-    def send_raw_telegram(self, data):
-        telegram = [0x04, (0x80 | self.address), 0x02] + self.escape(data) + [0x03] + [self.checksum(data + [0x03])]
-        if self.debug:
-            print(debug_hex(telegram, readable_ascii=False, readable_ctrl=False))
-        self.port.setRTS(1)
-        self.port.write(telegram)
-        time.sleep(0.1)
-        self.port.setRTS(0)
-    
-    def send_command(self, code, subcode, data):
-        return self.send_raw_telegram([code, subcode] + data)
-    
-    def merge_attributes(self, text):
-        if type(text) in (tuple, list):
-            merged = ""
-            for t, attrs in text:
-                merged += "\x00" + chr(attrs) + t
-            return merged
-        return text
-
-    def simple_text(self, page, row, col, text, align = ALIGN_LEFT):
-        text = self.merge_attributes(text)
-        text = text.encode("CP437")
-        data = [align, page, row, col] + list(text)
-        return self.send_command(0x11, 0x00, data)
-
-    def text(self, page, row, col_start, col_end, text, align = ALIGN_LEFT):
-        text = self.merge_attributes(text)
-        text = text.encode("CP437")
-        data = [align, page, row, col_start >> 8, col_start & 0xFF, col_end >> 8, col_end & 0xFF] + list(text)
-        return self.send_command(0x15, 0x00, data)
-    
-    def set_pages(self, pages):
-        flat_pages = [item for sublist in pages for item in sublist]
-        data = [0x00] + flat_pages
-        return self.send_command(0x24, 0x00, data)
-    
-    def set_page(self, page):
-        return self.set_pages([(page, 255)])
-    
-    def set_clock(self, year, month, day, hour, minute, second):
-        # apparently unsupported
-        data = list(divmod(second, 10)[::-1])
-        data += divmod(minute, 10)[::-1]
-        data += divmod(hour, 10)[::-1]
-        data += divmod(day, 10)[::-1]
-        data += divmod(month, 10)[::-1]
-        data += divmod(year, 10)[::-1]
-        data += [0x00] # weekday, unused
-        return self.send_command(0x3A, 0x00, data)
-    
-    def set_clock_display(self, date_format, date_row, date_col_start, date_col_end, time_format, time_row, time_col_start, time_col_end):
-        # apparently unsupported
-        data = [date_format, date_row]
-        data += [date_col_start >> 8, date_col_start & 0xFF]
-        data += [date_col_end >> 8, date_col_end & 0xFF]
-        data += [time_format, time_row]
-        data += [time_col_start >> 8, time_col_start & 0xFF]
-        data += [time_col_end >> 8, time_col_end & 0xFF]
-        return self.send_command(0x3D, 0x00, data)
-    
-    def set_outputs(self, states):
-        # states: array of 8 bools representing outputs 0 through 7
-        state_byte = 0x00
-        for i in range(max(8, len(states))):
-            if states[i]:
-                state_byte |= (1 << i)
-        return self.send_command(0x41, 0x00, [0x00, 0x00, state_byte])
+"""
+Copyright (C) 2020-2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+import time
+
+from ..utils import debug_hex
+
+
+class MIS1GCUDisplay:
+    ALIGN_LEFT = 0x00
+    ALIGN_RIGHT = 0x01
+    ALIGN_CENTER = 0x02
+    ALIGN_SCROLL = 0x03 # apparently not supported
+    
+    ATTR_BLINK = 0x01
+    ATTR_INVERT = 0x02
+    ATTR_BLINK_INV = 0x08
+    
+    DATE_FORMAT_DISABLE = 0x00
+    DATE_FORMAT_DDMMYY = 0x01
+    DATE_FORMAT_MMDDYY = 0x02
+    DATE_FORMAT_YYMMDD = 0x03
+    
+    TIME_FORMAT_DISABLE = 0x00
+    TIME_FORMAT_24H = 0x01
+    TIME_FORMAT_12H_AM_PM = 0x02
+    TIME_FORMAT_12H = 0x03
+    
+    def __init__(self, port, address = 1, baudrate = 9600, exclusive = True, debug = False):
+        self.address = address
+        self.debug = debug
+        if isinstance(port, serial.Serial):
+            self.port = port
+        else:
+            self.port = serial.Serial(port, baudrate=baudrate, bytesize=8, parity="E", stopbits=1, exclusive=exclusive)
+
+    def checksum(self, data):
+        checksum = 0x00
+        for i, byte in enumerate(data):
+            checksum += byte
+        return (checksum % 256) | 0x80
+
+    def escape(self, data):
+        escaped = []
+        for byte in data:
+            if byte in (0x02, 0x03, 0x04, 0x05, 0x10):
+                escaped += [0x10, byte]
+            else:
+                escaped.append(byte)
+        return escaped
+    
+    def send_raw_telegram(self, data):
+        telegram = [0x04, (0x80 | self.address), 0x02] + self.escape(data) + [0x03] + [self.checksum(data + [0x03])]
+        if self.debug:
+            print(debug_hex(telegram, readable_ascii=False, readable_ctrl=False))
+        self.port.setRTS(1)
+        self.port.write(telegram)
+        time.sleep(0.1)
+        self.port.setRTS(0)
+    
+    def send_command(self, code, subcode, data):
+        return self.send_raw_telegram([code, subcode] + data)
+    
+    def merge_attributes(self, text):
+        if type(text) in (tuple, list):
+            merged = ""
+            for t, attrs in text:
+                merged += "\x00" + chr(attrs) + t
+            return merged
+        return text
+
+    def simple_text(self, page, row, col, text, align = ALIGN_LEFT):
+        text = self.merge_attributes(text)
+        text = text.encode("CP437")
+        data = [align, page, row, col] + list(text)
+        return self.send_command(0x11, 0x00, data)
+
+    def text(self, page, row, col_start, col_end, text, align = ALIGN_LEFT):
+        text = self.merge_attributes(text)
+        text = text.encode("CP437")
+        data = [align, page, row, col_start >> 8, col_start & 0xFF, col_end >> 8, col_end & 0xFF] + list(text)
+        return self.send_command(0x15, 0x00, data)
+    
+    def set_pages(self, pages):
+        flat_pages = [item for sublist in pages for item in sublist]
+        data = [0x00] + flat_pages
+        return self.send_command(0x24, 0x00, data)
+    
+    def set_page(self, page):
+        return self.set_pages([(page, 255)])
+    
+    def set_clock(self, year, month, day, hour, minute, second):
+        # apparently unsupported
+        data = list(divmod(second, 10)[::-1])
+        data += divmod(minute, 10)[::-1]
+        data += divmod(hour, 10)[::-1]
+        data += divmod(day, 10)[::-1]
+        data += divmod(month, 10)[::-1]
+        data += divmod(year, 10)[::-1]
+        data += [0x00] # weekday, unused
+        return self.send_command(0x3A, 0x00, data)
+    
+    def set_clock_display(self, date_format, date_row, date_col_start, date_col_end, time_format, time_row, time_col_start, time_col_end):
+        # apparently unsupported
+        data = [date_format, date_row]
+        data += [date_col_start >> 8, date_col_start & 0xFF]
+        data += [date_col_end >> 8, date_col_end & 0xFF]
+        data += [time_format, time_row]
+        data += [time_col_start >> 8, time_col_start & 0xFF]
+        data += [time_col_end >> 8, time_col_end & 0xFF]
+        return self.send_command(0x3D, 0x00, data)
+    
+    def set_outputs(self, states):
+        # states: array of 8 bools representing outputs 0 through 7
+        state_byte = 0x00
+        for i in range(max(8, len(states))):
+            if states[i]:
+                state_byte |= (1 << i)
+        return self.send_command(0x41, 0x00, [0x00, 0x00, state_byte])
```

### Comparing `pyFIS-1.8.1/pyfis/ibis/__init__.py` & `pyFIS-1.9.0/pyfis/ibis/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-Copyright (C) 2016 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .ibis_serial import SerialIBISMaster
+"""
+Copyright (C) 2016 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .ibis_serial import SerialIBISMaster
 from .ibis_tcp import TCPIBISMaster
```

### Comparing `pyFIS-1.8.1/pyfis/ibis/ibis_serial.py` & `pyFIS-1.9.0/pyfis/ibis/ibis_serial.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-"""
-Copyright (C) 2016 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-
-from .ibis_protocol import IBISProtocol
-
-class SerialIBISMaster(IBISProtocol):
-    """
-    An IBIS bus master, sending and receiving telegrams using a serial port
-    """
-    
-    def __init__(self, port, baudrate = 1200, bytesize = 7, parity = 'E',
-                 stopbits = 2, timeout = 2.0, exclusive = False, *args, **kwargs):
-        """
-        port:
-        The serial port to use for communication
-        """
-        
-        super().__init__(*args, **kwargs)
-        
-        if isinstance(port, serial.Serial):
-            self.device = port
-            self.port = self.device.port
-        else:
-            self.port = port
-            self.device = serial.Serial(
-                self.port,
-                baudrate = baudrate,
-                bytesize = bytesize,
-                parity = parity,
-                stopbits = stopbits,
-                timeout = timeout,
-                exclusive=exclusive
-            )
-    
-    def _send(self, telegram):
-        """
-        Actually send the telegram.
-        This varies depending on implementation
-        """
-        
-        self.device.write(telegram)
-    
-    def _receive(self, length):
-        """
-        Actually receive data.
-        This varies depending on implementation and needs to be overridden
-        """
-        
-        return self.device.read(length)
-
-    def __del__(self):
-        self.device.close()
+"""
+Copyright (C) 2016 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+
+from .ibis_protocol import IBISProtocol
+
+class SerialIBISMaster(IBISProtocol):
+    """
+    An IBIS bus master, sending and receiving telegrams using a serial port
+    """
+    
+    def __init__(self, port, baudrate = 1200, bytesize = 7, parity = 'E',
+                 stopbits = 2, timeout = 2.0, exclusive = False, *args, **kwargs):
+        """
+        port:
+        The serial port to use for communication
+        """
+        
+        super().__init__(*args, **kwargs)
+        
+        if isinstance(port, serial.Serial):
+            self.device = port
+            self.port = self.device.port
+        else:
+            self.port = port
+            self.device = serial.Serial(
+                self.port,
+                baudrate = baudrate,
+                bytesize = bytesize,
+                parity = parity,
+                stopbits = stopbits,
+                timeout = timeout,
+                exclusive=exclusive
+            )
+    
+    def _send(self, telegram):
+        """
+        Actually send the telegram.
+        This varies depending on implementation
+        """
+        
+        self.device.write(telegram)
+    
+    def _receive(self, length):
+        """
+        Actually receive data.
+        This varies depending on implementation and needs to be overridden
+        """
+        
+        return self.device.read(length)
+
+    def __del__(self):
+        self.device.close()
```

### Comparing `pyFIS-1.8.1/pyfis/krone/__init__.py` & `pyFIS-1.9.0/pyfis/krone/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"""
-Copyright (C) 2019 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .k9000_fbm import Krone9000FBM
-from .k9000_fbk import Krone9000FBK
-from .k9000_hlst import Krone9000HLST
-from .k8200 import Krone8200Display
+"""
+Copyright (C) 2019 - 2022 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .k9000_fbm import Krone9000FBM
+from .k9000_fbk import Krone9000FBK
+from .k9000_hlst import Krone9000HLST
+from .k8200 import Krone8200Display
+from .k8200_pst import Krone8200PST
```

### Comparing `pyFIS-1.8.1/pyfis/krone/exceptions.py` & `pyFIS-1.9.0/pyfis/lawo/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,19 @@
-"""
-Copyright 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-class CommunicationError(IOError):
-    pass
-
-class NACKError(CommunicationError):
-    pass
-
-class BusyError(CommunicationError):
-    pass
+"""
+Copyright (C) 2016 - 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .mono_serial import SerialMONOMaster
+from .lawo_font import LawoFont
```

### Comparing `pyFIS-1.8.1/pyfis/krone/k9000_fbk.py` & `pyFIS-1.9.0/pyfis/krone/k9000_fbk.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-"""
-Copyright (C) 2019 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-
-from itertools import groupby
-
-from .k9000_rs485 import Krone9000RS485Controller
-from .exceptions import CommunicationError
-
-
-class Krone9000FBK(Krone9000RS485Controller):
-    """
-    Controls a FBK (Fallblatt-Buskopfkarte)
-    (split-flap group control) board.
-    """
-    
-    BOARD_ID = 0xB2
-    BOARD_NAME = "FBK"
-    
-    FLAG_START_IMMEDIATELY = 0x80
-    FLAG_FBM_COMMAND = 0x40
-    FLAG_ENABLE_COMPRESSION = 0x20
-    
-    CMD_GET_FBK_STATUS = 0x01
-    CMD_GET_LINE_INIT_DATA = 0x02
-    CMD_GET_LINE_DATA = 0x03
-    CMD_SET_BLINKER = 0x0B
-    CMD_SET_FBM_VALUE_TABLE = 0x0E
-    CMD_LOCK_FBK = 0xC6
-    CMD_UNLOCK_FBK = 0xC7
-    
-    CMD_FBM_START = 0x00 | FLAG_START_IMMEDIATELY
-    CMD_GET_FBM_STATUS = 0x03 | FLAG_FBM_COMMAND
-    CMD_GET_FBM_CONTENT = 0x04 | FLAG_FBM_COMMAND
-    CMD_CLEAR_FBM = 0x05 | FLAG_FBM_COMMAND
-    CMD_LOCK_FBM = 0x06 | FLAG_FBM_COMMAND | FLAG_START_IMMEDIATELY
-    CMD_UNLOCK_FBM = 0x07 | FLAG_FBM_COMMAND | FLAG_START_IMMEDIATELY
-    CMD_SET_FBM_CODES_SEQ = 0x08 | FLAG_FBM_COMMAND
-    CMD_SET_FBM_CODES_ADDR = 0x09 | FLAG_FBM_COMMAND
-    
-    def _get_fbm_status(self, stat):
-        # Return human-readable error strings
-        # based on FBM error bits
-        if stat & 0x08:
-            lut = {
-                0b1000: "comm_error",
-                0b1001: "start_missing",
-                0b1010: "unknown_char",
-                0b1011: "external_rotation",
-                0b1100: "rotation_timeout",
-                0b1101: "fbm_missing",
-                0b1111: "rotating"
-            }
-            return [lut.get(stat & 0x0f, "")]
-        else:
-            errors = []
-            if stat & 0x04:
-                errors.append("no_ac")
-            if stat & 0x02:
-                errors.append("no_flap_imps")
-            if stat & 0x01:
-                errors.append("no_home_imp")
-            return errors
-    
-    def _rle(self, data):
-        # Simple run-length encoding
-        rle_data = []
-        for k,i in groupby(data):
-            run = list(i)
-            if(len(run) > 2):
-                while len(run) > 128:
-                    rle_data.extend([(len(run) - 1) | 0x80, k])
-                    run = run[128:]
-                rle_data.extend([(len(run) - 1) | 0x80, k])
-            else:
-                rle_data.extend(run)
-        return rle_data
-    
-    def get_status(self):
-        # Get the status of the FBK board
-        payload = self.send_command(self.CMD_GET_FBK_STATUS, response=True)
-        stat = payload[1]
-        status = {
-            'comm_err': bool(stat & 0x40),
-            'reset': bool(stat & 0x20),
-            'locked': bool(stat & 0x10),
-            'fbm_err': bool(stat & 0x08),
-            'blinker_err': bool(stat & 0x04),
-            'fbm_start_missing': bool(stat & 0x02),
-            'sw_ver': f"{payload[2]}.{payload[3]}"
-        }
-        return status
-    
-    def get_fbm_ids(self):
-        # Get a list of all connected FBM IDs
-        payload = self.send_command(self.CMD_GET_LINE_INIT_DATA, response=True)
-        module_data = payload[1:]
-        modules_present = []
-        addr = 0
-        for byte in module_data:
-            for bit in range(7):
-                if byte & (1 << bit):
-                    modules_present.append(addr)
-                addr += 1
-                if addr > 255:
-                    break
-        return modules_present
-    
-    def get_fbm_statuses(self):
-        # True means okay, False means FBM error or not present
-        # (see get_fbm_ids to get a list of present FBMs)
-        payload = self.send_command(self.CMD_GET_LINE_DATA, response=True)
-        module_data = payload[1:]
-        module_statuses = {}
-        addr = 0
-        for byte in module_data:
-            for bit in range(7):
-                module_statuses[addr] = bool(byte & (1 << bit))
-                addr += 1
-                if addr > 255:
-                    break
-        return module_statuses
-    
-    def set_blinker(self, state):
-        # Set the blinker associated with this FBK on or off
-        return self.send_command(self.CMD_SET_BLINKER, 0x31 if state else 0x30)
-    
-    def set_fbm_value_table(self, addr, table):
-        # Set the internal mapping of character code to flap position
-        # on the selected FBM
-        # table is a list of characters to be mapped to flaps,
-        # starting at flap 0
-        parameters = [addr] + table
-        self.send_command(self.CMD_SET_FBM_VALUE_TABLE, parameters)
-        # Special case here: The FBK sends the number of flap codes transferred
-        # as a single byte after it has finished sending the data to the FBM.
-        # As this is the only case in which this sort of response occurs,
-        # we are just handling it manually here.
-        num_xferred = b""
-        tries = 0
-        # Try for roughly five seconds (exact value depends on the port timeout)
-        while num_xferred == b"":
-            if tries >= 5.0 / self.port.timeout:
-                raise CommunicationError("Timeout while waiting for result of FBM value table transfer")
-            num_xferred = self.port.read(1)
-            tries += 1
-        self.debug_print(bytearray(num_xferred), receive=True)
-        # Return the number of transferred flap codes
-        return ord(num_xferred)
-    
-    def lock(self):
-        # Lock the entire FBK
-        return self.send_command(self.CMD_LOCK_FBK)
-    
-    def unlock(self):
-        # Unlock the entire FBK
-        return self.send_command(self.CMD_UNLOCK_FBK)
-    
-    def start_fbm(self):
-        return self.send_command(self.CMD_FBM_START)
-    
-    def get_detailed_fbm_statuses(self, addrs):
-        # Get detailed FBM status information for up to 10 FBMs.
-        # addrs is a list of FBM IDs to be queried
-        payload = self.send_command(self.CMD_GET_FBM_STATUS, addrs, response=True)
-        module_statuses = {}
-        data = payload[1:]
-        for i in range(0, len(data), 2):
-            addr = data[i]
-            stat = data[i + 1]
-            module_statuses[addr] = {
-                'home_pos': bool(stat & 0x40),
-                'reset': bool(stat & 0x20),
-                'locked': bool(stat & 0x10),
-                'status': self._get_fbm_status(stat & 0x0f)
-            }
-        return module_statuses
-    
-    def get_all_detailed_fbm_statuses(self):
-        # Automatically read the list of connected FBM IDs
-        # and query all of them for detailed status information
-        module_statuses = {}
-        for addrs in self._chunks(self.get_fbm_ids(), 10):
-            module_statuses.update(self.get_detailed_fbm_statuses(addrs))
-        return module_statuses
-    
-    def get_fbm_contents(self, addrs):
-        # Get the currently displayed character for up to 10 FBMs.
-        # addrs is a list of FBM IDs to be queried
-        payload = self.send_command(self.CMD_GET_FBM_CONTENT, addrs, response=True)
-        module_contents = {}
-        data = payload[1:]
-        for i in range(0, len(data), 2):
-            addr = data[i]
-            char = data[i + 1]
-            module_contents[addr] = chr(char)
-        return module_contents
-    
-    def get_all_fbm_contents(self):
-        # Automatically read the list of connected FBM IDs
-        # and query all of them for their content
-        module_contents = {}
-        for addrs in self._chunks(self.get_fbm_ids(), 10):
-            module_contents.update(self.get_fbm_contents(addrs))
-        return module_contents
-    
-    def clear_fbm(self, addrs = None, immediate = True):
-        # Clear all or the selected FBMs
-        cmd = self.CMD_CLEAR_FBM
-        if immediate:
-            cmd |= self.FLAG_START_IMMEDIATELY
-        return self.send_command(cmd, addrs)
-    
-    def lock_fbm(self, addrs = None):
-        # Lock all or the selected FBMs
-        return self.send_command(self.CMD_LOCK_FBM, addrs)
-    
-    def unlock_fbm(self, addrs = None):
-        # Unlock all or the selected FBMs
-        return self.send_command(self.CMD_UNLOCK_FBM, addrs)
-    
-    def set_fbm_codes_seq(self, codes, immediate = False, compress = False):
-        # Set FBM character codes to be displayed
-        # sequentially (without explicit addressing)
-        cmd = self.CMD_SET_FBM_CODES_SEQ
-        if immediate:
-            cmd |= self.FLAG_START_IMMEDIATELY
-        if compress:
-            cmd |= self.FLAG_ENABLE_COMPRESSION
-            codes = self._rle(codes)
-        return self.send_command(cmd, codes)
-    
-    def set_fbm_codes_addr(self, codes, immediate = False):
-        # Set FBM character codes to be displayed
-        # with explicit addressing
-        cmd = self.CMD_SET_FBM_CODES_ADDR
-        if immediate:
-            cmd |= self.FLAG_START_IMMEDIATELY
-        return self.send_command(cmd, codes)
-    
-    def d_set_module_data(self, module_data):
-        # Compatibility function for SplitFlapDisplay class
-        for chunk in self._chunks(module_data, 50):
-            self.set_fbm_codes_addr([i for s in chunk for i in s])
-    
-    def d_update(self):
-        # Compatibility function for SplitFlapDisplay class
-        self.start_fbm()
+"""
+Copyright (C) 2019 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+
+from itertools import groupby
+
+from .k9000_rs485 import Krone9000RS485Controller
+from .exceptions import CommunicationError
+
+
+class Krone9000FBK(Krone9000RS485Controller):
+    """
+    Controls a FBK (Fallblatt-Buskopfkarte)
+    (split-flap group control) board.
+    """
+    
+    BOARD_ID = 0xB2
+    BOARD_NAME = "FBK"
+    
+    FLAG_START_IMMEDIATELY = 0x80
+    FLAG_FBM_COMMAND = 0x40
+    FLAG_ENABLE_COMPRESSION = 0x20
+    
+    CMD_GET_FBK_STATUS = 0x01
+    CMD_GET_LINE_INIT_DATA = 0x02
+    CMD_GET_LINE_DATA = 0x03
+    CMD_SET_BLINKER = 0x0B
+    CMD_SET_FBM_VALUE_TABLE = 0x0E
+    CMD_LOCK_FBK = 0xC6
+    CMD_UNLOCK_FBK = 0xC7
+    
+    CMD_FBM_START = 0x00 | FLAG_START_IMMEDIATELY
+    CMD_GET_FBM_STATUS = 0x03 | FLAG_FBM_COMMAND
+    CMD_GET_FBM_CONTENT = 0x04 | FLAG_FBM_COMMAND
+    CMD_CLEAR_FBM = 0x05 | FLAG_FBM_COMMAND
+    CMD_LOCK_FBM = 0x06 | FLAG_FBM_COMMAND | FLAG_START_IMMEDIATELY
+    CMD_UNLOCK_FBM = 0x07 | FLAG_FBM_COMMAND | FLAG_START_IMMEDIATELY
+    CMD_SET_FBM_CODES_SEQ = 0x08 | FLAG_FBM_COMMAND
+    CMD_SET_FBM_CODES_ADDR = 0x09 | FLAG_FBM_COMMAND
+    
+    def _get_fbm_status(self, stat):
+        # Return human-readable error strings
+        # based on FBM error bits
+        if stat & 0x08:
+            lut = {
+                0b1000: "comm_error",
+                0b1001: "start_missing",
+                0b1010: "unknown_char",
+                0b1011: "external_rotation",
+                0b1100: "rotation_timeout",
+                0b1101: "fbm_missing",
+                0b1111: "rotating"
+            }
+            return [lut.get(stat & 0x0f, "")]
+        else:
+            errors = []
+            if stat & 0x04:
+                errors.append("no_ac")
+            if stat & 0x02:
+                errors.append("no_flap_imps")
+            if stat & 0x01:
+                errors.append("no_home_imp")
+            return errors
+    
+    def _rle(self, data):
+        # Simple run-length encoding
+        rle_data = []
+        for k,i in groupby(data):
+            run = list(i)
+            if(len(run) > 2):
+                while len(run) > 128:
+                    rle_data.extend([(len(run) - 1) | 0x80, k])
+                    run = run[128:]
+                rle_data.extend([(len(run) - 1) | 0x80, k])
+            else:
+                rle_data.extend(run)
+        return rle_data
+    
+    def get_status(self):
+        # Get the status of the FBK board
+        payload = self.send_command(self.CMD_GET_FBK_STATUS, response=True)
+        stat = payload[1]
+        status = {
+            'comm_err': bool(stat & 0x40),
+            'reset': bool(stat & 0x20),
+            'locked': bool(stat & 0x10),
+            'fbm_err': bool(stat & 0x08),
+            'blinker_err': bool(stat & 0x04),
+            'fbm_start_missing': bool(stat & 0x02),
+            'sw_ver': f"{payload[2]}.{payload[3]}"
+        }
+        return status
+    
+    def get_fbm_ids(self):
+        # Get a list of all connected FBM IDs
+        payload = self.send_command(self.CMD_GET_LINE_INIT_DATA, response=True)
+        module_data = payload[1:]
+        modules_present = []
+        addr = 0
+        for byte in module_data:
+            for bit in range(7):
+                if byte & (1 << bit):
+                    modules_present.append(addr)
+                addr += 1
+                if addr > 255:
+                    break
+        return modules_present
+    
+    def get_fbm_statuses(self):
+        # True means okay, False means FBM error or not present
+        # (see get_fbm_ids to get a list of present FBMs)
+        payload = self.send_command(self.CMD_GET_LINE_DATA, response=True)
+        module_data = payload[1:]
+        module_statuses = {}
+        addr = 0
+        for byte in module_data:
+            for bit in range(7):
+                module_statuses[addr] = bool(byte & (1 << bit))
+                addr += 1
+                if addr > 255:
+                    break
+        return module_statuses
+    
+    def set_blinker(self, state):
+        # Set the blinker associated with this FBK on or off
+        return self.send_command(self.CMD_SET_BLINKER, 0x31 if state else 0x30)
+    
+    def set_fbm_value_table(self, addr, table):
+        # Set the internal mapping of character code to flap position
+        # on the selected FBM
+        # table is a list of characters to be mapped to flaps,
+        # starting at flap 0
+        parameters = [addr] + table
+        self.send_command(self.CMD_SET_FBM_VALUE_TABLE, parameters)
+        # Special case here: The FBK sends the number of flap codes transferred
+        # as a single byte after it has finished sending the data to the FBM.
+        # As this is the only case in which this sort of response occurs,
+        # we are just handling it manually here.
+        num_xferred = b""
+        tries = 0
+        # Try for roughly five seconds (exact value depends on the port timeout)
+        while num_xferred == b"":
+            if tries >= 5.0 / self.port.timeout:
+                raise CommunicationError("Timeout while waiting for result of FBM value table transfer")
+            num_xferred = self.port.read(1)
+            tries += 1
+        self.debug_print(bytearray(num_xferred), receive=True)
+        # Return the number of transferred flap codes
+        return ord(num_xferred)
+    
+    def lock(self):
+        # Lock the entire FBK
+        return self.send_command(self.CMD_LOCK_FBK)
+    
+    def unlock(self):
+        # Unlock the entire FBK
+        return self.send_command(self.CMD_UNLOCK_FBK)
+    
+    def start_fbm(self):
+        return self.send_command(self.CMD_FBM_START)
+    
+    def get_detailed_fbm_statuses(self, addrs):
+        # Get detailed FBM status information for up to 10 FBMs.
+        # addrs is a list of FBM IDs to be queried
+        payload = self.send_command(self.CMD_GET_FBM_STATUS, addrs, response=True)
+        module_statuses = {}
+        data = payload[1:]
+        for i in range(0, len(data), 2):
+            addr = data[i]
+            stat = data[i + 1]
+            module_statuses[addr] = {
+                'home_pos': bool(stat & 0x40),
+                'reset': bool(stat & 0x20),
+                'locked': bool(stat & 0x10),
+                'status': self._get_fbm_status(stat & 0x0f)
+            }
+        return module_statuses
+    
+    def get_all_detailed_fbm_statuses(self):
+        # Automatically read the list of connected FBM IDs
+        # and query all of them for detailed status information
+        module_statuses = {}
+        for addrs in self._chunks(self.get_fbm_ids(), 10):
+            module_statuses.update(self.get_detailed_fbm_statuses(addrs))
+        return module_statuses
+    
+    def get_fbm_contents(self, addrs):
+        # Get the currently displayed character for up to 10 FBMs.
+        # addrs is a list of FBM IDs to be queried
+        payload = self.send_command(self.CMD_GET_FBM_CONTENT, addrs, response=True)
+        module_contents = {}
+        data = payload[1:]
+        for i in range(0, len(data), 2):
+            addr = data[i]
+            char = data[i + 1]
+            module_contents[addr] = chr(char)
+        return module_contents
+    
+    def get_all_fbm_contents(self):
+        # Automatically read the list of connected FBM IDs
+        # and query all of them for their content
+        module_contents = {}
+        for addrs in self._chunks(self.get_fbm_ids(), 10):
+            module_contents.update(self.get_fbm_contents(addrs))
+        return module_contents
+    
+    def clear_fbm(self, addrs = None, immediate = True):
+        # Clear all or the selected FBMs
+        cmd = self.CMD_CLEAR_FBM
+        if immediate:
+            cmd |= self.FLAG_START_IMMEDIATELY
+        return self.send_command(cmd, addrs)
+    
+    def lock_fbm(self, addrs = None):
+        # Lock all or the selected FBMs
+        return self.send_command(self.CMD_LOCK_FBM, addrs)
+    
+    def unlock_fbm(self, addrs = None):
+        # Unlock all or the selected FBMs
+        return self.send_command(self.CMD_UNLOCK_FBM, addrs)
+    
+    def set_fbm_codes_seq(self, codes, immediate = False, compress = False):
+        # Set FBM character codes to be displayed
+        # sequentially (without explicit addressing)
+        cmd = self.CMD_SET_FBM_CODES_SEQ
+        if immediate:
+            cmd |= self.FLAG_START_IMMEDIATELY
+        if compress:
+            cmd |= self.FLAG_ENABLE_COMPRESSION
+            codes = self._rle(codes)
+        return self.send_command(cmd, codes)
+    
+    def set_fbm_codes_addr(self, codes, immediate = False):
+        # Set FBM character codes to be displayed
+        # with explicit addressing
+        cmd = self.CMD_SET_FBM_CODES_ADDR
+        if immediate:
+            cmd |= self.FLAG_START_IMMEDIATELY
+        return self.send_command(cmd, codes)
+    
+    def d_set_module_data(self, module_data):
+        # Compatibility function for SplitFlapDisplay class
+        for chunk in self._chunks(module_data, 50):
+            self.set_fbm_codes_addr([i for s in chunk for i in s])
+    
+    def d_update(self):
+        # Compatibility function for SplitFlapDisplay class
+        self.start_fbm()
```

### Comparing `pyFIS-1.8.1/pyfis/krone/k9000_fbm.py` & `pyFIS-1.9.0/pyfis/krone/k9000_fbm.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,171 @@
-"""
-Copyright 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-import time
-
-
-class Krone9000FBM:
-    """
-    Controls one or several FBM (Fallblattmodul)
-    (split flap module) boards.
-    """
-    
-    CMD_SET_ALL = 0b0001
-    CMD_SET_HOME = 0b0010
-    CMD_RESET = 0b0011
-    CMD_READ_STATUS = 0b0100
-    CMD_READ_CODE = 0b0101
-    CMD_LOCK = 0b0110
-    CMD_UNLOCK = 0b0111
-    CMD_SET_CODE = 0b1000
-    CMD_START_CALIBRATION_BR2 = 0b1001
-    CMD_START_CALIBRATION_BR1 = 0b1010
-    CMD_STOP_CALIBRATION = 0b1011
-    CMD_GET_CALIBRATION_VALUES = 0b1100
-    CMD_SET_TABLE = 0b1101
-    CMD_DELETE_TABLE = 0b1110
-    
-    def _get_fbm_status(self, stat):
-        # Return human-readable error strings
-        # based on FBM error bits
-        if stat & 0x08:
-            lut = {
-                0b1000: "comm_error",
-                0b1001: "start_missing",
-                0b1010: "unknown_char",
-                0b1011: "external_rotation",
-                0b1100: "rotation_timeout",
-                0b1101: "fbm_missing",
-                0b1111: "rotating"
-            }
-            return [lut.get(stat & 0x0f, "")]
-        else:
-            errors = []
-            if stat & 0x04:
-                errors.append("no_ac")
-            if stat & 0x02:
-                errors.append("no_flap_imps")
-            if stat & 0x01:
-                errors.append("no_home_imp")
-            return errors
-
-    def __init__(self, port, debug = False, exclusive = False):
-        self.debug = debug
-        if isinstance(port, serial.Serial):
-            self.port = port
-        else:
-            self.port = serial.Serial(port, baudrate=4800, parity=serial.PARITY_EVEN, timeout=2.0, exclusive=exclusive)
-    
-    def send_command(self, command, address = None, code = None, position = None, num_response_bytes = 0):
-        # Build base command byte
-        cmd_bytes = []
-        cmd_base = 0b10010000
-
-        # Address expansion bit
-        if address is not None and address > 127:
-            cmd_base |= 0b01000000
-        
-        # Code expansion bit
-        if code is not None and (code > 127 or (position is not None and position > 127)):
-            cmd_base |= 0b00100000
-        
-        # Command bits
-        cmd_base |= command
-        
-        # Build the data to be sent
-        cmd_bytes.append(cmd_base)
-        if address is not None:
-            cmd_bytes.append(address & 0b01111111)
-        if code is not None:
-            cmd_bytes.append(code & 0b01111111)
-        if position is not None:
-            cmd_bytes.append(position & 0b01111111)
-        
-        if self.debug:
-            print(" ".join((format(x, "#010b") for x in cmd_bytes)))
-            print(" ".join((format(x, "02X") for x in cmd_bytes)))
-        
-        # Send it
-        self.port.write(bytearray(cmd_bytes))
-
-        # Read response
-        if num_response_bytes > 0:
-            return self.port.read(num_response_bytes)
-        else:
-            return None
-    
-    def set_all(self):
-        return self.send_command(self.CMD_SET_ALL)
-    
-    def set_home(self):
-        return self.send_command(self.CMD_SET_HOME)
-    
-    def reset(self):
-        return self.send_command(self.CMD_RESET)
-    
-    def read_status(self, address):
-        return self.send_command(self.CMD_READ_STATUS, address, num_response_bytes=1)
-    
-    def read_code(self, address):
-        return self.send_command(self.CMD_READ_CODE, address, num_response_bytes=1)
-    
-    def lock(self, address):
-        return self.send_command(self.CMD_LOCK, address)
-    
-    def unlock(self, address):
-        return self.send_command(self.CMD_UNLOCK, address)
-    
-    def set_code(self, address, code):
-        return self.send_command(self.CMD_SET_CODE, address, code)
-    
-    def start_calibration_br2(self):
-        return self.send_command(self.CMD_START_CALIBRATION_BR2)
-    
-    def start_calibration_br1(self):
-        return self.send_command(self.CMD_START_CALIBRATION_BR1)
-    
-    def stop_calibration(self):
-        return self.send_command(self.CMD_STOP_CALIBRATION)
-    
-    def get_calibration_values(self, address):
-        return self.send_command(self.CMD_GET_CALIBRATION_VALUES, address, num_response_bytes=1)
-    
-    def set_table(self, address, code, position):
-        return self.send_command(self.CMD_SET_TABLE, address, position, code, num_response_bytes=1)
-    
-    def delete_table(self, address):
-        return self.send_command(self.CMD_DELETE_TABLE, address, num_response_bytes=1)
-    
-    def set_text(self, text, start_address, length = None, descending = False):
-        if length is not None:
-            text = text[:length].ljust(length)
-        for i, char in enumerate(text):
-            address = start_address - i if descending else start_address + i
-            self.set_code(address, ord(char.encode('iso-8859-1')))
-    
-    def get_status(self, addr):
-        return self._get_fbm_status(self.read_status(addr)[0])
-    
-    def d_set_module_data(self, module_data):
-        # Compatibility function for SplitFlapDisplay class
-        for addr, code in module_data:
-            self.set_code(addr, code)
-    
-    def d_update(self):
-        # Compatibility function for SplitFlapDisplay class
+"""
+Copyright 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+import time
+
+
+class Krone9000FBM:
+    """
+    Controls one or several FBM (Fallblattmodul)
+    (split flap module) boards.
+    """
+    
+    CMD_SET_ALL = 0b0001
+    CMD_SET_HOME = 0b0010
+    CMD_RESET = 0b0011
+    CMD_READ_STATUS = 0b0100
+    CMD_READ_CODE = 0b0101
+    CMD_LOCK = 0b0110
+    CMD_UNLOCK = 0b0111
+    CMD_SET_CODE = 0b1000
+    CMD_START_CALIBRATION_BR2 = 0b1001
+    CMD_START_CALIBRATION_BR1 = 0b1010
+    CMD_STOP_CALIBRATION = 0b1011
+    CMD_GET_CALIBRATION_VALUES = 0b1100
+    CMD_SET_TABLE = 0b1101
+    CMD_DELETE_TABLE = 0b1110
+    
+    def _get_fbm_status(self, stat):
+        # Return human-readable error strings
+        # based on FBM error bits
+        if stat & 0x08:
+            lut = {
+                0b1000: "comm_error",
+                0b1001: "start_missing",
+                0b1010: "unknown_char",
+                0b1011: "external_rotation",
+                0b1100: "rotation_timeout",
+                0b1101: "fbm_missing",
+                0b1111: "rotating"
+            }
+            return [lut.get(stat & 0x0f, "")]
+        else:
+            errors = []
+            if stat & 0x04:
+                errors.append("no_ac")
+            if stat & 0x02:
+                errors.append("no_flap_imps")
+            if stat & 0x01:
+                errors.append("no_home_imp")
+            return errors
+
+    def __init__(self, port, debug = False, exclusive = False):
+        self.debug = debug
+        if isinstance(port, serial.Serial):
+            self.port = port
+        else:
+            self.port = serial.Serial(port, baudrate=4800, parity=serial.PARITY_EVEN, timeout=2.0, exclusive=exclusive)
+    
+    def send_command(self, command, address = None, code = None, position = None, num_response_bytes = 0):
+        # Build base command byte
+        cmd_bytes = []
+        cmd_base = 0b10010000
+
+        # Address expansion bit
+        if address is not None and address > 127:
+            cmd_base |= 0b01000000
+        
+        # Code expansion bit
+        if code is not None and (code > 127 or (position is not None and position > 127)):
+            cmd_base |= 0b00100000
+        
+        # Command bits
+        cmd_base |= command
+        
+        # Build the data to be sent
+        cmd_bytes.append(cmd_base)
+        if address is not None:
+            cmd_bytes.append(address & 0b01111111)
+        if code is not None:
+            cmd_bytes.append(code & 0b01111111)
+        if position is not None:
+            cmd_bytes.append(position & 0b01111111)
+        
+        if self.debug:
+            print(" ".join((format(x, "#010b") for x in cmd_bytes)))
+            print(" ".join((format(x, "02X") for x in cmd_bytes)))
+        
+        # Send it
+        self.port.write(bytearray(cmd_bytes))
+
+        # Read response
+        if num_response_bytes > 0:
+            return self.port.read(num_response_bytes)
+        else:
+            return None
+    
+    def set_all(self):
+        return self.send_command(self.CMD_SET_ALL)
+    
+    def set_home(self):
+        return self.send_command(self.CMD_SET_HOME)
+    
+    def reset(self):
+        return self.send_command(self.CMD_RESET)
+    
+    def read_status(self, address):
+        return self.send_command(self.CMD_READ_STATUS, address, num_response_bytes=1)
+    
+    def read_code(self, address):
+        return self.send_command(self.CMD_READ_CODE, address, num_response_bytes=1)
+    
+    def lock(self, address):
+        return self.send_command(self.CMD_LOCK, address)
+    
+    def unlock(self, address):
+        return self.send_command(self.CMD_UNLOCK, address)
+    
+    def set_code(self, address, code):
+        return self.send_command(self.CMD_SET_CODE, address, code)
+    
+    def start_calibration_br2(self):
+        return self.send_command(self.CMD_START_CALIBRATION_BR2)
+    
+    def start_calibration_br1(self):
+        return self.send_command(self.CMD_START_CALIBRATION_BR1)
+    
+    def stop_calibration(self):
+        return self.send_command(self.CMD_STOP_CALIBRATION)
+    
+    def get_calibration_values(self, address):
+        return self.send_command(self.CMD_GET_CALIBRATION_VALUES, address, num_response_bytes=1)
+    
+    def set_table(self, address, code, position):
+        return self.send_command(self.CMD_SET_TABLE, address, position, code, num_response_bytes=1)
+    
+    def delete_table(self, address):
+        return self.send_command(self.CMD_DELETE_TABLE, address, num_response_bytes=1)
+    
+    def set_text(self, text, start_address, length = None, descending = False):
+        if length is not None:
+            text = text[:length].ljust(length)
+        for i, char in enumerate(text):
+            address = start_address - i if descending else start_address + i
+            self.set_code(address, ord(char.encode('iso-8859-1')))
+    
+    def get_status(self, addr):
+        return self._get_fbm_status(self.read_status(addr)[0])
+    
+    def d_set_module_data(self, module_data):
+        # Compatibility function for SplitFlapDisplay class
+        for addr, code in module_data:
+            self.set_code(addr, code)
+    
+    def d_update(self):
+        # Compatibility function for SplitFlapDisplay class
         self.set_all()
```

### Comparing `pyFIS-1.8.1/pyfis/krone/k9000_hlst.py` & `pyFIS-1.9.0/pyfis/krone/k9000_hlst.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-"""
-Copyright (C) 2019 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-
-from .k9000_rs485 import Krone9000RS485Controller
-
-
-class Krone9000HLST(Krone9000RS485Controller):
-    """
-    Controls a HLST (Heizungs- und Lichtsteuerung)
-    (heater, fan and light control) board.
-    """
-    
-    BOARD_ID = 0x10
-    BOARD_NAME = "HLST"
-    
-    CMD_GET_STATUS = 0x01
-    CMD_LOCK = 0xC6
-    CMD_UNLOCK = 0xC7
-    CMD_CONTROL = 0x0A
-    
-    def _build_parameters(self, light, heater, fan, force_heater, force_fan, low_min_temp):
-        """
-        light: 1=on, 0=off
-        heater: 1=on, 0=off
-        fan: 1=on, 0=off
-        force_heater: 1=force on, 0=automatic
-        force_fan: 1=force on, 0=automatic
-        low_min_temp: 1=-20°C temperature limit, 0=0°C temperature limit
-        """
-        parameter_byte = 0x00
-        parameter_byte |= int(light) << 7
-        parameter_byte |= int(heater) << 6
-        parameter_byte |= int(fan) << 5
-        parameter_byte |= int(force_heater) << 2
-        parameter_byte |= int(force_fan) << 1
-        parameter_byte |= int(low_min_temp)
-        return parameter_byte
-    
-    def get_status(self):
-        # Get the status of the FBK board
-        payload = self.send_command(self.CMD_GET_STATUS, response=True)
-        stat1 = payload[1]
-        stat2 = payload[2]
-        status = {
-            'comm_err': bool(stat1 & 0x40),
-            'reset': bool(stat1 & 0x20),
-            'locked': bool(stat1 & 0x10),
-            'light_err': bool(stat1 & 0x08),
-            'hlst_err': bool(stat1 & 0x04),
-            'force_ctrl': bool(stat1 & 0x02),
-            'low_min_temp': bool(stat1 & 0x01),
-            'light_on_set': bool(stat2 & 0x80),
-            'heater_on': bool(stat2 & 0x40),
-            'fan_on': bool(stat2 & 0x20),
-            'light_on_feedback': bool(stat2 & 0x10),
-            'temp_above_40c': bool(stat2 & 0x08),
-            'temp_above_0c': bool(stat2 & 0x04),
-            'temp_above_neg20c': bool(stat2 & 0x02),
-            'sw_ver': f"{payload[3]}.{payload[4]}"
-        }
-        return status
-    
-    def lock(self):
-        # Lock the entire HLST
-        return self.send_command(self.CMD_LOCK)
-    
-    def unlock(self):
-        # Unlock the entire HLST
-        return self.send_command(self.CMD_UNLOCK)
-    
-    def control(self, light, heater, fan, force_heater, force_fan, low_min_temp):
-        return self.send_command(self.CMD_CONTROL, self._build_parameters(light, heater, fan, force_heater, force_fan, low_min_temp))
+"""
+Copyright (C) 2019 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+
+from .k9000_rs485 import Krone9000RS485Controller
+
+
+class Krone9000HLST(Krone9000RS485Controller):
+    """
+    Controls a HLST (Heizungs- und Lichtsteuerung)
+    (heater, fan and light control) board.
+    """
+    
+    BOARD_ID = 0x10
+    BOARD_NAME = "HLST"
+    
+    CMD_GET_STATUS = 0x01
+    CMD_LOCK = 0xC6
+    CMD_UNLOCK = 0xC7
+    CMD_CONTROL = 0x0A
+    
+    def _build_parameters(self, light, heater, fan, force_heater, force_fan, low_min_temp):
+        """
+        light: 1=on, 0=off
+        heater: 1=on, 0=off
+        fan: 1=on, 0=off
+        force_heater: 1=force on, 0=automatic
+        force_fan: 1=force on, 0=automatic
+        low_min_temp: 1=-20°C temperature limit, 0=0°C temperature limit
+        """
+        parameter_byte = 0x00
+        parameter_byte |= int(light) << 7
+        parameter_byte |= int(heater) << 6
+        parameter_byte |= int(fan) << 5
+        parameter_byte |= int(force_heater) << 2
+        parameter_byte |= int(force_fan) << 1
+        parameter_byte |= int(low_min_temp)
+        return parameter_byte
+    
+    def get_status(self):
+        # Get the status of the FBK board
+        payload = self.send_command(self.CMD_GET_STATUS, response=True)
+        stat1 = payload[1]
+        stat2 = payload[2]
+        status = {
+            'comm_err': bool(stat1 & 0x40),
+            'reset': bool(stat1 & 0x20),
+            'locked': bool(stat1 & 0x10),
+            'light_err': bool(stat1 & 0x08),
+            'hlst_err': bool(stat1 & 0x04),
+            'force_ctrl': bool(stat1 & 0x02),
+            'low_min_temp': bool(stat1 & 0x01),
+            'light_on_set': bool(stat2 & 0x80),
+            'heater_on': bool(stat2 & 0x40),
+            'fan_on': bool(stat2 & 0x20),
+            'light_on_feedback': bool(stat2 & 0x10),
+            'temp_above_40c': bool(stat2 & 0x08),
+            'temp_above_0c': bool(stat2 & 0x04),
+            'temp_above_neg20c': bool(stat2 & 0x02),
+            'sw_ver': f"{payload[3]}.{payload[4]}"
+        }
+        return status
+    
+    def lock(self):
+        # Lock the entire HLST
+        return self.send_command(self.CMD_LOCK)
+    
+    def unlock(self):
+        # Unlock the entire HLST
+        return self.send_command(self.CMD_UNLOCK)
+    
+    def control(self, light, heater, fan, force_heater, force_fan, low_min_temp):
+        return self.send_command(self.CMD_CONTROL, self._build_parameters(light, heater, fan, force_heater, force_fan, low_min_temp))
```

### Comparing `pyFIS-1.8.1/pyfis/krone/k9000_rs485.py` & `pyFIS-1.9.0/pyfis/krone/k9000_rs485.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-"""
-Copyright (C) 2019 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-import time
-
-from .exceptions import CommunicationError, NACKError, BusyError
-
-
-class Krone9000RS485Controller:
-    """
-    Basic control scheme for the internal RS485 bus
-    in the KRONE 9000 system.
-    """
-    
-    FLAG_ACK = 0x80
-    
-    CTRL_READ = 0x01
-    CTRL_WRITE_SINGLE = 0x02
-    CTRL_WRITE_BLOCK = 0x04
-    
-    STATUS_ACK = 0x06
-    STATUS_BUSY = 0x10
-    STATUS_NACK = 0x15
-    
-    MAX_CHUNK_SIZE = 128
-    RETRY_COUNT = 10
-    RETRY_INTERVAL = 0.2
-
-    def __init__(self, port, address, timeout = 1.0, debug = False, exclusive = False):
-        self.address = address
-        self.debug = debug
-        if isinstance(port, serial.Serial):
-            self.port = port
-        else:
-            self.port = serial.Serial(port, baudrate=19200, timeout=timeout, exclusive=exclusive)
-    
-    @staticmethod
-    def _chunks(lst, n):
-        """Yield successive n-sized chunks from lst."""
-        for i in range(0, len(lst), n):
-            yield lst[i:i + n]
-    
-    def debug_print(self, data, receive = False):
-        if self.debug:
-            print(f"{self.BOARD_NAME:<4} {self.address} {'RX' if receive else 'TX'}: " + " ".join((format(x, "02X") for x in data)))
-    
-    def make_checksum(self, payload):
-        checksum = 0x00
-        for byte in payload:
-            checksum ^= byte
-        return checksum
-    
-    def check_checksum(self, data):
-        checksum = self.make_checksum(data[2:-1])
-        return checksum == data[-1]
-            
-    def send_command(self, command, parameters = None, response = False, ack = True, block = False):
-        def _chunks(lst, n):
-            # Yield successive n-sized chunks from lst.
-            for i in range(0, len(lst), n):
-                yield lst[i:i + n]
-        
-        data = [command]
-        if parameters is not None:
-            if type(parameters) in (list, tuple):
-                data.extend(parameters)
-            else:
-                data.append(parameters)
-        
-        if len(data) > self.MAX_CHUNK_SIZE and block == False:
-            raise CommunicationError("Data too long for single-block transfer. Use multi-block mode!")
-        
-        if response:
-            control = self.CTRL_READ
-        else:
-            if block:
-                control = self.CTRL_WRITE_BLOCK
-            else:
-                control = self.CTRL_WRITE_SINGLE
-        
-        if ack:
-            control |= self.FLAG_ACK
-        
-        for chunk_id, chunk in enumerate(_chunks(data, self.MAX_CHUNK_SIZE)):
-            for retry in range(self.RETRY_COUNT):
-                payload = [self.BOARD_ID, self.address, 0x00, control, chunk_id + 1] + chunk + [0x00]
-                length = len(payload)
-                payload[2] = length
-                checksum = self.make_checksum(payload)
-                cmd_bytes = [0xFF, 0xFF] + payload + [checksum]
-                
-                # Debug output if enabled
-                self.debug_print(cmd_bytes)
-                
-                # Send it
-                self.port.write(bytearray(cmd_bytes))
-                
-                # Check status
-                if not response:
-                    if control & self.FLAG_ACK:
-                        try:
-                            self.check_status()
-                        except BusyError:
-                            if retry >= self.RETRY_COUNT - 1:
-                                raise
-                            else:
-                                time.sleep(self.RETRY_INTERVAL)
-                        else:
-                            break
-                else:
-                    break
-
-        # Read response
-        if response:
-            return self.read_response()
-        else:
-            return None
-    
-    def check_status(self):
-        status = bytearray(self.port.read(1))[0]
-        self.debug_print([status], receive=True)
-        if status == self.STATUS_ACK:
-            return True
-        elif status == self.STATUS_BUSY:
-            raise BusyError()
-        elif status == self.STATUS_NACK:
-            raise NACKError()
-        else:
-            raise CommunicationError(f"Unknown status byte {status:02X}")
-    
-    def read_response(self):
-        data = bytearray()
-        header = bytearray(self.port.read(4))
-        if len(header) != 4:
-            if len(header) == 1:
-                if header[0] == self.STATUS_BUSY:
-                    raise BusyError()
-                if header[0] == self.STATUS_NACK:
-                    raise NACKError()
-            header_fmt = " ".join((format(x, "02X") for x in header))
-            raise CommunicationError(f"Incomplete header: {header_fmt}")
-        if header[0] != 0xFF or header[1] != 0xFF:
-            raise CommunicationError(f"Invalid start sequence {header[0]:02X} {header[1]:02X}")
-        if header[2] != self.BOARD_ID:
-            raise CommunicationError(f"Invalid board ID {header[2]:02X}")
-        if header[3] != self.address:
-            raise CommunicationError(f"Invalid address {header[3]:02X}")
-        data.extend(header)
-        
-        length = bytearray(self.port.read(1))[0]
-        payload = bytearray(self.port.read(length - 3))
-        checksum = bytearray(self.port.read(1))[0]
-        
-        data.append(length)
-        data.extend(payload)
-        data.append(checksum)
-        
-        self.debug_print(data, receive=True)
-        if not self.check_checksum(data):
-            raise CommunicationError("Checksum mismatch")
-        return payload[2:-1]
-    
-    def send_heartbeat(self):
-        cmd_bytes = [0xFF, 0xFF, self.BOARD_ID, self.address, 0x00]
-        self.debug_print(cmd_bytes)
+"""
+Copyright (C) 2019 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+import time
+
+from .exceptions import CommunicationError, NACKError, BusyError
+
+
+class Krone9000RS485Controller:
+    """
+    Basic control scheme for the internal RS485 bus
+    in the KRONE 9000 system.
+    """
+    
+    FLAG_ACK = 0x80
+    
+    CTRL_READ = 0x01
+    CTRL_WRITE_SINGLE = 0x02
+    CTRL_WRITE_BLOCK = 0x04
+    
+    STATUS_ACK = 0x06
+    STATUS_BUSY = 0x10
+    STATUS_NACK = 0x15
+    
+    MAX_CHUNK_SIZE = 128
+    RETRY_COUNT = 10
+    RETRY_INTERVAL = 0.2
+
+    def __init__(self, port, address, timeout = 1.0, debug = False, exclusive = False):
+        self.address = address
+        self.debug = debug
+        if isinstance(port, serial.Serial):
+            self.port = port
+        else:
+            self.port = serial.Serial(port, baudrate=19200, timeout=timeout, exclusive=exclusive)
+    
+    @staticmethod
+    def _chunks(lst, n):
+        """Yield successive n-sized chunks from lst."""
+        for i in range(0, len(lst), n):
+            yield lst[i:i + n]
+    
+    def debug_print(self, data, receive = False):
+        if self.debug:
+            print(f"{self.BOARD_NAME:<4} {self.address} {'RX' if receive else 'TX'}: " + " ".join((format(x, "02X") for x in data)))
+    
+    def make_checksum(self, payload):
+        checksum = 0x00
+        for byte in payload:
+            checksum ^= byte
+        return checksum
+    
+    def check_checksum(self, data):
+        checksum = self.make_checksum(data[2:-1])
+        return checksum == data[-1]
+            
+    def send_command(self, command, parameters = None, response = False, ack = True, block = False):
+        def _chunks(lst, n):
+            # Yield successive n-sized chunks from lst.
+            for i in range(0, len(lst), n):
+                yield lst[i:i + n]
+        
+        data = [command]
+        if parameters is not None:
+            if type(parameters) in (list, tuple):
+                data.extend(parameters)
+            else:
+                data.append(parameters)
+        
+        if len(data) > self.MAX_CHUNK_SIZE and block == False:
+            raise CommunicationError("Data too long for single-block transfer. Use multi-block mode!")
+        
+        if response:
+            control = self.CTRL_READ
+        else:
+            if block:
+                control = self.CTRL_WRITE_BLOCK
+            else:
+                control = self.CTRL_WRITE_SINGLE
+        
+        if ack:
+            control |= self.FLAG_ACK
+        
+        for chunk_id, chunk in enumerate(_chunks(data, self.MAX_CHUNK_SIZE)):
+            for retry in range(self.RETRY_COUNT):
+                payload = [self.BOARD_ID, self.address, 0x00, control, chunk_id + 1] + chunk + [0x00]
+                length = len(payload)
+                payload[2] = length
+                checksum = self.make_checksum(payload)
+                cmd_bytes = [0xFF, 0xFF] + payload + [checksum]
+                
+                # Debug output if enabled
+                self.debug_print(cmd_bytes)
+                
+                # Send it
+                self.port.write(bytearray(cmd_bytes))
+                
+                # Check status
+                if not response:
+                    if control & self.FLAG_ACK:
+                        try:
+                            self.check_status()
+                        except BusyError:
+                            if retry >= self.RETRY_COUNT - 1:
+                                raise
+                            else:
+                                time.sleep(self.RETRY_INTERVAL)
+                        else:
+                            break
+                else:
+                    break
+
+        # Read response
+        if response:
+            return self.read_response()
+        else:
+            return None
+    
+    def check_status(self):
+        status = bytearray(self.port.read(1))[0]
+        self.debug_print([status], receive=True)
+        if status == self.STATUS_ACK:
+            return True
+        elif status == self.STATUS_BUSY:
+            raise BusyError()
+        elif status == self.STATUS_NACK:
+            raise NACKError()
+        else:
+            raise CommunicationError(f"Unknown status byte {status:02X}")
+    
+    def read_response(self):
+        data = bytearray()
+        header = bytearray(self.port.read(4))
+        if len(header) != 4:
+            if len(header) == 1:
+                if header[0] == self.STATUS_BUSY:
+                    raise BusyError()
+                if header[0] == self.STATUS_NACK:
+                    raise NACKError()
+            header_fmt = " ".join((format(x, "02X") for x in header))
+            raise CommunicationError(f"Incomplete header: {header_fmt}")
+        if header[0] != 0xFF or header[1] != 0xFF:
+            raise CommunicationError(f"Invalid start sequence {header[0]:02X} {header[1]:02X}")
+        if header[2] != self.BOARD_ID:
+            raise CommunicationError(f"Invalid board ID {header[2]:02X}")
+        if header[3] != self.address:
+            raise CommunicationError(f"Invalid address {header[3]:02X}")
+        data.extend(header)
+        
+        length = bytearray(self.port.read(1))[0]
+        payload = bytearray(self.port.read(length - 3))
+        checksum = bytearray(self.port.read(1))[0]
+        
+        data.append(length)
+        data.extend(payload)
+        data.append(checksum)
+        
+        self.debug_print(data, receive=True)
+        if not self.check_checksum(data):
+            raise CommunicationError("Checksum mismatch")
+        return payload[2:-1]
+    
+    def send_heartbeat(self):
+        cmd_bytes = [0xFF, 0xFF, self.BOARD_ID, self.address, 0x00]
+        self.debug_print(cmd_bytes)
         self.port.write(bytearray(cmd_bytes))
```

### Comparing `pyFIS-1.8.1/pyfis/krone/util.py` & `pyFIS-1.9.0/pyfis/krone/util.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-import time
-
-
-def calibrate_fbm_interactive(fbm, addr):
-    """
-    Interactive process for calibrating the flap count
-    and home position on small FBM units
-    """
-    print("\nStep 0: Testing home position")
-    print("Check if calibration is necessary by moving to the home position")
-    print("and seeing if the unit hits it correctly.")
-    input("Press Enter to start.")
-    fbm.set_home()
-    print("\nWait for the unit to stop rotating!")
-    time.sleep(3)
-    res = ""
-    while res not in ("Y", "N"):
-        res = input("Was the home position reached? [Y/N]: ").upper()
-        if res == "Y":
-            print("\nGreat! No need to calibrate.")
-            return
-    
-    print("Step 1: Flap count (BR1) calibration")
-    print("The unit will rotate once or twice and stop.")
-    print("There is no need to do anything while it is rotating.")
-    input("Press Enter to start.")
-    fbm.start_calibration_br1()
-    print("\nWait for the unit to stop rotating!")
-    time.sleep(5)
-    
-    success = False
-    back_to_step_2 = False
-    while not success:
-        exit_step_2 = False
-        while not exit_step_2:
-            print("\nStep 2: Home position (BR2) calibration")
-            print("The unit will start rotating.")
-            print("As soon as the desired home position is reached, hit Enter.")
-            print("This might take a few tries.")
-            print("The unit should complete one more rotation after you hit Enter!")
-            print("If the unit stops rotating as soon as you hit Enter,")
-            print("your timing was not correct. Try again in this case.")
-            input("Press Enter to start and get ready to hit Enter again!")
-            fbm.start_calibration_br2()
-            input("Press Enter if the home position is reached!")
-            fbm.stop_calibration()
-            print("\nWait for the unit to stop rotating!")
-            res = ""
-            while res not in ("Y", "N"):
-                res = input("Was the desired position reached? [Y/N]: ").upper()
-                if res == "Y":
-                    exit_step_2 = True
-        
-        print("\nStep 3: Testing home position")
-        print("Test the calibration by moving to the home position again")
-        print("and seeing if the unit hits it correctly.")
-        input("Press Enter to start.")
-        fbm.set_home()
-        print("\nWait for the unit to stop rotating!")
-        time.sleep(3)
-        res = ""
-        while res not in ("Y", "N"):
-            res = input("Was the home position reached? [Y/N]: ").upper()
-            if res == "N":
-                success = False
-                back_to_step_2 = True
-                break
-            elif res == "Y":
-                back_to_step_2 = False
-                break
-        
-        if back_to_step_2:
-            continue
-        
-        exit_step_4 = False
-        while not exit_step_4:
-            print("\nStep 4: Testing characters")
-            print("Test the calibration by entering letters")
-            print("and seeing if the unit hits them correctly.")
-            char = ""
-            while len(char) != 1 or ord(char) not in range(128):
-                char = input("Enter a character to test or nothing to finish: ").upper()
-                if char == "":
-                    exit_step_4 = True
-                    success = True
-                    break
-                if len(char) > 1 or ord(char) not in range(128):
-                    continue
-                else:
-                    fbm.set_code(addr, ord(char))
-                    time.sleep(0.1)
-                    fbm.set_all()
-                    time.sleep(0.1)
-                    res = ""
-                    while res not in ("Y", "N"):
-                        res = input("Was the desired character hit? [Y/N]: ").upper()
-                        if res == "N":
-                            exit_step_4 = True
-                            success = False
-    
-    fbm.set_home()
-    print("\nGreat! The unit is now calibrated.")
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+import time
+
+
+def calibrate_fbm_interactive(fbm, addr):
+    """
+    Interactive process for calibrating the flap count
+    and home position on small FBM units
+    """
+    print("\nStep 0: Testing home position")
+    print("Check if calibration is necessary by moving to the home position")
+    print("and seeing if the unit hits it correctly.")
+    input("Press Enter to start.")
+    fbm.set_home()
+    print("\nWait for the unit to stop rotating!")
+    time.sleep(3)
+    res = ""
+    while res not in ("Y", "N"):
+        res = input("Was the home position reached? [Y/N]: ").upper()
+        if res == "Y":
+            print("\nGreat! No need to calibrate.")
+            return
+    
+    print("Step 1: Flap count (BR1) calibration")
+    print("The unit will rotate once or twice and stop.")
+    print("There is no need to do anything while it is rotating.")
+    input("Press Enter to start.")
+    fbm.start_calibration_br1()
+    print("\nWait for the unit to stop rotating!")
+    time.sleep(5)
+    
+    success = False
+    back_to_step_2 = False
+    while not success:
+        exit_step_2 = False
+        while not exit_step_2:
+            print("\nStep 2: Home position (BR2) calibration")
+            print("The unit will start rotating.")
+            print("As soon as the desired home position is reached, hit Enter.")
+            print("This might take a few tries.")
+            print("The unit should complete one more rotation after you hit Enter!")
+            print("If the unit stops rotating as soon as you hit Enter,")
+            print("your timing was not correct. Try again in this case.")
+            input("Press Enter to start and get ready to hit Enter again!")
+            fbm.start_calibration_br2()
+            input("Press Enter if the home position is reached!")
+            fbm.stop_calibration()
+            print("\nWait for the unit to stop rotating!")
+            res = ""
+            while res not in ("Y", "N"):
+                res = input("Was the desired position reached? [Y/N]: ").upper()
+                if res == "Y":
+                    exit_step_2 = True
+        
+        print("\nStep 3: Testing home position")
+        print("Test the calibration by moving to the home position again")
+        print("and seeing if the unit hits it correctly.")
+        input("Press Enter to start.")
+        fbm.set_home()
+        print("\nWait for the unit to stop rotating!")
+        time.sleep(3)
+        res = ""
+        while res not in ("Y", "N"):
+            res = input("Was the home position reached? [Y/N]: ").upper()
+            if res == "N":
+                success = False
+                back_to_step_2 = True
+                break
+            elif res == "Y":
+                back_to_step_2 = False
+                break
+        
+        if back_to_step_2:
+            continue
+        
+        exit_step_4 = False
+        while not exit_step_4:
+            print("\nStep 4: Testing characters")
+            print("Test the calibration by entering letters")
+            print("and seeing if the unit hits them correctly.")
+            char = ""
+            while len(char) != 1 or ord(char) not in range(128):
+                char = input("Enter a character to test or nothing to finish: ").upper()
+                if char == "":
+                    exit_step_4 = True
+                    success = True
+                    break
+                if len(char) > 1 or ord(char) not in range(128):
+                    continue
+                else:
+                    fbm.set_code(addr, ord(char))
+                    time.sleep(0.1)
+                    fbm.set_all()
+                    time.sleep(0.1)
+                    res = ""
+                    while res not in ("Y", "N"):
+                        res = input("Was the desired character hit? [Y/N]: ").upper()
+                        if res == "N":
+                            exit_step_4 = True
+                            success = False
+    
+    fbm.set_home()
+    print("\nGreat! The unit is now calibrated.")
```

### Comparing `pyFIS-1.8.1/pyfis/lawo/__init__.py` & `pyFIS-1.9.0/pyfis/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""
-Copyright (C) 2016 - 2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .mono_serial import SerialMONOMaster
-from .lawo_font import LawoFont
+"""
+Copyright (C) 2016 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .metadata import version as __version__
```

### Comparing `pyFIS-1.8.1/pyfis/lawo/lawo_font.py` & `pyFIS-1.9.0/pyfis/lawo/lawo_font.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-"""
-Copyright (C) 2016 - 2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import argparse
-import crccheck
-import math
-
-from PIL import Image, ImageDraw, ImageFont
-from pprint import pprint
-
-
-class LawoFont:
-    """
-    LAWO font files, typically named FONTNAME.FXX, where XX is the glyph height
-    """
-    
-    def __init__(self):
-        self.name = None
-        self.change_signature = None
-        self.file_size = None
-        self.file_name = None
-        self.glyph_h = None
-        self.baseline = None
-        self.min_char = None
-        self.max_char = None
-        self.char_spacing = None
-        self.preview_text = None
-        self.num_blocks = None
-        self.glyph_metadata = None
-        self.glyph_data = None
-        self.num_glyphs = None
-        self.widest_glyph = None
-        self.narrowest_glyph = None
-        self.charset = None
-    
-    @staticmethod
-    def _read_c_str(data):
-        result = ""
-        for byte in data:
-            if byte == 0x00:
-                return result
-            else:
-                result += bytes([byte]).decode('cp1252')
-        return result
-    
-    @staticmethod
-    def _read_until_double_null(data):
-        result = ""
-        for i, byte in enumerate(data):
-            if byte == 0x00 and i < len(data) - 1 and data[i+1] == 0x00:
-                return result
-            else:
-                result += bytes([byte]).decode('cp1252')
-        return result
-    
-    @staticmethod
-    def _chunks(lst, n):
-        for i in range(0, len(lst), n):
-            yield lst[i:i + n]
-    
-    def read_file(self, file):
-        with open(file, 'rb') as f:
-            data = f.read()
-        
-        self.name = self._read_c_str(data[6:14]).strip()
-        self.change_signature = data[16] << 8 | data[7] # Changes with every file change
-        self.file_size = data[20] << 8 | data[21]
-        self.file_name = self._read_c_str(data[32:45])
-        self.glyph_h = data[45]
-        self.baseline = data[46]
-        self.min_char = data[47]
-        self.max_char = data[48]
-        self.char_spacing = data[52]
-        self.preview_text = self._read_c_str(data[56:60])
-        self.num_blocks = data[60] << 8 | data[61] # A block is a column of bytes with a length equal to the glyph height
-        self.glyph_metadata = dict(zip(range(self.min_char, self.max_char+1), [None]*(self.max_char-self.min_char+1)))
-        self.glyph_data = dict(zip(range(self.min_char, self.max_char+1), [None]*(self.max_char-self.min_char+1)))
-        
-        extra_data_start = 70 + 3 * (self.max_char - self.min_char + 1)
-        if data[extra_data_start] == 0x00:
-            # There is no extra data block, just skip the two 0x00 bytes
-            glyph_data_block_start = extra_data_start + 2
-        else:
-            # There is an extra data block
-            # Read it and skip the null terminator and the two 0x00 bytes
-            self.extra_data = self._read_until_double_null(data[extra_data_start:])
-            glyph_data_block_start = extra_data_start + len(self.extra_data) + 3
-        
-        self.num_glyphs = 0
-        self.widest_glyph = 0
-        self.narrowest_glyph = 255
-        self.charset = ""
-        for c in range(self.min_char, self.max_char+1):
-            i = 70 + 3 * (c - self.min_char)
-            self.glyph_metadata[c] = {
-                'glyph_w': data[i],
-                'offset': data[i+1] << 8 | data[i+2] # Offset from start of glyph data block in bits
-            }
-            if data[i] > 0:
-                self.num_glyphs += 1
-                self.charset += bytes([c]).decode('cp1252')
-                if data[i] > self.widest_glyph:
-                    self.widest_glyph = data[i]
-                if data[i] < self.narrowest_glyph:
-                    self.narrowest_glyph = data[i]
-        
-        for c in range(self.min_char, self.max_char+1):
-            width = self.glyph_metadata[c]['glyph_w']
-            glyph_start = glyph_data_block_start + self.glyph_metadata[c]['offset'] // 8
-            i = glyph_start
-            glyph_data = []
-            for y in range(self.glyph_h):
-                for x_byte in range(math.ceil(width / 8)):
-                    glyph_data.append(data[i + x_byte])
-                i += self.num_blocks
-            self.glyph_data[c] = glyph_data
-    
-    def print_info(self):
-        print("\n".join([f"Name:              {self.name}",
-                         f"File Name:         {self.file_name}",
-                         f"File Size:         {self.file_size} Bytes",
-                         f"Change Sig:        {self.change_signature}",
-                         f"Glyph Height:      {self.glyph_h} px",
-                         f"Glyph Baseline:    {self.baseline} px",
-                         f"Glyph Spacing:     {self.char_spacing} px",
-                         f"Widest Glyph:      {self.widest_glyph} px",
-                         f"Narrowest Glyph:   {self.narrowest_glyph} px",
-                         f"Lowest Character:  {self.min_char} ({bytes([self.min_char]).decode('cp1252')})",
-                         f"Highest Character: {self.max_char} ({bytes([self.max_char]).decode('cp1252')})",
-                         f"Preview Text:      {self.preview_text}",
-                         f"# Glyphs:          {self.num_glyphs}",
-                         f"# Data Blocks:     {self.num_blocks}",
-                         f"Character Set:     {self.charset}"]))
-    
-    def get_glyph_width(self, code):
-        if code not in self.glyph_metadata:
-            return 0
-        return self.glyph_metadata[code]['glyph_w']
-    
-    def render_glyph(self, code):
-        if code not in self.glyph_metadata:
-            return None
-        glyph_metadata = self.glyph_metadata[code]
-        glyph_data = self.glyph_data[code]
-        width = glyph_metadata['glyph_w']
-        height = self.glyph_h
-        if width == 0:
-            return None
-        img = Image.new('L', (width, height), 0)
-        px = img.load()
-        i = 0
-        for y in range(height):
-            for x_byte in range(math.ceil(width / 8)):
-                byte = glyph_data[i]
-                for x_bit in range(8):
-                    x = x_byte * 8 + 7 - x_bit
-                    if x >= width:
-                        continue
-                    px[x,y] = 255 if (byte & (1 << x_bit)) else 0
-                i += 1
-        return img
-    
-    def render_glyph_table(self, x_spacing=5, x_offset=25, y_spacing=5, row_min_height=12, num_cols=16):
-        num_chars = self.max_char - self.min_char + 1
-        
-        # Calculate the displayed table range based on the font's character range
-        # This new range is sure to leave no half filled rows
-        table_range_min = self.min_char - (self.min_char % num_cols)
-        table_range_max = self.max_char - (self.max_char % num_cols) + num_cols - 1
-        
-        row_list = range(table_range_min, table_range_max + 1, num_cols)
-        num_rows = len(row_list)
-        row_height = max(row_min_height, self.glyph_h) + y_spacing
-        
-        # Calculate widths of each column based on maximum glyph width in that column
-        # taking into account spacings
-        col_widths = {}
-        for row, char_code_base in enumerate(row_list):
-            for col in range(num_cols):
-                char_code = char_code_base + col
-                if char_code < 0 or char_code > 255:
-                    continue
-                if col not in col_widths or self.glyph_metadata.get(char_code, {'glyph_w': 0})['glyph_w'] + x_spacing + x_offset > col_widths[col]:
-                    col_widths[col] = self.glyph_metadata[char_code]['glyph_w'] + x_spacing + x_offset
-        
-        # Calculate X start positions of each column
-        x_tmp = 0
-        col_offsets = {}
-        for col, width in sorted(col_widths.items(), key=lambda i: i[0]):
-            col_offsets[col] = x_tmp
-            x_tmp += width
-        
-        # Calculate total glyph table dimensions
-        width = sum(col_widths.values())
-        height = num_rows * row_height
-        
-        # Create image
-        table = Image.new('L', (width, height), 0)
-        draw = ImageDraw.Draw(table)
-        font = ImageFont.truetype("arial.ttf", row_min_height)
-        
-        # Render grid, skipping the first row / column
-        for row, char_code_base in list(enumerate(row_list))[1:]:
-            y = row * row_height
-            draw.line((0, y, width - 1, y), 255, 1)
-        
-        for col in range(1, num_cols):
-            x = col_offsets[col]
-            draw.line((x, 0, x, height - 1), 255, 1)
-        
-        # Render glyphs
-        for row, char_code_base in enumerate(row_list):
-            for col in range(num_cols):
-                char_code = char_code_base + col
-                x_base = col_offsets[col]
-                y_base = row * row_height
-                draw.text((x_base + 3, y_base), str(char_code), 255, font)
-                glyph = self.render_glyph(char_code)
-                if glyph:
-                    table.paste(glyph, (x_base + x_offset + math.ceil(x_spacing / 2), y_base + math.ceil(y_spacing / 2)))
-        
-        return table
-    
-    def render_text(self, text):
-        chars = bytes(text, 'cp1252', 'ignore')
-        width = 0
-        for code in chars:
-            width += self.get_glyph_width(code) + self.char_spacing
-        width -= self.char_spacing
-        
-        img = Image.new('L', (width, self.glyph_h), 0)
-        x = 0
-        for code in chars:
-            glyph = self.render_glyph(code)
-            img.paste(glyph, (x, 0))
-            x += self.get_glyph_width(code) + self.char_spacing
-        return img
-
-
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser("Tool for using LAWO font files")
-    parser.add_argument("-f", "--file", type=str, required=True, help="Font file")
-    parser.add_argument("-i", "--info", action='store_true', help="Show font info")
-    parser.add_argument("-sg", "--show-glyph", type=int, required=False, help="Show glyph with given code")
-    parser.add_argument("-gt", "--glyph-table", action='store_true', help="Show glyph table")
-    parser.add_argument("-rt", "--render-text", type=str, required=False, help="Render given text")
-    parser.add_argument("-o", "--output", type=str, required=False, help="Save output images to file instead of showing")
-    args = parser.parse_args()
-    
-    font = LawoFont()
-    font.read_file(args.file)
-    
-    if args.info:
-        font.print_info()
-    
-    if args.render_text is not None:
-        img = font.render_text(args.render_text)
-        if args.output:
-            img.save(args.output)
-        else:
-            img.show()
-    elif args.glyph_table:
-        img = font.render_glyph_table()
-        if args.output:
-            img.save(args.output)
-        else:
-            img.show()
-    elif args.show_glyph is not None:
-        img = font.render_glyph(args.show_glyph)
-        if img:
-            if args.output:
-                img.save(args.output)
-            else:
-                img.show()
-        else:
-            print("Glyph is empty")
+"""
+Copyright (C) 2016 - 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import argparse
+import crccheck
+import math
+
+from PIL import Image, ImageDraw, ImageFont
+from pprint import pprint
+
+
+class LawoFont:
+    """
+    LAWO font files, typically named FONTNAME.FXX, where XX is the glyph height
+    """
+    
+    def __init__(self):
+        self.name = None
+        self.change_signature = None
+        self.file_size = None
+        self.file_name = None
+        self.glyph_h = None
+        self.baseline = None
+        self.min_char = None
+        self.max_char = None
+        self.char_spacing = None
+        self.preview_text = None
+        self.num_blocks = None
+        self.glyph_metadata = None
+        self.glyph_data = None
+        self.num_glyphs = None
+        self.widest_glyph = None
+        self.narrowest_glyph = None
+        self.charset = None
+    
+    @staticmethod
+    def _read_c_str(data):
+        result = ""
+        for byte in data:
+            if byte == 0x00:
+                return result
+            else:
+                result += bytes([byte]).decode('cp1252')
+        return result
+    
+    @staticmethod
+    def _read_until_double_null(data):
+        result = ""
+        for i, byte in enumerate(data):
+            if byte == 0x00 and i < len(data) - 1 and data[i+1] == 0x00:
+                return result
+            else:
+                result += bytes([byte]).decode('cp1252')
+        return result
+    
+    @staticmethod
+    def _chunks(lst, n):
+        for i in range(0, len(lst), n):
+            yield lst[i:i + n]
+    
+    def read_file(self, file):
+        with open(file, 'rb') as f:
+            data = f.read()
+        
+        self.name = self._read_c_str(data[6:14]).strip()
+        self.change_signature = data[16] << 8 | data[7] # Changes with every file change
+        self.file_size = data[20] << 8 | data[21]
+        self.file_name = self._read_c_str(data[32:45])
+        self.glyph_h = data[45]
+        self.baseline = data[46]
+        self.min_char = data[47]
+        self.max_char = data[48]
+        self.char_spacing = data[52]
+        self.preview_text = self._read_c_str(data[56:60])
+        self.num_blocks = data[60] << 8 | data[61] # A block is a column of bytes with a length equal to the glyph height
+        self.glyph_metadata = dict(zip(range(self.min_char, self.max_char+1), [None]*(self.max_char-self.min_char+1)))
+        self.glyph_data = dict(zip(range(self.min_char, self.max_char+1), [None]*(self.max_char-self.min_char+1)))
+        
+        extra_data_start = 70 + 3 * (self.max_char - self.min_char + 1)
+        if data[extra_data_start] == 0x00:
+            # There is no extra data block, just skip the two 0x00 bytes
+            glyph_data_block_start = extra_data_start + 2
+        else:
+            # There is an extra data block
+            # Read it and skip the null terminator and the two 0x00 bytes
+            self.extra_data = self._read_until_double_null(data[extra_data_start:])
+            glyph_data_block_start = extra_data_start + len(self.extra_data) + 3
+        
+        self.num_glyphs = 0
+        self.widest_glyph = 0
+        self.narrowest_glyph = 255
+        self.charset = ""
+        for c in range(self.min_char, self.max_char+1):
+            i = 70 + 3 * (c - self.min_char)
+            self.glyph_metadata[c] = {
+                'glyph_w': data[i],
+                'offset': data[i+1] << 8 | data[i+2] # Offset from start of glyph data block in bits
+            }
+            if data[i] > 0:
+                self.num_glyphs += 1
+                self.charset += bytes([c]).decode('cp1252')
+                if data[i] > self.widest_glyph:
+                    self.widest_glyph = data[i]
+                if data[i] < self.narrowest_glyph:
+                    self.narrowest_glyph = data[i]
+        
+        for c in range(self.min_char, self.max_char+1):
+            width = self.glyph_metadata[c]['glyph_w']
+            glyph_start = glyph_data_block_start + self.glyph_metadata[c]['offset'] // 8
+            i = glyph_start
+            glyph_data = []
+            for y in range(self.glyph_h):
+                for x_byte in range(math.ceil(width / 8)):
+                    glyph_data.append(data[i + x_byte])
+                i += self.num_blocks
+            self.glyph_data[c] = glyph_data
+    
+    def print_info(self):
+        print("\n".join([f"Name:              {self.name}",
+                         f"File Name:         {self.file_name}",
+                         f"File Size:         {self.file_size} Bytes",
+                         f"Change Sig:        {self.change_signature}",
+                         f"Glyph Height:      {self.glyph_h} px",
+                         f"Glyph Baseline:    {self.baseline} px",
+                         f"Glyph Spacing:     {self.char_spacing} px",
+                         f"Widest Glyph:      {self.widest_glyph} px",
+                         f"Narrowest Glyph:   {self.narrowest_glyph} px",
+                         f"Lowest Character:  {self.min_char} ({bytes([self.min_char]).decode('cp1252')})",
+                         f"Highest Character: {self.max_char} ({bytes([self.max_char]).decode('cp1252')})",
+                         f"Preview Text:      {self.preview_text}",
+                         f"# Glyphs:          {self.num_glyphs}",
+                         f"# Data Blocks:     {self.num_blocks}",
+                         f"Character Set:     {self.charset}"]))
+    
+    def get_glyph_width(self, code):
+        if code not in self.glyph_metadata:
+            return 0
+        return self.glyph_metadata[code]['glyph_w']
+    
+    def render_glyph(self, code):
+        if code not in self.glyph_metadata:
+            return None
+        glyph_metadata = self.glyph_metadata[code]
+        glyph_data = self.glyph_data[code]
+        width = glyph_metadata['glyph_w']
+        height = self.glyph_h
+        if width == 0:
+            return None
+        img = Image.new('L', (width, height), 0)
+        px = img.load()
+        i = 0
+        for y in range(height):
+            for x_byte in range(math.ceil(width / 8)):
+                byte = glyph_data[i]
+                for x_bit in range(8):
+                    x = x_byte * 8 + 7 - x_bit
+                    if x >= width:
+                        continue
+                    px[x,y] = 255 if (byte & (1 << x_bit)) else 0
+                i += 1
+        return img
+    
+    def render_glyph_table(self, x_spacing=5, x_offset=25, y_spacing=5, row_min_height=12, num_cols=16):
+        num_chars = self.max_char - self.min_char + 1
+        
+        # Calculate the displayed table range based on the font's character range
+        # This new range is sure to leave no half filled rows
+        table_range_min = self.min_char - (self.min_char % num_cols)
+        table_range_max = self.max_char - (self.max_char % num_cols) + num_cols - 1
+        
+        row_list = range(table_range_min, table_range_max + 1, num_cols)
+        num_rows = len(row_list)
+        row_height = max(row_min_height, self.glyph_h) + y_spacing
+        
+        # Calculate widths of each column based on maximum glyph width in that column
+        # taking into account spacings
+        col_widths = {}
+        for row, char_code_base in enumerate(row_list):
+            for col in range(num_cols):
+                char_code = char_code_base + col
+                if char_code < 0 or char_code > 255:
+                    continue
+                if col not in col_widths or self.glyph_metadata.get(char_code, {'glyph_w': 0})['glyph_w'] + x_spacing + x_offset > col_widths[col]:
+                    col_widths[col] = self.glyph_metadata[char_code]['glyph_w'] + x_spacing + x_offset
+        
+        # Calculate X start positions of each column
+        x_tmp = 0
+        col_offsets = {}
+        for col, width in sorted(col_widths.items(), key=lambda i: i[0]):
+            col_offsets[col] = x_tmp
+            x_tmp += width
+        
+        # Calculate total glyph table dimensions
+        width = sum(col_widths.values())
+        height = num_rows * row_height
+        
+        # Create image
+        table = Image.new('L', (width, height), 0)
+        draw = ImageDraw.Draw(table)
+        font = ImageFont.truetype("arial.ttf", row_min_height)
+        
+        # Render grid, skipping the first row / column
+        for row, char_code_base in list(enumerate(row_list))[1:]:
+            y = row * row_height
+            draw.line((0, y, width - 1, y), 255, 1)
+        
+        for col in range(1, num_cols):
+            x = col_offsets[col]
+            draw.line((x, 0, x, height - 1), 255, 1)
+        
+        # Render glyphs
+        for row, char_code_base in enumerate(row_list):
+            for col in range(num_cols):
+                char_code = char_code_base + col
+                x_base = col_offsets[col]
+                y_base = row * row_height
+                draw.text((x_base + 3, y_base), str(char_code), 255, font)
+                glyph = self.render_glyph(char_code)
+                if glyph:
+                    table.paste(glyph, (x_base + x_offset + math.ceil(x_spacing / 2), y_base + math.ceil(y_spacing / 2)))
+        
+        return table
+    
+    def render_text(self, text):
+        chars = bytes(text, 'cp1252', 'ignore')
+        width = 0
+        for code in chars:
+            width += self.get_glyph_width(code) + self.char_spacing
+        width -= self.char_spacing
+        
+        img = Image.new('L', (width, self.glyph_h), 0)
+        x = 0
+        for code in chars:
+            glyph = self.render_glyph(code)
+            img.paste(glyph, (x, 0))
+            x += self.get_glyph_width(code) + self.char_spacing
+        return img
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser("Tool for using LAWO font files")
+    parser.add_argument("-f", "--file", type=str, required=True, help="Font file")
+    parser.add_argument("-i", "--info", action='store_true', help="Show font info")
+    parser.add_argument("-sg", "--show-glyph", type=int, required=False, help="Show glyph with given code")
+    parser.add_argument("-gt", "--glyph-table", action='store_true', help="Show glyph table")
+    parser.add_argument("-rt", "--render-text", type=str, required=False, help="Render given text")
+    parser.add_argument("-o", "--output", type=str, required=False, help="Save output images to file instead of showing")
+    args = parser.parse_args()
+    
+    font = LawoFont()
+    font.read_file(args.file)
+    
+    if args.info:
+        font.print_info()
+    
+    if args.render_text is not None:
+        img = font.render_text(args.render_text)
+        if args.output:
+            img.save(args.output)
+        else:
+            img.show()
+    elif args.glyph_table:
+        img = font.render_glyph_table()
+        if args.output:
+            img.save(args.output)
+        else:
+            img.show()
+    elif args.show_glyph is not None:
+        img = font.render_glyph(args.show_glyph)
+        if img:
+            if args.output:
+                img.save(args.output)
+            else:
+                img.show()
+        else:
+            print("Glyph is empty")
```

### Comparing `pyFIS-1.8.1/pyfis/lawo/mono_protocol.py` & `pyFIS-1.9.0/pyfis/lawo/mono_protocol.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,378 +1,378 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import math
-import time
-
-try:
-    from PIL import Image
-except ImportError:
-    _HAS_PIL = False
-else:
-    _HAS_PIL = True
-
-class MONOProtocol:
-    """
-    All the logic related to the MONO protocol
-    """
-    
-    CMD_QUERY = 0x80
-    CMD_PRE_BITMAP_FLIPDOT = 0x90
-    CMD_COLUMN_DATA_FLIPDOT = 0xA0
-    CMD_PRE_BITMAP_LED_1 = 0xB0
-    CMD_PRE_BITMAP_LED_2 = 0xC0
-    CMD_BITMAP_DATA_LED = 0xD0
-    CMD_DISPLAY_BITMAP_LED = 0xE0
-    
-    def __init__(self, debug = False):
-        """
-        debug:
-        Whether to print the sent and received frames
-        """
-        
-        self.debug = debug
-        self.connected_displays = {}
-    
-    def _send(self, frame):
-        """
-        Actually send the frame.
-        This varies depending on implementation and needs to be overridden
-        """
-        pass
-    
-    def _receive(self, length):
-        """
-        Actually receive data.
-        This varies depending on implementation and needs to be overridden
-        """
-        pass
-    
-    def set_display_attributes(self, address, attributes):
-        """
-        Set attributes of given display.
-        Used internally to manage resolution.
-        """
-        
-        self.connected_displays[address] = attributes.copy()
-    
-    def debug_frame(self, frame, receive = False):
-        """
-        Print a frame to standard output if the debug flag is set.
-        
-        frame:
-        The frame to print
-        
-        receive:
-        Whether to print the frame as sent or received
-        """
-        
-        if self.debug:
-            action = "Received" if receive else "Sending"
-            frame_debug = " ".join("{:02X}".format(byte) for byte in frame)
-            print("{} frame:".format(action))
-            print(frame_debug)
-    
-    def checksum_led(self, payload):
-        """
-        MONO LED CHECKSUM: XOR every byte, start with 0xED
-        
-        payload:
-        The payload to calculate the checksum for
-        """
-        
-        chk = 0xED
-        for b in payload:
-            chk ^= b
-        return chk
-    
-    def checksum_flipdot(self, payload):
-        """
-        MONO flipdot CHECKSUM: XOR every byte, start with 0xFF
-        
-        payload:
-        The payload to calculate the checksum for
-        """
-        
-        chk = 0xFF
-        for b in payload:
-            chk ^= b
-        return chk
-    
-    def escape_frame(self, frame):
-        """
-        Escape the start/stop byte and the escape byte in the given frame.
-        
-        frame:
-        The frame to escape.
-        """
-        
-        escaped_frame = []
-        for b in frame:
-            if b == 0x7e:
-                escaped_frame += [0x7d, 0x5e]
-            elif b == 0x7d:
-                escaped_frame += [0x7d, 0x5d]
-            else:
-                escaped_frame.append(b)
-        return escaped_frame
-    
-    def prepare_frame(self, frame):
-        """
-        This function does the following:
-        1. Escape the frame
-        2. Prepend the start byte and append the stop byte
-        
-        frame:
-        The frame (as a bytearray) to prepare
-        
-        Returns:
-        The prepared frame (as a bytearray)
-        """
-        
-        prepared_frame = self.escape_frame(frame)
-        prepared_frame = [0x7e] + prepared_frame + [0x7e]
-        return prepared_frame
-    
-    def send_frame(self, frame, reply_length = 0):
-        """
-        Send an arbitrary frame. Calls prepare_frame internally.
-        
-        frame:
-        The frame to send
-        
-        reply_length:
-        How many bytes to expect as a reply
-        
-        Returns:
-        The received frame OR None
-        
-        TODO: Actually check the checksum
-        """
-        
-        frame = bytearray(frame)
-        frame = self.prepare_frame(frame)
-        self.debug_frame(frame)
-        self._send(frame)
-        if reply_length:
-            reply = self._receive(reply_length + 3)
-            self.debug_frame(reply, receive=True)
-            reply = reply[1:-2]
-            return reply
-    
-    def get_command_byte(self, command, address):
-        """
-        Combine a command nibble with an address nibble.
-        
-        command:
-        Command byte/nibble
-        
-        address:
-        Address byte/nibble
-        """
-        
-        return (command & 0xF0) | (address & 0x0F)
-    
-    def send_command(self, address, command, payload, reply_length = 0):
-        """
-        Send a command frame to a display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        command:
-        The command byte (0x00 ... 0xF0, upper 4 bits only)
-        
-        payload:
-        The payload to send after the command byte
-        
-        reply_length:
-        How many bytes to expect as a reply
-        """
-        
-        frame = []
-        frame.append(self.get_command_byte(command, address))
-        frame += payload
-        return self.send_frame(frame, reply_length=reply_length)
-    
-    def send_bitmap_data_led(self, address, bitmap_data):
-        """
-        Send bitmap data to an LED display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        bitmap_data:
-        The bitmap data in MONO LED format:
-        - 8-bit columns
-        - bottom-most column first
-        - LSB topmost in column
-        - Left to right
-        """
-        
-        payload = [0xFF, len(bitmap_data)] + bitmap_data
-        payload.append(self.checksum_led(bitmap_data))
-        return self.send_command(address, self.CMD_BITMAP_DATA_LED, payload)
-    
-    def send_image_led(self, address, image):
-        """
-        Send an image to an LED display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        image:
-        Either a path to an image file or a PIL Image object.
-        White pixels will be on, black pixels will be off.
-        """
-        
-        if not _HAS_PIL:
-            raise RuntimeError("The PIL / Pillow module is not installed. It is required for sending image files over MONO.")
-        
-        if type(image) is str:
-            image = Image.open(image)
-        elif type(image) is not Image:
-            raise ValueError("image needs to be either a file path or a PIL Image instance")
-        
-        pixels = image.load()
-        width, height = image.size
-        max_col_end = math.ceil(height / 8) * 8
-        img_data = []
-        for x in range(width):
-            for col_start in range(max_col_end-8, -1, -8):
-                col_byte = 0x00
-                for y in range(col_start, col_start+8):
-                    col_byte |= (pixels[x, y] > 0) << (y%8)
-                img_data.append(col_byte)
-        return self.send_bitmap_data_led(address, img_data)
-    
-    def display_image_led(self, address, image):
-        """
-        Display an image on an LED display.
-        Compared to send_image_led, this also sends all required
-        pre and post commands to actually update the display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        image:
-        Either a path to an image file or a PIL Image object.
-        White pixels will be on, black pixels will be off.
-        """
-        
-        attributes = self.connected_displays.get(address)
-        if attributes is None:
-            raise RuntimeError("Display attributes are not set for address {}".format(address))
-        
-        width = attributes.get('width')
-        height = attributes.get('height')
-        num_img_bytes = width * math.ceil(height/8)
-        width_blocks = math.ceil(width/4)
-        height_blocks = math.ceil(height/4)
-        
-        self.send_command(address, self.CMD_PRE_BITMAP_LED_1, [0x00, 0xff, 0x2f, 0x10, 0x20, 0x40, 0x60, 0x90, 0xc0, 0xf0, 0x03, 0x13, 0x33, 0x53, 0x83, 0xb3, 0xe3, 0x89])
-        time.sleep(0.05)
-        self.send_command(address, self.CMD_PRE_BITMAP_LED_2, [0x01, 0x00, 0x00, 0x00, 0x00, 0x00, num_img_bytes, width_blocks, height_blocks])
-        time.sleep(0.05)
-        self.send_image_led(address, image)
-        time.sleep(0.05)
-        self.send_command(address, self.CMD_DISPLAY_BITMAP_LED, [0x1a])
-        time.sleep(0.05)
-    
-    def send_column_data_flipdot(self, address, col_address, column_data):
-        """
-        Send column data to a flipdot display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        col_address:
-        The address of the column (left to right)
-        
-        column_data:
-        The column data in MONO flipdot format:
-        - 4 pixels per byte, appropriate number of bytes per column
-        - First byte: topmost pixels
-        - Bit order per byte:
-            - Bit 7: topmost pixel enable (1=flip, 0=skip)
-            - Bit 6: topmost pixel color (1=yellow, 0=black)
-            - Bits 5 to 0 are the same for the other 3 pixels
-        """
-        
-        payload = [col_address] + column_data + [0x00]
-        payload.append(self.checksum_flipdot([self.get_command_byte(self.CMD_COLUMN_DATA_FLIPDOT, address)] + payload))
-        return self.send_command(address, self.CMD_COLUMN_DATA_FLIPDOT, payload)
-    
-    def send_image_flipdot(self, address, image, col_offset):
-        """
-        Send an image to a flipdot display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        image:
-        Either a path to an image file or a PIL Image object.
-        White pixels will be on, black pixels will be off.
-        
-        col_offset:
-        The column address offset, i.e. the address of the leftmost column
-        """
-        
-        if not _HAS_PIL:
-            raise RuntimeError("The PIL / Pillow module is not installed. It is required for sending image files over MONO.")
-        
-        if type(image) is str:
-            image = Image.open(image)
-        elif not isinstance(image, Image.Image):
-            raise ValueError("image needs to be either a file path or a PIL Image instance")
-        
-        pixels = image.convert('L').load()
-        width, height = image.size
-        max_col_end = math.ceil(height / 4) * 4
-        col_addr = col_offset
-        for x in range(width):
-            col_data = []
-            for col_start in range(max_col_end-4, -1, -4):
-                col_byte = 0b10101010 # Default: all pixels flipped, none skipped
-                for y in range(col_start, col_start+4):
-                    col_byte |= (pixels[x, height-y-1] > 0) << (6-((y%4)*2))
-                col_data.append(col_byte)
-            self.send_column_data_flipdot(address, col_addr, col_data)
-            col_addr += 1
-            if x != 0 and (x+1) % 28 == 0:
-                col_addr += 4
-            time.sleep(0.02)
-    
-    def display_image_flipdot(self, address, image, col_offset):
-        """
-        Display an image on a flipdot display.
-        Compared to send_image_flipdot, this also sends all required
-        pre and post commands to actually update the display.
-        
-        address:
-        The bus address of the display (0x00 ... 0x0F)
-        
-        image:
-        Either a path to an image file or a PIL Image object.
-        White pixels will be on, black pixels will be off.
-        
-        col_offset:
-        The column address offset, i.e. the address of the leftmost column
-        """
-        
-        self.send_command(address, self.CMD_PRE_BITMAP_FLIPDOT, [0x00, 0x10, 0x00, 0x50, 0x00, 0x02, 0x2E])
-        time.sleep(0.05)
-        self.send_image_flipdot(address, image, col_offset)
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import math
+import time
+
+try:
+    from PIL import Image
+except ImportError:
+    _HAS_PIL = False
+else:
+    _HAS_PIL = True
+
+class MONOProtocol:
+    """
+    All the logic related to the MONO protocol
+    """
+    
+    CMD_QUERY = 0x80
+    CMD_PRE_BITMAP_FLIPDOT = 0x90
+    CMD_COLUMN_DATA_FLIPDOT = 0xA0
+    CMD_PRE_BITMAP_LED_1 = 0xB0
+    CMD_PRE_BITMAP_LED_2 = 0xC0
+    CMD_BITMAP_DATA_LED = 0xD0
+    CMD_DISPLAY_BITMAP_LED = 0xE0
+    
+    def __init__(self, debug = False):
+        """
+        debug:
+        Whether to print the sent and received frames
+        """
+        
+        self.debug = debug
+        self.connected_displays = {}
+    
+    def _send(self, frame):
+        """
+        Actually send the frame.
+        This varies depending on implementation and needs to be overridden
+        """
+        pass
+    
+    def _receive(self, length):
+        """
+        Actually receive data.
+        This varies depending on implementation and needs to be overridden
+        """
+        pass
+    
+    def set_display_attributes(self, address, attributes):
+        """
+        Set attributes of given display.
+        Used internally to manage resolution.
+        """
+        
+        self.connected_displays[address] = attributes.copy()
+    
+    def debug_frame(self, frame, receive = False):
+        """
+        Print a frame to standard output if the debug flag is set.
+        
+        frame:
+        The frame to print
+        
+        receive:
+        Whether to print the frame as sent or received
+        """
+        
+        if self.debug:
+            action = "Received" if receive else "Sending"
+            frame_debug = " ".join("{:02X}".format(byte) for byte in frame)
+            print("{} frame:".format(action))
+            print(frame_debug)
+    
+    def checksum_led(self, payload):
+        """
+        MONO LED CHECKSUM: XOR every byte, start with 0xED
+        
+        payload:
+        The payload to calculate the checksum for
+        """
+        
+        chk = 0xED
+        for b in payload:
+            chk ^= b
+        return chk
+    
+    def checksum_flipdot(self, payload):
+        """
+        MONO flipdot CHECKSUM: XOR every byte, start with 0xFF
+        
+        payload:
+        The payload to calculate the checksum for
+        """
+        
+        chk = 0xFF
+        for b in payload:
+            chk ^= b
+        return chk
+    
+    def escape_frame(self, frame):
+        """
+        Escape the start/stop byte and the escape byte in the given frame.
+        
+        frame:
+        The frame to escape.
+        """
+        
+        escaped_frame = []
+        for b in frame:
+            if b == 0x7e:
+                escaped_frame += [0x7d, 0x5e]
+            elif b == 0x7d:
+                escaped_frame += [0x7d, 0x5d]
+            else:
+                escaped_frame.append(b)
+        return escaped_frame
+    
+    def prepare_frame(self, frame):
+        """
+        This function does the following:
+        1. Escape the frame
+        2. Prepend the start byte and append the stop byte
+        
+        frame:
+        The frame (as a bytearray) to prepare
+        
+        Returns:
+        The prepared frame (as a bytearray)
+        """
+        
+        prepared_frame = self.escape_frame(frame)
+        prepared_frame = [0x7e] + prepared_frame + [0x7e]
+        return prepared_frame
+    
+    def send_frame(self, frame, reply_length = 0):
+        """
+        Send an arbitrary frame. Calls prepare_frame internally.
+        
+        frame:
+        The frame to send
+        
+        reply_length:
+        How many bytes to expect as a reply
+        
+        Returns:
+        The received frame OR None
+        
+        TODO: Actually check the checksum
+        """
+        
+        frame = bytearray(frame)
+        frame = self.prepare_frame(frame)
+        self.debug_frame(frame)
+        self._send(frame)
+        if reply_length:
+            reply = self._receive(reply_length + 3)
+            self.debug_frame(reply, receive=True)
+            reply = reply[1:-2]
+            return reply
+    
+    def get_command_byte(self, command, address):
+        """
+        Combine a command nibble with an address nibble.
+        
+        command:
+        Command byte/nibble
+        
+        address:
+        Address byte/nibble
+        """
+        
+        return (command & 0xF0) | (address & 0x0F)
+    
+    def send_command(self, address, command, payload, reply_length = 0):
+        """
+        Send a command frame to a display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        command:
+        The command byte (0x00 ... 0xF0, upper 4 bits only)
+        
+        payload:
+        The payload to send after the command byte
+        
+        reply_length:
+        How many bytes to expect as a reply
+        """
+        
+        frame = []
+        frame.append(self.get_command_byte(command, address))
+        frame += payload
+        return self.send_frame(frame, reply_length=reply_length)
+    
+    def send_bitmap_data_led(self, address, bitmap_data):
+        """
+        Send bitmap data to an LED display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        bitmap_data:
+        The bitmap data in MONO LED format:
+        - 8-bit columns
+        - bottom-most column first
+        - LSB topmost in column
+        - Left to right
+        """
+        
+        payload = [0xFF, len(bitmap_data)] + bitmap_data
+        payload.append(self.checksum_led(bitmap_data))
+        return self.send_command(address, self.CMD_BITMAP_DATA_LED, payload)
+    
+    def send_image_led(self, address, image):
+        """
+        Send an image to an LED display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        image:
+        Either a path to an image file or a PIL Image object.
+        White pixels will be on, black pixels will be off.
+        """
+        
+        if not _HAS_PIL:
+            raise RuntimeError("The PIL / Pillow module is not installed. It is required for sending image files over MONO.")
+        
+        if type(image) is str:
+            image = Image.open(image)
+        elif type(image) is not Image:
+            raise ValueError("image needs to be either a file path or a PIL Image instance")
+        
+        pixels = image.load()
+        width, height = image.size
+        max_col_end = math.ceil(height / 8) * 8
+        img_data = []
+        for x in range(width):
+            for col_start in range(max_col_end-8, -1, -8):
+                col_byte = 0x00
+                for y in range(col_start, col_start+8):
+                    col_byte |= (pixels[x, y] > 0) << (y%8)
+                img_data.append(col_byte)
+        return self.send_bitmap_data_led(address, img_data)
+    
+    def display_image_led(self, address, image):
+        """
+        Display an image on an LED display.
+        Compared to send_image_led, this also sends all required
+        pre and post commands to actually update the display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        image:
+        Either a path to an image file or a PIL Image object.
+        White pixels will be on, black pixels will be off.
+        """
+        
+        attributes = self.connected_displays.get(address)
+        if attributes is None:
+            raise RuntimeError("Display attributes are not set for address {}".format(address))
+        
+        width = attributes.get('width')
+        height = attributes.get('height')
+        num_img_bytes = width * math.ceil(height/8)
+        width_blocks = math.ceil(width/4)
+        height_blocks = math.ceil(height/4)
+        
+        self.send_command(address, self.CMD_PRE_BITMAP_LED_1, [0x00, 0xff, 0x2f, 0x10, 0x20, 0x40, 0x60, 0x90, 0xc0, 0xf0, 0x03, 0x13, 0x33, 0x53, 0x83, 0xb3, 0xe3, 0x89])
+        time.sleep(0.05)
+        self.send_command(address, self.CMD_PRE_BITMAP_LED_2, [0x01, 0x00, 0x00, 0x00, 0x00, 0x00, num_img_bytes, width_blocks, height_blocks])
+        time.sleep(0.05)
+        self.send_image_led(address, image)
+        time.sleep(0.05)
+        self.send_command(address, self.CMD_DISPLAY_BITMAP_LED, [0x1a])
+        time.sleep(0.05)
+    
+    def send_column_data_flipdot(self, address, col_address, column_data):
+        """
+        Send column data to a flipdot display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        col_address:
+        The address of the column (left to right)
+        
+        column_data:
+        The column data in MONO flipdot format:
+        - 4 pixels per byte, appropriate number of bytes per column
+        - First byte: topmost pixels
+        - Bit order per byte:
+            - Bit 7: topmost pixel enable (1=flip, 0=skip)
+            - Bit 6: topmost pixel color (1=yellow, 0=black)
+            - Bits 5 to 0 are the same for the other 3 pixels
+        """
+        
+        payload = [col_address] + column_data + [0x00]
+        payload.append(self.checksum_flipdot([self.get_command_byte(self.CMD_COLUMN_DATA_FLIPDOT, address)] + payload))
+        return self.send_command(address, self.CMD_COLUMN_DATA_FLIPDOT, payload)
+    
+    def send_image_flipdot(self, address, image, col_offset):
+        """
+        Send an image to a flipdot display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        image:
+        Either a path to an image file or a PIL Image object.
+        White pixels will be on, black pixels will be off.
+        
+        col_offset:
+        The column address offset, i.e. the address of the leftmost column
+        """
+        
+        if not _HAS_PIL:
+            raise RuntimeError("The PIL / Pillow module is not installed. It is required for sending image files over MONO.")
+        
+        if type(image) is str:
+            image = Image.open(image)
+        elif not isinstance(image, Image.Image):
+            raise ValueError("image needs to be either a file path or a PIL Image instance")
+        
+        pixels = image.convert('L').load()
+        width, height = image.size
+        max_col_end = math.ceil(height / 4) * 4
+        col_addr = col_offset
+        for x in range(width):
+            col_data = []
+            for col_start in range(max_col_end-4, -1, -4):
+                col_byte = 0b10101010 # Default: all pixels flipped, none skipped
+                for y in range(col_start, col_start+4):
+                    col_byte |= (pixels[x, height-y-1] > 0) << (6-((y%4)*2))
+                col_data.append(col_byte)
+            self.send_column_data_flipdot(address, col_addr, col_data)
+            col_addr += 1
+            if x != 0 and (x+1) % 28 == 0:
+                col_addr += 4
+            time.sleep(0.02)
+    
+    def display_image_flipdot(self, address, image, col_offset):
+        """
+        Display an image on a flipdot display.
+        Compared to send_image_flipdot, this also sends all required
+        pre and post commands to actually update the display.
+        
+        address:
+        The bus address of the display (0x00 ... 0x0F)
+        
+        image:
+        Either a path to an image file or a PIL Image object.
+        White pixels will be on, black pixels will be off.
+        
+        col_offset:
+        The column address offset, i.e. the address of the leftmost column
+        """
+        
+        self.send_command(address, self.CMD_PRE_BITMAP_FLIPDOT, [0x00, 0x10, 0x00, 0x50, 0x00, 0x02, 0x2E])
+        time.sleep(0.05)
+        self.send_image_flipdot(address, image, col_offset)
```

### Comparing `pyFIS-1.8.1/pyfis/lawo/mono_serial.py` & `pyFIS-1.9.0/pyfis/lawo/mono_serial.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-
-from .mono_protocol import MONOProtocol
-
-class SerialMONOMaster(MONOProtocol):
-    """
-    A MONO bus master, sending and receiving frames using a serial port
-    """
-    
-    def __init__(self, port, baudrate = 19200, bytesize = 8, parity = 'N',
-                 stopbits = 1, timeout = 2.0, *args, **kwargs):
-        """
-        port:
-        The serial port to use for communication
-        """
-        
-        super().__init__(*args, **kwargs)
-        
-        if isinstance(port, serial.Serial):
-            self.device = port
-            self.port = self.device.port
-        else:
-            self.port = port
-            self.device = serial.Serial(
-                self.port,
-                baudrate = baudrate,
-                bytesize = bytesize,
-                parity = parity,
-                stopbits = stopbits,
-                timeout = timeout
-            )
-    
-    def _send(self, frame):
-        """
-        Actually send the frame.
-        This varies depending on implementation
-        """
-        
-        self.device.write(frame)
-    
-    def _receive(self, length):
-        """
-        Actually receive data.
-        This varies depending on implementation and needs to be overridden
-        """
-        
-        return self.device.read(length)
-
-    def __del__(self):
-        self.device.close()
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+
+from .mono_protocol import MONOProtocol
+
+class SerialMONOMaster(MONOProtocol):
+    """
+    A MONO bus master, sending and receiving frames using a serial port
+    """
+    
+    def __init__(self, port, baudrate = 19200, bytesize = 8, parity = 'N',
+                 stopbits = 1, timeout = 2.0, *args, **kwargs):
+        """
+        port:
+        The serial port to use for communication
+        """
+        
+        super().__init__(*args, **kwargs)
+        
+        if isinstance(port, serial.Serial):
+            self.device = port
+            self.port = self.device.port
+        else:
+            self.port = port
+            self.device = serial.Serial(
+                self.port,
+                baudrate = baudrate,
+                bytesize = bytesize,
+                parity = parity,
+                stopbits = stopbits,
+                timeout = timeout
+            )
+    
+    def _send(self, frame):
+        """
+        Actually send the frame.
+        This varies depending on implementation
+        """
+        
+        self.device.write(frame)
+    
+    def _receive(self, length):
+        """
+        Actually receive data.
+        This varies depending on implementation and needs to be overridden
+        """
+        
+        return self.device.read(length)
+
+    def __del__(self):
+        self.device.close()
```

### Comparing `pyFIS-1.8.1/pyfis/metadata.py` & `pyFIS-1.9.0/pyfis/metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-name = "pyFIS"
-version = "1.8.1"
-description = "A library for controlling devices in the passenger information realm"
-license = "GPLv3"
-author = "Julian Metzler"
-author_email = "git@mezgr.de"
-requires = ['pyserial']
-url = "https://github.com/Mezgrman/pyFIS"
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+name = "pyFIS"
+version = "1.9.0"
+description = "A library for controlling devices in the passenger information realm"
+license = "GPLv3"
+author = "Julian Metzler"
+author_email = "git@mezgr.de"
+requires = ['pyserial']
+url = "https://github.com/Mezgrman/pyFIS"
 keywords = "led sign message board effect library wrapper serial text display ibis vdv300 bus next stop train mono lawo splitflap industrial factory"
```

### Comparing `pyFIS-1.8.1/pyfis/microsyst/__init__.py` & `pyFIS-1.9.0/pyfis/aegmis/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .migra import MigraTCP
+"""
+Copyright (C) 2020-2022 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .ecs_lcd import ECSLCDisplay
+from .mis1_gcu import MIS1GCUDisplay
+from .mis2_gcu import MIS2GCUDisplay
```

### Comparing `pyFIS-1.8.1/pyfis/microsyst/migra.py` & `pyFIS-1.9.0/pyfis/microsyst/migra.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,572 +1,572 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-import socket
-
-
-class MigraTCP:
-    """
-    microSYST migra industrial LED sign with Ethernet and TCP/IP connection
-    """
-    
-    COLOR_BLACK = "0"
-    COLOR_GREEN = "1"
-    COLOR_RED = "2"
-    COLOR_YELLOW = "3"
-    COLOR_TRANSPARENT = "T"
-    COLOR_NAMES = {
-        COLOR_BLACK: ["black", "off"],
-        COLOR_GREEN: ["green"],
-        COLOR_RED: ["red"],
-        COLOR_YELLOW: ["yellow", "orange"],
-        COLOR_TRANSPARENT: ["transparent", "transparency", "alpha"],
-    }
-    
-    DIR_OFF = "0"
-    DIR_UP = "1"
-    DIR_DOWN = "2"
-    DIRECTIONS = (DIR_OFF, DIR_UP, DIR_DOWN)
-    
-    TRIG_NORMAL = "="
-    TRIG_HISTORY = "#"
-    TRIGGER_MODES = (TRIG_NORMAL, TRIG_HISTORY)
-    
-    def __init__(self, host, port=10001, timeout=2.0, debug=False):
-        """
-        host:
-          The hostname or IP to connect to
-        
-        port:
-          The TCP port to use for communication
-        
-        timeout:
-          The socket timeout in seconds
-        """
-        
-        self.debug = debug
-        self.command_queue_enabled = False
-        self.command_queue = []
-        
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.socket.connect((host, port))
-        self.socket.settimeout(timeout)
-
-    def __del__(self):
-        self.socket.close()
-    
-    def _printable(self, char):
-        """
-        Replace non-printable chars with printable variants.
-        """
-        
-        if char in range(0, 32):
-            return "<{:02X}>".format(char)
-        else:
-            return chr(char)
-    
-    def debug_telegram(self, telegram, receive=False):
-        """
-        Print a telegram to standard output if the debug flag is set.
-        
-        telegram:
-          The telegram to print
-        
-        receive:
-          Whether to print the telegram as sent or received
-        """
-        
-        if self.debug:
-            action = "Received" if receive else "Sending"
-            telegram_debug = "\n".join("{:02X} {}".format(
-                byte, self._printable(byte)) for byte in telegram)
-            print("{} telegram:\n".format(action))
-            print(telegram_debug)
-    
-    def _send(self, telegram):
-        self.debug_telegram(telegram)
-        self.socket.send(telegram)
-    
-    def _receive(self, length):
-        data = self.socket.recv(length)
-        self.debug_telegram(data, receive=True)
-        return data
-    
-    def send_telegram(self, payload, response=True, checksum=True, response_length=1):
-        """
-        Send a raw telegram. Header and trailer will be added.
-        
-        payload:
-          The data to be sent
-        
-        response:
-          Whether to request and read a response from the display
-        
-        checksum:
-          Whether to use checksum and length bytes
-        
-        response_length:
-          The length of the payload of the expected response
-        """
-        
-        length = len(payload)
-        if length > 230:
-            raise ValueError("Telegram is too long (max. 230 bytes)")
-        
-        frame_ctrl = 0x80
-        if response:
-            frame_ctrl |= 0x01
-        if checksum:
-            frame_ctrl |= 0x02
-        dest_addr = 0x81
-        src_addr = 0x80
-        telegram = bytearray([0x02, dest_addr, src_addr, frame_ctrl])
-        if checksum:
-            len_h = 0xF0 | ((length & 0xF0) >> 4)
-            len_l = 0xF0 | (length & 0x0F)
-            telegram.extend([len_h, len_l])
-        telegram.extend(payload)
-        if checksum:
-            chk_sum = sum(telegram[1:]) % 256
-            chk_h = 0xF0 | ((chk_sum & 0xF0) >> 4)
-            chk_l = 0xF0 | (chk_sum & 0x0F)
-            telegram.extend([chk_h, chk_l])
-        telegram.append(0x03)
-        
-        self._send(telegram)
-        
-        if response:
-            return self.receive_response(payload_length=response_length)
-    
-    def receive_response(self, payload_length=1):
-        """
-        Read the response from the display.
-        
-        payload_length:
-          The expected length of the payload (usually 1 byte for status code)
-        """
-        
-        telegram = bytearray()
-        telegram.extend(self._receive(5 + payload_length))
-        payload = telegram[4:-1]
-        return payload
-    
-    def get_color_flag(self, color):
-        """
-        Return the character used to describe the given color
-        """
-        
-        color = color.lower()
-        choices = [inner for outer in self.COLOR_NAMES.values() for inner in outer]
-        if color not in choices:
-            raise ValueError(f"Invalid color name '{color}'. Choices are: {', '.join(choices)}")
-        return [key for key, value in self.COLOR_NAMES.items() if color in value][0]
-    
-    def send_command(self, command, escape=True, *args, **kwargs):
-        """
-        Send a command (consisting of an escape character and some ASCII chars)
-        
-        command:
-          The command to be sent (string)
-        
-        escape:
-          Whether to prepend an escape character (0x1B) - not needed for text
-        
-        *args, **kwargs:
-          Passed to send_telegram
-        """
-        
-        payload = bytearray()
-        if escape:
-            payload.append(0x1B)
-        if not escape and self.command_queue_enabled:
-            # Separate non-escaped commands (texts) by 0x1F when queueing
-            payload.append(0x1F)
-        payload.extend(command.encode('ascii'))
-        if self.command_queue_enabled:
-            self.command_queue.append(payload)
-        else:
-            return self.send_telegram(payload, *args, **kwargs)
-    
-    def start_command_queue(self):
-        """
-        Causes subsequent calls to send_command() to queue up telegrams
-        for sending them as one unit when send_command_queue() is called.
-        """
-        
-        self.command_queue_enabled = True
-    
-    def send_command_queue(self, *args, **kwargs):
-        """
-        Send all queued commands.
-        
-        *args, **kwargs:
-          Passed to send_command
-        """
-        
-        try:
-            telegram = b"".join(self.command_queue)
-            response = self.send_telegram(telegram, *args, **kwargs)
-            return response
-        finally:
-            self.command_queue_enabled = False
-            self.command_queue = []
-    
-    def text(self, text):
-        """
-        Print a text at the current cursor position with the current attributes
-        """
-        
-        return self.send_command(text, escape=False)
-        
-    def select_font(self, font_id, monospace=False):
-        """
-        Select a font for all subsequent texts
-        
-        font_id:
-          ID of the font to be selected (0 to 99)
-        
-        monospace:
-          Whether to force equal character widths
-        """
-        
-        mono_flag = "z" if monospace else "Z"
-        return self.send_command(f"{mono_flag}{font_id:02}")
-        
-    def set_cursor_pos(self, x, y):
-        """
-        Set the cursor to the specified X and Y coordinates
-        """
-        
-        return self.send_command(f"C{x:03}{y:03}")
-        
-    def set_attributes(self, fg_color, bg_color, blink):
-        """
-        Set foreground color, background color and blink attributes
-        for subsequent texts
-        
-        fg_color:
-          One of self.COLORS
-        
-        bg_color:
-          One of self.COLORS or 'transparent'
-        
-        blink:
-          True for blinking text, False for static text
-        """
-        
-        fg_flag = self.get_color_flag(fg_color)
-        bg_flag = self.get_color_flag(bg_color)
-        return self.send_command(f"A{fg_flag}{bg_flag}{str(int(blink))}")
-    
-    def set_scroll_speed(self, speed):
-        """
-        Set the scroll interval for all scrolling texts
-        
-        speed:
-          0 - stopped
-          1 - 1.8 seconds
-          2 - 1.6 seconds
-          3 - 1.4 seconds
-          4 - 1.2 seconds
-          5 - 1 second
-          6 - 0.8 seconds
-          7 - 0.6 seconds
-          8 - 0.4 seconds
-          9 - 0.2 seconds
-        """
-        
-        return self.send_command(f"L{speed}")
-    
-    def show_text(self, text_id):
-        """
-        Show the stored text with the given ID
-        """
-        
-        return self.send_command(f"T+{text_id:03}")
-    
-    def hide_text(self, text_id):
-        """
-        Hide the stored text with the given ID
-        """
-        
-        return self.send_command(f"T-{text_id:03}")
-    
-    def show_image(self, image_id):
-        """
-        Show the stored image with the given ID
-        """
-        
-        return self.send_command(f"G+{image_id:03}")
-    
-    def hide_image(self, image_id):
-        """
-        Hide the stored image with the given ID
-        """
-        
-        return self.send_command(f"G-{image_id:03}")
-    
-    def show_variable(self, var_id):
-        """
-        Show the stored variable with the given ID
-        """
-        
-        return self.send_command(f"V+{var_id:03}")
-    
-    def hide_variable(self, var_id):
-        """
-        Hide the stored variable with the given ID
-        """
-        
-        return self.send_command(f"V-{var_id:03}")
-    
-    def set_variable_value(self, var_id, value):
-        """
-        Set the value of the stored variable with the given ID
-        """
-        
-        return self.send_command(f"V={var_id:03}{value}")
-    
-    def increment_variable(self, var_id):
-        """
-        Increment the stored variable with the given ID
-        """
-        
-        return self.send_command(f"VI{var_id:03}")
-    
-    def decrement_variable(self, var_id):
-        """
-        Decrement the stored variable with the given ID
-        """
-        
-        return self.send_command(f"VD{var_id:03}")
-    
-    def set_variable_pos(self, var_id, x, y):
-        """
-        Set the display position of the stored variable with the given ID
-        to the given X and Y coordinates
-        """
-        
-        return self.send_command(f"VP{var_id:03}{x:03}{y:03}")
-    
-    def show_bargraph(self, bg_id):
-        """
-        Show the stored bargraph with the given ID
-        """
-        
-        return self.send_command(f"W+{bg_id:03}")
-    
-    def hide_bargraph(self, bg_id):
-        """
-        Hide the stored bargraph with the given ID
-        """
-        
-        return self.send_command(f"W-{bg_id:03}")
-    
-    def set_bargraph_value(self, bg_id, value):
-        """
-        Set the value of the stored variable with the given ID
-        """
-        
-        # Alternative command format: raw signed integer
-        # f"W={bg_id:03}I{high_byte}{low_byte}"
-        
-        sign = "+" if value >= 0 else "-"
-        return self.send_command(f"W={bg_id:03}A{sign}{abs(value):05}")
-    
-    def fill(self, color):
-        """
-        Fill the entire display with one color
-        
-        color:
-          One of self.COLORS
-        """
-        
-        color_flag = self.get_color_flag(color)
-        return self.send_command(f"F{color_flag}")
-    
-    def set_pixel(self, x, y, color):
-        """
-        Set the given pixel to the given color
-        
-        color:
-          One of self.COLORS
-        """
-        
-        color_flag = self.get_color_flag(color)
-        return self.send_command(f"P{color_flag}{x:03}{y:03}")
-    
-    def get_pixel(self, x, y):
-        """
-        Get the color of the given pixel
-        """
-        
-        response = self.send_command(f"P?{x:03}{y:03}", response_length=3)
-        color = self.COLORS[response[2] - ord("0")]
-        return color
-    
-    def rectangle(self, x1, y1, x2, y2, fg_color, bg_color):
-        """
-        Draw a rectangle with the given colors.
-        
-        x1, y1:
-          Coordinates of the top left corner
-        
-        x2, y2:
-          Coordinates of the bottom right corner
-        
-        fg_color:
-          One of self.COLORS
-        
-        bg_color:
-          One of self.COLORS or 'transparent'
-        """
-        
-        fg_flag = self.get_color_flag(fg_color)
-        bg_flag = self.get_color_flag(bg_color)
-        return self.send_command(f"R{fg_flag}{bg_flag}{x1:03}{y1:03}{x2:03}{y2:03}")
-    
-    def scroll_area_vertical(self, direction, speed, step, y1, y2, extended_range=False):
-        """
-        Scroll the area between lines y1 and y2 in the given direction,
-        at the given scroll interval, with the given step size.
-        
-        direction:
-          One of self.DIRECTIONS
-        
-        speed:
-          See set_scroll_speed
-        
-        step:
-          0 - No movement
-          1 to 9 - 1 to 9 pixels
-        
-        extended_range:
-          If True, use three characters for y1 and y2 (for displays with more than 64 rows)
-        """
-        
-        if extended_range:
-            return self.send_command(f"S{direction}{speed}{step}{y1:03}{y2:03}")
-        else:
-            return self.send_command(f"S{direction}{speed}{step}{y1:02}{y2:02}")
-    
-    def set_blink_period(self, period):
-        """
-        Set the blink period for all blinking texts
-        
-        period:
-          0 - 2 seconds
-          1 - 1.8 seconds
-          2 - 1.6 seconds
-          3 - 1.4 seconds
-          4 - 1.2 seconds
-          5 - 1 second
-          6 - 0.8 seconds
-          7 - 0.6 seconds
-          8 - 0.4 seconds
-          9 - 0.2 seconds
-        """
-        
-        return self.send_command(f"B{period}")
-    
-    def set_brightness(self, color, brightness):
-        """
-        Set the brightness for all LEDs of the given color
-        
-        color:
-          self.COLOR_RED or self.COLOR_GREEN
-        
-        brightness:
-          0 to 100
-        """
-        
-        color_flag = self.get_color_flag(color)
-        if color_flag not in (self.COLOR_RED, self.COLOR_GREEN):
-            raise ValueError("Color for set_brightness can only be red or green")
-        if color_flag == self.COLOR_GREEN:
-            color_flag = "1"
-        elif color_flag == self.COLOR_RED:
-            color_flag = "2"
-        return self.send_command(f"H{color_flag}{brightness:03}")
-    
-    def set_and_get_gpio(self, outputs):
-        """
-        Set the 16 general purpose outputs and return the state of the 16 inputs
-        
-        outputs:
-          List of 16 values:
-            True - Turn output on
-            False - Turn output off
-            None - Don't change output
-        
-        Returns:
-          A list in the same form as the outputs parameter
-        """
-        
-        def _get_output_flag(value):
-            if value is True:
-                return "1"
-            elif value is False:
-                return "0"
-            else:
-                return "N"
-        
-        output_flags = "".join(map(_get_output_flag, outputs))
-        response = self.send_command(f"D{output_flags}", response_length=18)
-        inputs = [(v == ord("1")) for v in response[2:]]
-        return inputs
-    
-    def run_macros(self, macro_id):
-        """
-        Run macros starting at the given ID
-        """
-        
-        return self.send_command(f"M{macro_id:03}")
-    
-    def run_macro_conditional(self, macro_id, input_channel, trigger_mode, trigger_state):
-        """
-        Run the macro with the given ID if the given digital input (0 to 15)
-        is currently in the given state (trigger mode NORMAL)
-        or has been in the given state at least once since the last call of this command
-        (trigger mode HISTORY)
-        
-        trigger_mode:
-          self.TRIG_NORMAL or self.TRIG_HISTORY
-        
-        trigger_state:
-          True or False (on or off)
-        """
-        
-        return self.send_command(f"M{macro_id:03}E{input_channel:1X}{trigger_mode}{trigger_state:1}")
-    
-    def wait(self, duration):
-        """
-        Pause macro execution for the given duration.
-        
-        duration:
-          Time to wait in seconds (0 to 99.9)
-        """
-        
-        duration_flag = int(duration * 10)
-        return self.send_command(f"w{duration_flag:03}")
-    
-    def stop_macros(self):
-        """
-        Stop macro execution.
-        """
-        
-        return self.send_command("E")
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+import socket
+
+
+class MigraTCP:
+    """
+    microSYST migra industrial LED sign with Ethernet and TCP/IP connection
+    """
+    
+    COLOR_BLACK = "0"
+    COLOR_GREEN = "1"
+    COLOR_RED = "2"
+    COLOR_YELLOW = "3"
+    COLOR_TRANSPARENT = "T"
+    COLOR_NAMES = {
+        COLOR_BLACK: ["black", "off"],
+        COLOR_GREEN: ["green"],
+        COLOR_RED: ["red"],
+        COLOR_YELLOW: ["yellow", "orange"],
+        COLOR_TRANSPARENT: ["transparent", "transparency", "alpha"],
+    }
+    
+    DIR_OFF = "0"
+    DIR_UP = "1"
+    DIR_DOWN = "2"
+    DIRECTIONS = (DIR_OFF, DIR_UP, DIR_DOWN)
+    
+    TRIG_NORMAL = "="
+    TRIG_HISTORY = "#"
+    TRIGGER_MODES = (TRIG_NORMAL, TRIG_HISTORY)
+    
+    def __init__(self, host, port=10001, timeout=2.0, debug=False):
+        """
+        host:
+          The hostname or IP to connect to
+        
+        port:
+          The TCP port to use for communication
+        
+        timeout:
+          The socket timeout in seconds
+        """
+        
+        self.debug = debug
+        self.command_queue_enabled = False
+        self.command_queue = []
+        
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.socket.connect((host, port))
+        self.socket.settimeout(timeout)
+
+    def __del__(self):
+        self.socket.close()
+    
+    def _printable(self, char):
+        """
+        Replace non-printable chars with printable variants.
+        """
+        
+        if char in range(0, 32):
+            return "<{:02X}>".format(char)
+        else:
+            return chr(char)
+    
+    def debug_telegram(self, telegram, receive=False):
+        """
+        Print a telegram to standard output if the debug flag is set.
+        
+        telegram:
+          The telegram to print
+        
+        receive:
+          Whether to print the telegram as sent or received
+        """
+        
+        if self.debug:
+            action = "Received" if receive else "Sending"
+            telegram_debug = "\n".join("{:02X} {}".format(
+                byte, self._printable(byte)) for byte in telegram)
+            print("{} telegram:\n".format(action))
+            print(telegram_debug)
+    
+    def _send(self, telegram):
+        self.debug_telegram(telegram)
+        self.socket.send(telegram)
+    
+    def _receive(self, length):
+        data = self.socket.recv(length)
+        self.debug_telegram(data, receive=True)
+        return data
+    
+    def send_telegram(self, payload, response=True, checksum=True, response_length=1):
+        """
+        Send a raw telegram. Header and trailer will be added.
+        
+        payload:
+          The data to be sent
+        
+        response:
+          Whether to request and read a response from the display
+        
+        checksum:
+          Whether to use checksum and length bytes
+        
+        response_length:
+          The length of the payload of the expected response
+        """
+        
+        length = len(payload)
+        if length > 230:
+            raise ValueError("Telegram is too long (max. 230 bytes)")
+        
+        frame_ctrl = 0x80
+        if response:
+            frame_ctrl |= 0x01
+        if checksum:
+            frame_ctrl |= 0x02
+        dest_addr = 0x81
+        src_addr = 0x80
+        telegram = bytearray([0x02, dest_addr, src_addr, frame_ctrl])
+        if checksum:
+            len_h = 0xF0 | ((length & 0xF0) >> 4)
+            len_l = 0xF0 | (length & 0x0F)
+            telegram.extend([len_h, len_l])
+        telegram.extend(payload)
+        if checksum:
+            chk_sum = sum(telegram[1:]) % 256
+            chk_h = 0xF0 | ((chk_sum & 0xF0) >> 4)
+            chk_l = 0xF0 | (chk_sum & 0x0F)
+            telegram.extend([chk_h, chk_l])
+        telegram.append(0x03)
+        
+        self._send(telegram)
+        
+        if response:
+            return self.receive_response(payload_length=response_length)
+    
+    def receive_response(self, payload_length=1):
+        """
+        Read the response from the display.
+        
+        payload_length:
+          The expected length of the payload (usually 1 byte for status code)
+        """
+        
+        telegram = bytearray()
+        telegram.extend(self._receive(5 + payload_length))
+        payload = telegram[4:-1]
+        return payload
+    
+    def get_color_flag(self, color):
+        """
+        Return the character used to describe the given color
+        """
+        
+        color = color.lower()
+        choices = [inner for outer in self.COLOR_NAMES.values() for inner in outer]
+        if color not in choices:
+            raise ValueError(f"Invalid color name '{color}'. Choices are: {', '.join(choices)}")
+        return [key for key, value in self.COLOR_NAMES.items() if color in value][0]
+    
+    def send_command(self, command, escape=True, *args, **kwargs):
+        """
+        Send a command (consisting of an escape character and some ASCII chars)
+        
+        command:
+          The command to be sent (string)
+        
+        escape:
+          Whether to prepend an escape character (0x1B) - not needed for text
+        
+        *args, **kwargs:
+          Passed to send_telegram
+        """
+        
+        payload = bytearray()
+        if escape:
+            payload.append(0x1B)
+        if not escape and self.command_queue_enabled:
+            # Separate non-escaped commands (texts) by 0x1F when queueing
+            payload.append(0x1F)
+        payload.extend(command.encode('ascii'))
+        if self.command_queue_enabled:
+            self.command_queue.append(payload)
+        else:
+            return self.send_telegram(payload, *args, **kwargs)
+    
+    def start_command_queue(self):
+        """
+        Causes subsequent calls to send_command() to queue up telegrams
+        for sending them as one unit when send_command_queue() is called.
+        """
+        
+        self.command_queue_enabled = True
+    
+    def send_command_queue(self, *args, **kwargs):
+        """
+        Send all queued commands.
+        
+        *args, **kwargs:
+          Passed to send_command
+        """
+        
+        try:
+            telegram = b"".join(self.command_queue)
+            response = self.send_telegram(telegram, *args, **kwargs)
+            return response
+        finally:
+            self.command_queue_enabled = False
+            self.command_queue = []
+    
+    def text(self, text):
+        """
+        Print a text at the current cursor position with the current attributes
+        """
+        
+        return self.send_command(text, escape=False)
+        
+    def select_font(self, font_id, monospace=False):
+        """
+        Select a font for all subsequent texts
+        
+        font_id:
+          ID of the font to be selected (0 to 99)
+        
+        monospace:
+          Whether to force equal character widths
+        """
+        
+        mono_flag = "z" if monospace else "Z"
+        return self.send_command(f"{mono_flag}{font_id:02}")
+        
+    def set_cursor_pos(self, x, y):
+        """
+        Set the cursor to the specified X and Y coordinates
+        """
+        
+        return self.send_command(f"C{x:03}{y:03}")
+        
+    def set_attributes(self, fg_color, bg_color, blink):
+        """
+        Set foreground color, background color and blink attributes
+        for subsequent texts
+        
+        fg_color:
+          One of self.COLORS
+        
+        bg_color:
+          One of self.COLORS or 'transparent'
+        
+        blink:
+          True for blinking text, False for static text
+        """
+        
+        fg_flag = self.get_color_flag(fg_color)
+        bg_flag = self.get_color_flag(bg_color)
+        return self.send_command(f"A{fg_flag}{bg_flag}{str(int(blink))}")
+    
+    def set_scroll_speed(self, speed):
+        """
+        Set the scroll interval for all scrolling texts
+        
+        speed:
+          0 - stopped
+          1 - 1.8 seconds
+          2 - 1.6 seconds
+          3 - 1.4 seconds
+          4 - 1.2 seconds
+          5 - 1 second
+          6 - 0.8 seconds
+          7 - 0.6 seconds
+          8 - 0.4 seconds
+          9 - 0.2 seconds
+        """
+        
+        return self.send_command(f"L{speed}")
+    
+    def show_text(self, text_id):
+        """
+        Show the stored text with the given ID
+        """
+        
+        return self.send_command(f"T+{text_id:03}")
+    
+    def hide_text(self, text_id):
+        """
+        Hide the stored text with the given ID
+        """
+        
+        return self.send_command(f"T-{text_id:03}")
+    
+    def show_image(self, image_id):
+        """
+        Show the stored image with the given ID
+        """
+        
+        return self.send_command(f"G+{image_id:03}")
+    
+    def hide_image(self, image_id):
+        """
+        Hide the stored image with the given ID
+        """
+        
+        return self.send_command(f"G-{image_id:03}")
+    
+    def show_variable(self, var_id):
+        """
+        Show the stored variable with the given ID
+        """
+        
+        return self.send_command(f"V+{var_id:03}")
+    
+    def hide_variable(self, var_id):
+        """
+        Hide the stored variable with the given ID
+        """
+        
+        return self.send_command(f"V-{var_id:03}")
+    
+    def set_variable_value(self, var_id, value):
+        """
+        Set the value of the stored variable with the given ID
+        """
+        
+        return self.send_command(f"V={var_id:03}{value}")
+    
+    def increment_variable(self, var_id):
+        """
+        Increment the stored variable with the given ID
+        """
+        
+        return self.send_command(f"VI{var_id:03}")
+    
+    def decrement_variable(self, var_id):
+        """
+        Decrement the stored variable with the given ID
+        """
+        
+        return self.send_command(f"VD{var_id:03}")
+    
+    def set_variable_pos(self, var_id, x, y):
+        """
+        Set the display position of the stored variable with the given ID
+        to the given X and Y coordinates
+        """
+        
+        return self.send_command(f"VP{var_id:03}{x:03}{y:03}")
+    
+    def show_bargraph(self, bg_id):
+        """
+        Show the stored bargraph with the given ID
+        """
+        
+        return self.send_command(f"W+{bg_id:03}")
+    
+    def hide_bargraph(self, bg_id):
+        """
+        Hide the stored bargraph with the given ID
+        """
+        
+        return self.send_command(f"W-{bg_id:03}")
+    
+    def set_bargraph_value(self, bg_id, value):
+        """
+        Set the value of the stored variable with the given ID
+        """
+        
+        # Alternative command format: raw signed integer
+        # f"W={bg_id:03}I{high_byte}{low_byte}"
+        
+        sign = "+" if value >= 0 else "-"
+        return self.send_command(f"W={bg_id:03}A{sign}{abs(value):05}")
+    
+    def fill(self, color):
+        """
+        Fill the entire display with one color
+        
+        color:
+          One of self.COLORS
+        """
+        
+        color_flag = self.get_color_flag(color)
+        return self.send_command(f"F{color_flag}")
+    
+    def set_pixel(self, x, y, color):
+        """
+        Set the given pixel to the given color
+        
+        color:
+          One of self.COLORS
+        """
+        
+        color_flag = self.get_color_flag(color)
+        return self.send_command(f"P{color_flag}{x:03}{y:03}")
+    
+    def get_pixel(self, x, y):
+        """
+        Get the color of the given pixel
+        """
+        
+        response = self.send_command(f"P?{x:03}{y:03}", response_length=3)
+        color = self.COLORS[response[2] - ord("0")]
+        return color
+    
+    def rectangle(self, x1, y1, x2, y2, fg_color, bg_color):
+        """
+        Draw a rectangle with the given colors.
+        
+        x1, y1:
+          Coordinates of the top left corner
+        
+        x2, y2:
+          Coordinates of the bottom right corner
+        
+        fg_color:
+          One of self.COLORS
+        
+        bg_color:
+          One of self.COLORS or 'transparent'
+        """
+        
+        fg_flag = self.get_color_flag(fg_color)
+        bg_flag = self.get_color_flag(bg_color)
+        return self.send_command(f"R{fg_flag}{bg_flag}{x1:03}{y1:03}{x2:03}{y2:03}")
+    
+    def scroll_area_vertical(self, direction, speed, step, y1, y2, extended_range=False):
+        """
+        Scroll the area between lines y1 and y2 in the given direction,
+        at the given scroll interval, with the given step size.
+        
+        direction:
+          One of self.DIRECTIONS
+        
+        speed:
+          See set_scroll_speed
+        
+        step:
+          0 - No movement
+          1 to 9 - 1 to 9 pixels
+        
+        extended_range:
+          If True, use three characters for y1 and y2 (for displays with more than 64 rows)
+        """
+        
+        if extended_range:
+            return self.send_command(f"S{direction}{speed}{step}{y1:03}{y2:03}")
+        else:
+            return self.send_command(f"S{direction}{speed}{step}{y1:02}{y2:02}")
+    
+    def set_blink_period(self, period):
+        """
+        Set the blink period for all blinking texts
+        
+        period:
+          0 - 2 seconds
+          1 - 1.8 seconds
+          2 - 1.6 seconds
+          3 - 1.4 seconds
+          4 - 1.2 seconds
+          5 - 1 second
+          6 - 0.8 seconds
+          7 - 0.6 seconds
+          8 - 0.4 seconds
+          9 - 0.2 seconds
+        """
+        
+        return self.send_command(f"B{period}")
+    
+    def set_brightness(self, color, brightness):
+        """
+        Set the brightness for all LEDs of the given color
+        
+        color:
+          self.COLOR_RED or self.COLOR_GREEN
+        
+        brightness:
+          0 to 100
+        """
+        
+        color_flag = self.get_color_flag(color)
+        if color_flag not in (self.COLOR_RED, self.COLOR_GREEN):
+            raise ValueError("Color for set_brightness can only be red or green")
+        if color_flag == self.COLOR_GREEN:
+            color_flag = "1"
+        elif color_flag == self.COLOR_RED:
+            color_flag = "2"
+        return self.send_command(f"H{color_flag}{brightness:03}")
+    
+    def set_and_get_gpio(self, outputs):
+        """
+        Set the 16 general purpose outputs and return the state of the 16 inputs
+        
+        outputs:
+          List of 16 values:
+            True - Turn output on
+            False - Turn output off
+            None - Don't change output
+        
+        Returns:
+          A list in the same form as the outputs parameter
+        """
+        
+        def _get_output_flag(value):
+            if value is True:
+                return "1"
+            elif value is False:
+                return "0"
+            else:
+                return "N"
+        
+        output_flags = "".join(map(_get_output_flag, outputs))
+        response = self.send_command(f"D{output_flags}", response_length=18)
+        inputs = [(v == ord("1")) for v in response[2:]]
+        return inputs
+    
+    def run_macros(self, macro_id):
+        """
+        Run macros starting at the given ID
+        """
+        
+        return self.send_command(f"M{macro_id:03}")
+    
+    def run_macro_conditional(self, macro_id, input_channel, trigger_mode, trigger_state):
+        """
+        Run the macro with the given ID if the given digital input (0 to 15)
+        is currently in the given state (trigger mode NORMAL)
+        or has been in the given state at least once since the last call of this command
+        (trigger mode HISTORY)
+        
+        trigger_mode:
+          self.TRIG_NORMAL or self.TRIG_HISTORY
+        
+        trigger_state:
+          True or False (on or off)
+        """
+        
+        return self.send_command(f"M{macro_id:03}E{input_channel:1X}{trigger_mode}{trigger_state:1}")
+    
+    def wait(self, duration):
+        """
+        Pause macro execution for the given duration.
+        
+        duration:
+          Time to wait in seconds (0 to 99.9)
+        """
+        
+        duration_flag = int(duration * 10)
+        return self.send_command(f"w{duration_flag:03}")
+    
+    def stop_macros(self):
+        """
+        Stop macro execution.
+        """
+        
+        return self.send_command("E")
```

### Comparing `pyFIS-1.8.1/pyfis/omega/__init__.py` & `pyFIS-1.9.0/pyfis/omega/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .rs485 import OmegaRS485Controller
+"""
+Copyright (C) 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .rs485 import OmegaRS485Controller
```

### Comparing `pyFIS-1.8.1/pyfis/omega/rs485.py` & `pyFIS-1.9.0/pyfis/xatlabs/splitflap.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,113 @@
-"""
-Copyright (C) 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-import time
-
-
-class OmegaRS485Controller:
-    """
-    Controls split-flap modules using Omega's RS485 protocol.
-    Commonly found in Swiss (SBB CFF FFS) station displays.
-    """
-
-    def __init__(self, port, debug = False, exclusive = False):
-        self.debug = debug
-        if isinstance(port, serial.Serial):
-            self.port = port
-        else:
-            self.port = serial.Serial(port, baudrate=19200, timeout=1.0, exclusive=exclusive)
-
-    def prepare_message(self, address, command, value):
-        message = [0xFF, command, address]
-        if value is not None:
-            if type(value) in (tuple, list):
-                message.extend(value)
-            else:
-                message.append(value)
-        return message
-
-    def init_communication(self):
-        """
-        Initialize communication by asserting a break condition
-        on the serial Tx line for a certain time
-        """
-        self.port.break_condition = True
-        time.sleep(0.05)
-        self.port.break_condition = False
-
-    def send_raw_message(self, message):
-        if self.debug:
-            print(" ".join((format(x, "02X") for x in message)))
-        self.init_communication()
-        self.port.write(message)
-
-    def read_response(self, length):
-        return self.port.read(length)
-
-    def send_command(self, address, command, value = None):
-        message = self.prepare_message(address, command, value)
-        self.send_raw_message(message)
-
-    def set_home(self, address):
-        self.send_command(address, 0xC5)
-
-    def set_position(self, address, position):
-        self.send_command(address, 0xC0, position)
-
-    def set_address(self, address, new_address):
-        self.send_command(address, 0xCE, new_address)
-
-    def read_position(self, address):
-        self.send_command(address, 0xD0)
-        return self.read_response(4)
-
-    def read_serial_number(self, address):
-        self.send_command(address, 0xDF)
-        return self.read_response(1)
-
-    def d_set_module_data(self, module_data):
-        # Compatibility function for SplitFlapDisplay class
-        
-        # Turn module data into blocks of contiguous addresses
-        items = sorted(module_data, key=lambda i:i[0])
-        last_addr = None
-        start_addr = None
-        pos_block = []
-        for i, (addr, pos) in enumerate(items):
-            if (last_addr is not None and addr - last_addr > 1):
-                self.set_position(start_addr, pos_block)
-                time.sleep(0.05)
-                pos_block = []
-            if pos_block == []:
-                start_addr = addr
-            pos_block.append(pos)
-            if i == len(items) - 1:
-                self.set_position(start_addr, pos_block)
-                time.sleep(0.05)
-                pos_block = []
-            last_addr = addr
-
-    def d_update(self):
-        # Compatibility function for SplitFlapDisplay class
-        pass
+"""
+Copyright (C) 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+import time
+
+
+from .exceptions import CommunicationError
+
+
+class xatLabsSplitFlapController:
+    """
+    Controls the xatLabs Arduino-based generic split-flap controller.
+    This is basically just a very simple serial protocol for
+    setting specified split-flap units to specified positions.
+    """
+
+    ACT_SET_SEQ = 0xA0  # Set units sequentially
+    ACT_SET_ADDR = 0xA1 # Set units addressed
+    ACT_SET_HOME = 0xA2 # Set all units to home
+    ACT_UPDATE = 0xA3   # Start the units
+
+    def __init__(self, port, debug = False, exclusive = True):
+        self.debug = debug
+        if isinstance(port, serial.Serial):
+            self.port = port
+        else:
+            self.port = serial.Serial(port, baudrate=115200, timeout=2.0, exclusive=exclusive)
+
+    def debug_message(self, message):
+        """
+        Turn a message into a readable form
+        """
+        result = ""
+        for byte in message:
+            if byte in range(0, 32) or byte >= 127:
+                result += "<{:02X}>".format(byte)
+            else:
+                result += chr(byte)
+            result += " "
+        return result
+
+    def read_response(self):
+        """
+        Read the response from the addressed station
+        """
+        response = self.port.read(1)
+        if not response:
+            raise CommunicationError("Timeout waiting for response")
+        if self.debug:
+            print("RX: " + self.debug_message(response))
+        return response
+
+    def send_command(self, action, payload):
+        data = [0xFF, action, len(payload)] + payload
+        print("TX: " + self.debug_message(data))
+        self.port.write(bytearray(data))
+
+    def send_command_with_response(self, action, payload):
+        """
+        Send a command and retrieve the response data
+        """
+        self.send_command(action, payload)
+        return self.read_response()
+
+    def set_home(self):
+        """
+        Set all units to their home position
+        """
+        return self.send_command_with_response(self.ACT_SET_HOME, [])
+
+    def set_positions(self, positions):
+        """
+        Set all units with sequential addressing
+        positions: list of positions for units starting at address 0
+        """
+        return self.send_command_with_response(self.ACT_SET_SEQ, positions)
+
+    def set_positions_addressed(self, positions):
+        """
+        Set all units with explicit addressing
+        positions: dict of format {address: position}
+        """
+        pos_map = [item for k in positions for item in (k, positions[k])]
+        return self.send_command_with_response(self.ACT_SET_ADDR, pos_map)
+
+    def update(self):
+        """
+        Start the update of all units
+        """
+        return self.send_command_with_response(self.ACT_UPDATE, [])
+
+    def d_set_module_data(self, module_data):
+        # Compatibility function for SplitFlapDisplay class
+        self.set_positions_addressed(dict(module_data))
+
+    def d_update(self):
+        # Compatibility function for SplitFlapDisplay class
+        self.update()
```

### Comparing `pyFIS-1.8.1/pyfis/splitflap_display/display.py` & `pyFIS-1.9.0/pyfis/splitflap_display/display.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,287 +1,287 @@
-"""
-Copyright (C) 2019 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import random
-import time
-
-from .ascii_graphics import AsciiGraphics
-
-class SplitFlapDisplay:
-    TRANSITION_LEFT_TO_RIGHT = 'ltr'
-    TRANSITION_RIGHT_TO_LEFT = 'rtl'
-    TRANSITION_TOP_TO_BOTTOM = 'ttb'
-    TRANSITION_BOTTOM_TO_TOP = 'btt'
-    TRANSITION_MIDDLE_OUT_HORIZONTAL = 'moh'
-    TRANSITION_MIDDLE_OUT_VERTICAL = 'mov'
-    TRANSITION_MIDDLE_IN_HORIZONTAL = 'mih'
-    TRANSITION_MIDDLE_IN_VERTICAL = 'miv'
-    TRANSITION_SEQUENTIAL = 'seq'
-    TRANSITION_SEQUENTIAL_REVERSE = 'seq-rev'
-    TRANSITION_RANDOM = 'rnd'
-    TRANSITION_RANDOM_CHOICE = 'rndc'
-    
-    TRANSITIONS = [
-        TRANSITION_LEFT_TO_RIGHT,
-        TRANSITION_RIGHT_TO_LEFT,
-        TRANSITION_TOP_TO_BOTTOM,
-        TRANSITION_BOTTOM_TO_TOP,
-        TRANSITION_MIDDLE_OUT_HORIZONTAL,
-        TRANSITION_MIDDLE_OUT_VERTICAL,
-        TRANSITION_MIDDLE_IN_HORIZONTAL,
-        TRANSITION_MIDDLE_IN_VERTICAL,
-        TRANSITION_SEQUENTIAL,
-        TRANSITION_SEQUENTIAL_REVERSE,
-        TRANSITION_RANDOM
-    ]
-
-    def __init__(self, backend):
-        self.backend = backend
-        self.check_address_collisions()
-
-    def _group(self, data, key):
-        sorted_data = sorted(data, key=key)
-        prev_group = None
-        output = {}
-        for item in sorted_data:
-            group = key(item)
-            if group != prev_group:
-                prev_group = group
-                output[group] = [item]
-            else:
-                output[group].append(item)
-        return output
-    
-    def _interleave(self, list1, list2):
-        newlist = []
-        a1 = len(list1)
-        a2 = len(list2)
-        for i in range(max(a1, a2)):
-            if i < a1:
-                newlist.append(list1[i])
-            if i < a2:
-                newlist.append(list2[i])
-        return newlist
-    
-    def get_fields(self):
-        fields = []
-        for name in dir(self):
-            candidate = getattr(self, name)
-            if hasattr(candidate, '_is_field') and candidate._is_field == True:
-                fields.append((name, candidate))
-        return fields
-    
-    def clear(self):
-        """
-        Clear all fields
-        """
-        for name, field in self.get_fields():
-            field.clear()
-    
-    def check_address_collisions(self):
-        """
-        Checks if any of the addresses used by the fields are occupied
-        by more than one field and raises an exception is necessary
-        """
-        addresses = []
-        for name, field in self.get_fields():
-            addresses += field.address_mapping
-        if len(addresses) != len(set(addresses)):
-            raise ValueError("Some addresses are occupied by more than one field")
-    
-    def get_module_data(self):
-        """
-        Returns all addresses and associated codes of the modules
-        making up the display
-        """
-        module_data = []
-        fields = self.get_fields()
-        for name, field in fields:
-            module_data += field.get_module_data()
-        module_data.sort(key=lambda d:d[0])
-        return module_data
-    
-    def update(self, transition = None, interval = 0.1):
-        fields = self.get_fields()
-        module_data = self.get_module_data()
-        
-        if transition == self.TRANSITION_RANDOM_CHOICE:
-            transition = random.choice(self.TRANSITIONS)
-
-        if transition == self.TRANSITION_LEFT_TO_RIGHT:
-            module_data_by_x = self._group(module_data, lambda i: i[2])
-            min_x = min(module_data_by_x.keys())
-            max_x = max(module_data_by_x.keys())
-            for x in range(min_x, max_x+1):
-                if x in module_data_by_x:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
-                    self.backend.d_update()
-                time.sleep(interval)
-        elif transition == self.TRANSITION_RIGHT_TO_LEFT:
-            module_data_by_x = self._group(module_data, lambda i: i[2])
-            min_x = min(module_data_by_x.keys())
-            max_x = max(module_data_by_x.keys())
-            for x in range(max_x, min_x-1, -1):
-                if x in module_data_by_x:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
-                    self.backend.d_update()
-                time.sleep(interval)
-        elif transition == self.TRANSITION_TOP_TO_BOTTOM:
-            module_data_by_y = self._group(module_data, lambda i: i[3])
-            min_y = min(module_data_by_y.keys())
-            max_y = max(module_data_by_y.keys())
-            for y in range(min_y, max_y+1):
-                if y in module_data_by_y:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
-                    self.backend.d_update()
-                time.sleep(interval)
-        elif transition == self.TRANSITION_BOTTOM_TO_TOP:
-            module_data_by_y = self._group(module_data, lambda i: i[3])
-            min_y = min(module_data_by_y.keys())
-            max_y = max(module_data_by_y.keys())
-            for y in range(max_y, min_y-1, -1):
-                if y in module_data_by_y:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
-                    self.backend.d_update()
-                time.sleep(interval)
-        elif transition == self.TRANSITION_MIDDLE_OUT_HORIZONTAL:
-            module_data_by_x = self._group(module_data, lambda i: i[2])
-            min_x = min(module_data_by_x.keys())
-            max_x = max(module_data_by_x.keys())
-            mid_x = min_x + (max_x - min_x) // 2
-            pair_complete = True
-            for x in self._interleave(range(mid_x, min_x-1, -1), range(mid_x+1, max_x+1)):
-                if x in module_data_by_x:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
-                    self.backend.d_update()
-                pair_complete = not pair_complete
-                if pair_complete:
-                    time.sleep(interval)
-        elif transition == self.TRANSITION_MIDDLE_IN_HORIZONTAL:
-            module_data_by_x = self._group(module_data, lambda i: i[2])
-            min_x = min(module_data_by_x.keys())
-            max_x = max(module_data_by_x.keys())
-            mid_x = min_x + (max_x - min_x) // 2
-            pair_complete = True
-            for x in self._interleave(range(mid_x, min_x-1, -1), range(mid_x+1, max_x+1))[::-1]:
-                if x in module_data_by_x:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
-                    self.backend.d_update()
-                pair_complete = not pair_complete
-                if pair_complete:
-                    time.sleep(interval)
-        elif transition == self.TRANSITION_MIDDLE_OUT_VERTICAL:
-            module_data_by_y = self._group(module_data, lambda i: i[3])
-            min_y = min(module_data_by_y.keys())
-            max_y = max(module_data_by_y.keys())
-            mid_y = min_y + (max_y - min_y) // 2
-            pair_complete = True
-            for y in self._interleave(range(mid_y, min_y-1, -1), range(mid_y+1, max_y+1)):
-                if y in module_data_by_y:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
-                    self.backend.d_update()
-                pair_complete = not pair_complete
-                if pair_complete:
-                    time.sleep(interval)
-        elif transition == self.TRANSITION_MIDDLE_IN_VERTICAL:
-            module_data_by_y = self._group(module_data, lambda i: i[3])
-            min_y = min(module_data_by_y.keys())
-            max_y = max(module_data_by_y.keys())
-            mid_y = min_y + (max_y - min_y) // 2
-            pair_complete = True
-            for y in self._interleave(range(mid_y, min_y-1, -1), range(mid_y+1, max_y+1))[::-1]:
-                if y in module_data_by_y:
-                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
-                    self.backend.d_update()
-                pair_complete = not pair_complete
-                if pair_complete:
-                    time.sleep(interval)
-        elif transition == self.TRANSITION_SEQUENTIAL:
-            addrs = [md[0] for md in module_data]
-            codes = [md[1] for md in module_data]
-            min_addr = min(addrs)
-            max_addr = max(addrs)
-            for addr in range(min_addr, max_addr+1):
-                if addr in addrs:
-                    self.backend.d_set_module_data([(addr, codes[addrs.index(addr)])])
-                    self.backend.d_update()
-                time.sleep(interval)
-        elif transition == self.TRANSITION_SEQUENTIAL_REVERSE:
-            addrs = [md[0] for md in module_data]
-            codes = [md[1] for md in module_data]
-            min_addr = min(addrs)
-            max_addr = max(addrs)
-            for addr in range(max_addr, min_addr-1, -1):
-                if addr in addrs:
-                    self.backend.d_set_module_data([(addr, codes[addrs.index(addr)])])
-                    self.backend.d_update()
-                time.sleep(interval)
-        elif transition == self.TRANSITION_RANDOM:
-            random.shuffle(module_data)
-            for addr, pos, x, y in module_data:
-                self.backend.d_set_module_data([(addr, pos)])
-                self.backend.d_update()
-                time.sleep(interval)
-        else:
-            self.backend.d_set_module_data([md[:2] for md in module_data])
-            self.backend.d_update()
-    
-    def get_size(self):
-        """
-        Calculates the size of the display based on the position and size
-        of its fields
-        """
-        width = 0
-        height = 0
-        for name, field in self.get_fields():
-            f_params = field.get_ascii_render_parameters()
-            x = f_params['x']
-            y = f_params['y']
-            f_end_x = x + f_params['width']
-            f_end_y = y + f_params['height']
-            if f_end_x > width:
-                width = f_end_x
-            if f_end_y > height:
-                height = f_end_y
-        return (width, height)
-    
-    def render_ascii(self):
-        """
-        Renders the display layout as ASCII graphics using ASCII frame symbols
-        """
-        width, height = self.get_size()
-        graphics = AsciiGraphics(width, height)
-        for name, field in self.get_fields():
-            f_params = field.get_ascii_render_parameters()
-            x = f_params['x']
-            y = f_params['y']
-            graphics.draw_rectangle(x, y, f_params['width'], f_params['height'])
-            f_value = field.get()
-            if type(f_value) in (list, tuple):
-                for i, text in enumerate(f_value):
-                    rendered_text = text[:f_params['text_max_length']]
-                    if field.text_align == 'left':
-                        rendered_text = rendered_text.ljust(f_params['text_max_length'])
-                    elif field.text_align == 'center':
-                        rendered_text = rendered_text.center(f_params['text_max_length'])
-                    elif field.text_align == 'right':
-                        rendered_text = rendered_text.rjust(f_params['text_max_length'])
-                    graphics.draw_text(x + f_params['x_offset'] + i * f_params['spacing'], y + f_params['y_offset'], rendered_text, f_params['text_spacing'])
-            else:
-                graphics.draw_text(x + f_params['x_offset'], y + f_params['y_offset'], field.get(), f_params['text_spacing'])
-            for i in range(field.length - 1):
-                graphics.draw_line(x + f_params['spacing'] * (i+1), y, f_params['height'], 'v', t_ends=True)
-        return graphics.render()
+"""
+Copyright (C) 2019 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import random
+import time
+
+from .ascii_graphics import AsciiGraphics
+
+class SplitFlapDisplay:
+    TRANSITION_LEFT_TO_RIGHT = 'ltr'
+    TRANSITION_RIGHT_TO_LEFT = 'rtl'
+    TRANSITION_TOP_TO_BOTTOM = 'ttb'
+    TRANSITION_BOTTOM_TO_TOP = 'btt'
+    TRANSITION_MIDDLE_OUT_HORIZONTAL = 'moh'
+    TRANSITION_MIDDLE_OUT_VERTICAL = 'mov'
+    TRANSITION_MIDDLE_IN_HORIZONTAL = 'mih'
+    TRANSITION_MIDDLE_IN_VERTICAL = 'miv'
+    TRANSITION_SEQUENTIAL = 'seq'
+    TRANSITION_SEQUENTIAL_REVERSE = 'seq-rev'
+    TRANSITION_RANDOM = 'rnd'
+    TRANSITION_RANDOM_CHOICE = 'rndc'
+    
+    TRANSITIONS = [
+        TRANSITION_LEFT_TO_RIGHT,
+        TRANSITION_RIGHT_TO_LEFT,
+        TRANSITION_TOP_TO_BOTTOM,
+        TRANSITION_BOTTOM_TO_TOP,
+        TRANSITION_MIDDLE_OUT_HORIZONTAL,
+        TRANSITION_MIDDLE_OUT_VERTICAL,
+        TRANSITION_MIDDLE_IN_HORIZONTAL,
+        TRANSITION_MIDDLE_IN_VERTICAL,
+        TRANSITION_SEQUENTIAL,
+        TRANSITION_SEQUENTIAL_REVERSE,
+        TRANSITION_RANDOM
+    ]
+
+    def __init__(self, backend):
+        self.backend = backend
+        self.check_address_collisions()
+
+    def _group(self, data, key):
+        sorted_data = sorted(data, key=key)
+        prev_group = None
+        output = {}
+        for item in sorted_data:
+            group = key(item)
+            if group != prev_group:
+                prev_group = group
+                output[group] = [item]
+            else:
+                output[group].append(item)
+        return output
+    
+    def _interleave(self, list1, list2):
+        newlist = []
+        a1 = len(list1)
+        a2 = len(list2)
+        for i in range(max(a1, a2)):
+            if i < a1:
+                newlist.append(list1[i])
+            if i < a2:
+                newlist.append(list2[i])
+        return newlist
+    
+    def get_fields(self):
+        fields = []
+        for name in dir(self):
+            candidate = getattr(self, name)
+            if hasattr(candidate, '_is_field') and candidate._is_field == True:
+                fields.append((name, candidate))
+        return fields
+    
+    def clear(self):
+        """
+        Clear all fields
+        """
+        for name, field in self.get_fields():
+            field.clear()
+    
+    def check_address_collisions(self):
+        """
+        Checks if any of the addresses used by the fields are occupied
+        by more than one field and raises an exception is necessary
+        """
+        addresses = []
+        for name, field in self.get_fields():
+            addresses += field.address_mapping
+        if len(addresses) != len(set(addresses)):
+            raise ValueError("Some addresses are occupied by more than one field")
+    
+    def get_module_data(self):
+        """
+        Returns all addresses and associated codes of the modules
+        making up the display
+        """
+        module_data = []
+        fields = self.get_fields()
+        for name, field in fields:
+            module_data += field.get_module_data()
+        module_data.sort(key=lambda d:d[0])
+        return module_data
+    
+    def update(self, transition = None, interval = 0.1):
+        fields = self.get_fields()
+        module_data = self.get_module_data()
+        
+        if transition == self.TRANSITION_RANDOM_CHOICE:
+            transition = random.choice(self.TRANSITIONS)
+
+        if transition == self.TRANSITION_LEFT_TO_RIGHT:
+            module_data_by_x = self._group(module_data, lambda i: i[2])
+            min_x = min(module_data_by_x.keys())
+            max_x = max(module_data_by_x.keys())
+            for x in range(min_x, max_x+1):
+                if x in module_data_by_x:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
+                    self.backend.d_update()
+                time.sleep(interval)
+        elif transition == self.TRANSITION_RIGHT_TO_LEFT:
+            module_data_by_x = self._group(module_data, lambda i: i[2])
+            min_x = min(module_data_by_x.keys())
+            max_x = max(module_data_by_x.keys())
+            for x in range(max_x, min_x-1, -1):
+                if x in module_data_by_x:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
+                    self.backend.d_update()
+                time.sleep(interval)
+        elif transition == self.TRANSITION_TOP_TO_BOTTOM:
+            module_data_by_y = self._group(module_data, lambda i: i[3])
+            min_y = min(module_data_by_y.keys())
+            max_y = max(module_data_by_y.keys())
+            for y in range(min_y, max_y+1):
+                if y in module_data_by_y:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
+                    self.backend.d_update()
+                time.sleep(interval)
+        elif transition == self.TRANSITION_BOTTOM_TO_TOP:
+            module_data_by_y = self._group(module_data, lambda i: i[3])
+            min_y = min(module_data_by_y.keys())
+            max_y = max(module_data_by_y.keys())
+            for y in range(max_y, min_y-1, -1):
+                if y in module_data_by_y:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
+                    self.backend.d_update()
+                time.sleep(interval)
+        elif transition == self.TRANSITION_MIDDLE_OUT_HORIZONTAL:
+            module_data_by_x = self._group(module_data, lambda i: i[2])
+            min_x = min(module_data_by_x.keys())
+            max_x = max(module_data_by_x.keys())
+            mid_x = min_x + (max_x - min_x) // 2
+            pair_complete = True
+            for x in self._interleave(range(mid_x, min_x-1, -1), range(mid_x+1, max_x+1)):
+                if x in module_data_by_x:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
+                    self.backend.d_update()
+                pair_complete = not pair_complete
+                if pair_complete:
+                    time.sleep(interval)
+        elif transition == self.TRANSITION_MIDDLE_IN_HORIZONTAL:
+            module_data_by_x = self._group(module_data, lambda i: i[2])
+            min_x = min(module_data_by_x.keys())
+            max_x = max(module_data_by_x.keys())
+            mid_x = min_x + (max_x - min_x) // 2
+            pair_complete = True
+            for x in self._interleave(range(mid_x, min_x-1, -1), range(mid_x+1, max_x+1))[::-1]:
+                if x in module_data_by_x:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_x[x]])
+                    self.backend.d_update()
+                pair_complete = not pair_complete
+                if pair_complete:
+                    time.sleep(interval)
+        elif transition == self.TRANSITION_MIDDLE_OUT_VERTICAL:
+            module_data_by_y = self._group(module_data, lambda i: i[3])
+            min_y = min(module_data_by_y.keys())
+            max_y = max(module_data_by_y.keys())
+            mid_y = min_y + (max_y - min_y) // 2
+            pair_complete = True
+            for y in self._interleave(range(mid_y, min_y-1, -1), range(mid_y+1, max_y+1)):
+                if y in module_data_by_y:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
+                    self.backend.d_update()
+                pair_complete = not pair_complete
+                if pair_complete:
+                    time.sleep(interval)
+        elif transition == self.TRANSITION_MIDDLE_IN_VERTICAL:
+            module_data_by_y = self._group(module_data, lambda i: i[3])
+            min_y = min(module_data_by_y.keys())
+            max_y = max(module_data_by_y.keys())
+            mid_y = min_y + (max_y - min_y) // 2
+            pair_complete = True
+            for y in self._interleave(range(mid_y, min_y-1, -1), range(mid_y+1, max_y+1))[::-1]:
+                if y in module_data_by_y:
+                    self.backend.d_set_module_data([md[:2] for md in module_data_by_y[y]])
+                    self.backend.d_update()
+                pair_complete = not pair_complete
+                if pair_complete:
+                    time.sleep(interval)
+        elif transition == self.TRANSITION_SEQUENTIAL:
+            addrs = [md[0] for md in module_data]
+            codes = [md[1] for md in module_data]
+            min_addr = min(addrs)
+            max_addr = max(addrs)
+            for addr in range(min_addr, max_addr+1):
+                if addr in addrs:
+                    self.backend.d_set_module_data([(addr, codes[addrs.index(addr)])])
+                    self.backend.d_update()
+                time.sleep(interval)
+        elif transition == self.TRANSITION_SEQUENTIAL_REVERSE:
+            addrs = [md[0] for md in module_data]
+            codes = [md[1] for md in module_data]
+            min_addr = min(addrs)
+            max_addr = max(addrs)
+            for addr in range(max_addr, min_addr-1, -1):
+                if addr in addrs:
+                    self.backend.d_set_module_data([(addr, codes[addrs.index(addr)])])
+                    self.backend.d_update()
+                time.sleep(interval)
+        elif transition == self.TRANSITION_RANDOM:
+            random.shuffle(module_data)
+            for addr, pos, x, y in module_data:
+                self.backend.d_set_module_data([(addr, pos)])
+                self.backend.d_update()
+                time.sleep(interval)
+        else:
+            self.backend.d_set_module_data([md[:2] for md in module_data])
+            self.backend.d_update()
+    
+    def get_size(self):
+        """
+        Calculates the size of the display based on the position and size
+        of its fields
+        """
+        width = 0
+        height = 0
+        for name, field in self.get_fields():
+            f_params = field.get_ascii_render_parameters()
+            x = f_params['x']
+            y = f_params['y']
+            f_end_x = x + f_params['width']
+            f_end_y = y + f_params['height']
+            if f_end_x > width:
+                width = f_end_x
+            if f_end_y > height:
+                height = f_end_y
+        return (width, height)
+    
+    def render_ascii(self):
+        """
+        Renders the display layout as ASCII graphics using ASCII frame symbols
+        """
+        width, height = self.get_size()
+        graphics = AsciiGraphics(width, height)
+        for name, field in self.get_fields():
+            f_params = field.get_ascii_render_parameters()
+            x = f_params['x']
+            y = f_params['y']
+            graphics.draw_rectangle(x, y, f_params['width'], f_params['height'])
+            f_value = field.get()
+            if type(f_value) in (list, tuple):
+                for i, text in enumerate(f_value):
+                    rendered_text = text[:f_params['text_max_length']]
+                    if field.text_align == 'left':
+                        rendered_text = rendered_text.ljust(f_params['text_max_length'])
+                    elif field.text_align == 'center':
+                        rendered_text = rendered_text.center(f_params['text_max_length'])
+                    elif field.text_align == 'right':
+                        rendered_text = rendered_text.rjust(f_params['text_max_length'])
+                    graphics.draw_text(x + f_params['x_offset'] + i * f_params['spacing'], y + f_params['y_offset'], rendered_text, f_params['text_spacing'])
+            else:
+                graphics.draw_text(x + f_params['x_offset'], y + f_params['y_offset'], field.get(), f_params['text_spacing'])
+            for i in range(field.length - 1):
+                graphics.draw_line(x + f_params['spacing'] * (i+1), y, f_params['height'], 'v', t_ends=True)
+        return graphics.render()
```

### Comparing `pyFIS-1.8.1/pyfis/splitflap_display/fields.py` & `pyFIS-1.9.0/pyfis/splitflap_display/fields.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-"""
-Copyright (C) 2019 - 2020 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-class BaseField:
-    # This is needed so Form.get_fields() will know what to include
-    _is_field = True
-    
-    def __init__(self, start_address = None, length = 1, descending = False,
-                 text_align = 'left',
-                 address_mapping = None, display_mapping = None,
-                 x = 0, y = 0, module_width = 1, module_height = 1, home_pos = 0):
-        """
-        start_address: the address of the first module in this field
-        length: How many modules make up this field
-        descending: If using start_address, select descending addresses
-        text_align: Alignment of the text (left, center, right)
-        address_mapping: If modules have non-sequential addresses, the list of
-                         addresses corresponding to the digits in this field
-        display_mapping: Optional mapping of split-flap card numbers to
-                         displayed text or symbols for all modules in this field
-        x: Horizontal offset of the field in multiples of the smallest unit size
-        y: Vertical offset of the field in multiples of the smallest unit size
-        module_width: Width of the modules making up the field in multiples
-                       of the smallest unit size
-        module_height: Height of the modules making up the field in multiples
-                       of the smallest unit size
-        home_pos: ID of the home position. Should be 0, but is different in some cases
-        """
-        if start_address is None and address_mapping is None:
-            raise AttributeError("Either start_address or address_mapping must be present")
-        if type(length) is not int or length <= 0:
-            raise ValueError("length must be a positive integer")
-        if start_address is not None:
-            if start_address not in range(256):
-                raise ValueError("start_address must be an int between 0 and 255")
-            if descending:
-                if start_address - length < 0:
-                    raise ValueError("Field is too long for given start address")
-            else:
-                if start_address + length > 256:
-                    raise ValueError("Field is too long for given start address")
-        if address_mapping is not None:
-            if len(address_mapping) != length:
-                raise ValueError("Length of address_mapping doesn't match field length")
-        self.start_address = start_address
-        self.length = length
-        self.descending = descending
-        if text_align not in ('left', 'center', 'right'):
-            raise ValueError("text_align must be left, center or right")
-        self.text_align = text_align
-        if address_mapping is not None:
-            self.address_mapping = address_mapping
-        else:
-            if self.descending:
-                self.address_mapping = list(range(start_address, start_address-length, -1))
-            else:
-                self.address_mapping = list(range(start_address, start_address+length))
-        self.display_mapping = display_mapping
-        if display_mapping is not None:
-            self.inverse_display_mapping = {v: k for k, v in display_mapping.items()}
-        else:
-            self.inverse_display_mapping = None
-        self.x = x
-        self.y = y
-        self.module_width = module_width
-        self.module_height = module_height
-        self.home_pos = home_pos
-        self.value = " " * self.length
-        self.mirrors = []
-    
-    def set(self, value):
-        self.value = value
-    
-    def get(self):
-        return self.value
-    
-    def clear(self):
-        self.value = " " * self.length
-    
-    def get_single_module_data(self, pos):
-        raise NotImplementedError
-    
-    def get_module_data(self):
-        module_data = []
-        for i in range(self.length):
-            module_data.append(self.get_single_module_data(i))
-        return module_data
-    
-    def get_ascii_render_parameters(self):
-        """
-        Calculate the parameters needed to render the field as ASCII graphics
-        """
-        parameters = {
-            'x': self.x * 2,
-            'y': self.y * 2,
-            'width': self.length * 2 * self.module_width + 1,
-            'height': 2 * self.module_height + 1,
-            'spacing': 2 * self.module_width,
-            'text_spacing': 2 * self.module_width,
-            'x_offset': self.module_width,
-            'y_offset': self.module_height,
-            'text_max_length': 2 * self.module_width - 1,
-        }
-        return parameters
-
-    def add_mirror(self, field):
-        """
-        Add a field to the list of mirror fields
-        """
-        if field not in self.mirrors:
-            self.mirrors.append(field)
-
-    def remove_mirror(self, field):
-        """
-        Remove a field from the list of mirror fields
-        """
-        while field in self.mirrors:
-            self.mirrors.remove(field)
-
-    def update_mirrors(self):
-        """
-        Update all mirror fields of this field
-        """
-        for field in self.mirrors:
-            if type(self.value) is list:
-                field.value = self.value.copy()
-            else:
-                field.value = self.value
-
-
-class MirrorField(BaseField):
-    """
-    This special field is set up so it mirrors an existing field.
-    """
-    def __init__(self, source_field, *args, **kwargs):
-        if not isinstance(source_field, BaseField):
-            raise ValueError("source_field must be an instance of a Field subclass")
-        if 'start_address' not in kwargs:
-            kwargs['start_address'] = source_field.start_address
-        if 'length' not in kwargs:
-            kwargs['length'] = source_field.length
-        if 'descending' not in kwargs:
-            kwargs['descending'] = source_field.descending
-        if 'text_align' not in kwargs:
-            kwargs['text_align'] = source_field.text_align
-        if 'display_mapping' not in kwargs:
-            kwargs['display_mapping'] = source_field.display_mapping
-        if 'x' not in kwargs:
-            kwargs['x'] = source_field.x
-        if 'y' not in kwargs:
-            kwargs['y'] = source_field.y
-        if 'module_width' not in kwargs:
-            kwargs['module_width'] = source_field.module_width
-        if 'module_height' not in kwargs:
-            kwargs['module_height'] = source_field.module_height
-        if 'home_pos' not in kwargs:
-            kwargs['home_pos'] = source_field.home_pos
-        super().__init__(*args, **kwargs)
-        self.source_field = source_field
-        source_field.add_mirror(self)
-
-    def set(self, value):
-        pass
-
-    def get(self):
-        return self.source_field.get()
-
-    def clear(self):
-        pass
-
-    def get_single_module_data(self, pos):
-        addr, code, dummy_x, dummy_y = self.source_field.get_single_module_data(pos)
-        x = self.x + pos * self.module_width
-        return self.address_mapping[pos], code, x, self.y
-
-    def get_module_data(self):
-        module_data = []
-        for i in range(self.length):
-            module_data.append(self.get_single_module_data(i))
-        return module_data
-
-    def get_ascii_render_parameters(self):
-        """
-        Get the base parameters from the source field,
-        but change the x and y values to allow for different placement
-        """
-        parameters = self.source_field.get_ascii_render_parameters()
-        parameters.update({
-            'x': self.x * 2,
-            'y': self.y * 2,
-        })
-        return parameters
-
-
-class TextField(BaseField):
-    def __init__(self, *args, value = "", upper_only = True, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.upper_only = upper_only
-        self.set(value)
-    
-    def set(self, value):
-        if type(value) is not str:
-            raise ValueError("value must be str")
-        if self.upper_only:
-            value = value.upper()
-        self.value = value[:self.length]
-        if self.text_align == 'left':
-            self.value = self.value.ljust(self.length)
-        elif self.text_align == 'center':
-            self.value = self.value.center(self.length)
-        elif self.text_align == 'right':
-            self.value = self.value.rjust(self.length)
-        self.update_mirrors()
-    
-    def get_single_module_data(self, pos):
-        """
-        Returns the split-flap module address and code for the given position
-        in the field with the current field value
-        """
-        if pos >= self.length:
-            raise ValueError("pos must be inside field boundaries")
-        addr = self.address_mapping[pos]
-        char = self.value[pos]
-        if self.display_mapping is not None:
-            code = self.inverse_display_mapping.get(char, self.home_pos)
-        else:
-            code = ord(char.encode('iso-8859-1'))
-        x = self.x + pos * self.module_width
-        return addr, code, x, self.y
-
-
-class CustomMapField(BaseField):
-    def __init__(self, display_mapping, *args, value = [], **kwargs):
-        super().__init__(*args, display_mapping=display_mapping, **kwargs)
-        self.value = [""] * self.length
-        self.set(value)
-
-    def set(self, value):
-        if type(value) not in (list, tuple):
-            value = [value] * self.length
-        value = value[:self.length] + [""] * (self.length - len(value))
-        for i, module_value in enumerate(value):
-            if module_value not in self.inverse_display_mapping:
-                self.value[i] = ""
-            else:
-                self.value[i] = module_value
-        self.update_mirrors()
-    
-    def clear(self):
-        self.value = [""] * self.length
-        self.update_mirrors()
-    
-    def get_single_module_data(self, pos):
-        """
-        Returns the split-flap module address and code for the given position
-        in the field with the current field value
-        """
-        if pos >= self.length:
-            raise ValueError("pos must be inside field boundaries")
-        addr = self.address_mapping[pos]
-        display_value = self.value[pos]
-        code = self.inverse_display_mapping.get(display_value, self.home_pos)
-        x = self.x + pos * self.module_width
-        return addr, code, x, self.y
-    
-    def get_ascii_render_parameters(self):
-        parameters = super().get_ascii_render_parameters()
-        parameters['x_offset'] = 1
-        parameters['text_spacing'] = 1
+"""
+Copyright (C) 2019 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+class BaseField:
+    # This is needed so Form.get_fields() will know what to include
+    _is_field = True
+    
+    def __init__(self, start_address = None, length = 1, descending = False,
+                 text_align = 'left',
+                 address_mapping = None, display_mapping = None,
+                 x = 0, y = 0, module_width = 1, module_height = 1, home_pos = 0):
+        """
+        start_address: the address of the first module in this field
+        length: How many modules make up this field
+        descending: If using start_address, select descending addresses
+        text_align: Alignment of the text (left, center, right)
+        address_mapping: If modules have non-sequential addresses, the list of
+                         addresses corresponding to the digits in this field
+        display_mapping: Optional mapping of split-flap card numbers to
+                         displayed text or symbols for all modules in this field
+        x: Horizontal offset of the field in multiples of the smallest unit size
+        y: Vertical offset of the field in multiples of the smallest unit size
+        module_width: Width of the modules making up the field in multiples
+                       of the smallest unit size
+        module_height: Height of the modules making up the field in multiples
+                       of the smallest unit size
+        home_pos: ID of the home position. Should be 0, but is different in some cases
+        """
+        if start_address is None and address_mapping is None:
+            raise AttributeError("Either start_address or address_mapping must be present")
+        if type(length) is not int or length <= 0:
+            raise ValueError("length must be a positive integer")
+        if start_address is not None:
+            if start_address not in range(256):
+                raise ValueError("start_address must be an int between 0 and 255")
+            if descending:
+                if start_address - length < 0:
+                    raise ValueError("Field is too long for given start address")
+            else:
+                if start_address + length > 256:
+                    raise ValueError("Field is too long for given start address")
+        if address_mapping is not None:
+            if len(address_mapping) != length:
+                raise ValueError("Length of address_mapping doesn't match field length")
+        self.start_address = start_address
+        self.length = length
+        self.descending = descending
+        if text_align not in ('left', 'center', 'right'):
+            raise ValueError("text_align must be left, center or right")
+        self.text_align = text_align
+        if address_mapping is not None:
+            self.address_mapping = address_mapping
+        else:
+            if self.descending:
+                self.address_mapping = list(range(start_address, start_address-length, -1))
+            else:
+                self.address_mapping = list(range(start_address, start_address+length))
+        self.display_mapping = display_mapping
+        if display_mapping is not None:
+            self.inverse_display_mapping = {v: k for k, v in display_mapping.items()}
+        else:
+            self.inverse_display_mapping = None
+        self.x = x
+        self.y = y
+        self.module_width = module_width
+        self.module_height = module_height
+        self.home_pos = home_pos
+        self.value = " " * self.length
+        self.mirrors = []
+    
+    def set(self, value):
+        self.value = value
+    
+    def get(self):
+        return self.value
+    
+    def clear(self):
+        self.value = " " * self.length
+    
+    def get_single_module_data(self, pos):
+        raise NotImplementedError
+    
+    def get_module_data(self):
+        module_data = []
+        for i in range(self.length):
+            module_data.append(self.get_single_module_data(i))
+        return module_data
+    
+    def get_ascii_render_parameters(self):
+        """
+        Calculate the parameters needed to render the field as ASCII graphics
+        """
+        parameters = {
+            'x': self.x * 2,
+            'y': self.y * 2,
+            'width': self.length * 2 * self.module_width + 1,
+            'height': 2 * self.module_height + 1,
+            'spacing': 2 * self.module_width,
+            'text_spacing': 2 * self.module_width,
+            'x_offset': self.module_width,
+            'y_offset': self.module_height,
+            'text_max_length': 2 * self.module_width - 1,
+        }
+        return parameters
+
+    def add_mirror(self, field):
+        """
+        Add a field to the list of mirror fields
+        """
+        if field not in self.mirrors:
+            self.mirrors.append(field)
+
+    def remove_mirror(self, field):
+        """
+        Remove a field from the list of mirror fields
+        """
+        while field in self.mirrors:
+            self.mirrors.remove(field)
+
+    def update_mirrors(self):
+        """
+        Update all mirror fields of this field
+        """
+        for field in self.mirrors:
+            if type(self.value) is list:
+                field.value = self.value.copy()
+            else:
+                field.value = self.value
+
+
+class MirrorField(BaseField):
+    """
+    This special field is set up so it mirrors an existing field.
+    """
+    def __init__(self, source_field, *args, **kwargs):
+        if not isinstance(source_field, BaseField):
+            raise ValueError("source_field must be an instance of a Field subclass")
+        if 'start_address' not in kwargs:
+            kwargs['start_address'] = source_field.start_address
+        if 'length' not in kwargs:
+            kwargs['length'] = source_field.length
+        if 'descending' not in kwargs:
+            kwargs['descending'] = source_field.descending
+        if 'text_align' not in kwargs:
+            kwargs['text_align'] = source_field.text_align
+        if 'display_mapping' not in kwargs:
+            kwargs['display_mapping'] = source_field.display_mapping
+        if 'x' not in kwargs:
+            kwargs['x'] = source_field.x
+        if 'y' not in kwargs:
+            kwargs['y'] = source_field.y
+        if 'module_width' not in kwargs:
+            kwargs['module_width'] = source_field.module_width
+        if 'module_height' not in kwargs:
+            kwargs['module_height'] = source_field.module_height
+        if 'home_pos' not in kwargs:
+            kwargs['home_pos'] = source_field.home_pos
+        super().__init__(*args, **kwargs)
+        self.source_field = source_field
+        source_field.add_mirror(self)
+
+    def set(self, value):
+        pass
+
+    def get(self):
+        return self.source_field.get()
+
+    def clear(self):
+        pass
+
+    def get_single_module_data(self, pos):
+        addr, code, dummy_x, dummy_y = self.source_field.get_single_module_data(pos)
+        x = self.x + pos * self.module_width
+        return self.address_mapping[pos], code, x, self.y
+
+    def get_module_data(self):
+        module_data = []
+        for i in range(self.length):
+            module_data.append(self.get_single_module_data(i))
+        return module_data
+
+    def get_ascii_render_parameters(self):
+        """
+        Get the base parameters from the source field,
+        but change the x and y values to allow for different placement
+        """
+        parameters = self.source_field.get_ascii_render_parameters()
+        parameters.update({
+            'x': self.x * 2,
+            'y': self.y * 2,
+        })
+        return parameters
+
+
+class TextField(BaseField):
+    def __init__(self, *args, value = "", upper_only = True, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.upper_only = upper_only
+        self.set(value)
+    
+    def set(self, value):
+        if type(value) is not str:
+            raise ValueError("value must be str")
+        if self.upper_only:
+            value = value.upper()
+        self.value = value[:self.length]
+        if self.text_align == 'left':
+            self.value = self.value.ljust(self.length)
+        elif self.text_align == 'center':
+            self.value = self.value.center(self.length)
+        elif self.text_align == 'right':
+            self.value = self.value.rjust(self.length)
+        self.update_mirrors()
+    
+    def get_single_module_data(self, pos):
+        """
+        Returns the split-flap module address and code for the given position
+        in the field with the current field value
+        """
+        if pos >= self.length:
+            raise ValueError("pos must be inside field boundaries")
+        addr = self.address_mapping[pos]
+        char = self.value[pos]
+        if self.display_mapping is not None:
+            code = self.inverse_display_mapping.get(char, self.home_pos)
+        else:
+            code = ord(char.encode('iso-8859-1'))
+        x = self.x + pos * self.module_width
+        return addr, code, x, self.y
+
+
+class CustomMapField(BaseField):
+    def __init__(self, display_mapping, *args, value = [], **kwargs):
+        super().__init__(*args, display_mapping=display_mapping, **kwargs)
+        self.value = [""] * self.length
+        self.set(value)
+
+    def set(self, value):
+        if type(value) not in (list, tuple):
+            value = [value] * self.length
+        value = value[:self.length] + [""] * (self.length - len(value))
+        for i, module_value in enumerate(value):
+            if module_value not in self.inverse_display_mapping:
+                self.value[i] = ""
+            else:
+                self.value[i] = module_value
+        self.update_mirrors()
+    
+    def clear(self):
+        self.value = [""] * self.length
+        self.update_mirrors()
+    
+    def get_single_module_data(self, pos):
+        """
+        Returns the split-flap module address and code for the given position
+        in the field with the current field value
+        """
+        if pos >= self.length:
+            raise ValueError("pos must be inside field boundaries")
+        addr = self.address_mapping[pos]
+        display_value = self.value[pos]
+        code = self.inverse_display_mapping.get(display_value, self.home_pos)
+        x = self.x + pos * self.module_width
+        return addr, code, x, self.y
+    
+    def get_ascii_render_parameters(self):
+        parameters = super().get_ascii_render_parameters()
+        parameters['x_offset'] = 1
+        parameters['text_spacing'] = 1
         return parameters
```

### Comparing `pyFIS-1.8.1/pyfis/utils/__init__.py` & `pyFIS-1.9.0/pyfis/splitflap_display/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-"""
-Copyright (C) 2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .utils import *
+"""
+Copyright (C) 2019 - 2020 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .display import SplitFlapDisplay
+from .fields import TextField, CustomMapField, MirrorField
+from .ascii_graphics import AsciiGraphics
```

### Comparing `pyFIS-1.8.1/pyfis/utils/utils.py` & `pyFIS-1.9.0/pyfis/utils/utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-"""
-Copyright (C) 2021-2022 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import itertools
-
-
-def _debug_print(debug, *args, **kwargs):
-    if debug:
-        print(*args, **kwargs)
-
-def debug_hex(message, readable_ascii = False, readable_ctrl = False):
-    """
-    Turn a message into a readable form
-    """
-
-    CTRL_CHARS = {
-        0x02: "STX",
-        0x03: "ETX",
-        0x04: "EOT",
-        0x05: "ENQ",
-        0x10: "DLE",
-        0x15: "NAK",
-        0x17: "ETB"
-    }
-
-    result = []
-    for byte in message:
-        if readable_ctrl and byte in CTRL_CHARS:
-            result.append(CTRL_CHARS[byte])
-        elif readable_ascii and byte not in range(0, 32) and byte != 127:
-            result.append(chr(byte))
-        else:
-            result.append("{:02X}".format(byte))
-    return " ".join(result)
-
-
-def vias_in_route(route, vias):
-    # Check if the given vias are all present in the given route in the right order
-    # If an entry in vias is a list, all of its items will be considered to be aliases of each other
-    i = 0
-    j = 0
-    while i < len(route) and j < len(vias):
-        if type(vias[j]) in (tuple, list):
-            for alias in vias[j]:
-                if route[i] == alias:
-                    j += 1
-                    break
-        else:
-            if route[i] == vias[j]:
-                j += 1
-        i += 1
-    return j == len(vias)
-
-
-def get_vias(route, weights, *via_groups, check_dashes=True, debug=False):
-    # Get the ideal combination of vias based on split-flap modules
-    num_groups = len(via_groups)
-    
-    # Go through all via groups and take note of possible candidates
-    via_candidates = []
-    for group in via_groups:
-        group_candidates = []
-        for pos, entry in group.items():
-            if vias_in_route(route, entry['stations']):
-                group_candidates.append(pos)
-        via_candidates.append(group_candidates)
-    _debug_print(debug, "Via candidates:")
-    _debug_print(debug, via_candidates)
-    
-    # Check all combinations to see if the order makes sense
-    combinations = itertools.product(*via_candidates)
-    valid_combinations = []
-    _debug_print(debug, "\nVia candidates with sensible order:")
-    for combination in combinations:
-        stations = []
-        for group, pos in enumerate(combination):
-            stations.extend(via_groups[group][pos]['stations'])
-        if vias_in_route(route, stations):
-            _debug_print(debug, combination, stations)
-            valid_combinations.append(combination)
-    
-    # If check_dashes is True, check if the starts and endings are compatible,
-    # i.e. if the first segment ends on a dash, the next one
-    # cannot start with one.
-    if check_dashes:
-        valid_dash_combinations = []
-        _debug_print(debug, "\nCandidates after check_dashes:")
-        for combination in valid_combinations:
-            valid = True
-            prev_text = None
-            for group, pos in enumerate(combination):
-                text = via_groups[group][pos]['text'].strip()
-                if group > 0:
-                    if prev_text and text and prev_text.endswith("-") == text.startswith("-"):
-                        _debug_print(debug, "Excluded: ", prev_text, text)
-                        valid = False
-                        break
-                prev_text = text
-            if valid:
-                _debug_print(debug, combination)
-                valid_dash_combinations.append(combination)
-        valid_combinations = valid_dash_combinations
-    
-    # Build the texts of all valid combinations
-    final_combinations = []
-    for combination in valid_combinations:
-        text_stations = []
-        for group, pos in enumerate(combination):
-            text_stations.extend([s.strip() for s in via_groups[group][pos]['text'].split(" - ") if s.strip()])
-        final_combinations.append([combination, text_stations])
-    
-    # Calculate the total weight of each combinations
-    for i, entry in enumerate(final_combinations):
-        combination, text_stations = entry
-        weight = 0
-        for text_station in text_stations:
-            weight += weights.get(text_station, 1)
-        final_combinations[i].append(weight)
-    final_combinations.sort(key=lambda c: c[2], reverse=True)
-
-    _debug_print(debug, "\nFinal combinations (Score, Positions, Text):")
-    for entry in final_combinations:
-        _debug_print(debug, entry[2], entry[0], " - ".join(entry[1]))
-    _debug_print(debug, "")
-    
-    if final_combinations:
-        return final_combinations[0][0]
-    else:
+"""
+Copyright (C) 2021-2022 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import itertools
+
+
+def _debug_print(debug, *args, **kwargs):
+    if debug:
+        print(*args, **kwargs)
+
+def debug_hex(message, readable_ascii = False, readable_ctrl = False):
+    """
+    Turn a message into a readable form
+    """
+
+    CTRL_CHARS = {
+        0x02: "STX",
+        0x03: "ETX",
+        0x04: "EOT",
+        0x05: "ENQ",
+        0x10: "DLE",
+        0x15: "NAK",
+        0x17: "ETB"
+    }
+
+    result = []
+    for byte in message:
+        if readable_ctrl and byte in CTRL_CHARS:
+            result.append(CTRL_CHARS[byte])
+        elif readable_ascii and byte not in range(0, 32) and byte != 127:
+            result.append(chr(byte))
+        else:
+            result.append("{:02X}".format(byte))
+    return " ".join(result)
+
+
+def vias_in_route(route, vias):
+    # Check if the given vias are all present in the given route in the right order
+    # If an entry in vias is a list, all of its items will be considered to be aliases of each other
+    i = 0
+    j = 0
+    while i < len(route) and j < len(vias):
+        if type(vias[j]) in (tuple, list):
+            for alias in vias[j]:
+                if route[i] == alias:
+                    j += 1
+                    break
+        else:
+            if route[i] == vias[j]:
+                j += 1
+        i += 1
+    return j == len(vias)
+
+
+def get_vias(route, weights, *via_groups, check_dashes=True, debug=False):
+    # Get the ideal combination of vias based on split-flap modules
+    num_groups = len(via_groups)
+    
+    # Go through all via groups and take note of possible candidates
+    via_candidates = []
+    for group in via_groups:
+        group_candidates = []
+        for pos, entry in group.items():
+            if vias_in_route(route, entry['stations']):
+                group_candidates.append(pos)
+        via_candidates.append(group_candidates)
+    _debug_print(debug, "Via candidates:")
+    _debug_print(debug, via_candidates)
+    
+    # Check all combinations to see if the order makes sense
+    combinations = itertools.product(*via_candidates)
+    valid_combinations = []
+    _debug_print(debug, "\nVia candidates with sensible order:")
+    for combination in combinations:
+        stations = []
+        for group, pos in enumerate(combination):
+            stations.extend(via_groups[group][pos]['stations'])
+        if vias_in_route(route, stations):
+            _debug_print(debug, combination, stations)
+            valid_combinations.append(combination)
+    
+    # If check_dashes is True, check if the starts and endings are compatible,
+    # i.e. if the first segment ends on a dash, the next one
+    # cannot start with one.
+    if check_dashes:
+        valid_dash_combinations = []
+        _debug_print(debug, "\nCandidates after check_dashes:")
+        for combination in valid_combinations:
+            valid = True
+            prev_text = None
+            for group, pos in enumerate(combination):
+                text = via_groups[group][pos]['text'].strip()
+                if group > 0:
+                    if prev_text and text and prev_text.endswith("-") == text.startswith("-"):
+                        _debug_print(debug, "Excluded: ", prev_text, text)
+                        valid = False
+                        break
+                prev_text = text
+            if valid:
+                _debug_print(debug, combination)
+                valid_dash_combinations.append(combination)
+        valid_combinations = valid_dash_combinations
+    
+    # Build the texts of all valid combinations
+    final_combinations = []
+    for combination in valid_combinations:
+        text_stations = []
+        for group, pos in enumerate(combination):
+            text_stations.extend([s.strip() for s in via_groups[group][pos]['text'].split(" - ") if s.strip()])
+        final_combinations.append([combination, text_stations])
+    
+    # Calculate the total weight of each combinations
+    for i, entry in enumerate(final_combinations):
+        combination, text_stations = entry
+        weight = 0
+        for text_station in text_stations:
+            weight += weights.get(text_station, 1)
+        final_combinations[i].append(weight)
+    final_combinations.sort(key=lambda c: c[2], reverse=True)
+
+    _debug_print(debug, "\nFinal combinations (Score, Positions, Text):")
+    for entry in final_combinations:
+        _debug_print(debug, entry[2], entry[0], " - ".join(entry[1]))
+    _debug_print(debug, "")
+    
+    if final_combinations:
+        return final_combinations[0][0]
+    else:
         return None
```

### Comparing `pyFIS-1.8.1/pyfis/xatlabs/__init__.py` & `pyFIS-1.9.0/pyfis/xatlabs/exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""
-Copyright (C) 2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-from .splitflap import xatLabsSplitFlapController
-from .rgb_dsa import xatLabsRGBDSAController
+"""
+Copyright (C) 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+
+class CommunicationError(IOError):
+    pass
```

### Comparing `pyFIS-1.8.1/pyfis/xatlabs/exceptions.py` & `pyFIS-1.9.0/pyfis/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-"""
-Copyright (C) 2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-
-class CommunicationError(IOError):
-    pass
+"""
+Copyright (C) 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+from .utils import *
```

### Comparing `pyFIS-1.8.1/pyfis/xatlabs/rgb_dsa.py` & `pyFIS-1.9.0/pyfis/xatlabs/rgb_dsa.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-"""
-Copyright (C) 2021 Julian Metzler
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with this program.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import serial
-import time
-
-from pprint import pprint
-
-
-from .exceptions import CommunicationError
-
-
-class xatLabsRGBDSAController:
-    """
-    Protocol implementation for a custom built replacement
-    for the ubiquitous orange LED signs in DB stations.
-    Uses 8x8 WS2812 matrix boards and an Arduino-based controller.
-    Custom serial protocol is implemented here.
-    """
-
-    CMD_SET_TEXT = 0xA0
-    CMD_SET_BRIGHTNESS = 0xA1
-    CMD_DELETE_TEXT = 0xA2
-
-    SYNC = 0xCC
-
-    ERR_TIMEOUT = 0xE0
-    ERR_UNKNOWN_CMD = 0xE1
-    ERR_PAYLOAD_TOO_LARGE = 0xE2
-    ERR_GENERIC = 0xEE
-
-    SUCCESS = 0xFF
-
-    NO_CLEAR     = 0b00001000
-
-    ALIGN_LEFT   = 0b00000100
-    ALIGN_CENTER = 0b00000110
-    ALIGN_RIGHT  = 0b00000010
-
-    SCROLL       = 0b00000001
-
-    def __init__(self, port, debug = False, exclusive = True, no_dtr = False):
-        self.debug = debug
-        if isinstance(port, serial.Serial):
-            self.port = port
-        else:
-            self.port = serial.Serial()
-            self.port.port = port
-            self.port.baudrate = 115200
-            self.port.timeout = 2.0
-            self.port.exclusive = exclusive
-            if no_dtr:
-                self.port.setDTR(False)
-            self.port.open()
-
-    def debug_message(self, message):
-        """
-        Turn a message into a readable form
-        """
-        result = ""
-        for byte in message:
-            if True or byte in range(0, 32) or byte >= 127:
-                result += "{:02X}".format(byte)
-            else:
-                result += chr(byte)
-            result += " "
-        return result
-
-    def sync(self):
-        """
-        Wait for a sync byte from the serial port
-        """
-        # Flush buffer first since we must not read old sync bytes
-        self.port.read(self.port.inWaiting())
-        sync = None
-        while not sync:
-            if self.debug:
-                print("Syncing")
-            sync = self.port.read(1)
-        if self.debug:
-            print("Synced")
-        if sync[0] == self.SYNC:
-            return True
-        else:
-            raise CommunicationError("Sync: Unexpected byte 0x{:02X}".format(sync[0]))
-
-    def read_response(self):
-        """
-        Read the response
-        """
-        response = [self.SYNC]
-        while response and response[0] == self.SYNC:
-            response = self.port.read(1)
-        if not response:
-            raise CommunicationError("Timeout (no response)")
-        if self.debug:
-            print("RX: " + self.debug_message(response))
-        if response[0] == self.ERR_TIMEOUT:
-            raise CommunicationError("Timeout (device received incomplete message)")
-        if response[0] == self.ERR_UNKNOWN_CMD:
-            raise CommunicationError("Unknown command")
-        if response[0] == self.ERR_PAYLOAD_TOO_LARGE:
-            raise CommunicationError("Payload too large")
-        if response[0] == self.ERR_GENERIC:
-            raise CommunicationError("Generic error")
-        if response[0] == self.SUCCESS:
-            return True
-        return False
-
-    def send_command(self, action, payload):
-        data = [0xFF, action] + payload
-        if self.debug:
-            print("TX: " + self.debug_message(data))
-        self.port.write(bytearray(data))
-
-    def send_command_with_response(self, action, payload):
-        """
-        Send a command and retrieve the response data
-        """
-        self.send_command(action, payload)
-        return self.read_response()
-
-    def set_text(self, slot, text, attrs, duration):
-        """
-        Set text with color config.
-
-        slot: Which text slot to use
-        text: The text to be displayed (either str or list, see below)
-        attrs: Combination of attributes (NO_CLEAR, ALIGN, SCROLL)
-        duration: Duration for the text to be displayed in ms (Only relevant for non-scrolling texts)
-
-        text list structure:
-        [
-            {
-                "text": "Hello ",
-                "color": "ff0000"
-            },
-            {
-                "text": "World!",
-                "red": 255,
-                "green": 0,
-                "blue": 128
-            }
-        ]
-        """
-        payload = []
-
-        if type(text) in (list, tuple):
-            _text = "".join(d['text'] for d in text).encode("CP437")
-            _segments = []
-            pos = 0
-            for i, t in enumerate(text):
-                seg = {}
-                seg['start'] = pos
-                seg['end'] = pos + len(t['text'])
-                if "color" in t:
-                    append = True
-                    seg['red'] = int(t['color'][0:2], 16)
-                    seg['green'] = int(t['color'][2:4], 16)
-                    seg['blue'] = int(t['color'][4:6], 16)
-                elif "red" in t and "green" in t and "blue" in t:
-                    append = True
-                    seg['red'] = t['red']
-                    seg['green'] = t['green']
-                    seg['blue'] = t['blue']
-                else:
-                    append = False
-                if append:
-                    _segments.append(seg)
-                pos += len(t['text'])
-        else:
-            _text = str(text).encode("CP437")
-            _segments = []
-
-        payload.extend([slot, len(text) >> 8, len(_text) & 0xFF, attrs, duration >> 8, duration & 0xFF])
-        payload.extend(_text)
-        payload.extend([len(_segments)])
-        for seg in _segments:
-            payload.extend([0x01, 0x07, seg['start'] >> 8, seg['start'] & 0xFF, seg['end'] >> 8, seg['end'] & 0xFF, seg['red'], seg['green'], seg['blue']])
-        payload = [len(payload) >> 8, len(payload) & 0xFF] + payload
-
-        return self.send_command_with_response(self.CMD_SET_TEXT, payload)
-
-    def set_brightness(self, brightness):
-        """
-        Set display brightness (0 to 255)
-        """
-        return self.send_command_with_response(self.CMD_SET_BRIGHTNESS, [brightness])
-
-    def delete_text(self, slot):
-        """
-        Delete the text in the specified slot
-        """
-        return self.send_command_with_response(self.CMD_DELETE_TEXT, [slot])
+"""
+Copyright (C) 2021 Julian Metzler
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <http://www.gnu.org/licenses/>.
+"""
+
+import serial
+import time
+
+from pprint import pprint
+
+
+from .exceptions import CommunicationError
+
+
+class xatLabsRGBDSAController:
+    """
+    Protocol implementation for a custom built replacement
+    for the ubiquitous orange LED signs in DB stations.
+    Uses 8x8 WS2812 matrix boards and an Arduino-based controller.
+    Custom serial protocol is implemented here.
+    """
+
+    CMD_SET_TEXT = 0xA0
+    CMD_SET_BRIGHTNESS = 0xA1
+    CMD_DELETE_TEXT = 0xA2
+
+    SYNC = 0xCC
+
+    ERR_TIMEOUT = 0xE0
+    ERR_UNKNOWN_CMD = 0xE1
+    ERR_PAYLOAD_TOO_LARGE = 0xE2
+    ERR_GENERIC = 0xEE
+
+    SUCCESS = 0xFF
+
+    NO_CLEAR     = 0b00001000
+
+    ALIGN_LEFT   = 0b00000100
+    ALIGN_CENTER = 0b00000110
+    ALIGN_RIGHT  = 0b00000010
+
+    SCROLL       = 0b00000001
+
+    def __init__(self, port, debug = False, exclusive = True, no_dtr = False):
+        self.debug = debug
+        if isinstance(port, serial.Serial):
+            self.port = port
+        else:
+            self.port = serial.Serial()
+            self.port.port = port
+            self.port.baudrate = 115200
+            self.port.timeout = 2.0
+            self.port.exclusive = exclusive
+            if no_dtr:
+                self.port.setDTR(False)
+            self.port.open()
+
+    def debug_message(self, message):
+        """
+        Turn a message into a readable form
+        """
+        result = ""
+        for byte in message:
+            if True or byte in range(0, 32) or byte >= 127:
+                result += "{:02X}".format(byte)
+            else:
+                result += chr(byte)
+            result += " "
+        return result
+
+    def sync(self):
+        """
+        Wait for a sync byte from the serial port
+        """
+        # Flush buffer first since we must not read old sync bytes
+        self.port.read(self.port.inWaiting())
+        sync = None
+        while not sync:
+            if self.debug:
+                print("Syncing")
+            sync = self.port.read(1)
+        if self.debug:
+            print("Synced")
+        if sync[0] == self.SYNC:
+            return True
+        else:
+            raise CommunicationError("Sync: Unexpected byte 0x{:02X}".format(sync[0]))
+
+    def read_response(self):
+        """
+        Read the response
+        """
+        response = [self.SYNC]
+        while response and response[0] == self.SYNC:
+            response = self.port.read(1)
+        if not response:
+            raise CommunicationError("Timeout (no response)")
+        if self.debug:
+            print("RX: " + self.debug_message(response))
+        if response[0] == self.ERR_TIMEOUT:
+            raise CommunicationError("Timeout (device received incomplete message)")
+        if response[0] == self.ERR_UNKNOWN_CMD:
+            raise CommunicationError("Unknown command")
+        if response[0] == self.ERR_PAYLOAD_TOO_LARGE:
+            raise CommunicationError("Payload too large")
+        if response[0] == self.ERR_GENERIC:
+            raise CommunicationError("Generic error")
+        if response[0] == self.SUCCESS:
+            return True
+        return False
+
+    def send_command(self, action, payload):
+        data = [0xFF, action] + payload
+        if self.debug:
+            print("TX: " + self.debug_message(data))
+        self.port.write(bytearray(data))
+
+    def send_command_with_response(self, action, payload):
+        """
+        Send a command and retrieve the response data
+        """
+        self.send_command(action, payload)
+        return self.read_response()
+
+    def set_text(self, slot, text, attrs, duration):
+        """
+        Set text with color config.
+
+        slot: Which text slot to use
+        text: The text to be displayed (either str or list, see below)
+        attrs: Combination of attributes (NO_CLEAR, ALIGN, SCROLL)
+        duration: Duration for the text to be displayed in ms (Only relevant for non-scrolling texts)
+
+        text list structure:
+        [
+            {
+                "text": "Hello ",
+                "color": "ff0000"
+            },
+            {
+                "text": "World!",
+                "red": 255,
+                "green": 0,
+                "blue": 128
+            }
+        ]
+        """
+        payload = []
+
+        if type(text) in (list, tuple):
+            _text = "".join(d['text'] for d in text).encode("CP437")
+            _segments = []
+            pos = 0
+            for i, t in enumerate(text):
+                seg = {}
+                seg['start'] = pos
+                seg['end'] = pos + len(t['text'])
+                if "color" in t:
+                    append = True
+                    seg['red'] = int(t['color'][0:2], 16)
+                    seg['green'] = int(t['color'][2:4], 16)
+                    seg['blue'] = int(t['color'][4:6], 16)
+                elif "red" in t and "green" in t and "blue" in t:
+                    append = True
+                    seg['red'] = t['red']
+                    seg['green'] = t['green']
+                    seg['blue'] = t['blue']
+                else:
+                    append = False
+                if append:
+                    _segments.append(seg)
+                pos += len(t['text'])
+        else:
+            _text = str(text).encode("CP437")
+            _segments = []
+
+        payload.extend([slot, len(text) >> 8, len(_text) & 0xFF, attrs, duration >> 8, duration & 0xFF])
+        payload.extend(_text)
+        payload.extend([len(_segments)])
+        for seg in _segments:
+            payload.extend([0x01, 0x07, seg['start'] >> 8, seg['start'] & 0xFF, seg['end'] >> 8, seg['end'] & 0xFF, seg['red'], seg['green'], seg['blue']])
+        payload = [len(payload) >> 8, len(payload) & 0xFF] + payload
+
+        return self.send_command_with_response(self.CMD_SET_TEXT, payload)
+
+    def set_brightness(self, brightness):
+        """
+        Set display brightness (0 to 255)
+        """
+        return self.send_command_with_response(self.CMD_SET_BRIGHTNESS, [brightness])
+
+    def delete_text(self, slot):
+        """
+        Delete the text in the specified slot
+        """
+        return self.send_command_with_response(self.CMD_DELETE_TEXT, [slot])
```

