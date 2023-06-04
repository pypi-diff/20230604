# Comparing `tmp/muxtools-0.0.1.tar.gz` & `tmp/muxtools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxtools-0.0.1.tar", last modified: Wed May 31 22:05:42 2023, max compression
+gzip compressed data, was "muxtools-0.0.2.tar", last modified: Sun Jun  4 11:10:42 2023, max compression
```

## Comparing `muxtools-0.0.1.tar` & `muxtools-0.0.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.409409 muxtools-0.0.1/
--rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1115 2023-05-31 22:05:42.409409 muxtools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.372336 muxtools-0.0.1/muxtools/
--rw-rw-rw-   0        0        0      810 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.390350 muxtools-0.0.1/muxtools/audio/
--rw-rw-rw-   0        0        0      140 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/audio/__init__.py
--rw-rw-rw-   0        0        0     8494 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/audio/audioutils.py
--rw-rw-rw-   0        0        0    14935 2023-05-31 20:09:03.000000 muxtools-0.0.1/muxtools/audio/encoders.py
--rw-rw-rw-   0        0        0    16457 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/audio/extractors.py
--rw-rw-rw-   0        0        0      886 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/audio/tools.py
--rw-rw-rw-   0        0        0     7680 2023-05-31 19:37:10.000000 muxtools-0.0.1/muxtools/cli.py
--rw-rw-rw-   0        0        0     3278 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/functions.py
--rw-rw-rw-   0        0        0     4589 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.392836 muxtools-0.0.1/muxtools/misc/
--rw-rw-rw-   0        0        0       51 2023-05-31 19:37:10.000000 muxtools-0.0.1/muxtools/misc/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-05-31 19:37:10.000000 muxtools-0.0.1/muxtools/misc/chapters.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.396891 muxtools-0.0.1/muxtools/muxing/
--rw-rw-rw-   0        0        0      129 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/muxing/__init__.py
--rw-rw-rw-   0        0        0     4386 2023-05-31 21:00:32.000000 muxtools-0.0.1/muxtools/muxing/mux.py
--rw-rw-rw-   0        0        0     4098 2023-05-31 19:37:10.000000 muxtools-0.0.1/muxtools/muxing/muxfiles.py
--rw-rw-rw-   0        0        0     6371 2023-05-31 21:38:08.000000 muxtools-0.0.1/muxtools/muxing/tmdb.py
--rw-rw-rw-   0        0        0     6808 2023-05-31 21:37:46.000000 muxtools-0.0.1/muxtools/muxing/tracks.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.401409 muxtools-0.0.1/muxtools/subtitle/
--rw-rw-rw-   0        0        0      128 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/subtitle/__init__.py
--rw-rw-rw-   0        0        0     1621 2023-05-31 19:37:29.000000 muxtools-0.0.1/muxtools/subtitle/font.py
--rw-rw-rw-   0        0        0     3423 2023-05-31 19:37:29.000000 muxtools-0.0.1/muxtools/subtitle/styles.py
--rw-rw-rw-   0        0        0    19599 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/subtitle/sub.py
--rw-rw-rw-   0        0        0     1649 2023-05-31 19:37:29.000000 muxtools-0.0.1/muxtools/subtitle/subutils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.408409 muxtools-0.0.1/muxtools/utils/
--rw-rw-rw-   0        0        0      242 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/convert.py
--rw-rw-rw-   0        0        0     4168 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/download.py
--rw-rw-rw-   0        0        0     1449 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/env.py
--rw-rw-rw-   0        0        0     5357 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/files.py
--rw-rw-rw-   0        0        0     2426 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/format.py
--rw-rw-rw-   0        0        0     1248 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/glob.py
--rw-rw-rw-   0        0        0     1708 2023-05-31 19:37:29.000000 muxtools-0.0.1/muxtools/utils/log.py
--rw-rw-rw-   0        0        0     8123 2023-05-30 18:08:36.000000 muxtools-0.0.1/muxtools/utils/parsing.py
--rw-rw-rw-   0        0        0     2887 2023-05-31 20:01:28.000000 muxtools-0.0.1/muxtools/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:05:42.385845 muxtools-0.0.1/muxtools.egg-info/
--rw-rw-rw-   0        0        0     1115 2023-05-31 22:05:42.000000 muxtools-0.0.1/muxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-05-31 22:05:42.000000 muxtools-0.0.1/muxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:05:42.000000 muxtools-0.0.1/muxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-31 22:05:42.000000 muxtools-0.0.1/muxtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-05-31 22:05:42.000000 muxtools-0.0.1/muxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 22:05:42.000000 muxtools-0.0.1/muxtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1335 2023-05-30 18:08:33.000000 muxtools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 22:05:42.409409 muxtools-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.264687 muxtools-0.0.2/
+-rw-rw-rw-   0        0        0    17098 2023-05-19 19:09:14.000000 muxtools-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1115 2023-06-04 11:10:42.264687 muxtools-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-27 13:25:07.000000 muxtools-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.230345 muxtools-0.0.2/muxtools/
+-rw-rw-rw-   0        0        0      810 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.248352 muxtools-0.0.2/muxtools/audio/
+-rw-rw-rw-   0        0        0      190 2023-06-01 17:13:19.000000 muxtools-0.0.2/muxtools/audio/__init__.py
+-rw-rw-rw-   0        0        0    11068 2023-06-03 01:30:34.000000 muxtools-0.0.2/muxtools/audio/audioutils.py
+-rw-rw-rw-   0        0        0    14858 2023-06-04 10:23:26.000000 muxtools-0.0.2/muxtools/audio/encoders.py
+-rw-rw-rw-   0        0        0    16812 2023-06-03 00:49:40.000000 muxtools-0.0.2/muxtools/audio/extractors.py
+-rw-rw-rw-   0        0        0     9133 2023-06-03 01:36:04.000000 muxtools-0.0.2/muxtools/audio/memecoders.py
+-rw-rw-rw-   0        0        0      962 2023-06-01 11:53:30.000000 muxtools-0.0.2/muxtools/audio/tools.py
+-rw-rw-rw-   0        0        0     7680 2023-06-01 16:53:16.000000 muxtools-0.0.2/muxtools/cli.py
+-rw-rw-rw-   0        0        0     3282 2023-06-02 21:32:44.000000 muxtools-0.0.2/muxtools/functions.py
+-rw-rw-rw-   0        0        0     4589 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/main.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.250352 muxtools-0.0.2/muxtools/misc/
+-rw-rw-rw-   0        0        0       51 2023-06-01 16:53:33.000000 muxtools-0.0.2/muxtools/misc/__init__.py
+-rw-rw-rw-   0        0        0     7572 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/misc/chapters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.254352 muxtools-0.0.2/muxtools/muxing/
+-rw-rw-rw-   0        0        0      129 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/muxing/__init__.py
+-rw-rw-rw-   0        0        0     4386 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/muxing/mux.py
+-rw-rw-rw-   0        0        0     4403 2023-06-03 01:13:02.000000 muxtools-0.0.2/muxtools/muxing/muxfiles.py
+-rw-rw-rw-   0        0        0     6371 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/muxing/tmdb.py
+-rw-rw-rw-   0        0        0     6836 2023-06-04 10:19:37.000000 muxtools-0.0.2/muxtools/muxing/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.257354 muxtools-0.0.2/muxtools/subtitle/
+-rw-rw-rw-   0        0        0      128 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/subtitle/__init__.py
+-rw-rw-rw-   0        0        0     1621 2023-06-04 10:32:35.000000 muxtools-0.0.2/muxtools/subtitle/font.py
+-rw-rw-rw-   0        0        0     3423 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/subtitle/styles.py
+-rw-rw-rw-   0        0        0    19594 2023-06-04 10:24:58.000000 muxtools-0.0.2/muxtools/subtitle/sub.py
+-rw-rw-rw-   0        0        0     1649 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/subtitle/subutils.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.263687 muxtools-0.0.2/muxtools/utils/
+-rw-rw-rw-   0        0        0      242 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/convert.py
+-rw-rw-rw-   0        0        0     4270 2023-06-03 00:34:39.000000 muxtools-0.0.2/muxtools/utils/download.py
+-rw-rw-rw-   0        0        0     1449 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/env.py
+-rw-rw-rw-   0        0        0     5357 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/files.py
+-rw-rw-rw-   0        0        0     2426 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/format.py
+-rw-rw-rw-   0        0        0     1248 2023-05-31 22:50:01.000000 muxtools-0.0.2/muxtools/utils/glob.py
+-rw-rw-rw-   0        0        0     1708 2023-06-01 16:53:30.000000 muxtools-0.0.2/muxtools/utils/log.py
+-rw-rw-rw-   0        0        0     8163 2023-06-01 18:49:53.000000 muxtools-0.0.2/muxtools/utils/parsing.py
+-rw-rw-rw-   0        0        0     3382 2023-06-02 23:57:08.000000 muxtools-0.0.2/muxtools/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:10:42.244351 muxtools-0.0.2/muxtools.egg-info/
+-rw-rw-rw-   0        0        0     1115 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-04 11:10:42.000000 muxtools-0.0.2/muxtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1335 2023-06-04 11:10:17.000000 muxtools-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 11:10:42.264687 muxtools-0.0.2/setup.cfg
```

### Comparing `muxtools-0.0.1/LICENSE` & `muxtools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/PKG-INFO` & `muxtools-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.1/muxtools/__init__.py` & `muxtools-0.0.2/muxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/audio/audioutils.py` & `muxtools-0.0.2/muxtools/audio/audioutils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,94 @@
 import os
 import re
 import subprocess
 from shutil import rmtree
 from pymediainfo import Track
 from functools import cmp_to_key
