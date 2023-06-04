# Comparing `tmp/ventus-0.3.2.tar.gz` & `tmp/ventus-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ventus-0.3.2.tar", last modified: Wed Oct 19 21:45:51 2022, max compression
+gzip compressed data, was "ventus-0.3.4.tar", last modified: Sun Jun  4 20:43:17 2023, max compression
```

## Comparing `ventus-0.3.2.tar` & `ventus-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-10-19 21:45:51.691154 ventus-0.3.2/
--rw-rw-rw-   0        0        0    35823 2022-04-18 11:10:12.000000 ventus-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     3118 2022-10-19 21:45:51.691154 ventus-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2112 2022-10-19 21:06:54.000000 ventus-0.3.2/README.md
--rw-rw-rw-   0        0        0       42 2022-10-19 21:45:51.692155 ventus-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1970 2022-10-19 21:45:43.000000 ventus-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-19 21:45:51.685153 ventus-0.3.2/ventus/
--rw-rw-rw-   0        0        0      267 2022-10-19 18:07:31.000000 ventus-0.3.2/ventus/__init__.py
--rw-rw-rw-   0        0        0     1400 2022-10-19 21:44:37.000000 ventus-0.3.2/ventus/cli.py
--rw-rw-rw-   0        0        0      217 2022-04-19 20:23:49.000000 ventus-0.3.2/ventus/engine.py
--rw-rw-rw-   0        0        0     1933 2022-10-19 18:57:18.000000 ventus-0.3.2/ventus/extension.py
--rw-rw-rw-   0        0        0     1876 2022-04-19 20:22:04.000000 ventus-0.3.2/ventus/filters.py
--rw-rw-rw-   0        0        0      173 2022-04-19 20:24:10.000000 ventus-0.3.2/ventus/index.py
--rw-rw-rw-   0        0        0     8559 2022-09-20 17:28:40.000000 ventus-0.3.2/ventus/query.py
--rw-rw-rw-   0        0        0     1505 2022-09-20 17:26:15.000000 ventus-0.3.2/ventus/searcher.py
--rw-rw-rw-   0        0        0      817 2022-10-19 18:17:52.000000 ventus-0.3.2/ventus/sites.py
--rw-rw-rw-   0        0        0     1461 2022-10-19 21:00:27.000000 ventus-0.3.2/ventus/wrapper.py
-drwxrwxrwx   0        0        0        0 2022-10-19 21:45:51.690154 ventus-0.3.2/ventus.egg-info/
--rw-rw-rw-   0        0        0     3118 2022-10-19 21:45:51.000000 ventus-0.3.2/ventus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2022-10-19 21:45:51.000000 ventus-0.3.2/ventus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-19 21:45:51.000000 ventus-0.3.2/ventus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2022-10-19 21:45:51.000000 ventus-0.3.2/ventus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2022-10-19 21:45:51.000000 ventus-0.3.2/ventus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-19 21:45:51.000000 ventus-0.3.2/ventus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 20:43:17.063202 ventus-0.3.4/
+-rw-rw-rw-   0        0        0    35823 2023-06-04 19:17:55.000000 ventus-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     3172 2023-06-04 20:43:17.062202 ventus-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2207 2023-06-04 20:29:15.000000 ventus-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 20:43:17.063202 ventus-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1970 2023-06-04 20:27:25.000000 ventus-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:43:17.053201 ventus-0.3.4/ventus/
+-rw-rw-rw-   0        0        0      152 2023-06-04 20:21:54.000000 ventus-0.3.4/ventus/__init__.py
+-rw-rw-rw-   0        0        0     1834 2023-06-04 20:21:34.000000 ventus-0.3.4/ventus/cli.py
+-rw-rw-rw-   0        0        0     1933 2023-06-04 20:21:43.000000 ventus-0.3.4/ventus/extension.py
+-rw-rw-rw-   0        0        0     1876 2023-06-04 19:17:55.000000 ventus-0.3.4/ventus/filters.py
+-rw-rw-rw-   0        0        0     8559 2023-06-04 19:17:55.000000 ventus-0.3.4/ventus/query.py
+-rw-rw-rw-   0        0        0     1478 2023-06-04 20:32:43.000000 ventus-0.3.4/ventus/searcher.py
+-rw-rw-rw-   0        0        0      787 2023-06-04 20:15:34.000000 ventus-0.3.4/ventus/sites.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:43:17.061210 ventus-0.3.4/ventus.egg-info/
+-rw-rw-rw-   0        0        0     3172 2023-06-04 20:43:16.000000 ventus-0.3.4/ventus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-04 20:43:16.000000 ventus-0.3.4/ventus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 20:43:16.000000 ventus-0.3.4/ventus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 20:43:16.000000 ventus-0.3.4/ventus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-04 20:43:16.000000 ventus-0.3.4/ventus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-04 20:43:16.000000 ventus-0.3.4/ventus.egg-info/top_level.txt
```

### Comparing `ventus-0.3.2/LICENSE` & `ventus-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ventus-0.3.2/PKG-INFO` & `ventus-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ventus
-Version: 0.3.2
+Version: 0.3.4
 Summary: A google dorking library and cli.
 Home-page: https://github.com/aaronlyy/ventus
 Author: aaronlyy (Aaron Levi)
 Author-email: <aaronlevican@gmail.com>
