# Comparing `tmp/philbot_voice-1.8.0.tar.gz` & `tmp/philbot_voice-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.0.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.1.tar", max compression
```

## Comparing `philbot_voice-1.8.0.tar` & `philbot_voice-1.8.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33923 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33949 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-04 15:18:10.647516 philbot_voice-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.1/PKG-INFO
```

### Comparing `philbot_voice-1.8.0/philbot-voice/voice.py` & `philbot_voice-1.8.1/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -759,15 +759,15 @@
     context = get_context(body['guild_id'])
     return 'true' if context and context.is_connected() else 'false'
 
 def cleanup():
     for file in os.listdir(STORAGE_DIRECTORY):
         if os.path.getmtime(file) + 60 * 60 < time_seconds():
             try:
-                os.remove(file)
+                os.remove(STORAGE_DIRECTORY + '/' + file)
             except:
                 pass
 
 def cleanup_loop():
     while True:
         cleanup()
         time.sleep(60 * 60)
```

### Comparing `philbot_voice-1.8.0/pyproject.toml` & `philbot_voice-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.0"
+version = "1.8.1"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.0/PKG-INFO` & `philbot_voice-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.0
+Version: 1.8.1
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