+from pymediainfo import MediaInfo
 
-
-from ..utils.log import warn, error
+from ..utils.files import make_output
 from ..muxing.muxfiles import AudioFile
-from ..utils.env import get_temp_workdir
+from ..utils.log import debug, warn, error
 from ..utils.download import get_executable
-from ..utils.types import DitherType, Trim, AudioFormat
+from ..utils.env import get_temp_workdir, run_commandline
+from ..utils.types import DitherType, Trim, AudioFormat, ValidInputType
 
 __all__ = ["ensure_valid_in", "sanitize_trims", "format_from_track", "is_fancy_codec", "has_libFLAC", "has_libFDK"]
 
 
 def ensure_valid_in(
     input: AudioFile,
     supports_pipe: bool = True,
     dither: bool = True,
     dither_type: DitherType = DitherType.TRIANGULAR,
+    valid_type: ValidInputType = ValidInputType.FLAC,
     caller: any = None,
 ) -> AudioFile | subprocess.Popen:
     """
     Ensures valid input for any encoder that accepts flac (all of them).
     Passes existing file if no need to dither and is either wav or flac.
     """
     from .encoders import FF_FLAC
 
-    def getflac(input: AudioFile):
+    def get_flac(input: AudioFile):
         if supports_pipe:
             return FF_FLAC(dither=dither, dither_type=dither_type).get_pipe(input)
         else:
             return FF_FLAC(
                 compression_level=0, dither=dither, dither_type=dither_type, output=os.path.join(get_temp_workdir(), "tempflac")
             ).encode_audio(input, temp=True)
 
