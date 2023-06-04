# Comparing `tmp/philbot_voice-1.7.8.tar.gz` & `tmp/philbot_voice-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.8.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.9.tar", max compression
```

## Comparing `philbot_voice-1.7.8.tar` & `philbot_voice-1.7.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-04 11:48:38.590511 philbot_voice-1.7.8/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-04 11:48:38.590511 philbot_voice-1.7.8/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33892 2023-06-04 11:48:38.590511 philbot_voice-1.7.8/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-04 11:48:38.590511 philbot_voice-1.7.8/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33936 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.9/PKG-INFO
```

### Comparing `philbot_voice-1.7.8/philbot-voice/voice.py` & `philbot_voice-1.7.9/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -628,24 +628,26 @@
         self.__save()
         self.__try_start()
 
     def on_content_update(self, url):
         with self.lock:
             self.url = url
             self.paused = False
-        self.__try_start()
         self.__save()
+        self.__try_start()
 
     def pause(self):
         with self.lock:
             self.paused = True
+        self.__save()
 
     def resume(self):
         with self.lock:
             self.paused = False
+        self.__save()
     
     def is_connected(self):
         with self.lock:
             return self.ws is not None and self.listener is not None and self.streamer is not None
 
 contexts_lock = threading.Lock()
 contexts = {}
```

### Comparing `philbot_voice-1.7.8/pyproject.toml` & `philbot_voice-1.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.8"
+version = "1.7.9"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.8/PKG-INFO` & `philbot_voice-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.8
+Version: 1.7.9
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

