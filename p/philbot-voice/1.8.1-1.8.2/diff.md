# Comparing `tmp/philbot_voice-1.8.1.tar.gz` & `tmp/philbot_voice-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.1.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.2.tar", max compression
```

## Comparing `philbot_voice-1.8.1.tar` & `philbot_voice-1.8.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33949 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33982 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.2/PKG-INFO
```

### Comparing `philbot_voice-1.8.1/philbot-voice/voice.py` & `philbot_voice-1.8.2/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,14 +564,15 @@
                 # fault must be in the code somewhere
                 # lets wait a bit to avoid busy loops and try again
                 self.__stop()
                 time.sleep(5)
                 self.__try_start()
             case _: # something else
                 self.__stop()
+                time.sleep(5)
                 self.__try_start()
     
     def __try_start(self):
         with self.lock:
             if self.ws or not self.channel_id or not self.session_id or not self.endpoint or not self.token or not self.url:
                 return
             print('VOICE GATEWAY ' + self.guild_id + ' connection starting')
@@ -619,17 +620,17 @@
         if not self.channel_id:
             self.__stop()
         with self.lock:
             self.channel_id = channel_id
             self.user_id = user_id
             self.session_id = session_id
             self.callback_url = callback_url
-            if not self.channel_id:
-                self.endpoint = None
-                self.token = None
+            #if not self.channel_id:
+            #    self.endpoint = None
+            #    self.token = None
         self.__save()
         self.__try_start()
 
     def on_content_update(self, url):
         with self.lock:
             self.url = url
             self.paused = False
```

### Comparing `philbot_voice-1.8.1/pyproject.toml` & `philbot_voice-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.1"
+version = "1.8.2"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.1/PKG-INFO` & `philbot_voice-1.8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.1
+Version: 1.8.2
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