+    def get_pcm(input: AudioFile):
+        ffmpeg = get_executable("ffmpeg")
+        minfo = input.get_mediainfo()
+        cope = "pcm_s24be" if valid_type == ValidInputType.AIFF else "pcm_s24le"
+        args = [ffmpeg, "-i", str(input.file), "-map", "0:a:0", "-c:a", "pcm_s16le" if minfo.bit_depth == 16 or dither else cope]
+        if dither:
+            args.extend(["-sample_fmt", "s16", "-ar", "48000", "-resampler", "soxr", "-precision", "24", "-dither_method", dither_type.name.lower()])
+        output = make_output(input.file, "aiff" if valid_type == ValidInputType.AIFF else "w64", "ffmpeg", temp=True)
+
+        if supports_pipe:
+            debug(f"Piping audio to ensure valid input using ffmpeg...", caller)
+            args.extend(["-f", "aiff" if valid_type == ValidInputType.AIFF else "w64", "-"])
+            p = subprocess.Popen(args, stdin=subprocess.DEVNULL, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, text=False)
+            return p
+        else:
+            debug(f"Preparing audio to ensure valid input using ffmpeg...", caller)
+            args.append(str(output))
+            if not run_commandline(args):
+                return AudioFile(output, input.container_delay, input.source)
+            else:
+                raise error("Failed to convert to desired intermediary!", ensure_valid_in)
+
     if input.has_multiple_tracks(caller):
-        msg = f"'{input.name}' is a container with multiple tracks.\n"
+        msg = f"'{input.file.name}' is a container with multiple tracks.\n"
         msg += f"The first audio track will be {'piped' if supports_pipe else 'extracted'} using default ffmpeg."
         warn(msg, caller, 5)
-
-    minfo = input.get_mediainfo()
-    if is_fancy_codec(minfo):
+    minfo = MediaInfo.parse(input.file)
+    trackinfo = input.get_mediainfo(minfo)
+    container = input.get_containerinfo(minfo)
+    if is_fancy_codec(trackinfo):
         warn("Encoding tracks with special DTS Features or Atmos is very much discouraged.", caller, 10)
-    form = minfo.format.lower()
-    if "wav" in form or "flac" in form or "pcm" in form:
-        if minfo.bit_depth > 16 and dither:
-            return getflac(input)
-        return input
+    form = trackinfo.format.lower()
+    if input.is_lossy():
+        warn(f"It's strongly recommended to not reencode lossy audio! ({trackinfo.format})", caller, 5)
+
+    if form == "wave" or container.format.lower() == "wave":
+        if not (trackinfo.bit_depth > 16 and dither):
+            return input
+    if valid_type == ValidInputType.AIFF_OR_FLAC:
+        valid_type = ValidInputType.AIFF
+        if (form == "flac" or container.format.lower() == "flac") and not (trackinfo.bit_depth > 16 and dither):
+            return input
+
+    if valid_type == ValidInputType.FLAC:
+        return get_flac(input)
     else:
-        if input.is_lossy():
-            warn(f"It's strongly recommended to not reencode lossy audio! ({minfo.format})", caller, 5)
-        return getflac(input)
+        return get_pcm(input)
 
 
 def compare_trims(trim: Trim, trim2: Trim):
     if trim[0] is None and trim2[0] is not None:
         return -1
     elif trim[0] is not None and trim2[0] is None:
         return 1
