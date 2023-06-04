# Comparing `tmp/dartrig-0.1.4.tar.gz` & `tmp/dartrig-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.4.tar", last modified: Sun Jun  4 14:27:26 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.5.tar", last modified: Sun Jun  4 14:34:56 2023, max compression
```

## Comparing `dartrig-0.1.4.tar` & `dartrig-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:27:26.000000 dartrig-0.1.4/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:27:26.000000 dartrig-0.1.4/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.4/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.4/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-04 14:27:25.000000 dartrig-0.1.4/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    15503 2023-06-04 14:27:24.000000 dartrig-0.1.4/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.4/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-04 14:27:26.000000 dartrig-0.1.4/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-04 14:27:26.000000 dartrig-0.1.4/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:34:56.000000 dartrig-0.1.5/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:34:56.000000 dartrig-0.1.5/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.5/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.5/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-04 14:34:55.000000 dartrig-0.1.5/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    15543 2023-06-04 14:34:55.000000 dartrig-0.1.5/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.5/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-04 14:34:56.000000 dartrig-0.1.5/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-04 14:34:56.000000 dartrig-0.1.5/setup.cfg
```

### Comparing `dartrig-0.1.4/PKG-INFO` & `dartrig-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.4
+Version: 0.1.5
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.4/LICENSE` & `dartrig-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.4/README.md` & `dartrig-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.4/setup.py` & `dartrig-0.1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.4",
+    version="0.1.5",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.11'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.4/dartrig/__init__.py` & `dartrig-0.1.5/dartrig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,32 @@
 
         self.cache: AdtCache = cache
 
         self.file_cache = file_cache
         if self.file_cache is not None:
             self.logger.info(f"File cache is enabled. Cache directory: {file_cache.base_dir}")
 
-    def request_detail(self, rcp_no: str, dtd: str, ele_id: int = 0, offset: int = 0) -> str:
+    def request_detail(self, rcp_no: str, dtd: str, ele_id: int = 0, offset: int = 0, length: int = 0) -> str:
         """
         :param rcp_no:
         :param dtd: html | dart3.xsd
         :param ele_id:
         :param offset:
         :return:
         """
         dcm_no = self._get_dcm_no_by_rcp_no(rcp_no)
-        return self._request_detail_with_dcm(rcp_no, dtd, dcm_no, ele_id, offset)
+        return self.request_detail_with_dcm(rcp_no, dtd, dcm_no, ele_id, offset, length)
+
+    def request_detail_with_dcm(self, rcp_no, dtd, dcm_no, ele_id=0, offset=0, length=0):
+        dtd_split = dtd.split(".")[0]
+        file_cache_key = f"{rcp_no}_{dcm_no}_{dtd_split}_{ele_id}_{offset}"
+
+        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length={length}&dtd={dtd}"
+        self.logger.info(f"request_detail_with_dcm url : {url}")
+        return self._try_file_cache_request(url, "viewer", file_cache_key, ext="html" if dtd.lower() == "html" else "xml")
 
     def _try_file_cache_request(self, url, prefix, file_cache_key, ext="html"):
         if self.file_cache is not None:
             cached = self.file_cache.get_file(prefix=prefix, key=file_cache_key, ext=ext)
             if cached is not None:
                 self.logger.debug(f"file cache hit for key {file_cache_key}")
                 return cached
@@ -83,22 +91,14 @@
         # self.logger.debug(f"_try_file_cache_request response text : {text}")
 
         if self.file_cache is not None:
             self.file_cache.save_file(prefix=prefix, key=file_cache_key, ext=ext, data=text)
             self.logger.debug(f"file cache set for key {file_cache_key}")
         return text
 
-    def _request_detail_with_dcm(self, rcp_no, dtd, dcm_no, ele_id=0, offset=0):
-        dtd_split = dtd.split(".")[0]
-        file_cache_key = f"{rcp_no}_{dcm_no}_{dtd_split}_{ele_id}_{offset}"
-
-        url = f"{URLS['DART_VIEWER']}?rcpNo={rcp_no}&dcmNo={dcm_no}&eleId={ele_id}&offset={offset}&length=0&dtd={dtd}"
-        self.logger.info(f"request_detail_with_dcm url : {url}")
-        return self._try_file_cache_request(url, "viewer", file_cache_key, ext="html" if dtd.lower() == "html" else "xml")
-
     def _get_dcm_no_by_rcp_no(self, rcp_no):
         cache_key = f"dcm_no_{rcp_no}"
         try:
             if self.cache is not None:
                 cached = self.cache.get(cache_key)
                 if cached is not None:
                     logger.debug(f"dsaf001_report cache hit for rcp_no {rcp_no}")
```

### Comparing `dartrig-0.1.4/dartrig/annotations.py` & `dartrig-0.1.5/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.4/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.5/dartrig.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.4
+Version: 0.1.5
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

