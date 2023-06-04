# Comparing `tmp/pychasing-0.1.7.tar.gz` & `tmp/pychasing-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychasing-0.1.7.tar", last modified: Sun Jun  4 03:55:46 2023, max compression
+gzip compressed data, was "pychasing-0.1.8.tar", last modified: Sun Jun  4 20:51:21 2023, max compression
```

## Comparing `pychasing-0.1.7.tar` & `pychasing-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.926287 pychasing-0.1.7/
--rw-rw-rw-   0        0        0     1101 2023-06-04 03:49:26.000000 pychasing-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     8389 2023-06-04 03:55:46.908335 pychasing-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     5817 2023-06-04 03:43:02.000000 pychasing-0.1.7/README.md
--rw-rw-rw-   0        0        0     1644 2023-06-04 03:54:12.000000 pychasing-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-04 03:55:46.926287 pychasing-0.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.555524 pychasing-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.755563 pychasing-0.1.7/src/pychasing/
--rw-rw-rw-   0        0        0     1443 2023-06-04 03:33:43.000000 pychasing-0.1.7/src/pychasing/__init__.py
--rw-rw-rw-   0        0        0    32528 2023-06-04 03:41:03.000000 pychasing-0.1.7/src/pychasing/client.py
--rw-rw-rw-   0        0        0    11369 2023-06-04 03:33:27.000000 pychasing-0.1.7/src/pychasing/enums.py
--rw-rw-rw-   0        0        0     1719 2023-01-04 19:14:40.000000 pychasing-0.1.7/src/pychasing/models.py
-drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.877908 pychasing-0.1.7/src/pychasing.egg-info/
--rw-rw-rw-   0        0        0     8389 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.906341 pychasing-0.1.7/tests/
--rw-rw-rw-   0        0        0     6569 2022-12-04 22:40:02.000000 pychasing-0.1.7/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:51:21.277369 pychasing-0.1.8/
+-rw-rw-rw-   0        0        0     1101 2023-06-04 03:49:26.000000 pychasing-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     8389 2023-06-04 20:51:21.276374 pychasing-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5817 2023-06-04 03:43:02.000000 pychasing-0.1.8/README.md
+-rw-rw-rw-   0        0        0     1646 2023-06-04 20:50:24.000000 pychasing-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 20:51:21.277369 pychasing-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 20:51:21.212543 pychasing-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 20:51:21.242462 pychasing-0.1.8/src/pychasing/
+-rw-rw-rw-   0        0        0     1443 2023-06-04 20:50:40.000000 pychasing-0.1.8/src/pychasing/__init__.py
+-rw-rw-rw-   0        0        0    32892 2023-06-04 20:45:39.000000 pychasing-0.1.8/src/pychasing/client.py
+-rw-rw-rw-   0        0        0    11369 2023-06-04 03:33:27.000000 pychasing-0.1.8/src/pychasing/enums.py
+-rw-rw-rw-   0        0        0     1723 2023-06-04 20:40:11.000000 pychasing-0.1.8/src/pychasing/models.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:51:21.273380 pychasing-0.1.8/src/pychasing.egg-info/
+-rw-rw-rw-   0        0        0     8389 2023-06-04 20:51:21.000000 pychasing-0.1.8/src/pychasing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-04 20:51:21.000000 pychasing-0.1.8/src/pychasing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 20:51:21.000000 pychasing-0.1.8/src/pychasing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-04 20:51:21.000000 pychasing-0.1.8/src/pychasing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 20:51:21.000000 pychasing-0.1.8/src/pychasing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 20:51:21.274377 pychasing-0.1.8/tests/
+-rw-rw-rw-   0        0        0     6569 2022-12-04 22:40:02.000000 pychasing-0.1.8/tests/test.py
```

### Comparing `pychasing-0.1.7/LICENSE` & `pychasing-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pychasing-0.1.7/PKG-INFO` & `pychasing-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychasing
-Version: 0.1.7
+Version: 0.1.8
 Summary: Short description
 Author-email: "Tanner B. Corcoran" <tannerbcorcoran@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 Tanner B. Corcoran
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pychasing-0.1.7/README.md` & `pychasing-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pychasing-0.1.7/pyproject.toml` & `pychasing-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # [project] spec: https://peps.python.org/pep-0621/#details
 name = "pychasing"
 description = "Short description"
-version = "0.1.7"
+version = "0.1.8"
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = ["a", "b", "c"]
 authors = [
     { name = "Tanner B. Corcoran", email = "tannerbcorcoran@gmail.com" },
 ]
 requires-python = ">=3.7"
