# Comparing `tmp/douyin_tiktok_scraper-1.2.4.tar.gz` & `tmp/douyin_tiktok_scraper-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "douyin_tiktok_scraper-1.2.4.tar", last modified: Sat Jun  3 10:25:36 2023, max compression
+gzip compressed data, was "douyin_tiktok_scraper-1.2.5.tar", last modified: Sat Jun  3 10:30:15 2023, max compression
```

## Comparing `douyin_tiktok_scraper-1.2.4.tar` & `douyin_tiktok_scraper-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 10:25:36.536445 douyin_tiktok_scraper-1.2.4/
--rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    15665 2023-06-03 10:25:36.535446 douyin_tiktok_scraper-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 10:25:36.520444 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper/
--rw-rw-rw-   0        0        0    50081 2023-03-02 08:52:24.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper/X-Bogus.js
--rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper/__init__.py
--rw-rw-rw-   0        0        0    35210 2023-06-03 09:59:44.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-06-03 10:25:36.532445 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/
--rw-rw-rw-   0        0        0    15665 2023-06-03 10:25:36.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-06-03 10:25:36.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 10:25:36.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-03 10:25:36.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-03 10:25:36.000000 douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-03 10:25:36.536445 douyin_tiktok_scraper-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-06-03 10:25:32.000000 douyin_tiktok_scraper-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:30:15.941844 douyin_tiktok_scraper-1.2.5/
+-rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    15665 2023-06-03 10:30:15.940845 douyin_tiktok_scraper-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-03 10:30:15.926843 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper/
+-rw-rw-rw-   0        0        0    50081 2023-03-02 08:52:24.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper/X-Bogus.js
+-rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper/__init__.py
+-rw-rw-rw-   0        0        0    35308 2023-06-03 10:30:12.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-03 10:30:15.938842 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/
+-rw-rw-rw-   0        0        0    15665 2023-06-03 10:30:15.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-03 10:30:15.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 10:30:15.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-03 10:30:15.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-03 10:30:15.000000 douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-03 10:30:15.941844 douyin_tiktok_scraper-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-06-03 10:30:12.000000 douyin_tiktok_scraper-1.2.5/setup.py
```

### Comparing `douyin_tiktok_scraper-1.2.4/LICENSE` & `douyin_tiktok_scraper-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.4/PKG-INFO` & `douyin_tiktok_scraper-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin_tiktok_scraper
-Version: 1.2.4
+Version: 1.2.5
 Summary: Douyin/TikTok async data scraper.
 Home-page: https://github.com/Evil0ctal/Douyin_TikTok_Download_API
 Author: Evil0ctal
 Author-email: Evil0ctal1985@gmail.com
 License: MIT License
 Keywords: TikTok,Douyin,抖音,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.4 Summary:
+Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.5 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.4/README.md` & `douyin_tiktok_scraper-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper/X-Bogus.js` & `douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper/X-Bogus.js`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper/scraper.py` & `douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import execjs
 import aiohttp
 import platform
 import asyncio
 import traceback
 import configparser
 import urllib.parse
+import pkg_resources
 
 from typing import Union
 from tenacity import *
 
 
 class Scraper:
     """__________________________________________⬇️initialization(初始化)⬇️______________________________________"""
@@ -82,15 +83,16 @@
             print('Error in get_url:', e)
             return None
 
     # 生成X-Bogus签名/Generate X-Bogus signature
     @staticmethod
     def generate_x_bogus_url(url: str, headers: dict) -> str:
         query = urllib.parse.urlparse(url).query
-        xbogus = execjs.compile(open('./X-Bogus.js').read()).call('sign', query, headers['User-Agent'])
+        xbogus_file = pkg_resources.resource_filename(__name__, 'X-Bogus.js')
+        xbogus = execjs.compile(open(xbogus_file).read()).call('sign', query, headers['User-Agent'])
         new_url = url + "&X-Bogus=" + xbogus
         return new_url
 
     # 转换链接/convert url
     @retry(stop=stop_after_attempt(4), wait=wait_fixed(7))
     async def convert_share_urls(self, url: str) -> Union[str, None]:
         """
```

### Comparing `douyin_tiktok_scraper-1.2.4/douyin_tiktok_scraper.egg-info/PKG-INFO` & `douyin_tiktok_scraper-1.2.5/douyin_tiktok_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin-tiktok-scraper
-Version: 1.2.4
+Version: 1.2.5
 Summary: Douyin/TikTok async data scraper.
 Home-page: https://github.com/Evil0ctal/Douyin_TikTok_Download_API
 Author: Evil0ctal
 Author-email: Evil0ctal1985@gmail.com
 License: MIT License
 Keywords: TikTok,Douyin,抖音,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.4 Summary:
+Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.5 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.4/setup.py` & `douyin_tiktok_scraper-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='douyin_tiktok_scraper',
     author='Evil0ctal',
-    version='1.2.4',
+    version='1.2.5',
     license='MIT License',
     description='Douyin/TikTok async data scraper.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='Evil0ctal1985@gmail.com',
     url='https://github.com/Evil0ctal/Douyin_TikTok_Download_API',
     packages=setuptools.find_packages(
```

