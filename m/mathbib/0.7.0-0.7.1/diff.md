# Comparing `tmp/mathbib-0.7.0.tar.gz` & `tmp/mathbib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.7.0.tar", max compression
+gzip compressed data, was "mathbib-0.7.1.tar", max compression
```

## Comparing `mathbib-0.7.0.tar` & `mathbib-0.7.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.0/LICENSE
--rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.0/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.0/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.0/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.0/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.7.0/mathbib/citegen.py
--rw-r--r--   0        0        0    10823 2023-06-04 07:21:28.332360 mathbib-0.7.0/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.0/mathbib/partition.py
--rw-r--r--   0        0        0     9441 2023-06-04 07:04:03.110810 mathbib-0.7.0/mathbib/record.py
--rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.0/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.0/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.0/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.0/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.0/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.0/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.0/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.0/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.0/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     6435 2023-06-04 06:38:50.839466 mathbib-0.7.0/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.0/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.0/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.0/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.0/mathbib/term.py
--rw-r--r--   0        0        0      953 2023-06-04 07:22:15.699317 mathbib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5341 2023-06-04 07:15:23.414124 mathbib-0.7.1/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.7.1/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.7.1/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.7.1/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.7.1/mathbib/citegen.py
+-rw-r--r--   0        0        0    10823 2023-06-04 07:21:28.332360 mathbib-0.7.1/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.7.1/mathbib/partition.py
+-rw-r--r--   0        0        0     9441 2023-06-04 07:04:03.110810 mathbib-0.7.1/mathbib/record.py
+-rw-r--r--   0        0        0     5697 2023-06-04 06:38:46.252732 mathbib-0.7.1/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.7.1/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.7.1/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.7.1/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.7.1/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.7.1/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4260 2023-06-04 06:31:57.308890 mathbib-0.7.1/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.7.1/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.7.1/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     6688 2023-06-04 07:25:26.040065 mathbib-0.7.1/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.7.1/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270281 2023-05-30 19:36:41.814752 mathbib-0.7.1/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2785 2023-06-03 20:06:26.993600 mathbib-0.7.1/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.7.1/mathbib/term.py
+-rw-r--r--   0        0        0      953 2023-06-04 07:25:49.098944 mathbib-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     6230 1970-01-01 00:00:00.000000 mathbib-0.7.1/PKG-INFO
```

### Comparing `mathbib-0.7.0/LICENSE` & `mathbib-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/README.md` & `mathbib-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/bibtex.py` & `mathbib-0.7.1/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/citegen.py` & `mathbib-0.7.1/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/command.py` & `mathbib-0.7.1/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/partition.py` & `mathbib-0.7.1/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/record.py` & `mathbib-0.7.1/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/__init__.py` & `mathbib-0.7.1/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/arxiv.py` & `mathbib-0.7.1/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/doi.py` & `mathbib-0.7.1/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/error.py` & `mathbib-0.7.1/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/isbn.py` & `mathbib-0.7.1/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/ol.py` & `mathbib-0.7.1/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/utils.py` & `mathbib-0.7.1/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/zbl.py` & `mathbib-0.7.1/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/remote/zbmath.py` & `mathbib-0.7.1/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/request.py` & `mathbib-0.7.1/mathbib/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,28 +144,33 @@
         """
         if self.remote:
             if self.print_info:
                 TermWrite.remote(url)
             try:
                 res = self.session.get(url, timeout=self.timeout)
             except requests.Timeout:
+                TermWrite.warn("could not access record (connection timeout)")
                 return (None, False)
 
             if res.status_code == requests.codes.ok:
                 return (res.text, True)
             elif res.status_code == requests.codes.not_found:
                 return (None, True)
             else:
+                TermWrite.warn(
+                    f"could not access record (server returned code {res.status_code})"
+                )
                 return (None, False)
         return (None, True)
 
     def make_raw_streaming_request(self, url: str, target: Path) -> bool:
         """Attempt to download the file, and return a boolean indicating success."""
         if self.remote:
-            TermWrite.download(url)
+            if self.print_info:
+                TermWrite.download(url)
             res = self.session.get(url, stream=True, timeout=self.timeout)
 
             # stream the download, and display a progress bar if isatty
             if res.status_code == requests.codes.ok:
                 target.parent.mkdir(exist_ok=True, parents=True)
                 chunk_size = 8192
                 length = res.headers.get("content-length")
```

### Comparing `mathbib-0.7.0/mathbib/resources/journal_abbrevs.json` & `mathbib-0.7.1/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/session.py` & `mathbib-0.7.1/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/mathbib/term.py` & `mathbib-0.7.1/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.7.0/pyproject.toml` & `mathbib-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [virtualenv]
 in-project = true
 
 [tool.poetry]
 name = "mathbib"
-version = "0.7.0"
+version = "0.7.1"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.7.0/PKG-INFO` & `mathbib-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.7.0
+Version: 0.7.1
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

