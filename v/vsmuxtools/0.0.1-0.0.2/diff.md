# Comparing `tmp/vsmuxtools-0.0.1.tar.gz` & `tmp/vsmuxtools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.1.tar", last modified: Wed May 31 22:04:36 2023, max compression
+gzip compressed data, was "vsmuxtools-0.0.2.tar", last modified: Sun Jun  4 11:11:51 2023, max compression
```

## Comparing `vsmuxtools-0.0.1.tar` & `vsmuxtools-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:04:36.795320 vsmuxtools-0.0.1/
--rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      994 2023-05-31 22:04:36.794320 vsmuxtools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.1/README.md
--rw-rw-rw-   0        0        0     1078 2023-05-30 18:08:03.000000 vsmuxtools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 22:04:36.795320 vsmuxtools-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 22:04:36.772576 vsmuxtools-0.0.1/vsmuxtools/
--rw-rw-rw-   0        0        0      295 2023-05-30 18:54:57.000000 vsmuxtools-0.0.1/vsmuxtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:04:36.788096 vsmuxtools-0.0.1/vsmuxtools/extension/
--rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.1/vsmuxtools/extension/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.1/vsmuxtools/extension/audio.py
--rw-rw-rw-   0        0        0     1620 2023-05-30 18:54:08.000000 vsmuxtools-0.0.1/vsmuxtools/extension/chapters.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:04:36.790096 vsmuxtools-0.0.1/vsmuxtools/utils/
--rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.1/vsmuxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.1/vsmuxtools/utils/src.py
--rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.1/vsmuxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:04:36.793320 vsmuxtools-0.0.1/vsmuxtools/video/
--rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.1/vsmuxtools/video/__init__.py
--rw-rw-rw-   0        0        0    14788 2023-05-31 19:53:50.000000 vsmuxtools-0.0.1/vsmuxtools/video/encoders.py
--rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.1/vsmuxtools/video/resumable.py
--rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.1/vsmuxtools/video/settings.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:04:36.786095 vsmuxtools-0.0.1/vsmuxtools.egg-info/
--rw-rw-rw-   0        0        0      994 2023-05-31 22:04:36.000000 vsmuxtools-0.0.1/vsmuxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-05-31 22:04:36.000000 vsmuxtools-0.0.1/vsmuxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:04:36.000000 vsmuxtools-0.0.1/vsmuxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-31 22:04:36.000000 vsmuxtools-0.0.1/vsmuxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 22:04:36.000000 vsmuxtools-0.0.1/vsmuxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.289369 vsmuxtools-0.0.2/
+-rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      994 2023-06-04 11:11:51.288369 vsmuxtools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1078 2023-06-04 11:10:21.000000 vsmuxtools-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:11:51.289369 vsmuxtools-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.270976 vsmuxtools-0.0.2/vsmuxtools/
+-rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.2/vsmuxtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.283367 vsmuxtools-0.0.2/vsmuxtools/extension/
+-rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.2/vsmuxtools/extension/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.2/vsmuxtools/extension/audio.py
+-rw-rw-rw-   0        0        0     1620 2023-05-30 18:54:08.000000 vsmuxtools-0.0.2/vsmuxtools/extension/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.285369 vsmuxtools-0.0.2/vsmuxtools/utils/
+-rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.2/vsmuxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.2/vsmuxtools/utils/src.py
+-rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.2/vsmuxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.288369 vsmuxtools-0.0.2/vsmuxtools/video/
+-rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.2/vsmuxtools/video/__init__.py
+-rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.2/vsmuxtools/video/encoders.py
+-rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.2/vsmuxtools/video/resumable.py
+-rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.2/vsmuxtools/video/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:11:51.282368 vsmuxtools-0.0.2/vsmuxtools.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 11:11:51.000000 vsmuxtools-0.0.2/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.1/LICENSE` & `vsmuxtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.1/PKG-INFO` & `vsmuxtools-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.1/pyproject.toml` & `vsmuxtools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.1"
+version = "0.0.2"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
-    "muxtools>=0.0.1",
+    "muxtools>=0.0.2",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vsmuxtools-0.0.1/vsmuxtools/extension/audio.py` & `vsmuxtools-0.0.2/vsmuxtools/extension/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.1/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.0.2/vsmuxtools/extension/chapters.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.1/vsmuxtools/utils/src.py` & `vsmuxtools-0.0.2/vsmuxtools/utils/src.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.1/vsmuxtools/video/encoders.py` & `vsmuxtools-0.0.2/vsmuxtools/video/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,15 @@
         process.communicate()
         return out
 
 
 @dataclass
 class LosslessX264(VideoEncoder):
     """
-    Uses ffmpeg to encode clip to a lossless ffv1 stream.
+    Uses x264 to encode clip to a lossless avc stream.
 
     :param preset:          Can either be a string of some x264 preset or any of the 3 predefined presets.
     :param settings:        Any other settings you might want to pass. Entirely optional.
     :param add_props:       This will explicitly add all props taken from the clip to the command line.
     """
 
     preset: str | LosslessPreset = LosslessPreset.MIDDLEGROUND
```

### Comparing `vsmuxtools-0.0.1/vsmuxtools/video/resumable.py` & `vsmuxtools-0.0.2/vsmuxtools/video/resumable.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.1/vsmuxtools/video/settings.py` & `vsmuxtools-0.0.2/vsmuxtools/video/settings.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.1/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.0.2/vsmuxtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.1/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.0.2/vsmuxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

