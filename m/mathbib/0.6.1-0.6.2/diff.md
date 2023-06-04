# Comparing `tmp/mathbib-0.6.1.tar.gz` & `tmp/mathbib-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.6.1.tar", max compression
+gzip compressed data, was "mathbib-0.6.2.tar", max compression
```

## Comparing `mathbib-0.6.1.tar` & `mathbib-0.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.1/LICENSE
--rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.1/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.1/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.1/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.1/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.1/mathbib/citegen.py
--rw-r--r--   0        0        0    10051 2023-05-30 19:06:35.770568 mathbib-0.6.1/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.1/mathbib/partition.py
--rw-r--r--   0        0        0     9518 2023-06-03 19:53:05.633854 mathbib-0.6.1/mathbib/record.py
--rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.6.1/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.1/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.1/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.1/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.1/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.1/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4257 2023-05-28 15:10:12.248626 mathbib-0.6.1/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.1/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.1/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     5604 2023-06-03 19:50:07.002465 mathbib-0.6.1/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.1/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.6.1/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-05-30 19:29:22.770722 mathbib-0.6.1/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.1/mathbib/term.py
--rw-r--r--   0        0        0      917 2023-06-03 19:54:27.525920 mathbib-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.2/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.2/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.2/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.2/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.2/mathbib/citegen.py
+-rw-r--r--   0        0        0    10051 2023-05-30 19:06:35.770568 mathbib-0.6.2/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.2/mathbib/partition.py
+-rw-r--r--   0        0        0     9518 2023-06-03 19:53:05.633854 mathbib-0.6.2/mathbib/record.py
+-rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.6.2/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.2/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.2/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.2/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.2/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.2/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.6.2/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.2/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.2/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6496 2023-06-04 06:34:59.401807 mathbib-0.6.2/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.2/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.6.2/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.6.2/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.2/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-06-04 06:34:49.241365 mathbib-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.2/PKG-INFO
```

### Comparing `mathbib-0.6.1/LICENSE` & `mathbib-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/README.md` & `mathbib-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/bibtex.py` & `mathbib-0.6.2/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/citegen.py` & `mathbib-0.6.2/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/command.py` & `mathbib-0.6.2/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/partition.py` & `mathbib-0.6.2/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/record.py` & `mathbib-0.6.2/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/__init__.py` & `mathbib-0.6.2/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/arxiv.py` & `mathbib-0.6.2/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/doi.py` & `mathbib-0.6.2/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/error.py` & `mathbib-0.6.2/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/isbn.py` & `mathbib-0.6.2/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/ol.py` & `mathbib-0.6.2/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/utils.py` & `mathbib-0.6.2/mathbib/remote/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """In order to resolve, we need a RemoteSession instance in order to make
         the remote request, and also a source KeyId
         """
         if isinstance(self.related_identifier, str):
             return self.related_key, self.related_identifier
         else:
             url_builder, parser = self.related_identifier
-            response = session.make_request(source_key, url_builder)
+            response, _ = session.make_request(source_key, url_builder)
             if response is not None:
                 parsed = parser(response)
                 if parsed is not None:
                     return self.related_key, parsed
         return None
```

### Comparing `mathbib-0.6.1/mathbib/remote/zbl.py` & `mathbib-0.6.2/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/remote/zbmath.py` & `mathbib-0.6.2/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/request.py` & `mathbib-0.6.2/mathbib/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .term import TermWrite
 from .remote import get_remote_record
 
 
 class RemoteSession:
     def __init__(
         self,
-        timeout: float = 30,
+        timeout: float = 10,
         info: bool = True,
         cache: bool = True,
         remote: bool = True,
     ):
         self.session = requests.Session()
 
         try:
@@ -65,31 +65,32 @@
         except FileNotFoundError:
             pass
 
         return None
 
     def _load_remote_record(
         self, keyid: KeyId
-    ) -> tuple[Optional[dict], list[tuple[str, str]]]:
+    ) -> tuple[Optional[dict], bool, list[tuple[str, str]]]:
         """Load and parse the remote record."""
         remote_record = get_remote_record(keyid)
