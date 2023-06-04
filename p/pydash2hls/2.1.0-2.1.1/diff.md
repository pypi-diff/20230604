# Comparing `tmp/pydash2hls-2.1.0.tar.gz` & `tmp/pydash2hls-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydash2hls-2.1.0.tar", last modified: Sat Jun  3 14:17:31 2023, max compression
+gzip compressed data, was "pydash2hls-2.1.1.tar", last modified: Sun Jun  4 12:03:50 2023, max compression
```

## Comparing `pydash2hls-2.1.0.tar` & `pydash2hls-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 14:17:31.683598 pydash2hls-2.1.0/
--rw-rw-rw-   0        0        0    35823 2023-06-03 12:20:09.000000 pydash2hls-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     3127 2023-06-03 14:17:31.683598 pydash2hls-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2201 2023-06-03 13:52:07.000000 pydash2hls-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 14:17:31.667961 pydash2hls-2.1.0/pydash2hls/
--rw-rw-rw-   0        0        0       51 2023-06-03 13:15:40.000000 pydash2hls-2.1.0/pydash2hls/__init__.py
--rw-rw-rw-   0        0        0     7256 2023-06-03 13:14:55.000000 pydash2hls-2.1.0/pydash2hls/converter.py
--rw-rw-rw-   0        0        0      469 2023-06-03 13:17:40.000000 pydash2hls-2.1.0/pydash2hls/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-03 14:17:31.683598 pydash2hls-2.1.0/pydash2hls.egg-info/
--rw-rw-rw-   0        0        0     3127 2023-06-03 14:17:31.000000 pydash2hls-2.1.0/pydash2hls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-03 14:17:31.000000 pydash2hls-2.1.0/pydash2hls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 14:17:31.000000 pydash2hls-2.1.0/pydash2hls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-03 14:17:31.000000 pydash2hls-2.1.0/pydash2hls.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-03 14:17:31.000000 pydash2hls-2.1.0/pydash2hls.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 14:17:31.683598 pydash2hls-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1152 2023-06-03 13:50:46.000000 pydash2hls-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-06-03 12:20:09.000000 pydash2hls-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3128 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2202 2023-06-03 14:21:01.000000 pydash2hls-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 12:03:50.583502 pydash2hls-2.1.1/pydash2hls/
+-rw-rw-rw-   0        0        0       51 2023-06-04 12:00:32.000000 pydash2hls-2.1.1/pydash2hls/__init__.py
+-rw-rw-rw-   0        0        0     7234 2023-06-04 11:59:35.000000 pydash2hls-2.1.1/pydash2hls/converter.py
+-rw-rw-rw-   0        0        0      469 2023-06-03 13:17:40.000000 pydash2hls-2.1.1/pydash2hls/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/pydash2hls.egg-info/
+-rw-rw-rw-   0        0        0     3128 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-04 12:03:50.000000 pydash2hls-2.1.1/pydash2hls.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 12:03:50.599125 pydash2hls-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2023-06-04 12:00:32.000000 pydash2hls-2.1.1/setup.py
```

### Comparing `pydash2hls-2.1.0/LICENSE` & `pydash2hls-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydash2hls-2.1.0/PKG-INFO` & `pydash2hls-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyDash2HLS
 
 [![License](https://img.shields.io/github/license/hyugogirubato/PyDash2HLS)](https://github.com/hyugogirubato/PyDash2HLS/blob/master/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/releases)
-[![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls)
+[![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
 ## Installation
 
 You can install PyDash2HLS using pip:
```

### Comparing `pydash2hls-2.1.0/README.md` & `pydash2hls-2.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyDash2HLS
 
 [![License](https://img.shields.io/github/license/hyugogirubato/PyDash2HLS)](https://github.com/hyugogirubato/PyDash2HLS/blob/master/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/releases)
-[![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls)
+[![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
 ## Installation
 
 You can install PyDash2HLS using pip:
```

### Comparing `pydash2hls-2.1.0/pydash2hls/converter.py` & `pydash2hls-2.1.1/pydash2hls/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Converter:
 
     def __init__(self, mdp_srt: str, mdp_dict: dict, url: str = None):
         self.mdp_srt = mdp_srt
         self.mdp_dict = mdp_dict
         self.mdp_url = url
-        self.profile = self._manifest_profile()
+        self.profiles = self._manifest_profiles()
 
     @classmethod
     def from_remote(cls, url: str, **kwargs) -> Converter:
         r = requests.request(method=kwargs.get("method", "GET"), url=url, **kwargs)
         r.raise_for_status()
         mdp_srt = r.text
         try:
@@ -39,20 +39,20 @@
         return cls(mdp_srt, mdp_dict)
 
     @staticmethod
     def _get_key(adaptation: dict, representation: dict, key: str) -> str:
         return representation.get(key, adaptation.get(key, None))
 
     def _get_profile(self, profile_id: str) -> dict:
-        for profile in self.profile:
+        for profile in self.profiles:
             if profile["id"] == profile_id:
                 return profile
         raise InvalidProfile(f"Profile does not exist: {profile_id}")
 
-    def _manifest_profile(self) -> list:
+    def _manifest_profiles(self) -> list:
         source = None if self.mdp_url is None else "/".join(self.mdp_url.split("/")[:-1])
         profiles = []
 
         for adaptation in self.mdp_dict["MPD"]["Period"]["AdaptationSet"]:
             drm = {}
             if "ContentProtection" in adaptation:
                 for protection in adaptation["ContentProtection"]:
@@ -65,16 +65,15 @@
 
                     for key, value in keys.items():
                         if value in protection:
                             drm[key] = protection[value]
 
             if isinstance(adaptation["Representation"], list):
                 for representation in adaptation["Representation"]:
-                    mime_type = self._get_key(adaptation, representation, "@mimeType") or (
-                        "video/mp4" if "avc" in representation["@codecs"] else "audio/m4a")
+                    mime_type = self._get_key(adaptation, representation, "@mimeType") or ("video/mp4" if "avc" in representation["@codecs"] else "audio/m4a")
                     start_with_sap = self._get_key(adaptation, representation, "@startWithSAP") or "1"
                     profile = {
                         "id": representation["@id"],
                         "mimeType": mime_type,
                         "codecs": representation["@codecs"],
                         "bandwidth": int(representation["@bandwidth"]),
                         "startWithSAP": start_with_sap
```

### Comparing `pydash2hls-2.1.0/pydash2hls.egg-info/PKG-INFO` & `pydash2hls-2.1.1/pydash2hls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydash2hls
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python library for converting DASH manifest files to HLS format.
 Home-page: https://github.com/hyugogirubato/pydash2hls
 Author: hyugogirubato
 Author-email: hyugogirubato@gmail.com
 License: GPL-3.0-only
 Keywords: manifest,hls,m3u8,dash
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyDash2HLS
 
 [![License](https://img.shields.io/github/license/hyugogirubato/PyDash2HLS)](https://github.com/hyugogirubato/PyDash2HLS/blob/master/LICENSE)
 [![Release](https://img.shields.io/github/release-date/hyugogirubato/pydash2hls)](https://github.com/hyugogirubato/pydash2hls/releases)
-[![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls)
+[![Latest Version](https://img.shields.io/pypi/v/pydash2hls)](https://pypi.org/project/pydash2hls/)
 
 PyDash2HLS is a Python library for converting DASH (Dynamic Adaptive Streaming over HTTP) manifest files to HLS (HTTP
 Live Streaming) format.
 
 ## Installation
 
 You can install PyDash2HLS using pip:
```

### Comparing `pydash2hls-2.1.0/setup.py` & `pydash2hls-2.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pydash2hls",
-    version="2.1.0",
+    version="2.1.1",
     author="hyugogirubato",
     author_email="hyugogirubato@gmail.com",
     description="Python library for converting DASH manifest files to HLS format.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/hyugogirubato/pydash2hls",
     packages=find_packages(),
```

