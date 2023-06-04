# Comparing `tmp/mathbib-0.6.2.tar.gz` & `tmp/mathbib-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.6.2.tar", max compression
+gzip compressed data, was "mathbib-0.6.3.tar", max compression
```

## Comparing `mathbib-0.6.2.tar` & `mathbib-0.6.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.2/LICENSE
--rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.2/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.2/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.2/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.2/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.2/mathbib/citegen.py
--rw-r--r--   0        0        0    10051 2023-05-30 19:06:35.770568 mathbib-0.6.2/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.2/mathbib/partition.py
--rw-r--r--   0        0        0     9518 2023-06-03 19:53:05.633854 mathbib-0.6.2/mathbib/record.py
--rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.6.2/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.2/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.2/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.2/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.2/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.2/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.6.2/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.2/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.2/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6496 2023-06-04 06:34:59.401807 mathbib-0.6.2/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.2/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.6.2/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.6.2/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.2/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-06-04 06:34:49.241365 mathbib-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.6.3/LICENSE
+-rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.6.3/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.6.3/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.6.3/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.6.3/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.6.3/mathbib/citegen.py
+-rw-r--r--   0        0        0     9907 2023-06-04 06:38:05.985770 mathbib-0.6.3/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.6.3/mathbib/partition.py
+-rw-r--r--   0        0        0     9459 2023-06-04 06:39:11.761721 mathbib-0.6.3/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.6.3/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.6.3/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.6.3/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.6.3/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.6.3/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.6.3/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.6.3/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.6.3/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.6.3/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6435 2023-06-04 06:38:50.839466 mathbib-0.6.3/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.6.3/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.6.3/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.6.3/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.6.3/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-06-04 06:39:22.667000 mathbib-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.6.3/PKG-INFO
```

### Comparing `mathbib-0.6.2/LICENSE` & `mathbib-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/README.md` & `mathbib-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/bibtex.py` & `mathbib-0.6.3/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/citegen.py` & `mathbib-0.6.3/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/command.py` & `mathbib-0.6.3/mathbib/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -190,30 +190,28 @@
             raise click.ClickException("cannot add non-PDF record")
 
         if (
             not target.exists()
             or target.exists()
             and click.confirm("Overwrite existing file?")
         ):
-            target.parent.mkdir(exist_ok=True, parents=True)
             shutil.copyfile(source, target)
 
 
 @cli.command(name="edit", short_help="Edit local record.")
 @record_argument
 def edit_cmd(record: ArchiveRecord):
     """Edit local the record associated with KEY:ID."""
     toml_record = dumps(record.as_toml())
 
     while True:
         edited = click.edit(toml_record, extension=".toml")
         if edited is not None:
             try:
                 loads(edited)
-                record.keyid.toml_path().parent.mkdir(parents=True, exist_ok=True)
                 record.keyid.toml_path().write_text(edited)
                 return
 
             except TOMLDecodeError as e:
                 TermWrite.error(f"invalid TOML: {e}")
 
             if click.confirm("Edit again?"):
```

### Comparing `mathbib-0.6.2/mathbib/partition.py` & `mathbib-0.6.3/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/record.py` & `mathbib-0.6.3/mathbib/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,14 @@
                 return keyid.file_path()
         return None
 
     def download_file(self) -> Optional[Path]:
         for keyid in self.related_keys():
             download_url = get_remote_record(keyid).download_url
             path = keyid.file_path()
-            path.parent.mkdir(exist_ok=True, parents=True)
             if (
                 download_url is not None
                 and self.cli_session.remote_session.make_raw_streaming_request(
                     download_url(keyid.identifier), path
                 )
             ):
                 return path
```

### Comparing `mathbib-0.6.2/mathbib/remote/__init__.py` & `mathbib-0.6.3/mathbib/remote/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,52 +141,58 @@
 
     @classmethod
     def _from_str_no_check(cls, keyid_str: str) -> KeyId:
         tokens = keyid_str.split(":")
         return cls(RemoteKey[tokens[0].upper()], ":".join(tokens[1:]))
 
     def toml_path(self):
-        return (
+        ret = (
             xdg_data_home()
             / "mathbib"
             / "records"
             / str(self.key)
             / f"{self.identifier}.toml"
         )
+        ret.parent.mkdir(parents=True, exist_ok=True)
+        return ret
 
     def file_path(self, suffix: str = "pdf"):
-        return (
+        ret = (
             xdg_data_home()
             / "mathbib"
             / "files"
             / str(self.key)
             / f"{self.identifier}.{suffix}"
         )
+        ret.parent.mkdir(parents=True, exist_ok=True)
+        return ret
+
+    def cache_path(self):
+        ret = (
+            xdg_cache_home()
+            / "mathbib"
+            / "records"
+            / str(self.key)
+            / f"{self.identifier}.json"
+        )
+        ret.parent.mkdir(parents=True, exist_ok=True)
+        return ret
 
     def toml_record(self, warn: bool = False):
         try:
             return tomllib.loads(self.toml_path().read_text())
         except FileNotFoundError:
             return {}
         except tomllib.TOMLDecodeError as e:
             if warn:
                 TermWrite.warn(f"Invalid TOML in {self}: {e}")
                 return {}
             else:
                 raise e
 
-    def cache_path(self):
-        return (
-            xdg_cache_home()
-            / "mathbib"
-            / "records"
-            / str(self.key)
-            / f"{self.identifier}.json"
-        )
-
     def __str__(self):
         return f"{self.key}:{self.identifier}"
 
     def __repr__(self):
         return f"{self.key}:{self.identifier}"
```

### Comparing `mathbib-0.6.2/mathbib/remote/arxiv.py` & `mathbib-0.6.3/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/doi.py` & `mathbib-0.6.3/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/error.py` & `mathbib-0.6.3/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/isbn.py` & `mathbib-0.6.3/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/ol.py` & `mathbib-0.6.3/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/utils.py` & `mathbib-0.6.3/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/zbl.py` & `mathbib-0.6.3/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/remote/zbmath.py` & `mathbib-0.6.3/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/request.py` & `mathbib-0.6.3/mathbib/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,14 @@
         self,
         keyid: KeyId,
         record: Optional[dict],
         related: list[tuple[str, str]],
     ) -> None:
         if self.cache:
             target = keyid.cache_path()
-            target.parent.mkdir(parents=True, exist_ok=True)
             cache_object = {
                 "record": record,
                 "accessed": datetime.now().isoformat(),
                 "related": related,
             }
             target.write_text(json.dumps(cache_object))
```

### Comparing `mathbib-0.6.2/mathbib/resources/journal_abbrevs.json` & `mathbib-0.6.3/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/session.py` & `mathbib-0.6.3/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/mathbib/term.py` & `mathbib-0.6.3/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.6.2/pyproject.toml` & `mathbib-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.6.2"
+version = "0.6.3"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.6.2/PKG-INFO` & `mathbib-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.6.2
+Version: 0.6.3
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

