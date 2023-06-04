# Comparing `tmp/me_setups-1.7.1.tar.gz` & `tmp/me_setups-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.7.1.tar", last modified: Thu May 11 14:21:34 2023, max compression
+gzip compressed data, was "me_setups-1.8.0.tar", last modified: Sun Jun  4 10:01:12 2023, max compression
```

## Comparing `me_setups-1.7.1.tar` & `me_setups-1.8.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 14:21:34.749581 me_setups-1.7.1/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-05-11 14:21:34.749606 me_setups-1.7.1/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.7.1/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-05-11 14:21:34.751583 me_setups-1.7.1/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.7.1/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 14:21:34.712587 me_setups-1.7.1/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 14:21:34.721609 me_setups-1.7.1/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.7.1/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 14:21:34.738297 me_setups-1.7.1/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.7.1/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.7.1/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11273 2023-05-11 14:20:23.000000 me_setups-1.7.1/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.7.1/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 14:21:34.747587 me_setups-1.7.1/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.7.1/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8597 2023-05-11 14:20:23.000000 me_setups-1.7.1/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    12717 2023-05-11 12:09:03.000000 me_setups-1.7.1/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-11 12:09:03.000000 me_setups-1.7.1/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-11 13:28:50.000000 me_setups-1.7.1/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-03-15 13:23:19.000000 me_setups-1.7.1/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-05-11 14:21:34.731204 me_setups-1.7.1/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-05-11 14:21:34.000000 me_setups-1.7.1/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-05-11 14:21:34.000000 me_setups-1.7.1/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-05-11 14:21:34.000000 me_setups-1.7.1/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-05-11 14:21:34.000000 me_setups-1.7.1/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-05-11 14:21:34.000000 me_setups-1.7.1/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.509341 me_setups-1.8.0/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 10:01:12.509368 me_setups-1.8.0/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.0/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-04 10:01:12.512328 me_setups-1.8.0/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.0/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.461347 me_setups-1.8.0/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.479074 me_setups-1.8.0/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.0/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.497543 me_setups-1.8.0/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.0/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.0/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11273 2023-06-04 08:37:54.000000 me_setups-1.8.0/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.0/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.507356 me_setups-1.8.0/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.0/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8664 2023-06-04 09:59:02.000000 me_setups-1.8.0/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    12717 2023-05-18 10:10:02.000000 me_setups-1.8.0/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.0/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.0/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     2703 2023-06-04 09:59:02.000000 me_setups-1.8.0/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.489340 me_setups-1.8.0/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.7.1/PKG-INFO` & `me_setups-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.7.1
+Version: 1.8.0
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.7.1/setup.cfg` & `me_setups-1.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.7.1
+version = 1.8.0
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.7.1/src/me_setups/boards/default_boards.py` & `me_setups-1.8.0/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.7.1/src/me_setups/boards/gas52.py` & `me_setups-1.8.0/src/me_setups/boards/gas52.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.7.1/src/me_setups/components/comp.py` & `me_setups-1.8.0/src/me_setups/components/comp.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing_extensions import Literal
 
 from serial import Serial
 from serial import SerialException
 from serial.threaded import LineReader
 
 from me_setups.utils import filter_ansi_escape
+from me_setups.utils import lock_port
 
 logger = logging.getLogger(__name__)
 
 
 def add_line_timestamp(line: str) -> str:
     """adds timestamp to a given line
 
@@ -187,14 +188,15 @@
 
         Args:
             pbcm (str): pbcm for the Component
             port (str): path to the serial port.
         """
         self._pbcm = pbcm
         self.serial = SerialSniffer(port=port, baudrate=115200, timeout=5)
+        lock_port(port=port)
         self.logger = logging.getLogger(self.name)
 
     @property
     def prompt(self) -> bytes:
         raise NotImplementedError
 
     @property
```

### Comparing `me_setups-1.7.1/src/me_setups/components/eqs.py` & `me_setups-1.8.0/src/me_setups/components/eqs.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.7.1/src/me_setups/components/mcu.py` & `me_setups-1.8.0/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.7.1/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.8.0/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.7.1
+Version: 1.8.0
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.7.1/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.8.0/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