@@ -138,15 +170,15 @@
     
     # Lossless
     AudioFormat("FLAC",         "flac",     "A_FLAC", False),
     AudioFormat("MLP FBA*",     "thd",      "A_TRUEHD", False), # Atmos stuff has some more shit in the format name
     AudioFormat("PCM*",         "wav",      "A_PCM*", False),
 
     # Disgusting DTS Stuff
-    AudioFormat("DTS XLL",      "dtshd",    "A_DTS", False), # Can be HD-MA or Headphone X or X, who the fuck knows
+    AudioFormat("DTS XLL*",     "dtshd",    "A_DTS", False), # Can be HD-MA or Headphone X or X, who the fuck knows
     AudioFormat("DTS",          "dts",      "A_DTS"), # Can be lossy
 ]
 # fmt: on
 
 
 def format_from_track(track: Track) -> AudioFormat | None:
     for format in formats:
@@ -174,20 +206,24 @@
 def is_fancy_codec(track: Track) -> bool:
     """
     Tries to check if a track is some fancy DTS (X, Headphone X) or TrueHD with Atmos
 
     :param track:   Input track to check
     """
     codec_id = str(track.codec_id).casefold()
-    if codec_id == "A_TRUEHD".casefold():
-        # If it contains something other than "MLP FBA" it's probably atmos
-        return bool(re.sub("MLP FBA", "", str(track.format).strip(), re.IGNORECASE))
-    elif codec_id == "A_DTS".casefold():
+    if codec_id == "A_TRUEHD".casefold() or "truehd" in track.commercial_name.lower():
+        if "atmos" in track.commercial_name.lower():
+            return True
+        if not hasattr(track, "format_additionalfeatures") or not track.format_additionalfeatures:
+            return False
+        # If it contains something other than the fallback AC-3 track it's probably atmos
+        return "ch" in track.format_additionalfeatures
+    elif codec_id == "A_DTS".casefold() or "dts" in track.format.lower():
         # Not even lossless if this doesn't exist
-        if not hasattr(track, "format_additionalfeatures"):
+        if not hasattr(track, "format_additionalfeatures") or not track.format_additionalfeatures:
             return False
         # If those additional features contain something after removing "XLL" its some fancy stuff
         return bool(re.sub("XLL", "", str(track.format_additionalfeatures).strip(), re.IGNORECASE))
 
     return False
 
 
@@ -210,7 +246,17 @@
     """
     exe = get_executable("qaac")
     p = subprocess.run([exe, "--check"], capture_output=True, text=True)
     for line in p.stderr.splitlines():
         if "libflac" in line.lower():
             return True
     return False
+
+
+def qaac_compatcheck():
+    if not has_libFLAC():
+        raise error(
+            "Your installation of qaac does not have libFLAC.\nIt is needed for proper piping from ffmpeg etc."
+            + "\nYou can download it from https://github.com/xiph/flac/releases"
+            + "\nFor installation check https://github.com/nu774/qaac/wiki/Installation",
+            "QAAC",
+        )
```

### Comparing `muxtools-0.0.1/muxtools/audio/encoders.py` & `muxtools-0.0.2/muxtools/audio/encoders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from shlex import split as splitcommand
 from dataclasses import dataclass
 import subprocess
 import os
 
-
-from .tools import Encoder
+from .tools import Encoder, LosslessEncoder
 from ..muxing.muxfiles import AudioFile
-from .audioutils import ensure_valid_in, has_libFDK, has_libFLAC
+from ..utils.env import run_commandline
 from ..utils.download import get_executable
 from ..utils.log import warn, crit, debug, error
 from ..utils.files import make_output, clean_temp_files
-from ..utils.env import get_temp_workdir, run_commandline
-from ..utils.types import DitherType, qAAC_MODE, PathLike
+from ..utils.types import DitherType, ValidInputType, qAAC_MODE, PathLike
+from .audioutils import ensure_valid_in, has_libFDK, qaac_compatcheck
 
 __all__ = ["FLAC", "FLACCL", "FF_FLAC", "Opus", "qAAC", "FDK_AAC"]
 
 
 @dataclass
-class FLAC(Encoder):
+class FLAC(LosslessEncoder):
     """
     Uses the reference libFLAC encoder to encode audio to flac.
 
     :param compression_level:   Any int value from 0 to 8 (Higher = better but slower)
     :param dither:              Dithers any input down to 16 bit 48 khz if True
     :param dither_type:         FFMPEG dither_method used for dithering
     :param append:              Any other args one might pass to the encoder
@@ -36,15 +35,17 @@
     output: PathLike | None = None
 
     def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
         if not isinstance(input, AudioFile):
             input = AudioFile.from_file(input, self)
         flaccl = get_executable("flac")
         output = make_output(input.file, "flac", "libflac", self.output)
-        source = ensure_valid_in(input, dither=self.dither, dither_type=self.dither_type, caller=self, supports_pipe=False)
+        source = ensure_valid_in(
+            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False
+        )
         debug(f"Encoding '{input.file.stem}' to FLAC using libFLAC...", self)
 
         args = [flaccl, f"-{self.compression_level}", str(source.file.resolve()) if isinstance(source, AudioFile) else "-"]
         args.extend(["-o", str(output)])
         if self.append:
             args.extend(splitcommand(self.append))
 