-License: UNKNOWN
 Keywords: dorking,google,scraping,google dorking,hacking,cracking
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,15 +18,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-
 <p align="center">
   <img src=".\media\banner.png" alt="banner">
 </p>
 
 <h3 align="center">A Google Dorking library & Command-Line Interface ðŸ‘¾</h3>
 
 <p align="center">
@@ -45,17 +42,17 @@
 
 ## Usage (command-line interface)
 
 ```txt
 Usage: ventus [OPTIONS] QUERY
 
 Options:
-  --help                Show this message and exit.
-  -l, --leak            Search leaked images and pictures
-  -p, --presentation    Search for PDF & PPTX files
+  --help                Show this message and exit
+  -p, --paste           Search paste sites
+  -f, --files           Search filesharing sites
   -i, --index           Search index of /
   -d, --document        Search for DOCX files
 ```
 
 ## Usage (library)
 
 ### Example 1: Search a string
@@ -66,27 +63,29 @@
 results = search("test")
 
 for r in results:
     print(r)
 ```
 
 ### Example 2: Search a raw dork query
+
 ```py
 from ventus import search
 
 results = search("site:wikipedia.com mercedes")
 
 for r in results:
     print(r)
 
 for r in results:
     print(r)
 ```
 
 ### Example 3: Build and search a query using the query builder
+
 ```py
 from ventus import search, Query
 
 q = Query()
 q.site("finance.yahoo.com")
 q.intitle("AMD")
 
@@ -113,18 +112,18 @@
 # search query
 results = search(q)
 
 for r in results:
     print(r)
 ```
 
-## To Do
+## Roadmap
 
-- Add support for proxy lists
-- Add option to choose number of links to return
-- Add more Examples and Documentation
+- Move search wrapper directly into cli.py [DONE]
+- Option to choose number of links to return
+- Recode parts of the query builder
+- More pre configured searches in CLI
+- Option to use custom queries directly in the terminal
 
 ### About
 
 Made with â™¥ by [aaronlyy](https://github.com/aaronlyy)
-
-
```

### Comparing `ventus-0.3.2/README.md` & `ventus-0.3.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-
 <p align="center">
   <img src=".\media\banner.png" alt="banner">
 </p>
 
 <h3 align="center">A Google Dorking library & Command-Line Interface 👾</h3>
 
 <p align="center">
