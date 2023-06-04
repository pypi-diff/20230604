# Comparing `tmp/yomigana_ebook-0.2.1.tar.gz` & `tmp/yomigana_ebook-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yomigana_ebook-0.2.1.tar", max compression
+gzip compressed data, was "yomigana_ebook-0.2.2.tar", max compression
```

## Comparing `yomigana_ebook-0.2.1.tar` & `yomigana_ebook-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-23 10:39:32.761090 yomigana_ebook-0.2.1/LICENSE
--rw-r--r--   0        0        0      940 2023-06-03 18:46:36.534280 yomigana_ebook-0.2.1/README.md
--rw-r--r--   0        0        0      911 2023-06-04 11:08:42.925761 yomigana_ebook-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 09:51:06.753776 yomigana_ebook-0.2.1/yomigana_ebook/__init__.py
--rw-r--r--   0        0        0      920 2023-05-22 16:53:21.066068 yomigana_ebook-0.2.1/yomigana_ebook/checking.py
--rw-r--r--   0        0        0     1273 2023-06-04 11:00:53.585774 yomigana_ebook-0.2.1/yomigana_ebook/cli.py
--rw-r--r--   0        0        0      611 2023-05-06 19:16:41.232976 yomigana_ebook-0.2.1/yomigana_ebook/constants.py
--rw-r--r--   0        0        0      317 2023-04-26 17:24:19.377138 yomigana_ebook-0.2.1/yomigana_ebook/converter.py
--rw-r--r--   0        0        0     1794 2023-06-03 18:46:36.564280 yomigana_ebook-0.2.1/yomigana_ebook/process_ebook.py
--rw-r--r--   0        0        0        0 2023-05-26 13:17:15.396032 yomigana_ebook-0.2.1/yomigana_ebook/py.typed
--rw-r--r--   0        0        0     3455 2023-06-04 11:03:00.425772 yomigana_ebook-0.2.1/yomigana_ebook/yomituki.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 yomigana_ebook-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-23 10:39:32.761090 yomigana_ebook-0.2.2/LICENSE
+-rw-r--r--   0        0        0      940 2023-06-04 12:35:32.515774 yomigana_ebook-0.2.2/README.md
+-rw-r--r--   0        0        0      918 2023-06-04 13:16:07.625776 yomigana_ebook-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 09:51:06.753776 yomigana_ebook-0.2.2/yomigana_ebook/__init__.py
+-rw-r--r--   0        0        0      920 2023-05-22 16:53:21.066068 yomigana_ebook-0.2.2/yomigana_ebook/checking.py
+-rw-r--r--   0        0        0     1273 2023-06-04 11:00:53.585774 yomigana_ebook-0.2.2/yomigana_ebook/cli.py
+-rw-r--r--   0        0        0      611 2023-05-06 19:16:41.232976 yomigana_ebook-0.2.2/yomigana_ebook/constants.py
+-rw-r--r--   0        0        0      317 2023-04-26 17:24:19.377138 yomigana_ebook-0.2.2/yomigana_ebook/converter.py
+-rw-r--r--   0        0        0     1772 2023-06-04 13:06:27.755786 yomigana_ebook-0.2.2/yomigana_ebook/process_ebook.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:17:15.396032 yomigana_ebook-0.2.2/yomigana_ebook/py.typed
+-rw-r--r--   0        0        0     3446 2023-06-04 12:35:32.515774 yomigana_ebook-0.2.2/yomigana_ebook/yomituki.py
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 yomigana_ebook-0.2.2/PKG-INFO
```

### Comparing `yomigana_ebook-0.2.1/LICENSE` & `yomigana_ebook-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.1/README.md` & `yomigana_ebook-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.1/pyproject.toml` & `yomigana_ebook-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "yomigana-ebook"
-version = "0.2.1"
-keywords = ["japanese", "lightnovel", "ebook", "epub", "furigana", "yomigana", "kanji", "mecab", "unidic"]
+version = "0.2.2"
+keywords = ["japanese", "lightnovel", "ebook", "epub", "furigana", "yomigana", "kanji", "mecab", "unidic", "nlp"]
 description = "Make learning Japanese easier by adding readings for every kanji in the eBook"
 license = "MIT"
 authors = ["Yu Chen <rabbit19981023@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/rabbit19981023/yomigana-ebook"
 repository = "https://github.com/rabbit19981023/yomigana-ebook"
```

### Comparing `yomigana_ebook-0.2.1/yomigana_ebook/checking.py` & `yomigana_ebook-0.2.2/yomigana_ebook/checking.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.1/yomigana_ebook/cli.py` & `yomigana_ebook-0.2.2/yomigana_ebook/cli.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.1/yomigana_ebook/constants.py` & `yomigana_ebook-0.2.2/yomigana_ebook/constants.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.1/yomigana_ebook/process_ebook.py` & `yomigana_ebook-0.2.2/yomigana_ebook/process_ebook.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from warnings import filterwarnings
 from typing import IO
 from zipfile import ZipFile, ZIP_DEFLATED
 from concurrent.futures import Future, ProcessPoolExecutor, as_completed
 
 from bs4 import BeautifulSoup, NavigableString, Tag, XMLParsedAsHTMLWarning
-from yomigana_ebook.yomituki import yomituki_sentence
+from yomigana_ebook.yomituki import yomituki
 
 
 filterwarnings("ignore", category=XMLParsedAsHTMLWarning, module="bs4")
 
 
 def process_ebook(reader: IO[bytes], writer: IO[bytes]):
     with (
@@ -43,16 +43,16 @@
     return file, soup.encode(formatter=None)  # type: ignore
 
 
 def process_tag(tag: Tag):
     if tag.name == "ruby":
         return
 
-    if isinstance(tag, NavigableString):
-        tag.replace_with("".join(yomituki_sentence(tag)))
+    if type(tag) is NavigableString:
+        tag.replace_with("".join(yomituki(tag)))
         return
 
     if hasattr(tag, "children"):
         for child in tag.children:
             process_tag(child)  # type: ignore
```

### Comparing `yomigana_ebook-0.2.1/yomigana_ebook/yomituki.py` & `yomigana_ebook-0.2.2/yomigana_ebook/yomituki.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     is_kanji,
 )
 
 
 tagger = Tagger()  # type: ignore
 
 
-def yomituki_sentence(sentence: str) -> Generator[str, None, None]:
+def yomituki(sentence: str) -> Generator[str, None, None]:
     # split sentence by whitespaces
     sub_sentences = sentence.split(" ")
 
     last_index = len(sub_sentences) - 1
 
     # re-insert the whitespaces where they used to be
     for i, sub_sentence in enumerate(sub_sentences):
```

### Comparing `yomigana_ebook-0.2.1/PKG-INFO` & `yomigana_ebook-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: yomigana-ebook
-Version: 0.2.1
+Version: 0.2.2
 Summary: Make learning Japanese easier by adding readings for every kanji in the eBook
 Home-page: https://github.com/rabbit19981023/yomigana-ebook
 License: MIT
-Keywords: japanese,lightnovel,ebook,epub,furigana,yomigana,kanji,mecab,unidic
+Keywords: japanese,lightnovel,ebook,epub,furigana,yomigana,kanji,mecab,unidic,nlp
 Author: Yu Chen
 Author-email: rabbit19981023@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
```