@@ -55,15 +56,15 @@
             clean_temp_files()
             return AudioFile(output, input.container_delay, input.source)
         else:
             raise crit("Encoding to FLAC using libFLAC failed!", self)
 
 
 @dataclass
-class FLACCL(Encoder):
+class FLACCL(LosslessEncoder):
     """
     Uses the CUETools FLACCL encoder to encode audio to flac.
     This one uses OpenCL or Cuda depending on your GPU and claims to have better compression than libFLAC.
 
     :param compression_level:   Any int value from 0 to 8 (Higher = better but slower)
     :param dither:              Dithers any input down to 16 bit 48 khz if True
     :param dither_type:         FFMPEG dither_method used for dithering
@@ -79,15 +80,17 @@
     output: PathLike | None = None
 
     def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
         if not isinstance(input, AudioFile):
             input = AudioFile.from_file(input, self)
         flaccl = get_executable("CUETools.FLACCL.cmd")
         output = make_output(input.file, "flac", "flaccl", self.output)
-        source = ensure_valid_in(input, dither=self.dither, dither_type=self.dither_type, caller=self, supports_pipe=False)
+        source = ensure_valid_in(
+            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.FLAC, supports_pipe=False
+        )
         debug(f"Encoding '{input.file.stem}' to FLAC using FLACCL...", self)
 
         args = [flaccl, f"-{self.compression_level}", str(source.file.resolve()) if isinstance(source, AudioFile) else "-"]
         args.extend(["-o", str(output)])
         if self.append:
             args.extend(splitcommand(self.append))
 
@@ -98,15 +101,15 @@
             clean_temp_files()
             return AudioFile(output, input.container_delay, input.source)
         else:
             raise crit("Encoding to FLAC using FLACCL failed!", self)
 
 
 @dataclass
-class FF_FLAC(Encoder):
+class FF_FLAC(LosslessEncoder):
     """
     Uses the ffmpeg/libav FLAC encoder to encode audio to flac.
 
     :param compression_level:   Any int value from 0 to 12 (Higher = better but slower)
     :param dither:              Dithers any input down to 16 bit 48 khz if True
     :param dither_type:         FFMPEG dither_method used for dithering
     :param append:              Any other args one might pass to the encoder
@@ -193,15 +196,17 @@
                 case _:
                     self.bitrate = 320
             debug(f"Encoding '{input.file.stem}' to Opus ({self.bitrate} kbps) using opusenc...", self)
         else:
             debug(f"Encoding '{input.file.stem}' to Opus using opusenc...", self)
 
         output = make_output(input.file, "opus", "opusenc", self.output)
-        source = ensure_valid_in(input, dither=self.dither, dither_type=self.dither_type, caller=self, supports_pipe=True)
+        source = ensure_valid_in(
+            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=True
+        )
 
         args = [exe, "--vbr" if self.vbr else "--cvbr", "--bitrate", str(self.bitrate)]
         if self.append:
             args.extend(splitcommand(self.append))
         args.append(str(source.file.resolve()) if isinstance(source, AudioFile) else "-")
         args.append(str(output))
 
@@ -237,24 +242,19 @@
     append: str = ""
     output: PathLike | None = None
 
     def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
         if not isinstance(input, AudioFile):
             input = AudioFile.from_file(input, self)
         output = make_output(input.file, "aac", "qaac", self.output)
-        source = ensure_valid_in(input, dither=self.dither, dither_type=self.dither_type, caller=self, supports_pipe=False)
+        source = ensure_valid_in(
+            input, dither=self.dither, dither_type=self.dither_type, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False
+        )
         qaac = get_executable("qaac")
-
-        if not has_libFLAC():
-            raise error(
-                "Your installation of qaac does not have libFLAC.\nIt is needed for proper piping from ffmpeg etc."
-                + "\nYou can download it from https://github.com/xiph/flac/releases"
-                + "\nFor installation check https://github.com/nu774/qaac/wiki/Installation",
-                self,
-            )
+        qaac_compatcheck()
 
         debug(f"Encoding '{input.file.stem}' to AAC using qAAC...", self)
         args = [qaac, "--no-delay", "--no-optimize", "--threading", f"--{self.mode.name.lower()}", str(self.q)]
         if self.append:
             args.extend(splitcommand(self.append))
         args.extend(["-o", str(output), str(source.file.resolve()) if isinstance(source, AudioFile) else "-"])
```

### Comparing `muxtools-0.0.1/muxtools/audio/extractors.py` & `muxtools-0.0.2/muxtools/audio/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,45 +91,48 @@
         output: PathLike | None = None
 
         def extract_audio(self, input: PathLike, quiet: bool = True) -> AudioFile:
             ffmpeg = get_executable("ffmpeg")
             input = ensure_path_exists(input, self)
             track = get_absolute_track(input, self.track, TrackType.AUDIO, self)
             form = format_from_track(track)