@@ -20,17 +19,17 @@
 
 ## Usage (command-line interface)
 
 ```txt
 Usage: ventus [OPTIONS] QUERY
 
 Options:
-  --help                Show this message and exit.
-  -l, --leak            Search leaked images and pictures
-  -p, --presentation    Search for PDF & PPTX files
+  --help                Show this message and exit
+  -p, --paste           Search paste sites
+  -f, --files           Search filesharing sites
   -i, --index           Search index of /
   -d, --document        Search for DOCX files
 ```
 
 ## Usage (library)
 
 ### Example 1: Search a string
@@ -41,27 +40,29 @@
 results = search("test")
 
 for r in results:
     print(r)
 ```
 
 ### Example 2: Search a raw dork query
+
 ```py
 from ventus import search
 
 results = search("site:wikipedia.com mercedes")
 
 for r in results:
     print(r)
 
 for r in results:
     print(r)
 ```
 
 ### Example 3: Build and search a query using the query builder
+
 ```py
 from ventus import search, Query
 
 q = Query()
 q.site("finance.yahoo.com")
 q.intitle("AMD")
 
@@ -88,16 +89,18 @@
 # search query
 results = search(q)
 
 for r in results:
     print(r)
 ```
 
-## To Do
+## Roadmap
 
-- Add support for proxy lists
-- Add option to choose number of links to return
-- Add more Examples and Documentation
+- Move search wrapper directly into cli.py [DONE]
+- Option to choose number of links to return
+- Recode parts of the query builder
+- More pre configured searches in CLI
+- Option to use custom queries directly in the terminal
 
 ### About
 
 Made with ♥ by [aaronlyy](https://github.com/aaronlyy)
```