-        response = self.make_request(keyid, remote_record.build_url)
+        response, status = self.make_request(keyid, remote_record.build_url)
         if response is not None:
             record, related = get_remote_record(keyid).parse_record(response)
 
             # resolve the related records
             candidates = [rel.resolve(keyid, self) for rel in related]
 
             return (
                 record,
+                status,
                 [(str(keyid.key), keyid.identifier)]
                 + [rel for rel in candidates if rel is not None],
             )
 
-        return None, []
+        return None, status, []
 
     def load_record(self, keyid: KeyId) -> tuple[Optional[dict], list[tuple[str, str]]]:
         """Attempt to load the record associated with keyid and cache a list of
         related records. At this stage, the related records are not "final": they are
         resolved (so they are strings) but otherwise the related records may not actually
         be real records.
         """
@@ -99,16 +100,17 @@
             return None, []
 
         # load cached record
         cache = self._load_cached_record(keyid)
 
         # if no cache hit, get remote record and cache
         if cache is None:
-            record, related = self._load_remote_record(keyid)
-            self.serialize(keyid, record, related)
+            record, status, related = self._load_remote_record(keyid)
+            if status:
+                self.serialize(keyid, record, related)
             return record, related
 
         else:
             return cache
 
     def serialize(
         self,
@@ -122,26 +124,44 @@
             cache_object = {
                 "record": record,
                 "accessed": datetime.now().isoformat(),
                 "related": related,
             }
             target.write_text(json.dumps(cache_object))
 
-    def make_request(self, keyid: KeyId, build_url: URLBuilder) -> Optional[str]:
+    def make_request(
+        self, keyid: KeyId, build_url: URLBuilder
+    ) -> tuple[Optional[str], bool]:
         return self.make_raw_request(build_url(keyid.identifier))
 
-    def make_raw_request(self, url: str) -> Optional[str]:
+    def make_raw_request(self, url: str) -> tuple[Optional[str], bool]:
+        """Make a raw request at <url>, and return the success state.
+        The optional string is the text content of the response, and the
+        boolean indicates whether or not the request was made successfully.
+
+        - (None, False) indicates that no record was returned because of an error
+          such as timeout, or incorrect response code
+        - (None, True) indicates that no record was returned, but the record was
+          either missing or remote requests were disabled
+        """
         if self.remote:
             if self.print_info:
                 TermWrite.remote(url)
-            res = self.session.get(url, timeout=self.timeout)
+            try:
+                res = self.session.get(url, timeout=self.timeout)
+            except requests.Timeout:
+                return (None, False)
 
             if res.status_code == requests.codes.ok:
-                return res.text
-        return None
+                return (res.text, True)
+            elif res.status_code == requests.codes.not_found:
+                return (None, True)
+            else:
+                return (None, False)
+        return (None, True)
 
     def make_raw_streaming_request(self, url: str, target: Path) -> bool:
         """Attempt to download the file, and return a boolean indicating success."""
         if self.remote:
             TermWrite.download(url)
             res = self.session.get(url, stream=True, timeout=self.timeout)
```

### Comparing `mathbib-0.6.1/mathbib/resources/journal_abbrevs.json` & `mathbib-0.6.2/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/session.py` & `mathbib-0.6.2/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/mathbib/term.py` & `mathbib-0.6.2/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.1/pyproject.toml` & `mathbib-0.6.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[virtualenv]
+in-project = true
+
 [tool.poetry]
 name = "mathbib"
-version = "0.6.1"
+version = "0.6.2"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
@@ -25,15 +28,15 @@
 lxml = "^4.9.2"
 python-stdnum = "^1.18"
 requests = "^2.31.0"
 beautifulsoup4 = "^4.12.2"
 tomli-w = "^1.0.0"
 
 [tool.pyright]
-include = ["src"]
+include = ["mathbib"]
 exclude = [
     "**/__pycache__"
 ]
 ignore = []
 
 reportMissingImports = true
 reportMissingTypeStubs = false
```

### Comparing `mathbib-0.6.1/PKG-INFO` & `mathbib-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.6.1
+Version: 0.6.2
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

