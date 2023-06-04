# Comparing `tmp/yomigana_ebook-0.2.0.tar.gz` & `tmp/yomigana_ebook-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yomigana_ebook-0.2.0.tar", max compression
+gzip compressed data, was "yomigana_ebook-0.2.1.tar", max compression
```

## Comparing `yomigana_ebook-0.2.0.tar` & `yomigana_ebook-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-23 10:39:32.761090 yomigana_ebook-0.2.0/LICENSE
--rw-r--r--   0        0        0      936 2023-05-23 11:31:59.671092 yomigana_ebook-0.2.0/README.md
--rw-r--r--   0        0        0      911 2023-06-02 19:14:13.958123 yomigana_ebook-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 09:51:06.753776 yomigana_ebook-0.2.0/yomigana_ebook/__init__.py
--rw-r--r--   0        0        0      920 2023-05-22 16:53:21.066068 yomigana_ebook-0.2.0/yomigana_ebook/checking.py
--rw-r--r--   0        0        0     1273 2023-06-02 15:29:31.668198 yomigana_ebook-0.2.0/yomigana_ebook/cli.py
--rw-r--r--   0        0        0      611 2023-05-06 19:16:41.232976 yomigana_ebook-0.2.0/yomigana_ebook/constants.py
--rw-r--r--   0        0        0      317 2023-04-26 17:24:19.377138 yomigana_ebook-0.2.0/yomigana_ebook/converter.py
--rw-r--r--   0        0        0     1794 2023-06-02 19:10:14.068109 yomigana_ebook-0.2.0/yomigana_ebook/process_ebook.py
--rw-r--r--   0        0        0        0 2023-05-26 13:17:15.396032 yomigana_ebook-0.2.0/yomigana_ebook/py.typed
--rw-r--r--   0        0        0     3133 2023-06-02 12:04:18.928182 yomigana_ebook-0.2.0/yomigana_ebook/yomituki.py
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 yomigana_ebook-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-23 10:39:32.761090 yomigana_ebook-0.2.1/LICENSE
+-rw-r--r--   0        0        0      940 2023-06-03 18:46:36.534280 yomigana_ebook-0.2.1/README.md
+-rw-r--r--   0        0        0      911 2023-06-04 11:08:42.925761 yomigana_ebook-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 09:51:06.753776 yomigana_ebook-0.2.1/yomigana_ebook/__init__.py
+-rw-r--r--   0        0        0      920 2023-05-22 16:53:21.066068 yomigana_ebook-0.2.1/yomigana_ebook/checking.py
+-rw-r--r--   0        0        0     1273 2023-06-04 11:00:53.585774 yomigana_ebook-0.2.1/yomigana_ebook/cli.py
+-rw-r--r--   0        0        0      611 2023-05-06 19:16:41.232976 yomigana_ebook-0.2.1/yomigana_ebook/constants.py
+-rw-r--r--   0        0        0      317 2023-04-26 17:24:19.377138 yomigana_ebook-0.2.1/yomigana_ebook/converter.py
+-rw-r--r--   0        0        0     1794 2023-06-03 18:46:36.564280 yomigana_ebook-0.2.1/yomigana_ebook/process_ebook.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:17:15.396032 yomigana_ebook-0.2.1/yomigana_ebook/py.typed
+-rw-r--r--   0        0        0     3455 2023-06-04 11:03:00.425772 yomigana_ebook-0.2.1/yomigana_ebook/yomituki.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 yomigana_ebook-0.2.1/PKG-INFO
```

### Comparing `yomigana_ebook-0.2.0/LICENSE` & `yomigana_ebook-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.0/README.md` & `yomigana_ebook-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # yomigana ebook
 
-This project is aimed at making Japanese eBooks more friendly to those who are learning Japanese by adding readings for every Kanji in the eBooks.
+This project is aimed at making Japanese eBooks more friendly to those who are learning Japanese now by adding readings for every Kanji in the eBooks.
 
 To achieve this, the project utilizes Mecab, a Japanese morphological analyzer, and Unidic, a dictionary developed by NICT, to tokenize words and obtain the corresponding yomigana (reading) of each word. This information is then inserted above or besides the kanji characters in the eBook text, allowing readers to easily read and understand the pronunciation of each word.
 
 ## Usage
 
 you can install the package via `pip`:
 
-`$ pip install yomigana_ebook`
+`$ pip install yomigana-ebook`
 
 then download the `unidic` dictionary:
 
 `$ python -m unidic download`
 
 now you can use it:
