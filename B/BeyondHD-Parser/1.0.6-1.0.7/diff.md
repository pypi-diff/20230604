# Comparing `tmp/BeyondHD-Parser-1.0.6.tar.gz` & `tmp/BeyondHD-Parser-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyondHD-Parser-1.0.6.tar", last modified: Fri Dec 30 20:08:24 2022, max compression
+gzip compressed data, was "BeyondHD-Parser-1.0.7.tar", last modified: Sun Jun  4 16:57:27 2023, max compression
```

## Comparing `BeyondHD-Parser-1.0.6.tar` & `BeyondHD-Parser-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-12-30 20:08:24.163634 BeyondHD-Parser-1.0.6/
-drwxrwxrwx   0        0        0        0 2022-12-30 20:08:24.158633 BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/
--rw-rw-rw-   0        0        0     3636 2022-12-30 20:08:24.000000 BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2022-12-30 20:08:24.000000 BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-30 20:08:24.000000 BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-12-30 20:08:24.000000 BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2022-12-30 20:08:24.000000 BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2022-12-29 06:55:20.000000 BeyondHD-Parser-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3636 2022-12-30 20:08:24.163634 BeyondHD-Parser-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2022-12-30 20:07:45.000000 BeyondHD-Parser-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-30 20:08:24.160633 BeyondHD-Parser-1.0.6/beyondhd_parser/
--rw-rw-rw-   0        0        0        0 2022-12-30 16:19:16.000000 BeyondHD-Parser-1.0.6/beyondhd_parser/__init__.py
--rw-rw-rw-   0        0        0     5114 2022-12-30 03:33:26.000000 BeyondHD-Parser-1.0.6/beyondhd_parser/beyondhd_details.py
--rw-rw-rw-   0        0        0     5261 2022-12-30 20:07:45.000000 BeyondHD-Parser-1.0.6/beyondhd_parser/beyondhd_search.py
--rw-rw-rw-   0        0        0     3405 2022-12-29 08:12:07.000000 BeyondHD-Parser-1.0.6/beyondhd_parser/bhdstudio_nfo_parse.py
--rw-rw-rw-   0        0        0       42 2022-12-30 20:08:24.163634 BeyondHD-Parser-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1026 2022-12-30 20:03:10.000000 BeyondHD-Parser-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 16:57:27.210084 BeyondHD-Parser-1.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-04 16:57:27.204838 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/
+-rw-rw-rw-   0        0        0     4342 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4342 2023-06-04 16:57:27.208475 BeyondHD-Parser-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2919 2022-12-30 20:07:45.000000 BeyondHD-Parser-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 16:57:27.207920 BeyondHD-Parser-1.0.7/beyondhd_parser/
+-rw-rw-rw-   0        0        0        0 2022-12-30 16:19:16.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/__init__.py
+-rw-rw-rw-   0        0        0     5114 2023-01-14 05:35:33.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_details.py
+-rw-rw-rw-   0        0        0     6107 2023-06-04 16:54:50.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_search.py
+-rw-rw-rw-   0        0        0     3405 2022-12-29 08:12:07.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/bhdstudio_nfo_parse.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 16:57:27.210084 BeyondHD-Parser-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-06-04 16:57:08.000000 BeyondHD-Parser-1.0.7/setup.py
```

### Comparing `BeyondHD-Parser-1.0.6/BeyondHD_Parser.egg-info/PKG-INFO` & `BeyondHD-Parser-1.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: BeyondHD-Parser
-Version: 1.0.6
-Summary: Tool to search/scrape BeyondHD for torrent information
-Home-page: https://github.com/jlw4049/BeyondHD-Parser
-Author: Jessie Wilson
-Author-email: jessielw4049@gmail.com
-License: MIT
-Keywords: BeyondHD-Parser
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BeyondHD-Parser
 
 This package includes a way to utilize BeyondHD's search API as well as parse URL's for MediaInfo/NFO
 
 ## Install
 
 `pip install BeyondHD-Parser`
@@ -104,9 +84,7 @@
 
 `timeout` You can adjust the timeout time, default is 60 (seconds)
 
 ## BeyondHDScrape's .parse_nfo() parameters
 `bhdstudio` True or False, default is False. You can parse BHDStudio NFO's into a python dictionary
 
 `text_only` True or False, default is False. You can strip away anything that isn't text in the NFO output
