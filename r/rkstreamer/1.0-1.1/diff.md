# Comparing `tmp/rkstreamer-1.0-py3-none-any.whl.zip` & `tmp/rkstreamer-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 37452 bytes, number of entries: 51
--rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 09:22 rkstreamer/__init__.py
+Zip file size: 37816 bytes, number of entries: 51
+-rw-rw-rw-  2.0 fat       42 b- defN 23-Jun-04 09:46 rkstreamer/__init__.py
 -rw-rw-rw-  2.0 fat     1967 b- defN 23-May-27 23:32 rkstreamer/__main__.py
 -rw-rw-rw-  2.0 fat     2128 b- defN 23-May-28 01:03 rkstreamer/state.py
 -rw-rw-rw-  2.0 fat      164 b- defN 23-May-12 00:51 rkstreamer/controllers/__init__.py
 -rw-rw-rw-  2.0 fat     3989 b- defN 23-May-28 00:53 rkstreamer/controllers/album.py
 -rw-rw-rw-  2.0 fat      575 b- defN 23-May-12 00:43 rkstreamer/controllers/enums.py
 -rw-rw-rw-  2.0 fat     6457 b- defN 23-May-12 02:36 rkstreamer/controllers/patterns.py
 -rw-rw-rw-  2.0 fat     4200 b- defN 23-May-27 17:47 rkstreamer/controllers/playlist.py
@@ -40,14 +40,14 @@
 -rw-rw-rw-  2.0 fat      310 b- defN 23-May-15 16:37 rkstreamer/types/views.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-29 21:21 rkstreamer/utils/__init__.py
 -rw-rw-rw-  2.0 fat      569 b- defN 23-May-07 16:45 rkstreamer/utils/helper.py
 -rw-rw-rw-  2.0 fat      147 b- defN 23-May-12 00:52 rkstreamer/views/__init__.py
 -rw-rw-rw-  2.0 fat     1001 b- defN 23-May-11 00:56 rkstreamer/views/album.py
 -rw-rw-rw-  2.0 fat     1098 b- defN 23-May-27 17:47 rkstreamer/views/playlist.py
 -rw-rw-rw-  2.0 fat     2880 b- defN 23-May-12 17:56 rkstreamer/views/song.py
--rw-rw-rw-  2.0 fat     1084 b- defN 23-Jun-04 09:22 rkstreamer-1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3113 b- defN 23-Jun-04 09:22 rkstreamer-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 09:22 rkstreamer-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Jun-04 09:22 rkstreamer-1.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-04 09:22 rkstreamer-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     4333 b- defN 23-Jun-04 09:22 rkstreamer-1.0.dist-info/RECORD
-51 files, 106601 bytes uncompressed, 30530 bytes compressed:  71.4%
+-rw-rw-rw-  2.0 fat     1084 b- defN 23-Jun-04 09:47 rkstreamer-1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3941 b- defN 23-Jun-04 09:47 rkstreamer-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 09:47 rkstreamer-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-Jun-04 09:47 rkstreamer-1.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-04 09:47 rkstreamer-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     4333 b- defN 23-Jun-04 09:47 rkstreamer-1.1.dist-info/RECORD
+51 files, 107429 bytes uncompressed, 30894 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -129,26 +129,26 @@
 
 Filename: rkstreamer/views/playlist.py
 Comment: 
 
 Filename: rkstreamer/views/song.py
 Comment: 
 
-Filename: rkstreamer-1.0.dist-info/LICENSE
+Filename: rkstreamer-1.1.dist-info/LICENSE
 Comment: 
 
-Filename: rkstreamer-1.0.dist-info/METADATA
+Filename: rkstreamer-1.1.dist-info/METADATA
 Comment: 
 
-Filename: rkstreamer-1.0.dist-info/WHEEL
+Filename: rkstreamer-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: rkstreamer-1.0.dist-info/entry_points.txt
+Filename: rkstreamer-1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rkstreamer-1.0.dist-info/top_level.txt
+Filename: rkstreamer-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: rkstreamer-1.0.dist-info/RECORD
+Filename: rkstreamer-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rkstreamer/__init__.py

```diff
@@ -1,3 +1,3 @@
 """RK streamer"""
 
-__version__ = '1.0'
+__version__ = '1.1'
```

## Comparing `rkstreamer-1.0.dist-info/LICENSE` & `rkstreamer-1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rkstreamer-1.0.dist-info/METADATA` & `rkstreamer-1.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rkstreamer
-Version: 1.0
+Version: 1.1
 Summary: RK's CLI Music Player
 Author-email: "Ray A." <ray@raysecure.ml>
 License: MIT License
         
         Copyright (c) 2023 Ray A.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,18 +31,27 @@
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.2)
 Requires-Dist: python-vlc (>=3.0.18121)
 Requires-Dist: setuptools (>=67.0.0)
 
 ### RK Music Streamer
 
-A command-line music player that allows you to play/stream songs, albums, playlists.
-Powered by Jio Saavn Web APIs.
+A command-line music player that allows you to play/stream songs, albums, playlists. <br>
+**Powered by Jio Saavn Web APIs**
 
 ---