```

### Comparing `yomigana_ebook-0.2.0/pyproject.toml` & `yomigana_ebook-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yomigana-ebook"
-version = "0.2.0"
+version = "0.2.1"
 keywords = ["japanese", "lightnovel", "ebook", "epub", "furigana", "yomigana", "kanji", "mecab", "unidic"]
 description = "Make learning Japanese easier by adding readings for every kanji in the eBook"
 license = "MIT"
 authors = ["Yu Chen <rabbit19981023@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/rabbit19981023/yomigana-ebook"
 repository = "https://github.com/rabbit19981023/yomigana-ebook"
```

### Comparing `yomigana_ebook-0.2.0/yomigana_ebook/checking.py` & `yomigana_ebook-0.2.1/yomigana_ebook/checking.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.0/yomigana_ebook/cli.py` & `yomigana_ebook-0.2.1/yomigana_ebook/cli.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.0/yomigana_ebook/constants.py` & `yomigana_ebook-0.2.1/yomigana_ebook/constants.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.0/yomigana_ebook/process_ebook.py` & `yomigana_ebook-0.2.1/yomigana_ebook/process_ebook.py`

 * *Files identical despite different names*

### Comparing `yomigana_ebook-0.2.0/yomigana_ebook/yomituki.py` & `yomigana_ebook-0.2.1/yomigana_ebook/yomituki.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,31 +13,44 @@
 )
 
 
 tagger = Tagger()  # type: ignore
 
 
 def yomituki_sentence(sentence: str) -> Generator[str, None, None]:
-    for morpheme in tagger(sentence):  # type: ignore
+    # split sentence by whitespaces
+    sub_sentences = sentence.split(" ")
+
+    last_index = len(sub_sentences) - 1
+
+    # re-insert the whitespaces where they used to be
+    for i, sub_sentence in enumerate(sub_sentences):
+        yield from yomituki_text(sub_sentence)
+
+        if i < last_index:
+            yield " "
+
+
+def yomituki_text(text: str) -> Generator[str, None, None]:
+    for morpheme in tagger(text):  # type: ignore
         yield yomituki_word(morpheme.surface, morpheme.feature.kana)  # type: ignore
 
 
 def yomituki_word(surface: str, kata: str) -> str:
     if is_unknown(surface, kata):
         return surface
 
     if is_kana_only(surface):
         return surface
 
     if is_kanji_only(surface):
         return ruby_wrap(surface, kata2hira(kata))
 
     if is_latin_only(surface):
-        # add space for separating every latin word
-        return " " + surface
+        return surface
 
     # yomituki for:
     # hira + kanji: うれし涙
     # kanji + hira: 見上げて
     (prefix, (mid_text, mid_hira), suffix) = cut_by_hira(surface, kata2hira(kata))
     if is_kanji_only(mid_text):
         return f"{prefix}{ruby_wrap(mid_text, mid_hira)}{suffix}"
```

### Comparing `yomigana_ebook-0.2.0/PKG-INFO` & `yomigana_ebook-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yomigana-ebook
-Version: 0.2.0
+Version: 0.2.1
 Summary: Make learning Japanese easier by adding readings for every kanji in the eBook
 Home-page: https://github.com/rabbit19981023/yomigana-ebook
 License: MIT
 Keywords: japanese,lightnovel,ebook,epub,furigana,yomigana,kanji,mecab,unidic
 Author: Yu Chen
 Author-email: rabbit19981023@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -16,23 +16,23 @@
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: unidic (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/rabbit19981023/yomigana-ebook
 Description-Content-Type: text/markdown
 
 # yomigana ebook
 
-This project is aimed at making Japanese eBooks more friendly to those who are learning Japanese by adding readings for every Kanji in the eBooks.
+This project is aimed at making Japanese eBooks more friendly to those who are learning Japanese now by adding readings for every Kanji in the eBooks.
 
 To achieve this, the project utilizes Mecab, a Japanese morphological analyzer, and Unidic, a dictionary developed by NICT, to tokenize words and obtain the corresponding yomigana (reading) of each word. This information is then inserted above or besides the kanji characters in the eBook text, allowing readers to easily read and understand the pronunciation of each word.
 
 ## Usage
 
 you can install the package via `pip`:
 
-`$ pip install yomigana_ebook`
+`$ pip install yomigana-ebook`
 
 then download the `unidic` dictionary:
 
 `$ python -m unidic download`
 
 now you can use it:
```

