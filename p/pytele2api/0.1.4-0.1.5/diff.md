# Comparing `tmp/pytele2api-0.1.4.tar.gz` & `tmp/pytele2api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytele2api-0.1.4.tar", last modified: Thu Jun  1 12:39:45 2023, max compression
+gzip compressed data, was "pytele2api-0.1.5.tar", last modified: Sun Jun  4 21:30:07 2023, max compression
```

## Comparing `pytele2api-0.1.4.tar` & `pytele2api-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 12:39:45.699797 pytele2api-0.1.4/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.4/LICENSE
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.4/MANIFEST.in
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 12:39:45.699874 pytele2api-0.1.4/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.4/README.md
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 12:39:45.698861 pytele2api-0.1.4/pytele2api/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     4019 2023-06-01 09:16:55.000000 pytele2api-0.1.4/pytele2api/Tele2Api.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.4/pytele2api/__init__.py
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      484 2023-06-01 07:19:00.000000 pytele2api-0.1.4/pytele2api/const.py
-drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-01 12:39:45.699607 pytele2api-0.1.4/pytele2api.egg-info/
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-01 12:39:45.000000 pytele2api-0.1.4/pytele2api.egg-info/PKG-INFO
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-01 12:39:45.000000 pytele2api-0.1.4/pytele2api.egg-info/SOURCES.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-01 12:39:45.000000 pytele2api-0.1.4/pytele2api.egg-info/dependency_links.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-01 12:39:45.000000 pytele2api-0.1.4/pytele2api.egg-info/requires.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-01 12:39:45.000000 pytele2api-0.1.4/pytele2api.egg-info/top_level.txt
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-01 12:39:45.700085 pytele2api-0.1.4/setup.cfg
--rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-01 12:39:05.000000 pytele2api-0.1.4/setup.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-04 21:30:07.395653 pytele2api-0.1.5/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1062 2023-06-01 07:29:48.000000 pytele2api-0.1.5/LICENSE
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       16 2023-06-01 06:30:04.000000 pytele2api-0.1.5/MANIFEST.in
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-04 21:30:07.395702 pytele2api-0.1.5/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       65 2023-06-01 06:25:52.000000 pytele2api-0.1.5/README.md
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-04 21:30:07.394888 pytele2api-0.1.5/pytele2api/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     4396 2023-06-04 21:21:07.000000 pytele2api-0.1.5/pytele2api/Tele2Api.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       31 2023-06-01 07:21:21.000000 pytele2api-0.1.5/pytele2api/__init__.py
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      504 2023-06-04 21:19:17.000000 pytele2api-0.1.5/pytele2api/const.py
+drwxr-xr-x   0 fredrikhaggbom   (501) staff       (20)        0 2023-06-04 21:30:07.395546 pytele2api-0.1.5/pytele2api.egg-info/
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      835 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/PKG-INFO
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)      283 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/SOURCES.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)        1 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/dependency_links.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       18 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/requires.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       11 2023-06-04 21:30:07.000000 pytele2api-0.1.5/pytele2api.egg-info/top_level.txt
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)       79 2023-06-04 21:30:07.395884 pytele2api-0.1.5/setup.cfg
+-rw-r--r--   0 fredrikhaggbom   (501) staff       (20)     1045 2023-06-04 21:15:13.000000 pytele2api-0.1.5/setup.py
```

### Comparing `pytele2api-0.1.4/LICENSE` & `pytele2api-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytele2api-0.1.4/PKG-INFO` & `pytele2api-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.5.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.4/pytele2api/Tele2Api.py` & `pytele2api-0.1.5/pytele2api/Tele2Api.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     RES_LIMIT,
     RES_USAGE,
     RES_DATA_LEFT,
     RES_PERIOD_START,
     RES_PERIOD_END,
     CONF_SUBSCRIPTION,
     CONF_SUBSCRIPTIONMODEL,
