# Comparing `tmp/vsmuxtools-0.0.3.tar.gz` & `tmp/vsmuxtools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.3.tar", last modified: Sun Jun  4 11:23:26 2023, max compression
+gzip compressed data, was "vsmuxtools-0.0.4.tar", last modified: Sun Jun  4 11:43:22 2023, max compression
```

## Comparing `vsmuxtools-0.0.3.tar` & `vsmuxtools-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.311703 vsmuxtools-0.0.3/
--rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      994 2023-06-04 11:23:26.311703 vsmuxtools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.3/README.md
--rw-rw-rw-   0        0        0     1078 2023-06-04 11:22:07.000000 vsmuxtools-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 11:23:26.311703 vsmuxtools-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.293698 vsmuxtools-0.0.3/vsmuxtools/
--rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.3/vsmuxtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.306703 vsmuxtools-0.0.3/vsmuxtools/extension/
--rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.3/vsmuxtools/extension/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.3/vsmuxtools/extension/audio.py
--rw-rw-rw-   0        0        0     1620 2023-06-04 11:21:20.000000 vsmuxtools-0.0.3/vsmuxtools/extension/chapters.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.307703 vsmuxtools-0.0.3/vsmuxtools/utils/
--rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.3/vsmuxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.3/vsmuxtools/utils/src.py
--rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.3/vsmuxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.310702 vsmuxtools-0.0.3/vsmuxtools/video/
--rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.3/vsmuxtools/video/__init__.py
--rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.3/vsmuxtools/video/encoders.py
--rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.3/vsmuxtools/video/resumable.py
--rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.3/vsmuxtools/video/settings.py
-drwxrwxrwx   0        0        0        0 2023-06-04 11:23:26.304701 vsmuxtools-0.0.3/vsmuxtools.egg-info/
--rw-rw-rw-   0        0        0      994 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-04 11:23:26.000000 vsmuxtools-0.0.3/vsmuxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.737438 vsmuxtools-0.0.4/
+-rw-rw-rw-   0        0        0    17098 2023-05-27 19:14:49.000000 vsmuxtools-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      994 2023-06-04 11:43:22.737438 vsmuxtools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-05-27 19:14:49.000000 vsmuxtools-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1078 2023-06-04 11:42:11.000000 vsmuxtools-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:43:22.737438 vsmuxtools-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.722896 vsmuxtools-0.0.4/vsmuxtools/
+-rw-rw-rw-   0        0        0      266 2023-06-04 11:09:34.000000 vsmuxtools-0.0.4/vsmuxtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.732410 vsmuxtools-0.0.4/vsmuxtools/extension/
+-rw-rw-rw-   0        0        0       80 2023-05-30 18:54:48.000000 vsmuxtools-0.0.4/vsmuxtools/extension/__init__.py
+-rw-rw-rw-   0        0        0     2717 2023-05-31 21:39:04.000000 vsmuxtools-0.0.4/vsmuxtools/extension/audio.py
+-rw-rw-rw-   0        0        0     1477 2023-06-04 11:42:52.000000 vsmuxtools-0.0.4/vsmuxtools/extension/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.734409 vsmuxtools-0.0.4/vsmuxtools/utils/
+-rw-rw-rw-   0        0        0       84 2023-05-30 16:15:03.000000 vsmuxtools-0.0.4/vsmuxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     7915 2023-05-31 20:52:56.000000 vsmuxtools-0.0.4/vsmuxtools/utils/src.py
+-rw-rw-rw-   0        0        0      186 2023-05-30 16:15:19.000000 vsmuxtools-0.0.4/vsmuxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.736410 vsmuxtools-0.0.4/vsmuxtools/video/
+-rw-rw-rw-   0        0        0       97 2023-05-30 16:12:00.000000 vsmuxtools-0.0.4/vsmuxtools/video/__init__.py
+-rw-rw-rw-   0        0        0    14785 2023-05-31 22:17:09.000000 vsmuxtools-0.0.4/vsmuxtools/video/encoders.py
+-rw-rw-rw-   0        0        0     3075 2023-05-31 08:35:11.000000 vsmuxtools-0.0.4/vsmuxtools/video/resumable.py
+-rw-rw-rw-   0        0        0     9999 2023-05-30 16:43:59.000000 vsmuxtools-0.0.4/vsmuxtools/video/settings.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:43:22.730409 vsmuxtools-0.0.4/vsmuxtools.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 11:43:22.000000 vsmuxtools-0.0.4/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.3/LICENSE` & `vsmuxtools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.3/PKG-INFO` & `vsmuxtools-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.3
+Version: 0.0.4
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.3/pyproject.toml` & `vsmuxtools-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.3"
+version = "0.0.4"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
```

### Comparing `vsmuxtools-0.0.3/vsmuxtools/extension/audio.py` & `vsmuxtools-0.0.4/vsmuxtools/extension/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.3/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.0.4/vsmuxtools/extension/chapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,15 @@
         :param chapter_source:      Input either src_file/FileInfo, txt with ogm chapters, xml or (a list of) self defined chapters.
         :param fps:                 Needed for timestamp convertion. Gets the fps from the clip if src_file and otherwise assumes 24000/1001.
         :param _print:              Prints chapters after parsing and after trimming.
         """
         if isinstance(chapter_source, src_file):
             clip_fps = Fraction(chapter_source.src.fps_num, chapter_source.src.fps_den)
             self.fps = fps if fps else clip_fps
-            parse_chapters_bdmv(chapter_source.file, self.fps, chapter_source.src.num_frames, _print)
-            # self.chapters = parse_src_file(chapter_source, _print)
-            self.fps = Fraction(chapter_source.src.fps_num, chapter_source.src.fps_den)
+            self.chapters = parse_chapters_bdmv(chapter_source.file, self.fps, chapter_source.src.num_frames, _print)
             if chapter_source.trim:
                 self.trim(chapter_source.trim[0], chapter_source.trim[1], chapter_source.src.num_frames)
                 if _print:
                     print("After trim:")
                     self.print()
         else:
             super().__init__(chapter_source, fps if fps else Fraction(24000, 1001), _print)
```

### Comparing `vsmuxtools-0.0.3/vsmuxtools/utils/src.py` & `vsmuxtools-0.0.4/vsmuxtools/utils/src.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.3/vsmuxtools/video/encoders.py` & `vsmuxtools-0.0.4/vsmuxtools/video/encoders.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.3/vsmuxtools/video/resumable.py` & `vsmuxtools-0.0.4/vsmuxtools/video/resumable.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.3/vsmuxtools/video/settings.py` & `vsmuxtools-0.0.4/vsmuxtools/video/settings.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.3/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.0.4/vsmuxtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.3
+Version: 0.0.4
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `vsmuxtools-0.0.3/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.0.4/vsmuxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

