# Comparing `tmp/vsmuxtools-0.0.2.tar.gz` & `tmp/vsmuxtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.2.tar", last modified: Sun Jun  4 11:11:51 2023, max compression
+gzip compressed data, was "vsmuxtools-0.0.3.tar", last modified: Sun Jun  4 11:23:26 2023, max compression
```

## Comparing `vsmuxtools-0.0.2.tar` & `vsmuxtools-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.289369 vsmuxtools-0.0.2/
--rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      994 2023-06-04 11:11:51.288369 vsmuxtools-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.2/README.md
--rw-rw-rw-   0        0        0     1078 2023-06-04 11:10:21.000000 vsmuxtools-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 11:11:51.289369 vsmuxtools-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.270976 vsmuxtools-0.0.2/vsmuxtools/
--rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.2/vsmuxtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.283367 vsmuxtools-0.0.2/vsmuxtools/extension/
--rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.2/vsmuxtools/extension/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.2/vsmuxtools/extension/audio.py
--rw-rw-rw-   0        0        0     1620 2023-05-30 18:54:08.000000 vsmuxtools-0.0.2/vsmuxtools/extension/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.285369 vsmuxtools-0.0.2/vsmuxtools/utils/
--rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.2/vsmuxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.2/vsmuxtools/utils/src.py
--rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.2/vsmuxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.288369 vsmuxtools-0.0.2/vsmuxtools/video/
--rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.2/vsmuxtools/video/__init__.py
--rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.2/vsmuxtools/video/encoders.py
--rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.2/vsmuxtools/video/resumable.py
--rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.2/vsmuxtools/video/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.282368 vsmuxtools-0.0.2/vsmuxtools.egg-info/
--rw-rw-rw-   0        0        0      994 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.311703 vsmuxtools-0.0.3/
+-rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      994 2023-06-04 11:23:26.311703 vsmuxtools-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1078 2023-06-04 11:22:07.000000 vsmuxtools-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:23:26.311703 vsmuxtools-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.293698 vsmuxtools-0.0.3/vsmuxtools/
+-rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.3/vsmuxtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.306703 vsmuxtools-0.0.3/vsmuxtools/extension/
+-rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.3/vsmuxtools/extension/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.3/vsmuxtools/extension/audio.py
+-rw-rw-rw-   0        0        0     1620 2023-06-04 11:21:20.000000 vsmuxtools-0.0.3/vsmuxtools/extension/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.307703 vsmuxtools-0.0.3/vsmuxtools/utils/
+-rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.3/vsmuxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.3/vsmuxtools/utils/src.py
+-rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.3/vsmuxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.310702 vsmuxtools-0.0.3/vsmuxtools/video/
+-rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.3/vsmuxtools/video/__init__.py
+-rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.3/vsmuxtools/video/encoders.py
+-rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.3/vsmuxtools/video/resumable.py
+-rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.3/vsmuxtools/video/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.304701 vsmuxtools-0.0.3/vsmuxtools.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.2/LICENSE` & `vsmuxtools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/PKG-INFO` & `vsmuxtools-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.2/pyproject.toml` & `vsmuxtools-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.2"
+version = "0.0.3"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
-    "muxtools>=0.0.2",
+    "muxtools>=0.0.3",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vsmuxtools-0.0.2/vsmuxtools/extension/audio.py` & `vsmuxtools-0.0.3/vsmuxtools/extension/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.0.3/vsmuxtools/extension/chapters.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/vsmuxtools/utils/src.py` & `vsmuxtools-0.0.3/vsmuxtools/utils/src.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/vsmuxtools/video/encoders.py` & `vsmuxtools-0.0.3/vsmuxtools/video/encoders.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/vsmuxtools/video/resumable.py` & `vsmuxtools-0.0.3/vsmuxtools/video/resumable.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/vsmuxtools/video/settings.py` & `vsmuxtools-0.0.3/vsmuxtools/video/settings.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.2/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.0.3/vsmuxtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.2
+Version: 0.0.3
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.2/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.0.3/vsmuxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

