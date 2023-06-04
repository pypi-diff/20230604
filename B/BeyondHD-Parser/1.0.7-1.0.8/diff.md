# Comparing `tmp/BeyondHD-Parser-1.0.7.tar.gz` & `tmp/BeyondHD-Parser-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BeyondHD-Parser-1.0.7.tar", last modified: Sun Jun  4 16:57:27 2023, max compression
+gzip compressed data, was "BeyondHD-Parser-1.0.8.tar", last modified: Sun Jun  4 17:02:05 2023, max compression
```

## Comparing `BeyondHD-Parser-1.0.7.tar` & `BeyondHD-Parser-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 16:57:27.210084 BeyondHD-Parser-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-06-04 16:57:27.204838 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/
--rw-rw-rw-   0        0        0     4342 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-04 16:57:27.000000 BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4342 2023-06-04 16:57:27.208475 BeyondHD-Parser-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2919 2022-12-30 20:07:45.000000 BeyondHD-Parser-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 16:57:27.207920 BeyondHD-Parser-1.0.7/beyondhd_parser/
--rw-rw-rw-   0        0        0        0 2022-12-30 16:19:16.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/__init__.py
--rw-rw-rw-   0        0        0     5114 2023-01-14 05:35:33.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_details.py
--rw-rw-rw-   0        0        0     6107 2023-06-04 16:54:50.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_search.py
--rw-rw-rw-   0        0        0     3405 2022-12-29 08:12:07.000000 BeyondHD-Parser-1.0.7/beyondhd_parser/bhdstudio_nfo_parse.py
--rw-rw-rw-   0        0        0       42 2023-06-04 16:57:27.210084 BeyondHD-Parser-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-06-04 16:57:08.000000 BeyondHD-Parser-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 17:02:05.114603 BeyondHD-Parser-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-06-04 17:02:05.110681 BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/
+-rw-rw-rw-   0        0        0     4482 2023-06-04 17:02:05.000000 BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-04 17:02:05.000000 BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 17:02:05.000000 BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-04 17:02:05.000000 BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-04 17:02:05.000000 BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4482 2023-06-04 17:02:05.114603 BeyondHD-Parser-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3011 2023-06-04 17:01:29.000000 BeyondHD-Parser-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 17:02:05.113091 BeyondHD-Parser-1.0.8/beyondhd_parser/
+-rw-rw-rw-   0        0        0        0 2022-12-30 16:19:16.000000 BeyondHD-Parser-1.0.8/beyondhd_parser/__init__.py
+-rw-rw-rw-   0        0        0     5114 2023-01-14 05:35:33.000000 BeyondHD-Parser-1.0.8/beyondhd_parser/beyondhd_details.py
+-rw-rw-rw-   0        0        0     6107 2023-06-04 16:54:50.000000 BeyondHD-Parser-1.0.8/beyondhd_parser/beyondhd_search.py
+-rw-rw-rw-   0        0        0     3405 2022-12-29 08:12:07.000000 BeyondHD-Parser-1.0.8/beyondhd_parser/bhdstudio_nfo_parse.py
+-rw-rw-rw-   0        0        0       42 2023-06-04 17:02:05.114603 BeyondHD-Parser-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-06-04 17:01:43.000000 BeyondHD-Parser-1.0.8/setup.py
```

### Comparing `BeyondHD-Parser-1.0.7/BeyondHD_Parser.egg-info/PKG-INFO` & `BeyondHD-Parser-1.0.8/BeyondHD_Parser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BeyondHD-Parser
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tool to search/scrape BeyondHD for torrent information
 Home-page: https://github.com/jlw4049/BeyondHD-Parser
 Author: Jessie Wilson
 Author-email: jessielw4049@gmail.com
 License: MIT
 Description: # BeyondHD-Parser
         
@@ -28,15 +28,15 @@
         search_beyondhd.search(title="Gone In 60 Seconds")
         
         if search_beyondhd.success:
             print("Do something with results:\n" + str(search_beyondhd.get_results()))
         elif not search_beyondhd.success:
             print("No results")
         
-            
+        
         # full work flow with error handling ##################
         try:
             search_beyondhd = BeyondHDAPI(api_key="NEED KEY")
             search_beyondhd.search(title="Gone In 60 Seconds")
         
             if search_beyondhd.success:
                 print("Do something with results:\n" + str(search_beyondhd.get_results()))
