# Comparing `tmp/richspot-1.0.1.tar.gz` & `tmp/richspot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richspot-1.0.1.tar", last modified: Fri Apr 28 17:06:52 2023, max compression
+gzip compressed data, was "richspot-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `richspot-1.0.1.tar` & `richspot-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-04-09 12:26:55.492952 richspot-1.0.1/LICENSE
--rw-r--r--   0        0        0     2032 2023-04-28 16:56:40.314045 richspot-1.0.1/README.md
--rw-r--r--   0        0        0     1290 2023-04-28 17:03:40.874075 richspot-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4994 2023-04-28 17:04:03.860077 richspot-1.0.1/richspot.py
--rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 richspot-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 12:26:55.492952 richspot-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2032 2023-04-28 16:56:40.314045 richspot-1.0.2/README.md
+-rw-r--r--   0        0        0     1336 2023-06-04 15:20:31.976276 richspot-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5512 2023-06-04 15:16:16.006257 richspot-1.0.2/richspot.py
+-rw-r--r--   0        0        0     2970 1970-01-01 00:00:00.000000 richspot-1.0.2/PKG-INFO
```

### Comparing `richspot-1.0.1/LICENSE` & `richspot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `richspot-1.0.1/README.md` & `richspot-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `richspot-1.0.1/pyproject.toml` & `richspot-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "richspot"
 description = "ncspot discord rich presence"
