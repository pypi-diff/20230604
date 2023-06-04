# Comparing `tmp/ovos_stt_plugin_server-0.0.4a1-py3-none-any.whl.zip` & `tmp/ovos_stt_plugin_server-0.0.4a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9030 bytes, number of entries: 9
--rw-r--r--  2.0 unx     6096 b- defN 23-May-31 14:26 ovos_stt_plugin_server/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-May-31 14:26 ovos_stt_plugin_server/version.py
--rw-r--r--  2.0 unx    11343 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1654 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      278 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      868 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/RECORD
-9 files, 20532 bytes uncompressed, 7490 bytes compressed:  63.5%
+Zip file size: 9049 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jun-04 16:42 ovos_stt_plugin_server/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-04 16:42 ovos_stt_plugin_server/version.py
+-rw-r--r--  2.0 unx    11343 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1654 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      278 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      868 b- defN 23-Jun-04 16:43 ovos_stt_plugin_server-0.0.4a2.dist-info/RECORD
+9 files, 20584 bytes uncompressed, 7509 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_stt_plugin_server/__init__.py
 Comment: 
 
 Filename: ovos_stt_plugin_server/version.py
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/LICENSE
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/METADATA
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/METADATA
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/WHEEL
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/entry_points.txt
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/top_level.txt
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/zip-safe
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/RECORD
+Filename: ovos_stt_plugin_server-0.0.4a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_stt_plugin_server/__init__.py

```diff
@@ -5,15 +5,16 @@
 from ovos_utils.log import LOG
 from ovos_plugin_manager.stt import STT, StreamingSTT, StreamThread
 
 
 class OVOSHTTPServerSTT(STT):
     """STT interface for the OVOS-HTTP-STT-Server"""
     public_servers = [
-        "https://stt.openvoiceos.org/stt"
+        "https://stt.openvoiceos.org/stt",
+        "https://fasterwhisper.ziggyai.online/stt"
     ]
 
     def __init__(self, config=None):
         super().__init__(config)
         self.urls = self.config.get("url") or self.config.get("urls") or self.public_servers
         if not isinstance(self.urls, list):
             self.urls = [self.urls]
```

## ovos_stt_plugin_server/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 4
-VERSION_ALPHA = 1
+VERSION_ALPHA = 2
 # END_VERSION_BLOCK
```

## Comparing `ovos_stt_plugin_server-0.0.4a1.dist-info/LICENSE` & `ovos_stt_plugin_server-0.0.4a2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_stt_plugin_server-0.0.4a1.dist-info/METADATA` & `ovos_stt_plugin_server-0.0.4a2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-plugin-server
-Version: 0.0.4a1
+Version: 0.0.4a2
 Summary: ovos stt server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin stt
 Platform: UNKNOWN
```