@@ -50,23 +50,26 @@
             print("Invalid API Key")
         
         except BhdApiError as bhd_error:
             print(str(bhd_error))
         ```
         
         ## BeyondHDApi's .search() parameters
+        
         BeyondHDApi() only accepts URL, the .search() method is where all the magic happens
         
-        `title` Required, title to search for in the format of *The Matrix 1999*
+        `title` Optional, title to search for in the format of _The Matrix 1999_
+        
+        `categories` Optional, categories to search in the form of a list _['Movies', 'TV']_
         
-        `release_group` Optional, specify groups *BHDStudio, FraMeSToR, SacReD*
+        `release_group` Optional, specify groups _BHDStudio, FraMeSToR, SacReD_
         
-        `page` Optional, allows you to select which page *int e.g. 0, 1, 2*
+        `page` Optional, allows you to select which page _int e.g. 0, 1, 2_
         
-        `resolution` Optional, can filter resolutions *720p, 1080p, etc*
+        `resolution` Optional, can filter resolutions _720p, 1080p, etc_
         
         `search_timeout` You can adjust the timeout time, default is 60 (seconds)
         
         ## Example of how scrape BeyondHD
         
         ```python
         from beyondhd_parser.beyondhd_details import BeyondHDScrape
@@ -76,27 +79,30 @@
         )
         scrape_bhd.parse_media_info()
         scrape_bhd.parse_nfo()
         print(scrape_bhd.nfo)
         print(scrape_bhd.media_info)
         
         ```
+        
         ## BeyondHDScrape() parameters
+        
         `url` Required, url to the torrent to parse
         
         `cookie_key` Optional, but if you do not provide the key/value you must have logged in prior in a supported browser
         
         `cookie_value` Optional, but if you do not provide the key/value you must have logged in prior in a supported browser
         
         `auto_cookie_detection` Default is True, manual cookie input does override this. If you've logged into BeyondHD in any of the supported browsers, this will automatically inject your cookie.\
-        *chrome, chromium, opera, brave, edge, vivaldi, firefox and safari*
+        _chrome, chromium, opera, brave, edge, vivaldi, firefox and safari_
         
         `timeout` You can adjust the timeout time, default is 60 (seconds)
         
         ## BeyondHDScrape's .parse_nfo() parameters
+        
         `bhdstudio` True or False, default is False. You can parse BHDStudio NFO's into a python dictionary
         
         `text_only` True or False, default is False. You can strip away anything that isn't text in the NFO output
         
 Keywords: BeyondHD-Parser
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `BeyondHD-Parser-1.0.7/PKG-INFO` & `BeyondHD-Parser-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BeyondHD-Parser
-Version: 1.0.7
+Version: 1.0.8
 Summary: Tool to search/scrape BeyondHD for torrent information
 Home-page: https://github.com/jlw4049/BeyondHD-Parser
 Author: Jessie Wilson
 Author-email: jessielw4049@gmail.com
 License: MIT
 Description: # BeyondHD-Parser
         
@@ -28,15 +28,15 @@
         search_beyondhd.search(title="Gone In 60 Seconds")
         
         if search_beyondhd.success:
             print("Do something with results:\n" + str(search_beyondhd.get_results()))
         elif not search_beyondhd.success:
             print("No results")
         
-            
+        
         # full work flow with error handling ##################
         try:
             search_beyondhd = BeyondHDAPI(api_key="NEED KEY")
             search_beyondhd.search(title="Gone In 60 Seconds")
         
             if search_beyondhd.success:
                 print("Do something with results:\n" + str(search_beyondhd.get_results()))
@@ -50,23 +50,26 @@
             print("Invalid API Key")
         
         except BhdApiError as bhd_error:
             print(str(bhd_error))
         ```
         
         ## BeyondHDApi's .search() parameters
+        
         BeyondHDApi() only accepts URL, the .search() method is where all the magic happens
         
-        `title` Required, title to search for in the format of *The Matrix 1999*
+        `title` Optional, title to search for in the format of _The Matrix 1999_
+        
+        `categories` Optional, categories to search in the form of a list _['Movies', 'TV']_
         
-        `release_group` Optional, specify groups *BHDStudio, FraMeSToR, SacReD*
+        `release_group` Optional, specify groups _BHDStudio, FraMeSToR, SacReD_
         
-        `page` Optional, allows you to select which page *int e.g. 0, 1, 2*
+        `page` Optional, allows you to select which page _int e.g. 0, 1, 2_
         
-        `resolution` Optional, can filter resolutions *720p, 1080p, etc*
+        `resolution` Optional, can filter resolutions _720p, 1080p, etc_
         
         `search_timeout` You can adjust the timeout time, default is 60 (seconds)
         
         ## Example of how scrape BeyondHD
         
         ```python
         from beyondhd_parser.beyondhd_details import BeyondHDScrape