+    RES_ERROR,
     Tele2ApiResult,
 )
 
 
 class Tele2Api:
     def __init__(
         self,
@@ -27,14 +28,15 @@
         self._data = {
             RES_UNLIMITED: False,
             RES_USAGE: None,
             RES_LIMIT: None,
             RES_DATA_LEFT: None,
             RES_PERIOD_START: None,
             RES_PERIOD_END: None,
+            RES_ERROR: None,
         }
         self.BASE_URL = "https://my.tso.tele2.se"
         self.AUTH_URL = self.BASE_URL + "/auth/login"
         self._LOGGER = logger
 
         self.SUBSCRIPTION_URL = (
             self.BASE_URL + "/api/subscriptions?refreshableOnly=false"
@@ -66,54 +68,60 @@
                     CONF_SUBSCRIPTION: str(data[0]["subsId"]),
                     CONF_SUBSCRIPTIONMODEL: data[0]["name"],
                 }
 
         return {}
 
     def getDataUsage(self) -> dict:
-        resp = self.session.get(self.DATA_USAGE_URL)
-        if (resp.status_code == 401 or resp.status_code == 403) and self.tries < 1:
-            self.tries += 1
-            self.updateAuth()
-            return self.getDataUsage()
-        elif resp.status_code == 200:
-            data = json.loads(resp.content)
-            limit = data[Tele2ApiResult.packageLimit]
-            usage = data["usage"]
-            remaining = data[Tele2ApiResult.remaining]
-
-            self.log(
-                "Got result. Limit: %s, usage: %s, remaining: %s, unlimited: %s",
-                limit,
-                usage,
-                remaining,
-                data[Tele2ApiResult.unlimitedData],
-            )
-
-            if Tele2ApiResult.unlimitedData in data:
-                self._data[RES_UNLIMITED] = data[Tele2ApiResult.unlimitedData]
-
-            if Tele2ApiResult.buckets in data and len(data["buckets"]) > 0:
-                bucket = data["buckets"][0]
-                if Tele2ApiResult.startDate in bucket:
-                    startDate = datetime.datetime.strptime(
-                        bucket[Tele2ApiResult.startDate], "%Y-%m-%d"
-                    ).date()
-                    self._data[RES_PERIOD_START] = startDate
-                if Tele2ApiResult.endDate in bucket:
-                    endDate = datetime.datetime.strptime(
-                        bucket[Tele2ApiResult.endDate], "%Y-%m-%d"
-                    ).date()
-                    self._data[RES_PERIOD_END] = endDate
-
-            self.tries = 0
-            self._data[RES_LIMIT] = limit
-            self._data[RES_USAGE] = usage
-            self._data[RES_DATA_LEFT] = remaining
-            self.log("Setting native value to: %d", remaining)
+        try:
+            resp = self.session.get(self.DATA_USAGE_URL)
+            if (resp.status_code == 401 or resp.status_code == 403) and self.tries < 1:
+                self.tries += 1
+                self.updateAuth()
+                return self.getDataUsage()
+            elif resp.status_code == 200:
+                data = json.loads(resp.content)
+                limit = data[Tele2ApiResult.packageLimit]
+                usage = data["usage"]
+                remaining = data[Tele2ApiResult.remaining]
+
+                self.log(
+                    "Got result. Limit: %s, usage: %s, remaining: %s, unlimited: %s",
+                    limit,
+                    usage,
+                    remaining,
+                    data[Tele2ApiResult.unlimitedData],
+                )
+                self._data[RES_ERROR] = None
+
+                if Tele2ApiResult.unlimitedData in data:
+                    self._data[RES_UNLIMITED] = data[Tele2ApiResult.unlimitedData]
+
+                if Tele2ApiResult.buckets in data and len(data["buckets"]) > 0:
+                    bucket = data["buckets"][0]
+                    if Tele2ApiResult.startDate in bucket:
+                        startDate = datetime.datetime.strptime(
+                            bucket[Tele2ApiResult.startDate], "%Y-%m-%d"
+                        ).date()
+                        self._data[RES_PERIOD_START] = startDate
+                    if Tele2ApiResult.endDate in bucket:
+                        endDate = datetime.datetime.strptime(
+                            bucket[Tele2ApiResult.endDate], "%Y-%m-%d"
+                        ).date()
+                        self._data[RES_PERIOD_END] = endDate
+
+                self.tries = 0
+                self._data[RES_LIMIT] = limit
+                self._data[RES_USAGE] = usage
+                self._data[RES_DATA_LEFT] = remaining
+                self.log("Setting native value to: %d", remaining)
+                return self._data
+
+        except requests.exceptions.RequestException as e:
+            self._data[RES_ERROR] = e
             return self._data
 
         return {}
 
     def updateAuth(self) -> None:
         self.log("Updating authentication")
         self.session.post(self.AUTH_URL, data=self.CREDENTIALS)
```

### Comparing `pytele2api-0.1.4/pytele2api.egg-info/PKG-INFO` & `pytele2api-0.1.5/pytele2api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pytele2api
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library for communication with Tele2 My TSO
 Home-page: https://github.com/fredrikhaggbom/pytele2
 Author: Fredrik Häggbom
 Author-email: fredrik.haggbom@gmail.com
 License: MIT
-Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.5.tar.gz
 Keywords: tele2
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pytele2api-0.1.4/setup.py` & `pytele2api-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytele2api",
-    version="0.1.4",
+    version="0.1.5",
     author="Fredrik Häggbom",
     author_email="fredrik.haggbom@gmail.com",
     description="Python library for communication with Tele2 My TSO",
-    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.4.tar.gz",
+    download_url="https://github.com/fredrikhaggbom/pytele2/archive/refs/tags/0.1.5.tar.gz",
     keywords=["tele2"],
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredrikhaggbom/pytele2",
     packages=setuptools.find_packages(),
     install_requires=["requests", "datetime"],
```