-version = "1.0.1"
+version = "1.0.2"
 keywords = ["Spotify", "Spotify Rich Presence", "Rich Presence", "Ncspot", "Ncspot Rich Presence", "Discord", "Discord Rich Presence", "Spotify Connect"]
 authors = [
     { name = "Younes Ben El", email = "ybenel@duck.com" }
 ]
 dependencies = [
     "pypresence",
     "requests",
@@ -18,14 +18,15 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 Documentation = "https://github.com/m1ndo/RichSpot"
 Source = "https://github.com/m1ndo/RichSpot"
 
 [build-system]
@@ -41,9 +42,9 @@
 defineConstant = { DEBUG = true }
 venv = "venv"
 
 reportMissingImports = true
 # reportMissingTypeStubs = false
 reportGeneralTypeIssues = false
 
-pythonVersion = "3.10"
+pythonVersion = "3.11"
 pythonPlatform = "Linux"
```

### Comparing `richspot-1.0.1/richspot.py` & `richspot-1.0.2/richspot.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,64 +29,79 @@
         json.dump(data, filer)
 
 config = read_file(config_file)
 client_id = str(config['client_id'])
 user_token = config['user_token']
 RPC = Presence(client_id)
 RPC.connect()
-list_covers = []
 
 def image_asset(link, title):
     """ Upload / Delete Image to discord assets """
     assets_url = f'https://discord.com/api/v9/oauth2/applications/{client_id}/assets'
     headers = {
         'Content-Type': 'application/json',
         'Authorization': user_token,
     }
     assets = requests.get(assets_url, headers=headers)
     assets_list = json.loads(assets.content.decode())
+    cover_names = [asset['name'] for asset in assets_list]
     image_b64 = requests.get(link)
     image_b64 = base64.b64encode(image_b64.content).decode()
     remove_chars = ",.: '"
     img_title = title.translate(str.maketrans('', '', remove_chars)).lower()
     image_data = {
         'name': f"{img_title}",
         'image': f"data:image/png;base64,{image_b64}",
         'type': "1"
     }
+    to_delete = remove_dups(assets_list)
+    if to_delete:
+        for item in to_delete:
+            requests.delete(assets_url+f"/{item}", headers=headers)
     # delete eall assets
     # for asset in assets_list:
     #     requests.delete(assets_url+f"/{asset['id']}", headers=headers)
-    if len(assets_list) <= 300:
-        if not any(asset['name'] == img_title for asset in assets_list) and not any(img_title == img_c for img_c in list_covers):
-            list_covers.append(img_title)
-            upload_image = requests.post(assets_url, headers=headers, json=image_data)
-            # print(upload_image.content)
+    if len(assets_list) != 300:
+        if img_title not in cover_names:
+            requests.post(assets_url, headers=headers, json=image_data)
     else:
         last_assets = assets_list[-10:]
         for assets in last_assets:
             requests.delete(assets_url+f"/{assets['id']}", headers=headers)
-            image_asset(assets_url, title)
+        image_asset(link, title)
 
-def check_pod(url):
-    """Check if podcast cover image is repeatable."""
-    pod_data = read_file(pods_file)
-    ep_data = {url.split("/")[-1]: url}
+def remove_dups(assets: list) -> list:
+    """ Find and removes duplicates a FIX for older versions before >1.2 """
+    name_to_assets = {}
+    to_delete = []
+    for asset in assets:
+        name = asset['name']
+        if name in name_to_assets:
+            name_to_assets[name].append(asset)
+        else:
+            name_to_assets[name] = [asset]
+    for assets in name_to_assets.values():
+        if len(assets) > 1:
+            n1 = assets[0]['id']
+            for i, asset in enumerate(assets):
+                if i != 0 and asset['id'] != n1:
+                    to_delete.append(asset['id'])
+    return to_delete
+
+def check_url(url, pod_data, title=''):
+    """ Check if podcast/song cover image is already uploaded."""
+    if not title: title = url.split("/4")[-1]
     if not pod_data:
-        pod_data = {"purls": []}
-        pod_data['purls'].append(url)
-        pod_data.update(ep_data)
-        write_file(pods_file, pod_data)
-        image_asset(url, url.split("/4")[-1])
+            pod_data = {"purls": [url]}
+            image_asset(url, title)
     else:
         if url not in pod_data["purls"]:
             pod_data["purls"].append(url)
-            pod_data.update(ep_data)
-            write_file(pods_file, pod_data)
-            image_asset(url, url.split("/4")[-1])
+            image_asset(url, title)
+    write_file(pods_file, pod_data)
     return url.split('/')[-1]
 
 def getmusic():
     """ Connect to ncspot and get metadata and update rich presence """
     sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
     sock.connect(socket_file)
     while True:
@@ -96,35 +111,35 @@
             mode = list(song_info["mode"].keys())[0]
         except Exception:
             mode = song_info.get("mode", "Stopped")
         type_track = song_info['playable']['type']
         cover_url = song_info["playable"]["cover_url"]
         url = song_info["playable"]["uri"]
         duration = song_info["playable"]["duration"]
+        pod_data = read_file(pods_file)
         if type_track != "Episode":
             title = song_info["playable"]["title"]
             artists = song_info["playable"]["artists"]
             album = song_info["playable"]["album"]
             details = title
             state = f"By {artists[0]}\nAlbum: {album}"
             cover_img = title.replace(" ", "").lower()
-            image_asset(cover_url, title)
+            check_url(cover_url, pod_data, title=title)
         else:
             title = song_info['playable']['name']
             details = "Podcast"
             state = title
-            cover_img = check_pod(cover_url)
+            cover_img = check_url(cover_url, pod_data)
 
         if mode == "Playing":
             time_start = song_info["mode"]["Playing"]['secs_since_epoch']
             end_time = datetime.datetime.fromtimestamp(time_start)
             end_time += datetime.timedelta(milliseconds=duration)
             end_time = int(end_time.timestamp())
             RPC.update(details=details, state=state, start=time_start, end=end_time, join=url, large_image=cover_img, small_image=cover_img, large_text="Deez Nuts")
-
         else:
             RPC.update(details=details+" (Paused/Stopped)", state=state, join=url, large_image=cover_img, small_image=cover_img, large_text="Deez Nuts")
 
 def run():
     """ Run Continuously and don't stop """
     while True:
         try:
```

### Comparing `richspot-1.0.1/PKG-INFO` & `richspot-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: richspot
-Version: 1.0.1
+Version: 1.0.2
 Summary: ncspot discord rich presence
 Keywords: Spotify,Spotify Rich Presence,Rich Presence,Ncspot,Ncspot Rich Presence,Discord,Discord Rich Presence,Spotify Connect
 Author-email: Younes Ben El <ybenel@duck.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pypresence
 Requires-Dist: requests
 Requires-Dist: PyYaml
 Project-URL: Documentation, https://github.com/m1ndo/RichSpot
 Project-URL: Source, https://github.com/m1ndo/RichSpot
```