+#### Prerequisites
+- Python 3.9.x or above.
+- VLC player must be installed. This application uses the VLC player from streaming and python-vlc bindings for interaction. <br>
+(Install from [VLC](https://www.videolan.org/vlc/))
+
+#### Dependencies
+- [requests](https://pypi.org/project/requests/)
+- [python-vlc](https://pypi.org/project/python-vlc/)
+---
 ##### Installation
 ```
 > python3 -m pip install rkstreamer
 $ pip/pip3 install rkstreamer
 ```
 ---
 ##### Launch
@@ -53,18 +62,22 @@
 or
 > rkstreamer
 
 ```
 ---
 ##### Usage
 - Default mode is 'Song Search' Mode.
-- Modes can be switched using --album, --plist.
+- Modes can be switched using **--album, --plist**.
 - Supports search parameters for Songs, Albums -> 'search string' -n:number, -l:language, -b:bitrate.
-- -q, -r, -g displays Song Queue, Recommended Songs, Go-to-Album modes.
-- a, p, r followed by the song index can be used to Add, Play, Remove songs from the corresponding queues.
+- **-q, -r, -g** displays Song Queue, Recommended Songs, Go-to-Album modes.
+- **a, p, r** followed by the song index can be used to Add, Play, Remove songs from the corresponding queues.
+- **-c** used to control the player and media playback; supports volume, playback, output controls.
+- Player control actions should be suffixed with the '-c' switch such as -cp - play, -cs - stop, -cn - next song, -cpr - previous song.
+- Volume controls: v - display current volume, +number - volume increase, -number - volume decrease.
+- Playback controls: >seconds - seek forward, <seconds - seek backward, t - shows remaining time.
 
 ---
 ##### Examples
 
 ```
 > Enter the song name: pokkal pokkum -n:5 -l:tamil -b:320
 (Search string - pokkal pokkum, number of results to display - 5, language - tamil, bitrate - 320kpbs)
@@ -79,7 +92,10 @@
 
 > -qr1 - removes the first index song from queue
 > -qp1 - plays the first index song from queue
 > -qa1 - adds the first index song from search list
 
 Similar behaviors for -r (recommended songs), -g (go-to-album).
 Correct prefix and actions should be used such as -rr1, -ga1, etc.
+
+```
+
```

## Comparing `rkstreamer-1.0.dist-info/RECORD` & `rkstreamer-1.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-rkstreamer/__init__.py,sha256=6TuycfRvkH5YWwNjtdI7oUvUM3rQf4mDM99-I02HEgg,42
+rkstreamer/__init__.py,sha256=fDJqSguh3vK6dNVipy6Vws4j93-ED51ksolrTQKVjtc,42
 rkstreamer/__main__.py,sha256=nhSBCNMxgbiPSIIDvX1Jq72g83P0tb2fmQjhNSDiv64,1967
 rkstreamer/state.py,sha256=-3On5ags-itVp2jCzRe300gqvx98NYWP1zmELn-wRec,2128
 rkstreamer/controllers/__init__.py,sha256=cyViI1w1D-PZNN7CdsJmszrgwX7wRDMPWFQhyflr0i4,164
 rkstreamer/controllers/album.py,sha256=ZrSUKIeou7LRkdHqp9mwDcIph-Pyf3x4yuZipVFHdG8,3989
 rkstreamer/controllers/enums.py,sha256=eewgn7wJo2g8mX7gCO1K6PaWAHriIQem5k9YOK2AXR4,575
 rkstreamer/controllers/patterns.py,sha256=OCt4bDcykHG3_SH0aZ0-dBDRKXqTrBIF2EyHlCGmXrw,6457
 rkstreamer/controllers/playlist.py,sha256=Ua0GJ741_gK315za2yvBDHvknytd-DvksLTHE-OTcEY,4200
@@ -39,13 +39,13 @@
 rkstreamer/types/views.py,sha256=RlYzysqM9sF0rM0faEe_A9jCCQkSdwAuDQwlsE0gHYI,310
 rkstreamer/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rkstreamer/utils/helper.py,sha256=nWIKwzTDTbrHuIglidMNlBtJ5CK1Z15H2AAcbbexyPM,569
 rkstreamer/views/__init__.py,sha256=ol3582PpnZgPImuNZ3uSCoiH6ZLg3VTLAa9UI3vGGLU,147
 rkstreamer/views/album.py,sha256=mlmBsV1oQ75QIPOBCIS3fD4O8T4XAxahFbZNCNDWbJw,1001
 rkstreamer/views/playlist.py,sha256=_dBBrJZiT5WMqEtJyTWgtstOUYkkdL9jdt5Z-PvQyFM,1098
 rkstreamer/views/song.py,sha256=WqzHuGx-2ZCa44hY6WaP307EbAt9DQgADFsw5OXXbkQ,2880
-rkstreamer-1.0.dist-info/LICENSE,sha256=MmUT1t65BLGKiCWJucbmyXsgD3avV1qj6hjg41ygHlw,1084
-rkstreamer-1.0.dist-info/METADATA,sha256=uaNTuAWzokFQ1z9utTv7tkp58gkZmEbTmhNHKcon_F8,3113
-rkstreamer-1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rkstreamer-1.0.dist-info/entry_points.txt,sha256=RJxRgxQdzmohlys89s33n5thlwgt8xoGhyEDIDq7Sjk,56
-rkstreamer-1.0.dist-info/top_level.txt,sha256=NOEjBv8uSvkjyrPbCE6Rn7jSxZeq33B7B7i2JjAGQQs,11
-rkstreamer-1.0.dist-info/RECORD,,
+rkstreamer-1.1.dist-info/LICENSE,sha256=MmUT1t65BLGKiCWJucbmyXsgD3avV1qj6hjg41ygHlw,1084
+rkstreamer-1.1.dist-info/METADATA,sha256=M1H_i-3o-EsDcoxBR38YAqg7SY431XyCm2EAKcjYVAc,3941
+rkstreamer-1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rkstreamer-1.1.dist-info/entry_points.txt,sha256=RJxRgxQdzmohlys89s33n5thlwgt8xoGhyEDIDq7Sjk,56
+rkstreamer-1.1.dist-info/top_level.txt,sha256=NOEjBv8uSvkjyrPbCE6Rn7jSxZeq33B7B7i2JjAGQQs,11
+rkstreamer-1.1.dist-info/RECORD,,
```

