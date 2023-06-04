# Comparing `tmp/philbot_voice-1.8.2.tar.gz` & `tmp/philbot_voice-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.8.2.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.3.tar", max compression
```

## Comparing `philbot_voice-1.8.2.tar` & `philbot_voice-1.8.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33982 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-04 15:57:30.765341 philbot_voice-1.8.2/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-04 16:06:15.550122 philbot_voice-1.8.3/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-04 16:06:15.550122 philbot_voice-1.8.3/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    34008 2023-06-04 16:06:15.550122 philbot_voice-1.8.3/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-04 16:06:15.550122 philbot_voice-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.3/PKG-INFO
```

### Comparing `philbot_voice-1.8.2/philbot-voice/voice.py` & `philbot_voice-1.8.3/philbot-voice/voice.py`

 * *Files 0% similar despite different names*

```diff
@@ -758,15 +758,15 @@
     if request.headers['x-authorization'] != os.environ['DISCORD_API_TOKEN']: return Response('Forbidden', status=403)
     body = request.json
     context = get_context(body['guild_id'])
     return 'true' if context and context.is_connected() else 'false'
 
 def cleanup():
     for file in os.listdir(STORAGE_DIRECTORY):
-        if os.path.getmtime(file) + 60 * 60 < time_seconds():
+        if os.path.getmtime(STORAGE_DIRECTORY + '/' + file) + 60 * 60 < time_seconds():
             try:
                 os.remove(STORAGE_DIRECTORY + '/' + file)
             except:
                 pass
 
 def cleanup_loop():
     while True:
```

### Comparing `philbot_voice-1.8.2/pyproject.toml` & `philbot_voice-1.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.8.2"
+version = "1.8.3"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.8.2/PKG-INFO` & `philbot_voice-1.8.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.8.2
+Version: 1.8.3
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

