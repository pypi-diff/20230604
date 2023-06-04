# Comparing `tmp/caic_python-0.1.10.tar.gz` & `tmp/caic_python-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caic_python-0.1.10.tar", last modified: Sun Jun  4 21:01:16 2023, max compression
+gzip compressed data, was "caic_python-0.1.8.tar", last modified: Sun Jun  4 20:30:54 2023, max compression
```

## Comparing `caic_python-0.1.10.tar` & `caic_python-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 21:01:16.939571 caic_python-0.1.10/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-04 20:52:17.000000 caic_python-0.1.10/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     2465 2023-06-04 21:01:16.939438 caic_python-0.1.10/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      839 2023-06-04 20:52:17.000000 caic_python-0.1.10/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      648 2023-06-04 21:01:12.000000 caic_python-0.1.10/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-04 21:01:16.939610 caic_python-0.1.10/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 21:01:16.937058 caic_python-0.1.10/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 21:01:16.938592 caic_python-0.1.10/src/caic_python/
--rw-r--r--   0 gormo      (501) staff       (20)      511 2023-06-04 21:01:12.000000 caic_python-0.1.10/src/caic_python/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)     2117 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/__main__.py
--rw-r--r--   0 gormo      (501) staff       (20)     2830 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/_args.py
--rw-r--r--   0 gormo      (501) staff       (20)    24212 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/client.py
--rw-r--r--   0 gormo      (501) staff       (20)     3660 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/definitions.py
--rw-r--r--   0 gormo      (501) staff       (20)     4670 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/enums.py
--rw-r--r--   0 gormo      (501) staff       (20)      140 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)    16733 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/models.py
--rw-r--r--   0 gormo      (501) staff       (20)     1671 2023-06-04 20:52:17.000000 caic_python-0.1.10/src/caic_python/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 21:01:16.939268 caic_python-0.1.10/src/caic_python.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     2465 2023-06-04 21:01:16.000000 caic_python-0.1.10/src/caic_python.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      466 2023-06-04 21:01:16.000000 caic_python-0.1.10/src/caic_python.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-04 21:01:16.000000 caic_python-0.1.10/src/caic_python.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       54 2023-06-04 21:01:16.000000 caic_python-0.1.10/src/caic_python.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       12 2023-06-04 21:01:16.000000 caic_python-0.1.10/src/caic_python.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 20:30:54.257465 caic_python-0.1.8/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-05-27 16:17:26.000000 caic_python-0.1.8/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)      981 2023-06-04 20:30:54.257345 caic_python-0.1.8/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      839 2023-06-04 20:27:00.000000 caic_python-0.1.8/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      340 2023-06-04 20:30:50.000000 caic_python-0.1.8/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-04 20:30:54.257503 caic_python-0.1.8/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 20:30:54.255135 caic_python-0.1.8/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 20:30:54.256602 caic_python-0.1.8/src/caic_python/
+-rw-r--r--   0 gormo      (501) staff       (20)      510 2023-06-04 20:30:50.000000 caic_python-0.1.8/src/caic_python/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)     2117 2023-06-04 20:27:00.000000 caic_python-0.1.8/src/caic_python/__main__.py
+-rw-r--r--   0 gormo      (501) staff       (20)     2830 2023-06-04 20:27:00.000000 caic_python-0.1.8/src/caic_python/_args.py
+-rw-r--r--   0 gormo      (501) staff       (20)    24212 2023-06-04 20:27:00.000000 caic_python-0.1.8/src/caic_python/client.py
+-rw-r--r--   0 gormo      (501) staff       (20)     3660 2023-05-29 15:41:13.000000 caic_python-0.1.8/src/caic_python/definitions.py
+-rw-r--r--   0 gormo      (501) staff       (20)     4670 2023-05-29 15:41:13.000000 caic_python-0.1.8/src/caic_python/enums.py
+-rw-r--r--   0 gormo      (501) staff       (20)      140 2023-06-04 20:27:00.000000 caic_python-0.1.8/src/caic_python/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)    16733 2023-06-04 20:27:00.000000 caic_python-0.1.8/src/caic_python/models.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1671 2023-05-29 15:41:13.000000 caic_python-0.1.8/src/caic_python/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-04 20:30:54.257193 caic_python-0.1.8/src/caic_python.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)      981 2023-06-04 20:30:54.000000 caic_python-0.1.8/src/caic_python.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      466 2023-06-04 20:30:54.000000 caic_python-0.1.8/src/caic_python.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-04 20:30:54.000000 caic_python-0.1.8/src/caic_python.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       54 2023-06-04 20:30:54.000000 caic_python-0.1.8/src/caic_python.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       12 2023-06-04 20:30:54.000000 caic_python-0.1.8/src/caic_python.egg-info/top_level.txt
```

### Comparing `caic_python-0.1.10/LICENSE` & `caic_python-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caic_python-0.1.10/README.md` & `caic_python-0.1.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# caic-python
+# caic_python
 
 An async Python client for the [CAIC](https://avalanche.state.co.us) website data using the undocumented HTTP APIs.
 
-`caic-python` is capable of retrieving information on the following from the CAIC website:
+`caic_python` is capable of retrieving information on the following from the CAIC website:
 - Search field reports (aka observation reports) submitted to the CAIC website.
 - Search avalanche observation reports submitted as part of a field report.
 - Retrieve the CAIC's avalanche forecast on a given date.
 - Retrieve information on CAIC's defined backcountry zones and highway zones.
 - Retrieve individual observation objects of the following type:
     - Field Report
     - Avalanche Observation
     - Snowpack Observation
     - Weather Observation
 
-Read the [full documentation](https://gormo.co/caic-python/) for further details. It is also available locally via `make read-docs` or the `docs/` directory.
+Read the [full documentation](https://gormo.co/caic_python/) for further details. It is also available locally via `make read-docs` or the `docs/` directory.
```

### Comparing `caic_python-0.1.10/src/caic_python/__main__.py` & `caic_python-0.1.8/src/caic_python/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""A CLI entry point for caic-python - meant for testing."""
+"""A CLI entry point for caic_python - meant for testing."""
 
 import asyncio
 from pprint import pprint
 import sys
 
 from . import __version__
 from ._args import MAIN_PARSER
 from .client import CaicClient
 
 
 async def main():
-    """The caic-python CLI function."""
+    """The caic_python CLI function."""
 
     args = MAIN_PARSER.parse_args()
 
     if args.version:
-        print(f"caic-python v{__version__}")
+        print(f"caic_python v{__version__}")
         sys.exit(0)
 
     client = CaicClient()
 
     match args.command:
         case "avy-obs":
             obs = await client.avy_obs(args.start.isoformat(), args.end.isoformat())
```

### Comparing `caic_python-0.1.10/src/caic_python/_args.py` & `caic_python-0.1.8/src/caic_python/_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 ID_PARSER = argparse.ArgumentParser(add_help=False)
 ID_PARSER.add_argument(
     "id", help="The ID (or slug if applicable) of the object to query for."
 )
 
 MAIN_PARSER = argparse.ArgumentParser(
-    description="The caic-python CLI.",
+    description="The caic_python CLI.",
     prog="python3 -m caic_python"
 )
 MAIN_PARSER.add_argument(
     "--debug",
     help="Display debug output.",
     action="store_true",
 )
```

### Comparing `caic_python-0.1.10/src/caic_python/client.py` & `caic_python-0.1.8/src/caic_python/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
 
 class CaicClient:
     """An async HTTP client for the CAIC API(s)."""
 
     def __init__(self) -> None:
         self.headers = {
-            "User-Agent": f"{aiohttp.http.SERVER_SOFTWARE} caic-python/{__version__}"
+            "User-Agent": f"{aiohttp.http.SERVER_SOFTWARE} caic_python/{__version__}"
         }
         self.session = aiohttp.ClientSession()
 
     async def close(self) -> None:
         """Close the underlying session."""
         await self.session.close()
```

### Comparing `caic_python-0.1.10/src/caic_python/definitions.py` & `caic_python-0.1.8/src/caic_python/definitions.py`

 * *Files identical despite different names*

### Comparing `caic_python-0.1.10/src/caic_python/enums.py` & `caic_python-0.1.8/src/caic_python/enums.py`

 * *Files identical despite different names*

### Comparing `caic_python-0.1.10/src/caic_python/models.py` & `caic_python-0.1.8/src/caic_python/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Pydantic models used by caic-python."""
+"""Pydantic models used by caic_python."""
 
 import datetime
 from typing import Literal, Optional, Union
 
 import pydantic
 
 from . import enums
```

### Comparing `caic_python-0.1.10/src/caic_python/utils.py` & `caic_python-0.1.8/src/caic_python/utils.py`

 * *Files identical despite different names*

