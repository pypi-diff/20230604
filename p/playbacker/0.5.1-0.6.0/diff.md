# Comparing `tmp/playbacker-0.5.1.tar.gz` & `tmp/playbacker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playbacker-0.5.1.tar", max compression
+gzip compressed data, was "playbacker-0.6.0.tar", max compression
```

## Comparing `playbacker-0.5.1.tar` & `playbacker-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1254 2023-05-07 01:46:02.339974 playbacker-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/__init__.py
--rw-r--r--   0        0        0     5020 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/app.py
--rw-r--r--   0        0        0      527 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/config.py
--rw-r--r--   0        0        0        0 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/__init__.py
--rw-r--r--   0        0        0      850 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/audiofile.py
--rw-r--r--   0        0        0     1292 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/clock.py
--rw-r--r--   0        0        0     3423 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/playback.py
--rw-r--r--   0        0        0     1444 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/player.py
--rw-r--r--   0        0        0      952 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/setlist.py
--rw-r--r--   0        0        0     3408 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/settings.py
--rw-r--r--   0        0        0      892 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/song.py
--rw-r--r--   0        0        0     3137 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/stream.py
--rw-r--r--   0        0        0      757 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tempo.py
--rw-r--r--   0        0        0     2607 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/track.py
--rw-r--r--   0        0        0        0 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tracks/__init__.py
--rw-r--r--   0        0        0     1812 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tracks/countdown.py
--rw-r--r--   0        0        0     2064 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/tracks/metronome.py
--rw-r--r--   0        0        0     1078 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/core/validate.py
--rw-r--r--   0        0        0    21934 2023-05-07 01:46:01.779969 playbacker-0.5.1/src/playbacker/dist/assets/index-04f532a9.js
--rw-r--r--   0        0        0     8295 2023-05-07 01:46:01.779969 playbacker-0.5.1/src/playbacker/dist/assets/index-c1f1d727.css
--rw-r--r--   0        0        0      388 2023-05-07 01:46:01.779969 playbacker-0.5.1/src/playbacker/dist/index.html
--rw-r--r--   0        0        0     2807 2023-05-07 01:45:29.687705 playbacker-0.5.1/src/playbacker/main.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 playbacker-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1254 2023-06-04 10:56:30.501816 playbacker-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-04 10:55:57.257497 playbacker-0.6.0/src/playbacker/__init__.py
+-rw-r--r--   0        0        0     5020 2023-06-04 10:55:57.257497 playbacker-0.6.0/src/playbacker/app.py
+-rw-r--r--   0        0        0      527 2023-06-04 10:55:57.257497 playbacker-0.6.0/src/playbacker/config.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/__init__.py
+-rw-r--r--   0        0        0      850 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/audiofile.py
+-rw-r--r--   0        0        0     1292 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/clock.py
+-rw-r--r--   0        0        0     3423 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/playback.py
+-rw-r--r--   0        0        0     1444 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/player.py
+-rw-r--r--   0        0        0      974 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/setlist.py
+-rw-r--r--   0        0        0     3408 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/settings.py
+-rw-r--r--   0        0        0      892 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/song.py
+-rw-r--r--   0        0        0     3137 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/stream.py
+-rw-r--r--   0        0        0      757 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tempo.py
+-rw-r--r--   0        0        0     2607 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/track.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tracks/__init__.py
+-rw-r--r--   0        0        0     1812 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tracks/countdown.py
+-rw-r--r--   0        0        0     2064 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/tracks/metronome.py
+-rw-r--r--   0        0        0     1122 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/core/validate.py
+-rw-r--r--   0        0        0    21934 2023-06-04 10:56:29.545807 playbacker-0.6.0/src/playbacker/dist/assets/index-04f532a9.js
+-rw-r--r--   0        0        0     8295 2023-06-04 10:56:29.545807 playbacker-0.6.0/src/playbacker/dist/assets/index-c1f1d727.css
+-rw-r--r--   0        0        0      388 2023-06-04 10:56:29.545807 playbacker-0.6.0/src/playbacker/dist/index.html
+-rw-r--r--   0        0        0     2807 2023-06-04 10:55:57.261498 playbacker-0.6.0/src/playbacker/main.py
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 playbacker-0.6.0/PKG-INFO
```

### Comparing `playbacker-0.5.1/pyproject.toml` & `playbacker-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "playbacker"
-version = "v0.5.1"
+version = "v0.6.0"
 description = "Live music performance playback"
 authors = ["Lev Vereshchagin <mail@vrslev.com>"]
 license = "MIT"
 # TODO: readme
 # readme = "../README.md"
 include = ["src/playbacker/dist/**/*"]