-            ainfo = parse_audioinfo(input, self.track, self)
             debug(f"Extracting audio track from '{input.stem}' using ffmpeg...", self)
             if not form:
+                ainfo = parse_audioinfo(input, self.track, self)
                 lossy = getattr(track, "compression_mode", "lossless").lower() == "lossy"
                 if lossy:
                     raise error(f"Unrecognized lossy format found: {track.format}", self)
                 else:
                     extension = "wav"
                     warn("Unrecognized format: {track.format}\nWill extract as wav instead.", self, 2)
                     out = make_output(input, extension, f"extracted_{self.track}", self.output)
             else:
+                ainfo = parse_audioinfo(input, self.track, self, form.ext == "thd")
                 lossy = form.lossy
                 extension = form.ext
                 out = make_output(input, extension, f"extracted_{self.track}", self.output)
 
             args = [ffmpeg, "-hide_banner", "-i", str(input.resolve()), "-map_chapters", "-1", "-map", f"0:a:{self.track}"]
 
             specified_depth = getattr(track, "bit_depth", 16)
-            if str(specified_depth) not in ainfo.stats.bit_depth and not lossy and not is_fancy_codec(track):
+            if str(specified_depth) not in ainfo.stats.bit_depth and not lossy and not is_fancy_codec(track) and specified_depth is not None:
                 actual_depth = int(ainfo.stats.bit_depth) if "/" not in ainfo.stats.bit_depth else int(ainfo.stats.bit_depth.split("/")[0])
                 debug(f"Detected fake/padded {specified_depth} bit. Actual depth is {actual_depth} bit.", self)
                 if specified_depth - actual_depth > 4:
                     debug("Track will be outputted as flac and truncated to 16 bit instead.", self)
                     out = make_output(input, "flac", f"extracted_{self.track}", self.output)
                     args.extend(["-c:a", "flac", "-sample_fmt", "s16"])
             else:
                 if extension == "wav":
                     args.extend(["-c:a", "pcm_s16le" if specified_depth == 16 else "pcm_s24le"])
                 else:
                     args.extend(["-c:a", "copy"])
-
+                    if extension == "dtshd" or extension == "dts":
+                        # FFMPEG screams about dtshd not being a known output format but ffmpeg -formats lists it....
+                        args.extend(["-f", "dts"])
             args.append(str(out))
 
             if not run_commandline(args, quiet):
                 debug("Done", self)
                 return AudioFile(out, getattr(track, "delay_relative_to_video", 0) if self.preserve_delay else 0, input, ainfo)
             else:
                 raise error("Failed to extract audio track using ffmpeg", self)
```

### Comparing `muxtools-0.0.1/muxtools/cli.py` & `muxtools-0.0.2/muxtools/cli.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/functions.py` & `muxtools-0.0.2/muxtools/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             trimmer = Sox()
 
     if isinstance(encoder, AutoEncoder):
         if lossy:
             encoder = None
         elif is_fancy_codec(audio.get_mediainfo()):
             encoder = None
-            warn("Audio will be reencoded due to having Atmos or special DTS features.", do_audio, 2)
+            warn("Audio will not be reencoded due to having Atmos or special DTS features.", do_audio, 2)
         else:
             encoder = Opus()
 
     if trimmer and trims:
         setattr(trimmer, "trim", trims)
         setattr(trimmer, "fps", fps)
         setattr(trimmer, "num_frames", num_frames)
```

### Comparing `muxtools-0.0.1/muxtools/main.py` & `muxtools-0.0.2/muxtools/main.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/misc/chapters.py` & `muxtools-0.0.2/muxtools/misc/chapters.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/muxing/mux.py` & `muxtools-0.0.2/muxtools/muxing/mux.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/muxing/muxfiles.py` & `muxtools-0.0.2/muxtools/muxing/muxfiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,23 @@
 @dataclass
 class AudioFile(MuxingFile):
     info: AudioInfo | None = None
 
     def __post_init__(self):
         self.file = ensure_path_exists(self.file, self)
 
-    def get_mediainfo(self) -> Track:
-        return MediaInfo.parse(self.file).audio_tracks[0]
+    def get_containerinfo(self, mediainfo: MediaInfo | None = None) -> Track:
+        if not mediainfo:
+            mediainfo = MediaInfo.parse(self.file)
+        return mediainfo.general_tracks[0]
+
+    def get_mediainfo(self, mediainfo: MediaInfo | None = None) -> Track:
+        if not mediainfo:
+            mediainfo = MediaInfo.parse(self.file)
+        return mediainfo.audio_tracks[0]
 
     def is_lossy(self) -> bool:
         from ..audio.audioutils import format_from_track
 
         minfo = self.get_mediainfo()
         form = format_from_track(minfo)
         if form:
