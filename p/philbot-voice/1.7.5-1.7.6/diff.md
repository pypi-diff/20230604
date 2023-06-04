# Comparing `tmp/philbot_voice-1.7.5.tar.gz` & `tmp/philbot_voice-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.5.tar", max compression
+gzip compressed data, was "philbot_voice-1.7.6.tar", max compression
```

## Comparing `philbot_voice-1.7.5.tar` & `philbot_voice-1.7.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33620 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-03 20:56:56.363682 philbot_voice-1.7.5/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.5/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-04 11:38:41.419161 philbot_voice-1.7.6/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-04 11:38:41.419161 philbot_voice-1.7.6/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33857 2023-06-04 11:38:41.419161 philbot_voice-1.7.6/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-04 11:38:41.419161 philbot_voice-1.7.6/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.6/PKG-INFO
```

### Comparing `philbot_voice-1.7.5/philbot-voice/voice.py` & `philbot_voice-1.7.6/philbot-voice/voice.py`

 * *Files 1% similar despite different names*

```diff
@@ -751,17 +751,29 @@
 def voice_is_connected():
     if not request.headers.get('x-authorization'): return Response('Unauthorized', status=401)
     if request.headers['x-authorization'] != os.environ['DISCORD_API_TOKEN']: return Response('Forbidden', status=403)
     body = request.json
     context = get_context(body['guild_id'])
     return 'true' if context and context.is_connected() else 'false'
 
+def cleanup():
+    for file in os.listdir('.'):
+        if (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part') or file.endswith('.ytdl')) and os.path.getmtime(file) + 60 * 60 < time_seconds():
+            try:
+                os.remove(file)
+            except:
+                pass
+
+def cleanup_loop():
+    while True:
+        cleanup()
+        time.sleep(60 * 60)
+
 def main():
     for file in os.listdir('.'):
         if file.startswith('.state.') and file.endswith('.json'):
             get_context(file[len('.state.'):len(file) - len('.json')])
-        elif (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part') or file.endswith('.ytdl')) and os.path.getmtime(file) + 60 * 60 * 24 < time_seconds():
-            os.remove(file)
+    threading.Thread(target=cleanup_loop).start()
     print('VOICE ready')
     # app.run(port=HTTP_PORT, ssl_context='adhoc', threaded=True)
     app.run(port=HTTP_PORT, threaded=True)
```

### Comparing `philbot_voice-1.7.5/pyproject.toml` & `philbot_voice-1.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.5"
+version = "1.7.6"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.5/PKG-INFO` & `philbot_voice-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.5
+Version: 1.7.6
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