```

### Comparing `playbacker-0.5.1/src/playbacker/app.py` & `playbacker-0.6.0/src/playbacker/app.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/config.py` & `playbacker-0.6.0/src/playbacker/config.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/audiofile.py` & `playbacker-0.6.0/src/playbacker/core/audiofile.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/clock.py` & `playbacker-0.6.0/src/playbacker/core/clock.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/playback.py` & `playbacker-0.6.0/src/playbacker/core/playback.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/player.py` & `playbacker-0.6.0/src/playbacker/core/player.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/setlist.py` & `playbacker-0.6.0/src/playbacker/core/setlist.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __init__(self, message: str) -> None:
         self.message = message
         super().__init__()
 
 
 def _find_song_in_storage(name: str, storage: list[Song]):
     for song in storage:
-        if song.name == name:
+        if song.name.casefold() == name.casefold():
             return song
 
     raise NoSongInStorageError(f'Song "{name}" is not present in storage')
 
 
 class FileSetlist(BaseModel):
     __root__: list[str]
```

### Comparing `playbacker-0.5.1/src/playbacker/core/settings.py` & `playbacker-0.6.0/src/playbacker/core/settings.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/song.py` & `playbacker-0.6.0/src/playbacker/core/song.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/stream.py` & `playbacker-0.6.0/src/playbacker/core/stream.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/tempo.py` & `playbacker-0.6.0/src/playbacker/core/tempo.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/track.py` & `playbacker-0.6.0/src/playbacker/core/track.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/tracks/countdown.py` & `playbacker-0.6.0/src/playbacker/core/tracks/countdown.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/tracks/metronome.py` & `playbacker-0.6.0/src/playbacker/core/tracks/metronome.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/core/validate.py` & `playbacker-0.6.0/src/playbacker/core/validate.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,19 +20,21 @@
         content = yaml.safe_load(f)
     load_settings(content, "default")
 
 
 def get_unknown_songs(songs_file: Path, setlists_dir: Path):
     with songs_file.open() as f:
         content = yaml.safe_load(f)
-    songs = [s.name for s in load_songs(content)]
+    songs = [s.name.casefold() for s in load_songs(content)]
     res: dict[Path, list[str]] = {}
 
     for setlist_path in setlists_dir.glob("*.yaml"):
         with setlist_path.open() as f:
             content = yaml.safe_load(f)
         cur_songs = FileSetlist(__root__=content).__root__
 
-        if cur_unknown_songs := list(filter(lambda s: s not in songs, cur_songs)):
+        if cur_unknown_songs := list(
+            filter(lambda s: s.casefold() not in songs, cur_songs)
+        ):
             res[setlist_path] = cur_unknown_songs
 
     return res
```

### Comparing `playbacker-0.5.1/src/playbacker/dist/assets/index-04f532a9.js` & `playbacker-0.6.0/src/playbacker/dist/assets/index-04f532a9.js`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/dist/assets/index-c1f1d727.css` & `playbacker-0.6.0/src/playbacker/dist/assets/index-c1f1d727.css`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/src/playbacker/main.py` & `playbacker-0.6.0/src/playbacker/main.py`

 * *Files identical despite different names*

### Comparing `playbacker-0.5.1/PKG-INFO` & `playbacker-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playbacker
-Version: 0.5.1
+Version: 0.6.0
 Summary: Live music performance playback
 License: MIT
 Author: Lev Vereshchagin
 Author-email: mail@vrslev.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

