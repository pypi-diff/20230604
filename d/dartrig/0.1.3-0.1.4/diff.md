# Comparing `tmp/dartrig-0.1.3.tar.gz` & `tmp/dartrig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.3.tar", last modified: Fri May 26 05:28:23 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.4.tar", last modified: Sun Jun  4 14:27:26 2023, max compression
```

## Comparing `dartrig-0.1.3.tar` & `dartrig-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 05:28:23.000000 dartrig-0.1.3/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-26 05:28:23.000000 dartrig-0.1.3/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.3/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.3/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-05-26 05:28:22.000000 dartrig-0.1.3/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    13644 2023-05-26 05:25:15.000000 dartrig-0.1.3/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.3/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-26 05:28:23.000000 dartrig-0.1.3/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-26 05:28:23.000000 dartrig-0.1.3/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:27:26.000000 dartrig-0.1.4/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:27:26.000000 dartrig-0.1.4/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.4/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.4/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-04 14:27:25.000000 dartrig-0.1.4/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    15503 2023-06-04 14:27:24.000000 dartrig-0.1.4/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.4/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-04 14:27:26.000000 dartrig-0.1.4/setup.cfg
```

### Comparing `dartrig-0.1.3/PKG-INFO` & `dartrig-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.3
+Version: 0.1.4
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.3/LICENSE` & `dartrig-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.3/README.md` & `dartrig-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.3/setup.py` & `dartrig-0.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.3",
+    version="0.1.4",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.11'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.3/dartrig/__init__.py` & `dartrig-0.1.4/dartrig/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import requests
 import logging
 import traceback
 import time
-from typing import List
+from typing import List, Dict
 from datetime import datetime
 from bs4 import BeautifulSoup
 from cache import AdtCache, MemoryCache
 from cache.filecache import FileCache
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/51.0.2704.103 Safari/537.36"}
@@ -16,14 +16,29 @@
     "DART_BASE": "https://dart.fss.or.kr",
     "DART_LIST": "https://dart.fss.or.kr/dsab007/detailSearch.ax",
     "DART_VIEWER": "https://dart.fss.or.kr/report/viewer.do",
     "DART_DSAF": "https://dart.fss.or.kr/dsaf001/main.do",
 }
 logger = logging.getLogger("dartrig")
 
+def remove_strs_list(text, removes):
+    tmp = text
+    for remove in removes:
+        tmp = tmp.replace(remove, '')
+
+    return tmp
+
+def fun_splitter(s):
+    spl = s.split(" = ")
+    if len(spl) <= 1:
+        return None
+    try:
+        return int(spl[1])
+    except ValueError:
+        return None
 
 class DartWeb:
     def __init__(self, cache: AdtCache = None, file_cache: FileCache = None):
         self.logger = logging.getLogger("dart_web")
         self.session = requests.Session()
         self.session.get(URLS["DART_BASE"], headers=HEADERS)
 
@@ -52,15 +67,15 @@
         if self.file_cache is not None:
             cached = self.file_cache.get_file(prefix=prefix, key=file_cache_key, ext=ext)
             if cached is not None:
                 self.logger.debug(f"file cache hit for key {file_cache_key}")
                 return cached
 
         response = self.session.get(url, headers=HEADERS)
-        self.logger.info(response.headers)
+        self.logger.debug(response.headers)
         content_type = response.headers["Content-Type"]
         if content_type is not None and "MS949" in content_type.upper():
             self.logger.debug(f"response encoding is MS949. change to utf-8")
             response.encoding = "ms949"
             text = response.text
         else:
             text = response.text
@@ -85,42 +100,73 @@
         try:
             if self.cache is not None:
                 cached = self.cache.get(cache_key)
                 if cached is not None:
                     logger.debug(f"dsaf001_report cache hit for rcp_no {rcp_no}")
                     return cached
 
-            url = f"{URLS['DART_DSAF']}?rcpNo={rcp_no}"
-            html_text = self._try_file_cache_request(url, "dsaf", rcp_no)
+            html_text = self._try_file_cache_request(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", "dsaf", rcp_no)
             numbers = re.findall("\d{7}", html_text)
             dcm_no = numbers[2]
 
             if self.cache is not None:
                 self.cache.set(cache_key, dcm_no)
                 logger.debug(f"dsaf001_report cache set for rcp_no {rcp_no}")
         except Exception as ex:
             logger.exception(ex)
             raise ValueError(f"dcm number fetch failed for rcp_no : [{rcp_no}]")
 
         return dcm_no
 
+    def get_dsaf_meta(self, rcp_no, keyword="연결재무") -> Dict[str, any]:
+        cache_key = f"dcm_no_meta_{rcp_no}"
+        try:
+            if self.cache is not None:
+                cached = self.cache.hget(cache_key)
+                if cached is not None:
+                    logger.debug(f"dsaf001_report cache hit for rcp_no {rcp_no}")
+                    return cached
+
+            html_text = self._try_file_cache_request(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", "dsaf", rcp_no)
+            numbers = re.findall("\d{7}", html_text)
+            dcm_no = numbers[2]
+            find1_num = html_text.index(keyword)  # 여기 viewDoc에서 필요한 정보가 다 들어있음
+            res_text = remove_strs_list(html_text[find1_num:find1_num + 250],
+                                        ['\t', '\n', "\'", 'node1', 'dart3', '"', "'"])
+
+            find1_list = list(filter(lambda x: x is not None, map(fun_splitter, res_text.split(";"))))
+            ele_id = find1_list[3]
+            offset = find1_list[4]
+            length = find1_list[5]
+
+            meta = { "dcm_no" : dcm_no, "ele_id" : ele_id, "offset" : offset, "length" : length }
+            if self.cache is not None:
+                self.cache.hset(cache_key, meta)
+                logger.debug(f"dsaf001_report cache set for rcp_no {rcp_no}")
+
+            return meta
+        except Exception as ex:
+            logger.exception(ex)
+            raise ValueError(f"dsaf meta fetch failed for rcp_no : [{rcp_no}]")
+
     def _deprecated_get_dsaf_html(self, rcp_no):
         return self.session.get(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", headers=HEADERS).text
 
-    def get_document(self, rcp_no, dtd, ele_id=0, offset=0):
+    def get_document(self, rcp_no, dtd, ele_id=0, offset=0, length=0):
         """
         문서 리턴
         :param rcp_no:
         :param dtd:
-        :param ele_id:
-        :param offset:
+        :param ele_id: 생략시 0
+        :param offset: 생략시 0
+        :param length: 생략시 0
         :return: (content_type, content)
         """
         dcm_no = self._get_dcm_no_by_rcp_no(rcp_no)
-        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
+        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length={length}&dtd={dtd}"
         response = self.session.get(url, headers=HEADERS)
         content_type = response.headers.get("Content-Type")
         return content_type, response.content
 
     def search_report(self, num, start, end, srch_txt):
         data = {
             'currentPage': str(num),
```

### Comparing `dartrig-0.1.3/dartrig/annotations.py` & `dartrig-0.1.4/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.3/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.4/dartrig.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.3
+Version: 0.1.4
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

