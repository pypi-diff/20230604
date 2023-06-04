# Comparing `tmp/rofify-0.0.4-py3-none-any.whl.zip` & `tmp/rofify-0.0.40-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 24706 bytes, number of entries: 25
+Zip file size: 24717 bytes, number of entries: 25
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 20:31 rofify/__init__.py
 -rw-r--r--  2.0 unx     1345 b- defN 23-Jun-04 00:51 rofify/__main__.py
 -rw-r--r--  2.0 unx     1228 b- defN 23-Jun-03 20:31 rofify/src/AlbumMenu.py
 -rw-r--r--  2.0 unx     3235 b- defN 23-Jun-03 20:31 rofify/src/ArtistMenu.py
 -rw-r--r--  2.0 unx      746 b- defN 23-Jun-03 20:31 rofify/src/DeviceControls.py
 -rw-r--r--  2.0 unx     2562 b- defN 23-Jun-03 22:52 rofify/src/DeviceMenu.py
 -rw-r--r--  2.0 unx     2764 b- defN 23-Jun-03 20:31 rofify/src/DynamicNestedMenu.py
@@ -15,13 +15,13 @@
 -rw-r--r--  2.0 unx     1325 b- defN 23-Jun-03 22:43 rofify/src/SavedTracksMenu.py
 -rw-r--r--  2.0 unx     5701 b- defN 23-Jun-03 20:31 rofify/src/SearchMenu.py
 -rw-r--r--  2.0 unx     5297 b- defN 23-Jun-03 20:31 rofify/src/SpotifyAPI.py
 -rw-r--r--  2.0 unx     6519 b- defN 23-Jun-03 22:41 rofify/src/TrackMenu.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-03 21:16 rofify/src/__init__.py
 -rw-r--r--  2.0 unx    13061 b- defN 23-Jun-03 20:31 rofify/src/config.py
 -rw-r--r--  2.0 unx      983 b- defN 23-Jun-03 20:31 rofify/src/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jun-04 01:09 rofify-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2953 b- defN 23-Jun-04 01:09 rofify-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 01:09 rofify-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-04 01:09 rofify-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2000 b- defN 23-Jun-04 01:09 rofify-0.0.4.dist-info/RECORD
-25 files, 67611 bytes uncompressed, 21500 bytes compressed:  68.2%
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-04 01:13 rofify-0.0.40.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2954 b- defN 23-Jun-04 01:13 rofify-0.0.40.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 01:13 rofify-0.0.40.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-04 01:13 rofify-0.0.40.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2005 b- defN 23-Jun-04 01:13 rofify-0.0.40.dist-info/RECORD
+25 files, 67617 bytes uncompressed, 21501 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: rofify/src/config.py
 Comment: 
 
 Filename: rofify/src/utils.py
 Comment: 
 
-Filename: rofify-0.0.4.dist-info/LICENSE.txt
+Filename: rofify-0.0.40.dist-info/LICENSE.txt
 Comment: 
 
-Filename: rofify-0.0.4.dist-info/METADATA
+Filename: rofify-0.0.40.dist-info/METADATA
 Comment: 
 
-Filename: rofify-0.0.4.dist-info/WHEEL
+Filename: rofify-0.0.40.dist-info/WHEEL
 Comment: 
 
-Filename: rofify-0.0.4.dist-info/top_level.txt
+Filename: rofify-0.0.40.dist-info/top_level.txt
 Comment: 
 
-Filename: rofify-0.0.4.dist-info/RECORD
+Filename: rofify-0.0.40.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `rofify-0.0.4.dist-info/LICENSE.txt` & `rofify-0.0.40.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `rofify-0.0.4.dist-info/METADATA` & `rofify-0.0.40.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rofify
-Version: 0.0.4
+Version: 0.0.40
 Summary: Rofi menu script that controls spotify playback.
 Home-page: https://github.com/dbkosky/rofify.git
 Author: Daniel Kosky
 Author-email: dbkosky@gmail.com
 License: MIT
 Keywords: spotify,rofi
 Classifier: Programming Language :: Python :: 3
```

## Comparing `rofify-0.0.4.dist-info/RECORD` & `rofify-0.0.40.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 rofify/src/SavedTracksMenu.py,sha256=t6G98NY7Qtbxg_kxsBOdqu0Dr0tJG5CWRU82HwQgIus,1325
 rofify/src/SearchMenu.py,sha256=vqsW_lnmVRUT7tDLoU5KCRR9beNuJRQwfYriqi2GmbQ,5701
 rofify/src/SpotifyAPI.py,sha256=3hCys_N4O2QPjIb7fIjpNCH8Xa0Lch1U6mUam23tqTs,5297
 rofify/src/TrackMenu.py,sha256=ROIUJ0fe7hpjTf6A6BIpnqrFGiGfR-5GOZMSSHrUwu0,6519
 rofify/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 rofify/src/config.py,sha256=1Fkor7oBnc2aZ6EoD_b1yoZpfYkUfTS0su81pXMOLdU,13061
 rofify/src/utils.py,sha256=HShHsMDRWIby3tfCx2-_oMRYqeELyiaJR7J2NXLOlog,983
-rofify-0.0.4.dist-info/LICENSE.txt,sha256=vlWaEdN2U-3Q6Fx5i8MJAksklim5dYhNoC2oq6lje0o,1069
-rofify-0.0.4.dist-info/METADATA,sha256=RPVP80n5nE0GHq4Bi2rfBITYxEKdq8e_Z5yOqIzZF68,2953
-rofify-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rofify-0.0.4.dist-info/top_level.txt,sha256=ExUSoT-G5t_yS0xZjEvFe0iQer0AXneb6h7HhwjMQQ4,7
-rofify-0.0.4.dist-info/RECORD,,
+rofify-0.0.40.dist-info/LICENSE.txt,sha256=vlWaEdN2U-3Q6Fx5i8MJAksklim5dYhNoC2oq6lje0o,1069
+rofify-0.0.40.dist-info/METADATA,sha256=WvmUv23xEyEXaIKxod9-488VX2bSrODb9iNY5LoRBLk,2954
+rofify-0.0.40.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rofify-0.0.40.dist-info/top_level.txt,sha256=ExUSoT-G5t_yS0xZjEvFe0iQer0AXneb6h7HhwjMQQ4,7
+rofify-0.0.40.dist-info/RECORD,,
```