@@ -106,14 +113,14 @@
         if run_commandline(args, quiet) in [0, 1]:
             if delete:
                 self.file.unlink()
             return out
         else:
             raise error("Failed to mux AudioFile to mka.", self)
 
-    @classmethod
+    @staticmethod
     def from_file(pathIn: PathLike, caller: any):
-        from utils.log import warn
+        from ..utils.log import warn
 
         warn("It's strongly recommended to explicitly extract tracks first!", caller, 1)
         file = ensure_path_exists(pathIn, caller)
         return AudioFile(file, 0, file)
```

### Comparing `muxtools-0.0.1/muxtools/muxing/tmdb.py` & `muxtools-0.0.2/muxtools/muxing/tmdb.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/muxing/tracks.py` & `muxtools-0.0.2/muxtools/muxing/tracks.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,26 +151,26 @@
                     args += f" -d {abso}"
             else:
                 abso = get_absolute_tracknum(file, video, TrackType.VIDEO)
                 args += f" -d {abso}"
 
         if audio is None:
             args += " -A"
-        else:
+        elif audio != -1:
             if isinstance(audio, list):
                 for num in audio:
                     abso = get_absolute_tracknum(file, num, TrackType.AUDIO)
                     args += f" -a {abso}"
             else:
                 abso = get_absolute_tracknum(file, audio, TrackType.AUDIO)
                 args += f" -a {abso}"
 
         if subtitles is None:
             args += " -S"
-        else:
+        elif subtitles != -1:
             if isinstance(subtitles, list):
                 for num in audio:
                     abso = get_absolute_tracknum(file, num, TrackType.SUB)
                     args += f" -s {abso}"
             else:
                 abso = get_absolute_tracknum(file, subtitles, TrackType.SUB)
                 args += f" -s {abso}"
```

### Comparing `muxtools-0.0.1/muxtools/subtitle/font.py` & `muxtools-0.0.2/muxtools/subtitle/font.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/subtitle/styles.py` & `muxtools-0.0.2/muxtools/subtitle/styles.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/subtitle/sub.py` & `muxtools-0.0.2/muxtools/subtitle/sub.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             main = docs[0]
             existing_styles = [style.name for style in (main.styles)]
             docs.remove(main)
 
             for doc in docs:
                 main.events.extend(doc.events)
                 for style in doc.styles:
-                    if style.name.casefold() in [s.name.casefold() for s in existing_styles]:
+                    if style.name.casefold() in [s.casefold() for s in existing_styles]:
                         warn(f"Ignoring style '{style.name}' due to preexisting style of the same name.", self)
                         continue
                     main.styles.append(style)
 
             self.source = self.file[0]
             out = make_output(self.file[0], "ass", "merged")
             with open(out, "w", encoding=self.encoding) as writer:
```

### Comparing `muxtools-0.0.1/muxtools/subtitle/subutils.py` & `muxtools-0.0.2/muxtools/subtitle/subutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/convert.py` & `muxtools-0.0.2/muxtools/utils/convert.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/download.py` & `muxtools-0.0.2/muxtools/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     Tool("ffmpeg", "https://github.com/AnimMouse/ffmpeg-autobuild/releases/download/m-2023-05-08-05-43/ffmpeg-f009f84-3e8c1fa-win64-nonfree.7z", ["ffprobe"]),
     Tool("mkvmerge", "https://www.videohelp.com/download/mkvtoolnix-64-bit-76.0.7z", ['mkvextract', 'mkvinfo', 'mkvpropedit']), 
     Tool("eac3to", "https://files.catbox.moe/k0gzt0.7z"), # Custom package because of removed sounds and updated libFlac
     Tool("x264", "https://github.com/DJATOM/x264-aMod/releases/download/r3101+20/x264-aMod-x64-core164-r3101+20.7z"),
     Tool("x265", "https://github.com/DJATOM/x265-aMod/releases/download/3.5+67/x265-x64-v3.5+67-aMod-gcc12.2.1+opt.7z"),
     Tool("qaac", "https://files.catbox.moe/cxtxm4.7z"), # 2.79 with flac, w64 and iTunes libraries included
     Tool("opusenc", "https://archive.mozilla.org/pub/opus/win32/opus-tools-0.2-opus-1.3.zip"),
-    Tool("flac", "https://github.com/xiph/flac/releases/download/1.4.2/flac-1.4.2-win.zip")
+    Tool("flac", "https://github.com/xiph/flac/releases/download/1.4.2/flac-1.4.2-win.zip"),
+    Tool("wavpack", "https://github.com/dbry/WavPack/releases/download/5.6.0/wavpack-5.6.0-x64.zip")
 ]
 # fmt: on
 
 # TODO: check CPU to decide on which x264/5 file to use
 
 
 def get_executable(type: str, can_download: bool | None = None) -> str:
```

### Comparing `muxtools-0.0.1/muxtools/utils/env.py` & `muxtools-0.0.2/muxtools/utils/env.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/files.py` & `muxtools-0.0.2/muxtools/utils/files.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/format.py` & `muxtools-0.0.2/muxtools/utils/format.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/glob.py` & `muxtools-0.0.2/muxtools/utils/glob.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/log.py` & `muxtools-0.0.2/muxtools/utils/log.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.1/muxtools/utils/parsing.py` & `muxtools-0.0.2/muxtools/utils/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,28 +71,28 @@
                 m2tsFile = Path(match.group(1))
                 if m2tsFile.exists():
                     return m2tsFile
     print("Warning!\nCould not resolve origin file path from the dgindex input!")
     return dgiFile
 
 
-def parse_audioinfo(file: PathLike, track: int = 0, caller: any = None) -> AudioInfo:
+def parse_audioinfo(file: PathLike, track: int = 0, caller: any = None, is_thd: bool = False) -> AudioInfo:
     f_compiled = re.compile(AUDIOFRAME_REGEX, re.IGNORECASE)
     s_compiled = re.compile(AUDIOSTATS_REGEX, re.IGNORECASE)
     file = ensure_path_exists(file, parse_audioinfo)
     track = get_absolute_tracknum(file, track, TrackType.AUDIO)
     ffmpeg = get_executable("ffmpeg")
     out_var = "NUL" if os.name == "nt" else "/dev/null"
     args = [
         ffmpeg,
         "-hide_banner",
         "-i",
         file.resolve(),
         "-t",
-        "120",
+        "4" if is_thd else "10",
         "-map",
         f"0:{track}",
         "-filter:a",
         "astats=metadata=1,ashowinfo",
         "-f",
         "wav",
         out_var,
```

### Comparing `muxtools-0.0.1/muxtools/utils/types.py` & `muxtools-0.0.2/muxtools/utils/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from enum import IntEnum, Enum
 from pathlib import Path
 from typing import TypeVar, Union, Optional
 from datetime import timedelta
 from dataclasses import dataclass
 
-__all__ = ["PathLike", "Paths", "Trim", "TrackType", "AudioFormat", "AudioFrame", "AudioStats", "AudioInfo", "Chapter", "DitherType"]
+__all__ = [
+    "PathLike",
+    "Paths",
+    "Trim",
+    "TrackType",
+    "AudioFormat",
+    "AudioFrame",
+    "AudioStats",
+    "AudioInfo",
+    "Chapter",
+    "DitherType",
+    "LossyWavQuality",
+]
 
 PathLike = TypeVar("PathLike", str, Path, None)
 Trim = tuple[int | None, int | None]
 
 Paths = Union[PathLike, list[PathLike]]
 
 # Timedelta (or frame, which will be converted internally), Optional Name
@@ -52,14 +64,37 @@
 class qAAC_MODE(IntEnum):
     TVBR = 1
     CVBR = 2
     ABR = 3
     CBR = 4
 
 
+class LossyWavQuality(IntEnum):
+    """
+    LossyWAV Quality presets, see https://wiki.hydrogenaud.io/index.php?title=LossyWAV#Quality_presets
+
+    TL;DR: Insane the least lossy, ExtraPortable the most lossy.
+    """
+
+    INSANE = 1
+    EXTREME = 2
+    HIGH = 3
+    STANDARD = 4
+    ECONOMIC = 5
+    PORTABLE = 6
+    EXTRAPORTABLE = 7
+
+
+class ValidInputType(IntEnum):
+    FLAC = 1
+    AIFF = 2
+    W64 = 3
+    AIFF_OR_FLAC = 4
+
+
 @dataclass
 class AudioFrame:
     """
     A dataclass representing ffmpeg's `ashowdata` filter output.
 
     :param n:           The (sequential) number of the input frame, starting from 0
     :param pts:         The presentation timestamp of the input frame, in time base units
```

### Comparing `muxtools-0.0.1/muxtools.egg-info/PKG-INFO` & `muxtools-0.0.2/muxtools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/muxtools
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `muxtools-0.0.1/muxtools.egg-info/SOURCES.txt` & `muxtools-0.0.2/muxtools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 muxtools.egg-info/entry_points.txt
 muxtools.egg-info/requires.txt
 muxtools.egg-info/top_level.txt
 muxtools/audio/__init__.py
 muxtools/audio/audioutils.py
 muxtools/audio/encoders.py
 muxtools/audio/extractors.py
+muxtools/audio/memecoders.py
 muxtools/audio/tools.py
 muxtools/misc/__init__.py
 muxtools/misc/chapters.py
 muxtools/muxing/__init__.py
 muxtools/muxing/mux.py
 muxtools/muxing/muxfiles.py
 muxtools/muxing/tmdb.py
```

### Comparing `muxtools-0.0.1/pyproject.toml` & `muxtools-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "muxtools"
-version = "0.0.1"
+version = "0.0.2"
 description = "A library for various muxing and automation tools for anything and everything fansubbing related"
 authors = [
     { name="Vodes", email="vodes.imp@gmail.com" }
 ]
 dependencies = [
     "requests>=2.31.0",
     "fontcollector>=2.1.0",
```