@@ -76,27 +79,30 @@
         )
         scrape_bhd.parse_media_info()
         scrape_bhd.parse_nfo()
         print(scrape_bhd.nfo)
         print(scrape_bhd.media_info)
         
         ```
+        
         ## BeyondHDScrape() parameters
+        
         `url` Required, url to the torrent to parse
         
         `cookie_key` Optional, but if you do not provide the key/value you must have logged in prior in a supported browser
         
         `cookie_value` Optional, but if you do not provide the key/value you must have logged in prior in a supported browser
         
         `auto_cookie_detection` Default is True, manual cookie input does override this. If you've logged into BeyondHD in any of the supported browsers, this will automatically inject your cookie.\
-        *chrome, chromium, opera, brave, edge, vivaldi, firefox and safari*
+        _chrome, chromium, opera, brave, edge, vivaldi, firefox and safari_
         
         `timeout` You can adjust the timeout time, default is 60 (seconds)
         
         ## BeyondHDScrape's .parse_nfo() parameters
+        
         `bhdstudio` True or False, default is False. You can parse BHDStudio NFO's into a python dictionary
         
         `text_only` True or False, default is False. You can strip away anything that isn't text in the NFO output
         
 Keywords: BeyondHD-Parser
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `BeyondHD-Parser-1.0.7/README.md` & `BeyondHD-Parser-1.0.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 search_beyondhd.search(title="Gone In 60 Seconds")
 
 if search_beyondhd.success:
     print("Do something with results:\n" + str(search_beyondhd.get_results()))
 elif not search_beyondhd.success:
     print("No results")
 
-    
+
 # full work flow with error handling ##################
 try:
     search_beyondhd = BeyondHDAPI(api_key="NEED KEY")
     search_beyondhd.search(title="Gone In 60 Seconds")
 
     if search_beyondhd.success:
         print("Do something with results:\n" + str(search_beyondhd.get_results()))
@@ -42,23 +42,26 @@
     print("Invalid API Key")
 
 except BhdApiError as bhd_error:
     print(str(bhd_error))
 ```
 
 ## BeyondHDApi's .search() parameters
+
 BeyondHDApi() only accepts URL, the .search() method is where all the magic happens
 
-`title` Required, title to search for in the format of *The Matrix 1999*
+`title` Optional, title to search for in the format of _The Matrix 1999_
+
+`categories` Optional, categories to search in the form of a list _['Movies', 'TV']_
 
-`release_group` Optional, specify groups *BHDStudio, FraMeSToR, SacReD*
+`release_group` Optional, specify groups _BHDStudio, FraMeSToR, SacReD_
 
-`page` Optional, allows you to select which page *int e.g. 0, 1, 2*
+`page` Optional, allows you to select which page _int e.g. 0, 1, 2_
 
-`resolution` Optional, can filter resolutions *720p, 1080p, etc*
+`resolution` Optional, can filter resolutions _720p, 1080p, etc_
 
 `search_timeout` You can adjust the timeout time, default is 60 (seconds)
 
 ## Example of how scrape BeyondHD
 
 ```python
 from beyondhd_parser.beyondhd_details import BeyondHDScrape
@@ -68,23 +71,26 @@
 )
 scrape_bhd.parse_media_info()
 scrape_bhd.parse_nfo()
 print(scrape_bhd.nfo)
 print(scrape_bhd.media_info)
 
 ```
+
 ## BeyondHDScrape() parameters
+
 `url` Required, url to the torrent to parse
 
 `cookie_key` Optional, but if you do not provide the key/value you must have logged in prior in a supported browser
 
 `cookie_value` Optional, but if you do not provide the key/value you must have logged in prior in a supported browser
 
 `auto_cookie_detection` Default is True, manual cookie input does override this. If you've logged into BeyondHD in any of the supported browsers, this will automatically inject your cookie.\
-*chrome, chromium, opera, brave, edge, vivaldi, firefox and safari*
+_chrome, chromium, opera, brave, edge, vivaldi, firefox and safari_
 
 `timeout` You can adjust the timeout time, default is 60 (seconds)
 
 ## BeyondHDScrape's .parse_nfo() parameters
+
 `bhdstudio` True or False, default is False. You can parse BHDStudio NFO's into a python dictionary
 
 `text_only` True or False, default is False. You can strip away anything that isn't text in the NFO output
```

### Comparing `BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_details.py` & `BeyondHD-Parser-1.0.8/beyondhd_parser/beyondhd_details.py`

 * *Files identical despite different names*

### Comparing `BeyondHD-Parser-1.0.7/beyondhd_parser/beyondhd_search.py` & `BeyondHD-Parser-1.0.8/beyondhd_parser/beyondhd_search.py`

 * *Files identical despite different names*

### Comparing `BeyondHD-Parser-1.0.7/beyondhd_parser/bhdstudio_nfo_parse.py` & `BeyondHD-Parser-1.0.8/beyondhd_parser/bhdstudio_nfo_parse.py`

 * *Files identical despite different names*

### Comparing `BeyondHD-Parser-1.0.7/setup.py` & `BeyondHD-Parser-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as fd:
     ext_long_desc = fd.read()
 
 setup(
     name="BeyondHD-Parser",
-    version="1.0.7",
+    version="1.0.8",
     description="Tool to search/scrape BeyondHD for torrent information",
     long_description=ext_long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/jlw4049/BeyondHD-Parser",
     author="Jessie Wilson",
     author_email="jessielw4049@gmail.com",
     license="MIT",
```