### Comparing `ventus-0.3.2/setup.py` & `ventus-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # --- read readme.md ---
 with open("README.md", "r") as f:
     readme = f.read()
 
 # --- setting up ---
 setup(
     name="ventus",
-    version='0.3.2',
+    version='0.3.4',
     author="aaronlyy (Aaron Levi)",
     author_email="<aaronlevican@gmail.com>",
     url="https://github.com/aaronlyy/ventus",
     description='A google dorking library and cli.',
     long_description_content_type="text/markdown",
     long_description=readme,
     packages=["ventus"],
```

### Comparing `ventus-0.3.2/ventus/extension.py` & `ventus-0.3.4/ventus/extension.py`

 * *Files identical despite different names*

### Comparing `ventus-0.3.2/ventus/filters.py` & `ventus-0.3.4/ventus/filters.py`

 * *Files identical despite different names*

### Comparing `ventus-0.3.2/ventus/query.py` & `ventus-0.3.4/ventus/query.py`

 * *Files identical despite different names*

### Comparing `ventus-0.3.2/ventus/searcher.py` & `ventus-0.3.4/ventus/searcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import requests
 from bs4 import BeautifulSoup
 
-from .engine import Engine
 from .query import Query
 
 class Searcher:
-    def __init__(self, engine: str = Engine.GOOGLECOM):
-        """
-        Args:
-            engine (str): query url from a searchengine (ex. Engine.GOOGLECOM)
-        """
-        self._engine = engine
+    def __init__(self):
+        self._engine = "https://google.com/search"
 
     def _request(self, query: str) -> str:
         headers = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/100.0.4896.127 Safari/537.36'
         }
         res = requests.get(self._engine,
         headers=headers,
@@ -45,8 +40,13 @@
         if type(query) == Query:
             query_string = query.query
         else:
             query_string = query
         
         html = self._request(query_string)
         links = self._parse(html)
-        return links
+        return links
+    
+def search(query: Query) -> list:
+    """Wrapper around searcher.search"""
+    s = Searcher()
+    return s.search(query)
```

### Comparing `ventus-0.3.2/ventus/sites.py` & `ventus-0.3.4/ventus/sites.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 class Site:
     """Collection of some useful sites for dorking"""
     # file sharing
     GOOGLEDRIVE = "drive.google.com"
     GOFILE = "gofile.io"
     ANONFILE = "anonfile.com"
     BAYFILES = "bayfiles.com"
-    # leak
     COOMER = "coomer.party"
     # pasting
     JUSTPASTE = "justpaste.it"
     FAMOUSPASTE = "famouspaste.com"
     PASTELINK = "pastelink.net"
     NULLBIN = "0bin.net"
     RENTRY = "rentry.co"
     PASTESITE = "pastesite.org"
     FREEPASTE = "freepaste.link"
     LEAKLINKS = "leaklinks.com"
     JUSTPASTE = "justpaste.it"
     PASTEBIN = "pastebin.com"
     # lists
-    LIST_FILESHARING = [GOOGLEDRIVE, GOFILE, ANONFILE, BAYFILES]
-    LIST_PASTING = [JUSTPASTE, FAMOUSPASTE, PASTELINK, NULLBIN, RENTRY, PASTESITE, FREEPASTE, LEAKLINKS, JUSTPASTE, PASTEBIN]
-    LIST_LEAK = [COOMER]
+    LIST_FILESHARING = [GOOGLEDRIVE, GOFILE, ANONFILE, BAYFILES, COOMER]
+    LIST_PASTING = [JUSTPASTE, FAMOUSPASTE, PASTELINK, NULLBIN, RENTRY, PASTESITE, FREEPASTE, LEAKLINKS, JUSTPASTE, PASTEBIN]
```

### Comparing `ventus-0.3.2/ventus.egg-info/PKG-INFO` & `ventus-0.3.4/ventus.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: ventus
-Version: 0.3.2
+Version: 0.3.4
 Summary: A google dorking library and cli.
 Home-page: https://github.com/aaronlyy/ventus
 Author: aaronlyy (Aaron Levi)
 Author-email: <aaronlevican@gmail.com>
-License: UNKNOWN
 Keywords: dorking,google,scraping,google dorking,hacking,cracking
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,15 +18,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-
 <p align="center">
   <img src=".\media\banner.png" alt="banner">
 </p>
 
 <h3 align="center">A Google Dorking library & Command-Line Interface ðŸ‘¾</h3>
 
 <p align="center">
@@ -45,17 +42,17 @@
 
 ## Usage (command-line interface)
 
 ```txt
 Usage: ventus [OPTIONS] QUERY
 
 Options:
-  --help                Show this message and exit.
-  -l, --leak            Search leaked images and pictures
-  -p, --presentation    Search for PDF & PPTX files
+  --help                Show this message and exit
+  -p, --paste           Search paste sites
+  -f, --files           Search filesharing sites
   -i, --index           Search index of /
   -d, --document        Search for DOCX files
 ```
 
 ## Usage (library)
 
 ### Example 1: Search a string
@@ -66,27 +63,29 @@
 results = search("test")
 
 for r in results:
     print(r)
 ```
 
 ### Example 2: Search a raw dork query
+
 ```py
 from ventus import search
 
 results = search("site:wikipedia.com mercedes")
 
 for r in results:
     print(r)
 
 for r in results:
     print(r)
 ```
 
 ### Example 3: Build and search a query using the query builder
+
 ```py
 from ventus import search, Query
 
 q = Query()
 q.site("finance.yahoo.com")
 q.intitle("AMD")
 
@@ -113,18 +112,18 @@
 # search query
 results = search(q)
 
 for r in results:
     print(r)
 ```
 
-## To Do
+## Roadmap
 
-- Add support for proxy lists
-- Add option to choose number of links to return
-- Add more Examples and Documentation
+- Move search wrapper directly into cli.py [DONE]
+- Option to choose number of links to return
+- Recode parts of the query builder
+- More pre configured searches in CLI
+- Option to use custom queries directly in the terminal
 
 ### About
 
 Made with â™¥ by [aaronlyy](https://github.com/aaronlyy)
-
-
```

