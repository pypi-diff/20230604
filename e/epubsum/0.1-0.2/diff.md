# Comparing `tmp/epubsum-0.1.tar.gz` & `tmp/epubsum-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubsum-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "epubsum-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `epubsum-0.1.tar` & `epubsum-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       72 2023-06-04 03:35:53.450919 epubsum-0.1/.gitignore
--rw-r--r--   0        0        0      344 2023-05-20 22:00:00.000000 epubsum-0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-06-04 03:37:00.100590 epubsum-0.1/LICENSE
--rw-r--r--   0        0        0      168 2023-06-04 03:34:28.673574 epubsum-0.1/README.md
--rw-r--r--   0        0        0      806 2023-06-04 03:26:00.000000 epubsum-0.1/epubsum/__init__.py
--rw-r--r--   0        0        0       69 2022-08-29 23:28:00.000000 epubsum-0.1/epubsum/__main__.py
--rw-r--r--   0        0        0     1262 2023-06-04 03:25:00.000000 epubsum-0.1/epubsum/epubsum.py
--rw-r--r--   0        0        0      745 2023-06-03 22:49:00.000000 epubsum-0.1/pyproject.toml
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 epubsum-0.1/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-06-04 03:35:53.450919 epubsum-0.2/.gitignore
+-rw-r--r--   0        0        0      344 2023-05-20 22:00:00.000000 epubsum-0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-06-04 03:37:00.100590 epubsum-0.2/LICENSE
+-rw-r--r--   0        0        0      382 2023-06-04 05:50:00.000000 epubsum-0.2/README.md
+-rw-r--r--   0        0        0     1113 2023-06-04 05:04:00.000000 epubsum-0.2/epubsum/__init__.py
+-rw-r--r--   0        0        0       69 2022-08-29 23:28:00.000000 epubsum-0.2/epubsum/__main__.py
+-rw-r--r--   0        0        0     2242 2023-06-04 05:58:00.000000 epubsum-0.2/epubsum/epubsum.py
+-rw-r--r--   0        0        0      745 2023-06-03 22:49:00.000000 epubsum-0.2/pyproject.toml
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 epubsum-0.2/PKG-INFO
```

### Comparing `epubsum-0.1/LICENSE` & `epubsum-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epubsum-0.1/epubsum/epubsum.py` & `epubsum-0.2/epubsum/epubsum.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,65 @@
 import os
 from bs4 import BeautifulSoup
 from cleantext import clean
 from ebooklib import ITEM_DOCUMENT, epub
 from textsum.summarize import Summarizer
+from textwrap import wrap
 
 
 def extract_sections_from_epub(epub_file_path):
     book = epub.read_epub(epub_file_path)
-    section_texts = []
+    section_texts = {}
 
     for item in book.get_items():
-        # Check if the item is an XHTML content file
-        if item.get_type() == ITEM_DOCUMENT and item.media_type == 'application/xhtml+xml':
+        if isinstance(item, epub.EpubHtml) and item.is_chapter():
+            title = item.title if item.title else item.get_name()
             content = item.get_content()
             soup = BeautifulSoup(content, 'html.parser')
             text = soup.get_text(separator=' ').strip()
             if text:
-                section_texts.append(text)
+                section_texts[title] = text
 
     return section_texts
 
 
-def summarize_book(bookfile, preamble='', large=False, verbose=False):
+def summarize_epub_file(summarizer, bookfile, preamble=''):
+    print(f'Summarizing {bookfile}\n')
+    parts = []
+    for name, text in extract_sections_from_epub(bookfile).items():
+        parts.append(f'\n\n=====[ {name} ]=====\n\n')
+        summary = summarizer.summarize_string(preamble + clean(text))
+        paragraphs = summary.split('\n')
+        summary = '\n\n'.join(['\n'.join(wrap(p)) for p in paragraphs])
+        parts.append(summary)
+
+    return ''.join(parts)
+
+
+def summarize_epub_files(summarizer, directory, preamble, overwrite):
+    for root, dirs, files in os.walk(directory):
+        for file in files:
+            if file.endswith('.epub'):
+                epub_path = os.path.join(root, file)
+                summary_path = os.path.splitext(epub_path)[0] + '-summary.txt'
+                if overwrite or not os.path.exists(summary_path):
+                    summary = summarize_epub_file(summarizer, epub_path, preamble)
+                    with open(summary_path, 'w') as summary_file:
+                        summary_file.write(summary)
+
+
+def summarize(target, preamble='', large=False, overwrite=False):
     if large:
         summarizer = Summarizer(model_name_or_path='pszemraj/long-t5-tglobal-xl-16384-book-summary')
     else:
         # pszemraj/long-t5-tglobal-base-16384-book-summary
         summarizer = Summarizer()
-    parts = []
-    for i, text in enumerate(extract_sections_from_epub(bookfile)):
-        parts.append(f'\n\n=====[ Section {i} ]=======================================\n\n')
-        parts.append(summarizer.summarize_string(preamble + clean(text)))
-
-    return ''.join(parts)
 
+    if os.path.isdir(target):
+        summarize_epub_files(summarizer, target, preamble, overwrite)
+    else:
+        print(summarize_epub_file(summarizer, target, preamble))
+
```

### Comparing `epubsum-0.1/pyproject.toml` & `epubsum-0.2/pyproject.toml`

 * *Files identical despite different names*

