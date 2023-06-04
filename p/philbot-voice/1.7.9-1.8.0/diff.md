# Comparing `tmp/philbot_voice-1.7.9.tar.gz` & `tmp/philbot_voice-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "philbot_voice-1.7.9.tar", max compression
+gzip compressed data, was "philbot_voice-1.8.0.tar", max compression
```

## Comparing `philbot_voice-1.7.9.tar` & `philbot_voice-1.8.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       19 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/philbot-voice/__init__.py
--rw-r--r--   0        0        0       26 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/philbot-voice/__main__.py
--rw-r--r--   0        0        0    33936 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/philbot-voice/voice.py
--rw-r--r--   0        0        0      625 2023-06-04 12:04:14.733183 philbot_voice-1.7.9/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.7.9/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/philbot-voice/__init__.py
+-rw-r--r--   0        0        0       26 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/philbot-voice/__main__.py
+-rw-r--r--   0        0        0    33923 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/philbot-voice/voice.py
+-rw-r--r--   0        0        0      625 2023-06-04 14:34:10.447199 philbot_voice-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 philbot_voice-1.8.0/PKG-INFO
```

### Comparing `philbot_voice-1.7.9/philbot-voice/voice.py` & `philbot_voice-1.8.0/philbot-voice/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 )
 opentelemetry.trace.set_tracer_provider(tracer_provider)
 
 UDP_MAX_PAYLOAD = 65507
 HTTP_PORT = int(os.environ.get('HTTP_PORT', str(12345)))
 UDP_PORT_MIN = int(os.environ.get('UDP_PORT_MIN', str(12346)))
 UDP_PORT_MAX = int(os.environ.get('UDP_PORT_MAX', str(65535)))
+STORAGE_DIRECTORY = os.environ['STORAGE_DIRECTORY']
 
 meter = opentelemetry.metrics.get_meter_provider().get_meter('voice', '1.0.0')
 app = Flask(__name__)
 
 def time_seconds():
     return int(time.time())
 
@@ -90,15 +91,15 @@
 downloads = {}
 
 def download_from_youtube(guild_id, url):
     codec = 'wav'
     filename = url[url.index('v=') + 2:]
     if '&' in filename:
         filename = filename[:filename.index('&')]
-    filename = guild_id + '.' + filename
+    filename = STORAGE_DIRECTORY + '/' + guild_id + '.' + filename
     if os.path.exists(filename + '.' + codec):
         return filename + '.' + codec
     event = None
     download_in_progress = False
     with download_lock:
         download_in_progress = downloads.get(filename) and not downloads[filename].is_set()
         if not downloads.get(filename):
@@ -755,16 +756,16 @@
     if not request.headers.get('x-authorization'): return Response('Unauthorized', status=401)
     if request.headers['x-authorization'] != os.environ['DISCORD_API_TOKEN']: return Response('Forbidden', status=403)
     body = request.json
     context = get_context(body['guild_id'])
     return 'true' if context and context.is_connected() else 'false'
 
 def cleanup():
-    for file in os.listdir('.'):
-        if (file.endswith('.wav') or file.endswith('.aac') or file.endswith('.part') or file.endswith('.ytdl')) and os.path.getmtime(file) + 60 * 60 < time_seconds():
+    for file in os.listdir(STORAGE_DIRECTORY):
+        if os.path.getmtime(file) + 60 * 60 < time_seconds():
             try:
                 os.remove(file)
             except:
                 pass
 
 def cleanup_loop():
     while True:
```

### Comparing `philbot_voice-1.7.9/pyproject.toml` & `philbot_voice-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "philbot-voice"
-version = "1.7.9"
+version = "1.8.0"
 description = ""
 authors = ["philipp.lengauer <p.lengauer@gmail.com>"]
 packages = [{include = "philbot-voice"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `philbot_voice-1.7.9/PKG-INFO` & `philbot_voice-1.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: philbot-voice
-Version: 1.7.9
+Version: 1.8.0
 Summary: 
 Author: philipp.lengauer
 Author-email: p.lengauer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