@@ -51,8 +51,8 @@
     "http-prep >= 0.0.6",
     "rlim >= 0.0.2",
 ]
 
 [project.urls]
 repository = "https://github.com/tanrbobanr/pychasing"
 documentation = "https://github.com/tanrbobanr/pychasing/blob/main/README.md"
-changelog = "https://github.com/tanrbobanr/pychasing/blob/main/changelog.md"
+changelog = "https://github.com/tanrbobanr/pychasing/blob/main/changelog.md"
```

### Comparing `pychasing-0.1.7/src/pychasing/__init__.py` & `pychasing-0.1.8/src/pychasing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 __title__ = "pychasing"
 __author__ = "Tanner B. Corcoran"
 __email__ = "tannerbcorcoran@gmail.com"
 __license__ = "MIT License"
 __copyright__ = "Copyright (c) 2022 Tanner B. Corcoran"
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __description__ = "A full-functionality wrapper for the https://ballchasing.com API"
 __url__ = "https://github.com/tanrbobanr/pychasing"
 __download_url__ = "https://pypi.org/project/pychasing/"
 
 
 __all__ = (
     "Client",
```

### Comparing `pychasing-0.1.7/src/pychasing/client.py` & `pychasing-0.1.8/src/pychasing/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,32 +67,39 @@
     return v if v == ... or isinstance(v, str) else v.value
 
 
 class Client:
     """The main class used to interact with the Ballchasing API.
     
     """
-    def __init__(self, token: str, auto_rate_limit: bool, patreon_tier: enums.PatreonTier,
+    def __init__(self, token: str, auto_rate_limit: bool = True,
+                 patreon_tier: Union[str, enums.PatreonTier] = enums.PatreonTier.none,
                  rate_limit_safe_start: bool = False) -> None:
         """
         Arguments
         ---------
         token : str
             A ballchasing API key (acquirable from https://ballchasing.com/upload).
         auto_rate_limit : bool
             If `True`, the client will automatically limit API calls according to the given Patreon
             tier.
-        patreon_tier : enums.PatreonTier
+        patreon_tier : enums.PatreonTier or str, optional, default=PatreonTier.none
             The token-holder's Ballchasing Patreon tier.
         rate_limit_safe_start : bool, optional, default=False
             If `True`, the rate limiter will start out as fully maxed out on API calls.
 
         """
-        
+
         self._token = token
+        if isinstance(patreon_tier, str):
+            try:
+                patreon_tier = enums.PatreonTier[patreon_tier]
+            except KeyError as exc:
+                raise ValueError(f"{patreon_tier!r} is not a valid PatreonTier") from exc
+            
         if auto_rate_limit:
             for k, v in patreon_tier.value.items():
                 rlim.set_rate_limiter(getattr(self, k.name),
                                       rlim.RateLimiter(*v, safestart=rate_limit_safe_start))
     
     def ping(self, *, print_error: bool = True) -> requests.Response:
         """Ping the https://ballchasing.com servers.
```

### Comparing `pychasing-0.1.7/src/pychasing/enums.py` & `pychasing-0.1.8/src/pychasing/enums.py`

 * *Files identical despite different names*

### Comparing `pychasing-0.1.7/src/pychasing/models.py` & `pychasing-0.1.8/src/pychasing/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         minute : int, optional, default=0
         second : int, optional, default=0
         
         """
     def __new__(cls: "Date", year: int, month: int, day: int, hour: int = ...,
                 minute: int = ..., second: int = ...) -> "Date":
         return (f"{year}-{month:02}-{day:02}T{hour!=... and hour or 0:02}:"
-                f"{minute!=... and minute or 0:02}:"
-                f"{second!=... and second or 0:02}Z")
+                f"{minute != ... and minute or 0:02}:"
+                f"{second != ... and second or 0:02}Z")
 
 
 class ReplayBuffer(io.BufferedReader):
     """An object that can be used to store a replay file in-memory before uploading.
     
     """
     def __init__(self, name: str, raw: bytes = ..., buffer_size: int = ...) -> None:
```

### Comparing `pychasing-0.1.7/src/pychasing.egg-info/PKG-INFO` & `pychasing-0.1.8/src/pychasing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychasing
-Version: 0.1.7
+Version: 0.1.8
 Summary: Short description
 Author-email: "Tanner B. Corcoran" <tannerbcorcoran@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 Tanner B. Corcoran
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pychasing-0.1.7/tests/test.py` & `pychasing-0.1.8/tests/test.py`

 * *Files identical despite different names*

