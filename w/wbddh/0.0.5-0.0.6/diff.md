# Comparing `tmp/wbddh-0.0.5-py3-none-any.whl.zip` & `tmp/wbddh-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9120 bytes, number of entries: 11
+Zip file size: 9147 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-15 19:53 wbddh/__init__.py
 -rw-rw-rw-  2.0 fat      990 b- defN 23-May-15 19:53 wbddh/exceptions.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-Jun-01 13:39 wbddh/request_manager.py
+-rw-rw-rw-  2.0 fat     4173 b- defN 23-Jun-04 19:04 wbddh/request_manager.py
 -rw-rw-rw-  2.0 fat     8796 b- defN 23-May-11 22:36 wbddh/session.py
 -rw-rw-rw-  2.0 fat     6218 b- defN 23-May-21 04:48 wbddh/session_manager.py
 -rw-rw-rw-  2.0 fat       50 b- defN 23-May-13 18:53 wbddh/test.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-May-11 22:36 wbddh/utils.py
--rw-rw-rw-  2.0 fat      543 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      810 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/RECORD
-11 files, 22629 bytes uncompressed, 7768 bytes compressed:  65.7%
+-rw-rw-rw-  2.0 fat      543 b- defN 23-Jun-04 19:05 wbddh-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 19:05 wbddh-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-04 19:05 wbddh-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      810 b- defN 23-Jun-04 19:05 wbddh-0.0.6.dist-info/RECORD
+11 files, 23392 bytes uncompressed, 7795 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: wbddh/test.py
 Comment: 
 
 Filename: wbddh/utils.py
 Comment: 
 
-Filename: wbddh-0.0.5.dist-info/METADATA
+Filename: wbddh-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: wbddh-0.0.5.dist-info/WHEEL
+Filename: wbddh-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: wbddh-0.0.5.dist-info/top_level.txt
+Filename: wbddh-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: wbddh-0.0.5.dist-info/RECORD
+Filename: wbddh-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wbddh/request_manager.py

```diff
@@ -33,15 +33,15 @@
             if session:
                 session.check_tokens()
                 response = requests.get(get_endpoint(endpoint, session), params=params, verify=session.verify, headers=session.get_headers(headers))
             else:
                 response = requests.get(get_endpoint(endpoint), params=params)
             count = count + 1
         except requests.exceptions.RequestException as e:
-            print (f"[{count} try] An error occured: ", e)
+            print (f"[{count} try] Error: ", e)
 
         if response.status_code == 200:
             return response
         elif count > num_try:
             raise Exception(f"Request failed after {count} tries.")
 
 def post(endpoint, params=None, json=None, headers=None, session=None):
@@ -54,25 +54,41 @@
         headers:		additional headers
 
     Returns:
         a Response object (from the requests package)
     '''
     if session:
         session.check_tokens()
-        try:
-            response = requests.post(get_endpoint(endpoint, session), params=params, json=json, verify=session.verify, headers=session.get_headers(headers))
-        except requests.ConnectionError as e:
-            raise requests.ConnectionError(e.response)
-        except requests.exceptions.RequestException as e:
-            raise requests.ConnectionError(e.response)
-        return response
+        return requests.post(get_endpoint(endpoint, session), params=params, json=json, verify=session.verify, headers=session.get_headers(headers))
     else:
         raise DDHSessionException("DDH POST request requires a session")
 
+def try_pose(endpoint, params=None, json=None, headers=None, session=None, num_try=3, interval=300):
+    '''Repeat sending a POST request until it succeeds or it tries {num_try} times
 
+    Additional arguments:
+        num_try:        number of tries
+        interval:       interval between tries in seconds
+    '''
+    if session:
+        count = 0
+        while True:
+            try:
+                session.check_tokens()
+                response = requests.post(get_endpoint(endpoint, session), params=params, json=json, verify=session.verify, headers=session.get_headers(headers))
+                count = count + 1
+            except requests.exceptions.RequestException as e:
+                print (f"[{count} try] Error: ", e)
+                
+            if response.status_code == 200:
+                return response
+            elif count > num_try:
+                raise Exception(f"Request failed after {count} tries.")
+    else:
+        raise DDHSessionException("DDH POST request requires a session")
 
 def post_file(endpoint, files=None, headers=None, session=None):
     '''Send a POST request with file
 
     Arguments:
         endpoint:		the endpoint (e.g., "dataset/listpage")
         files:			multi-part form object
```

## Comparing `wbddh-0.0.5.dist-info/METADATA` & `wbddh-0.0.6.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbddh
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python wrapper for DDH Open API
 Home-page: https://github.com/WB-DECIS/WBDDH
 Author: DECIS
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Provides-Extra: admin
 Requires-Dist: msal ; extra == 'admin'
```

## Comparing `wbddh-0.0.5.dist-info/RECORD` & `wbddh-0.0.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 wbddh/__init__.py,sha256=Mzr-CFhoE5tVUGnBK0ErZp429LATAf-G0hBHW0NP4vE,396
 wbddh/exceptions.py,sha256=prNSwu_9o5NnGfRtZBe4OxifAcLM2eSlrgpiJkOz8-8,990
-wbddh/request_manager.py,sha256=dZmAQEGaRMjFOtKTMf5NgUNiqVmpJgi_3I6vZNVqc1o,3410
+wbddh/request_manager.py,sha256=DNmDhXSUiXS-DVHDV__xN7eBJFkDEAXXURmqtykkm8Y,4173
 wbddh/session.py,sha256=pW5SqU2LaWcsFqRlzYMjSDM3Dlag_7HsRQHDOufTeC0,8796
 wbddh/session_manager.py,sha256=Gtax6G_E5pbcjZGIvkEPYmc_mx2fKhu26vvMBnmHKc4,6218
 wbddh/test.py,sha256=tuUyiKBC5AHoFjelqqMXWX_TrlE80HB37gJ7GidUp7U,50
 wbddh/utils.py,sha256=UhNse6FN2NzOtqL2v_js-l48MxGWLJLc-jusWSe1Zt0,1318
-wbddh-0.0.5.dist-info/METADATA,sha256=cDsLPPpes1wggH_iKBOks8jrZ0jsWsfuxR98eDx24ms,543
-wbddh-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-wbddh-0.0.5.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
-wbddh-0.0.5.dist-info/RECORD,,
+wbddh-0.0.6.dist-info/METADATA,sha256=DIU0dfTkZ95inr5Gs2sLQ-0FHEEpQpjzMpxzagtONIY,543
+wbddh-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+wbddh-0.0.6.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
+wbddh-0.0.6.dist-info/RECORD,,
```

