# Comparing `tmp/douyin_tiktok_scraper-1.2.6.tar.gz` & `tmp/douyin_tiktok_scraper-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "douyin_tiktok_scraper-1.2.6.tar", last modified: Sun Jun  4 01:21:33 2023, max compression
+gzip compressed data, was "douyin_tiktok_scraper-1.2.7.tar", last modified: Sun Jun  4 01:26:30 2023, max compression
```

## Comparing `douyin_tiktok_scraper-1.2.6.tar` & `douyin_tiktok_scraper-1.2.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 01:21:33.644722 douyin_tiktok_scraper-1.2.6/
--rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.6/LICENSE
--rw-rw-rw-   0        0        0    15665 2023-06-04 01:21:33.644722 douyin_tiktok_scraper-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 01:21:33.630720 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper/
--rw-rw-rw-   0        0        0    50081 2023-03-02 08:52:24.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper/X-Bogus.js
--rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper/__init__.py
--rw-rw-rw-   0        0        0    35323 2023-06-04 01:21:30.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper/scraper.py
-drwxrwxrwx   0        0        0        0 2023-06-04 01:21:33.641722 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/
--rw-rw-rw-   0        0        0    15665 2023-06-04 01:21:33.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-06-04 01:21:33.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 01:21:33.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-04 01:21:33.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-04 01:21:33.000000 douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 01:21:33.644722 douyin_tiktok_scraper-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-06-04 01:21:30.000000 douyin_tiktok_scraper-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 01:26:30.285109 douyin_tiktok_scraper-1.2.7/
+-rw-rw-rw-   0        0        0     1087 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0    15665 2023-06-04 01:26:30.284109 douyin_tiktok_scraper-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    14844 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 01:26:30.272597 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper/
+-rw-rw-rw-   0        0        0    50081 2023-03-02 08:52:24.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper/X-Bogus.js
+-rw-rw-rw-   0        0        0        0 2022-12-17 05:33:45.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper/__init__.py
+-rw-rw-rw-   0        0        0    35308 2023-06-04 01:25:19.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-04 01:26:30.282108 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/
+-rw-rw-rw-   0        0        0    15665 2023-06-04 01:26:30.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-06-04 01:26:30.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 01:26:30.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-04 01:26:30.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-04 01:26:30.000000 douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 01:26:30.285109 douyin_tiktok_scraper-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-06-04 01:26:27.000000 douyin_tiktok_scraper-1.2.7/setup.py
```

### Comparing `douyin_tiktok_scraper-1.2.6/LICENSE` & `douyin_tiktok_scraper-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.6/PKG-INFO` & `douyin_tiktok_scraper-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin_tiktok_scraper
-Version: 1.2.6
+Version: 1.2.7
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
-Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.6 Summary:
+Metadata-Version: 2.1 Name: douyin_tiktok_scraper Version: 1.2.7 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.6/README.md` & `douyin_tiktok_scraper-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper/X-Bogus.js` & `douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper/X-Bogus.js`

 * *Files identical despite different names*

### Comparing `douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper/scraper.py` & `douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
             print('Error in get_url:', e)
             return None
 
     # 生成X-Bogus签名/Generate X-Bogus signature
     @staticmethod
     def generate_x_bogus_url(url: str, headers: dict) -> str:
         query = urllib.parse.urlparse(url).query
-        xbogus_file = pkg_resources.resource_filename('douyin_tiktok_scraper', 'X-Bogus.js')
-        xbogus = execjs.compile(open(xbogus_file).read()).call('sign', query, headers['User-Agent'])
+        xbogus_content = pkg_resources.resource_string(__name__, 'X-Bogus.js').decode()
+        xbogus = execjs.compile(xbogus_content).call('sign', query, headers['User-Agent'])
         new_url = url + "&X-Bogus=" + xbogus
         return new_url
 
     # 转换链接/convert url
     @retry(stop=stop_after_attempt(4), wait=wait_fixed(7))
     async def convert_share_urls(self, url: str) -> Union[str, None]:
         """
```

### Comparing `douyin_tiktok_scraper-1.2.6/douyin_tiktok_scraper.egg-info/PKG-INFO` & `douyin_tiktok_scraper-1.2.7/douyin_tiktok_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: douyin-tiktok-scraper
-Version: 1.2.6
+Version: 1.2.7
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
-Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.6 Summary:
+Metadata-Version: 2.1 Name: douyin-tiktok-scraper Version: 1.2.7 Summary:
 Douyin/TikTok async data scraper. Home-page: https://github.com/Evil0ctal/
 Douyin_TikTok_Download_API Author: Evil0ctal Author-email:
 Evil0ctal1985@gmail.com License: MIT License Keywords:
 TikTok,Douyin,æé³,Scraper,Crawler,API,Download,Video,No Watermark,Async
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

### Comparing `douyin_tiktok_scraper-1.2.6/setup.py` & `douyin_tiktok_scraper-1.2.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='douyin_tiktok_scraper',
     author='Evil0ctal',
-    version='1.2.6',
+    version='1.2.7',
     license='MIT License',
     description='Douyin/TikTok async data scraper.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='Evil0ctal1985@gmail.com',
     url='https://github.com/Evil0ctal/Douyin_TikTok_Download_API',
     packages=setuptools.find_packages(
```