-
-
```

### Comparing `BeyondHD-Parser-1.0.6/beyondhd_parser/beyondhd_details.py` & `BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_details.py`

 * *Files identical despite different names*

### Comparing `BeyondHD-Parser-1.0.6/beyondhd_parser/beyondhd_search.py` & `BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from typing import Union
 
 
 class ApiKeyError(Exception):
     """Custom exception for ApiKeyError"""
 
     pass
 
@@ -10,16 +11,15 @@
 class BhdApiError(Exception):
     """All generic BHD errors"""
 
     pass
 
 
 class BeyondHDAPI:
-    def __init__(self, api_key: str,
-                 rss_key: str = None):
+    def __init__(self, api_key: str, rss_key: str = None):
         """
         Search BeyondHD for torrents and return 100 results at a time.
 
         :param api_key: API key from BeyondHD.
         :param rss_key: RSS key from BeyondHD.
         """
 
@@ -33,43 +33,62 @@
         self.search_timeout = None
         self.run_check = None
         self.payload = None
         self.success = None
 
     def search(
         self,
-        title: str,
+        title: Union[str, None] = None,
+        categories: list = None,
         release_group: str = None,
         page: int = 0,
         resolution: str = None,
         search_timeout: int = 60,
     ):
         """
         Searches BeyondHD via the search API
 
         :param title: Title of the movie to check.
+        :param categories: List that contains 'Movies' and/or 'TV' (example: ['Movies', 'TV']).
         :param release_group: Release group in the format of BHDStudio, FraMeSToR, SacReD, is case sensitive.
         :param page: This returns 100 results by default, if for some reason there is more send a page number.
         :param resolution: Filters results by resolution, 720p... If left as None then it will return all results.
         :param search_timeout: Default is 60, can adjust this in seconds
         """
 
         # update variables
         self.title = title
+        self.categories = categories
         self.release_group = release_group
         self.page = page
         self.resolution = resolution
         self.search_timeout = search_timeout
 
         # base payload
         self.payload = {
             "action": "search",
-            "search": title,
         }
 
+        # add title to payload
+        if self.title and isinstance(self.title, str):
+            self.payload["search"] = self.title
+        else:
+            self.payload["search"] = ""
+
+        # parse categories
+        if self.categories and isinstance(self.categories, list):
+            if "Movies" in self.categories and "TV" in self.categories:
+                self.payload["categories"] = "Movies,TV"
+            elif "Movies" in self.categories:
+                self.payload["categories"] = "Movies"
+            elif "TV" in self.categories:
+                self.payload["categories"] = "TV"
+            else:
+                raise BhdApiError("Categories only support 'Movies' and 'TV'")
+
         # if user provides RSS key add it to the payload
         if self.rss_key:
             self.payload.update({"rsskey": self.rss_key})
 
         # if a page is specified add it to the payload
         if self.page >= 1:
             self.payload.update({"page": int(page)})
@@ -138,16 +157,15 @@
                     release_dict.update({x["name"]: x})
 
         return release_dict
 
 
 if __name__ == "__main__":
     try:
-        search_beyondhd = BeyondHDAPI(api_key="KEY",
-                                      rss_key="KEY")
+        search_beyondhd = BeyondHDAPI(api_key="KEY", rss_key="KEY")
         search_beyondhd.search(title="Gone In 60 Seconds")
 
         if search_beyondhd.success:
             print("Do something with results:\n" + str(search_beyondhd.get_results()))
         elif not search_beyondhd.success:
             print("No results")
```

### Comparing `BeyondHD-Parser-1.0.6/beyondhd_parser/bhdstudio_nfo_parse.py` & `BeyondHD-Parser-1.0.7/beyondhd_parser/bhdstudio_nfo_parse.py`

 * *Files identical despite different names*

### Comparing `BeyondHD-Parser-1.0.6/setup.py` & `BeyondHD-Parser-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fd:
     ext_long_desc = fd.read()
 
 setup(
     name="BeyondHD-Parser",
-    version="1.0.6",
+    version="1.0.7",
     description="Tool to search/scrape BeyondHD for torrent information",
     long_description=ext_long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/jlw4049/BeyondHD-Parser",
     author="Jessie Wilson",
     author_email="jessielw4049@gmail.com",
     license="MIT",
```

