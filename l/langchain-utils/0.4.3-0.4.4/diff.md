# Comparing `tmp/langchain_utils-0.4.3.tar.gz` & `tmp/langchain_utils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.4.3.tar", max compression
+gzip compressed data, was "langchain_utils-0.4.4.tar", max compression
```

## Comparing `langchain_utils-0.4.3.tar` & `langchain_utils-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    13101 2023-05-29 13:16:54.761092 langchain_utils-0.4.3/README.md
--rw-r--r--   0        0        0       22 2023-05-31 04:20:17.538384 langchain_utils-0.4.3/langchain_utils/__init__.py
--rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.3/langchain_utils/config.py
--rw-r--r--   0        0        0     4523 2023-05-31 04:07:36.378255 langchain_utils-0.4.3/langchain_utils/document_loaders.py
--rwxr-xr-x   0        0        0     2959 2023-05-31 04:06:21.103056 langchain_utils-0.4.3/langchain_utils/get_html_prompt.py
--rwxr-xr-x   0        0        0     4928 2023-05-31 04:18:55.050216 langchain_utils-0.4.3/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     3550 2023-05-31 04:11:22.760517 langchain_utils-0.4.3/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     3971 2023-05-31 04:11:27.982204 langchain_utils-0.4.3/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     3476 2023-04-17 03:23:31.837872 langchain_utils-0.4.3/langchain_utils/get_word_prompt.py
--rwxr-xr-x   0        0        0     2874 2023-05-23 10:30:00.649134 langchain_utils-0.4.3/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.3/langchain_utils/loaders.py
--rw-r--r--   0        0        0      509 2023-04-16 15:20:17.709721 langchain_utils-0.4.3/langchain_utils/prompts.py
--rw-r--r--   0        0        0    10699 2023-05-31 04:09:39.160287 langchain_utils-0.4.3/langchain_utils/utils.py
--rw-r--r--   0        0        0     2154 2023-04-16 15:19:45.633897 langchain_utils-0.4.3/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     3310 2023-05-31 04:08:37.439910 langchain_utils-0.4.3/langchain_utils/utils_doc_loaders.py
--rw-r--r--   0        0        0     1933 2023-05-31 04:20:17.535688 langchain_utils-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    14219 1970-01-01 00:00:00.000000 langchain_utils-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    13586 2023-06-04 03:25:32.738058 langchain_utils-0.4.4/README.md
+-rw-r--r--   0        0        0       22 2023-06-04 03:25:58.906110 langchain_utils-0.4.4/langchain_utils/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.4/langchain_utils/config.py
+-rw-r--r--   0        0        0     4523 2023-05-31 04:07:36.378255 langchain_utils-0.4.4/langchain_utils/document_loaders.py
+-rwxr-xr-x   0        0        0     2991 2023-06-04 03:25:10.362046 langchain_utils-0.4.4/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     4960 2023-06-04 03:25:10.439258 langchain_utils-0.4.4/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3582 2023-06-04 03:25:10.341545 langchain_utils-0.4.4/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     4003 2023-06-04 03:25:10.440421 langchain_utils-0.4.4/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     3508 2023-06-04 03:25:10.360593 langchain_utils-0.4.4/langchain_utils/get_word_prompt.py
+-rwxr-xr-x   0        0        0     2906 2023-06-04 03:25:10.338702 langchain_utils-0.4.4/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.4/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      537 2023-06-04 03:18:13.837836 langchain_utils-0.4.4/langchain_utils/prompts.py
+-rw-r--r--   0        0        0    10909 2023-06-04 03:24:20.155262 langchain_utils-0.4.4/langchain_utils/utils.py
+-rw-r--r--   0        0        0     2296 2023-06-04 03:25:12.243614 langchain_utils-0.4.4/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     3310 2023-05-31 04:08:37.439910 langchain_utils-0.4.4/langchain_utils/utils_doc_loaders.py
+-rw-r--r--   0        0        0     1933 2023-06-04 03:25:58.905306 langchain_utils-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    14704 1970-01-01 00:00:00.000000 langchain_utils-0.4.4/PKG-INFO
```

### Comparing `langchain_utils-0.4.3/README.md` & `langchain_utils-0.4.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,17 @@
 
 ### `urlprompt`
 
 ```
 $ urlprompt --help
 
 usage: urlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                 [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                 [-n] [-w WHAT] [-M] [-j] [-g] [--github-path GITHUB_PATH]
+                 [-P PARTS [PARTS ...]] [-r] [-R]
+                 [--print-percentage-non-ascii] [-n] [-w WHAT] [-M] [-j] [-g]
+                 [--github-path GITHUB_PATH]
                  [--github-revision GITHUB_REVISION]
                  URL
 
 Get a prompt consisting the text content of a webpage
 
 positional arguments:
   URL                   URL to the webpage
@@ -84,14 +85,15 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         webpage)
@@ -107,17 +109,17 @@
 ```
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
 usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                 [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                 [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
-                 [-o] [-L OCR_LANGUAGE]
+                 [-P PARTS [PARTS ...]] [-r] [-R]
+                 [--print-percentage-non-ascii] [-n] [-p PAGES [PAGES ...]]
+                 [-l PAGE_SLICE] [-M] [-w WHAT] [-o] [-L OCR_LANGUAGE]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -136,42 +138,44 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
   -l PAGE_SLICE, --page-slice PAGE_SLICE
                         Use Python slice syntax to select page numbers (e.g.
                         1:3, 1:10:2, etc.) (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a PDF
                         file)
-  -o, --fallback-ocr    Use OCR as fallback if no text detected on page
-                        (default: False)
+  -o, --fallback-ocr    Use OCR as fallback if no text detected on page,
+                        please set TESSDATA_PREFIX environment variable to the
+                        path of your tesseract data directory (default: False)
   -L OCR_LANGUAGE, --ocr-language OCR_LANGUAGE
                         Language to use for Tesseract OCR (default: chi_sim)
 
 ```
 ### `ytprompt`
 
 ```
 $ ytprompt --help
 
 usage: ytprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                [-n]
+                [-P PARTS [PARTS ...]] [-r] [-R]
+                [--print-percentage-non-ascii] [-n]
                 YouTube URL
 
 Get a prompt consisting Title and Transcript of a YouTube Video
 
 positional arguments:
   YouTube URL           YouTube URL
 
@@ -190,28 +194,29 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
 
 ```
 ### `textprompt`
 
 ```
 $ textprompt --help
 
 usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                  [-n] [-C] [-w WHAT] [-M]
+                  [-P PARTS [PARTS ...]] [-r] [-R]
+                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from text files
 
 positional arguments:
   PATH                  Paths to the text files, or stdin if not provided
                         (default: None)
@@ -231,14 +236,15 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
@@ -249,16 +255,16 @@
 ```
 ### `htmlprompt`
 
 ```
 $ htmlprompt --help
 
 usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                  [-n] [-C] [-w WHAT] [-M]
+                  [-P PARTS [PARTS ...]] [-r] [-R]
+                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from html files
 
 positional arguments:
   PATH                  Paths to the html files, or stdin if not provided
                         (default: None)
@@ -278,14 +284,15 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the text content of a
```

### Comparing `langchain_utils-0.4.3/langchain_utils/config.py` & `langchain_utils-0.4.4/langchain_utils/config.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.3/langchain_utils/document_loaders.py` & `langchain_utils-0.4.4/langchain_utils/document_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.3/langchain_utils/get_html_prompt.py` & `langchain_utils-0.4.4/langchain_utils/get_html_prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,13 +97,14 @@
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=html_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
+        raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.4.3/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.4.4/langchain_utils/get_pdf_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,13 +150,14 @@
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=pymupdf_doc_page_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
+        raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.4.3/langchain_utils/get_text_prompt.py` & `langchain_utils-0.4.4/langchain_utils/get_text_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,13 +110,14 @@
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
+        raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.4.3/langchain_utils/get_url_prompt.py` & `langchain_utils-0.4.4/langchain_utils/get_url_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,13 +121,14 @@
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
+        raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.4.3/langchain_utils/get_word_prompt.py` & `langchain_utils-0.4.4/langchain_utils/get_word_prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,13 +102,14 @@
         copy=args.copy,
         edit=args.edit,
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
+        raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.4.3/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.4.4/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,13 +81,14 @@
         should_be_only_one_doc=True,
         needs_splitting=needs_splitting,
         copy=args.copy,
         edit=args.edit,
         chunk_size=args.chunk_size,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
+        raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `langchain_utils-0.4.3/langchain_utils/loaders.py` & `langchain_utils-0.4.4/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.3/langchain_utils/utils.py` & `langchain_utils-0.4.4/langchain_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
 from typing import TYPE_CHECKING, Callable, NoReturn
 import sys
 from .prompts import (
+    RAW_TEMPLATE,
     RAW_TRIPLE_QUOTES_TEMPLATE,
     REPLY_OK_IF_YOU_READ_TEMPLATE,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST,
     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED,
 )
 
 
@@ -131,25 +132,28 @@
     copy: bool = True,
     edit: bool = False,
     chunk_size: int = 2000,
     extra_chunk_info_fn: Callable[['Document'], str] = lambda doc: '',
     dry_run: bool = False,
     parts: list[int] | None = None,
     raw_triple_quotes: bool = False,
+    raw: bool = False,
 ):
     from langchain.prompts import PromptTemplate
 
     def deliver_single_doc(document: 'Document'):
-        if raw_triple_quotes:
+        if raw:
+            template = RAW_TEMPLATE
+        elif raw_triple_quotes:
             template = RAW_TRIPLE_QUOTES_TEMPLATE
         else:
             template = REPLY_OK_IF_YOU_READ_TEMPLATE
         prompt = PromptTemplate.from_template(template)
         content = document.page_content
-        if raw_triple_quotes:
+        if raw or raw_triple_quotes:
             formatted_prompt = prompt.format(content=content)
         else:
             formatted_prompt = prompt.format(what=what, content=content)
 
         def edit_prompt(formatted_prompt: str = formatted_prompt):
             formatted_prompt_path = save_str_to_tempfile(
                 formatted_prompt, suffix='.txt'
@@ -181,27 +185,30 @@
         if len(documents) == 1:
             deliver_single_doc(documents[0])
             return
         if edit:
             print(f'Please copy the prompts after each edits.', file=sys.stderr)
         for i, doc in enumerate(documents):
             num_chunks = len(documents)
-            if raw_triple_quotes:
-                template = RAW_TRIPLE_QUOTES_TEMPLATE
+            if raw or raw_triple_quotes:
+                if raw:
+                    template = RAW_TEMPLATE
+                else:
+                    template = RAW_TRIPLE_QUOTES_TEMPLATE
                 prompt = PromptTemplate.from_template(template)
             elif i == 0:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_FIRST
                 )
             else:
                 prompt = PromptTemplate.from_template(
                     REPLY_OK_IF_YOU_READ_TEMPLATE_SPLITTED_CONTINUED
                 ).partial(x=str(i + 1))
             content = doc.page_content
-            if raw_triple_quotes:
+            if raw or raw_triple_quotes:
                 formatted_prompt = prompt.format(content=content)
             else:
                 formatted_prompt = prompt.format(what=what, content=content)
             if dry_run:
                 print(
                     f'Press Enter to copy prompt {i+1}/{num_chunks}. Word Count: {get_word_count(formatted_prompt)}, Char count: {len(formatted_prompt)}{extra_chunk_info_fn(doc)}: '
                 )
```

### Comparing `langchain_utils-0.4.3/langchain_utils/utils_argparse.py` & `langchain_utils-0.4.4/langchain_utils/utils_argparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,21 @@
         '-r',
         '--raw',
         help='Wraps the content in triple quotes with no extra text',
         action='store_true',
     )
 
     parser.add_argument(
+        '-R',
+        '--raw-no-quotes',
+        help='Output the content only',
+        action='store_true',
+    )
+
+    parser.add_argument(
         '--print-percentage-non-ascii',
         help='Print percentage of non-ascii characters',
         action='store_true',
     )
 
     parser.add_argument('-n', '--dry-run', help='Dry run', action='store_true')
     return parser
```

### Comparing `langchain_utils-0.4.3/langchain_utils/utils_doc_loaders.py` & `langchain_utils-0.4.4/langchain_utils/utils_doc_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.3/pyproject.toml` & `langchain_utils-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.4.3"
+version = "0.4.4"
 description = "Utilities built upon the langchain library"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.4.3/PKG-INFO` & `langchain_utils-0.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Utilities built upon the langchain library
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -83,16 +83,17 @@
 
 ### `urlprompt`
 
 ```
 $ urlprompt --help
 
 usage: urlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                 [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                 [-n] [-w WHAT] [-M] [-j] [-g] [--github-path GITHUB_PATH]
+                 [-P PARTS [PARTS ...]] [-r] [-R]
+                 [--print-percentage-non-ascii] [-n] [-w WHAT] [-M] [-j] [-g]
+                 [--github-path GITHUB_PATH]
                  [--github-revision GITHUB_REVISION]
                  URL
 
 Get a prompt consisting the text content of a webpage
 
 positional arguments:
   URL                   URL to the webpage
@@ -112,14 +113,15 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         webpage)
@@ -135,17 +137,17 @@
 ```
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
 usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                 [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                 [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
-                 [-o] [-L OCR_LANGUAGE]
+                 [-P PARTS [PARTS ...]] [-r] [-R]
+                 [--print-percentage-non-ascii] [-n] [-p PAGES [PAGES ...]]
+                 [-l PAGE_SLICE] [-M] [-w WHAT] [-o] [-L OCR_LANGUAGE]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -164,42 +166,44 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
   -l PAGE_SLICE, --page-slice PAGE_SLICE
                         Use Python slice syntax to select page numbers (e.g.
                         1:3, 1:10:2, etc.) (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a PDF
                         file)
-  -o, --fallback-ocr    Use OCR as fallback if no text detected on page
-                        (default: False)
+  -o, --fallback-ocr    Use OCR as fallback if no text detected on page,
+                        please set TESSDATA_PREFIX environment variable to the
+                        path of your tesseract data directory (default: False)
   -L OCR_LANGUAGE, --ocr-language OCR_LANGUAGE
                         Language to use for Tesseract OCR (default: chi_sim)
 
 ```
 ### `ytprompt`
 
 ```
 $ ytprompt --help
 
 usage: ytprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                [-n]
+                [-P PARTS [PARTS ...]] [-r] [-R]
+                [--print-percentage-non-ascii] [-n]
                 YouTube URL
 
 Get a prompt consisting Title and Transcript of a YouTube Video
 
 positional arguments:
   YouTube URL           YouTube URL
 
@@ -218,28 +222,29 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
 
 ```
 ### `textprompt`
 
 ```
 $ textprompt --help
 
 usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                  [-n] [-C] [-w WHAT] [-M]
+                  [-P PARTS [PARTS ...]] [-r] [-R]
+                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from text files
 
 positional arguments:
   PATH                  Paths to the text files, or stdin if not provided
                         (default: None)
@@ -259,14 +264,15 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
@@ -277,16 +283,16 @@
 ```
 ### `htmlprompt`
 
 ```
 $ htmlprompt --help
 
 usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
-                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
-                  [-n] [-C] [-w WHAT] [-M]
+                  [-P PARTS [PARTS ...]] [-r] [-R]
+                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from html files
 
 positional arguments:
   PATH                  Paths to the html files, or stdin if not provided
                         (default: None)
@@ -306,14 +312,15 @@
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
   -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
                         Parts to select in the processes list of Documents
                         (default: None)
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the text content of a
```

