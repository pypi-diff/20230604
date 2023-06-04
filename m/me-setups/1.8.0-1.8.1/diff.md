# Comparing `tmp/me_setups-1.8.0.tar.gz` & `tmp/me_setups-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.8.0.tar", last modified: Sun Jun  4 10:01:12 2023, max compression
+gzip compressed data, was "me_setups-1.8.1.tar", last modified: Sun Jun  4 13:25:36 2023, max compression
```

## Comparing `me_setups-1.8.0.tar` & `me_setups-1.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.509341 me_setups-1.8.0/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 10:01:12.509368 me_setups-1.8.0/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.0/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-04 10:01:12.512328 me_setups-1.8.0/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.0/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.461347 me_setups-1.8.0/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.479074 me_setups-1.8.0/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.0/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.497543 me_setups-1.8.0/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.0/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.0/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11273 2023-06-04 08:37:54.000000 me_setups-1.8.0/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.0/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.507356 me_setups-1.8.0/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.0/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8664 2023-06-04 09:59:02.000000 me_setups-1.8.0/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    12717 2023-05-18 10:10:02.000000 me_setups-1.8.0/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.0/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.0/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     2703 2023-06-04 09:59:02.000000 me_setups-1.8.0/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 10:01:12.489340 me_setups-1.8.0/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-04 10:01:12.000000 me_setups-1.8.0/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.335495 me_setups-1.8.1/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 13:25:36.335564 me_setups-1.8.1/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.1/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-04 13:25:36.337496 me_setups-1.8.1/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.1/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.304516 me_setups-1.8.1/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.312517 me_setups-1.8.1/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.1/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.326502 me_setups-1.8.1/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.1/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.1/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11273 2023-06-04 12:44:08.000000 me_setups-1.8.1/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.1/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.333598 me_setups-1.8.1/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.1/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8664 2023-06-04 12:17:51.000000 me_setups-1.8.1/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    12717 2023-06-04 12:44:08.000000 me_setups-1.8.1/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.1/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.1/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     2826 2023-06-04 13:24:16.000000 me_setups-1.8.1/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-04 13:25:36.319558 me_setups-1.8.1/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-04 13:25:36.000000 me_setups-1.8.1/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.8.0/PKG-INFO` & `me_setups-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.8.0
+Version: 1.8.1
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.0/setup.cfg` & `me_setups-1.8.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.8.0
+version = 1.8.1
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.8.0/src/me_setups/boards/default_boards.py` & `me_setups-1.8.1/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.0/src/me_setups/boards/gas52.py` & `me_setups-1.8.1/src/me_setups/boards/gas52.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.0/src/me_setups/components/comp.py` & `me_setups-1.8.1/src/me_setups/components/comp.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.0/src/me_setups/components/eqs.py` & `me_setups-1.8.1/src/me_setups/components/eqs.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.0/src/me_setups/components/mcu.py` & `me_setups-1.8.1/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.0/src/me_setups/utils.py` & `me_setups-1.8.1/src/me_setups/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,18 @@
 
 def lock_port(port: pathlib.Path | str) -> None:
     port_links = get_port_links(pathlib.Path(port))
     if in_use(port_links):
         raise PortInUse(f"Cannot lock {port}.")
     for port_link in port_links:
         lck_file_path = get_lck_file_path(port_link)
-        lck_file_path.write_text(f"   {os.getpid()}\n")
+        try:
+            lck_file_path.write_text(f"   {os.getpid()}\n")
+        except PermissionError:
+            logger.warning(f"Have no permission to edit {lck_file_path}")
 
 
 def release_port(port: pathlib.Path | str) -> None:
     port_links = get_port_links(pathlib.Path(port))
     if in_use(port_links):
         raise PortInUse(f"Cannot lock {port}.")
     for port_link in port_links:
```

### Comparing `me_setups-1.8.0/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.8.1/src/me_setups.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.8.0
+Version: 1.8.1
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.0/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.8.1/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

