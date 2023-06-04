# Comparing `tmp/netteikei-0.4.1.tar.gz` & `tmp/netteikei-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netteikei-0.4.1.tar", last modified: Sun May 28 19:03:49 2023, max compression
+gzip compressed data, was "netteikei-0.4.2.tar", last modified: Sun Jun  4 19:13:16 2023, max compression
```

## Comparing `netteikei-0.4.1.tar` & `netteikei-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 19:03:33.000000 netteikei-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-28 19:03:49.687676 netteikei-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-28 19:03:33.000000 netteikei-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/netteikei/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/netteikei/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/contrib/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/contrib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-28 19:03:33.000000 netteikei-0.4.1/netteikei/typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 19:03:49.687676 netteikei-0.4.1/netteikei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 19:03:49.000000 netteikei-0.4.1/netteikei.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-28 19:03:33.000000 netteikei-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-28 19:03:49.691676 netteikei-0.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:13:16.047735 netteikei-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-04 19:13:01.000000 netteikei-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 19:13:16.047735 netteikei-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-04 19:13:01.000000 netteikei-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:13:16.043735 netteikei-0.4.2/netteikei/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:13:16.047735 netteikei-0.4.2/netteikei/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/contrib/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/contrib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-04 19:13:01.000000 netteikei-0.4.2/netteikei/typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 19:13:16.043735 netteikei-0.4.2/netteikei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-04 19:13:16.000000 netteikei-0.4.2/netteikei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-04 19:13:16.000000 netteikei-0.4.2/netteikei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 19:13:16.000000 netteikei-0.4.2/netteikei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 19:13:15.000000 netteikei-0.4.2/netteikei.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-04 19:13:16.000000 netteikei-0.4.2/netteikei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-04 19:13:16.000000 netteikei-0.4.2/netteikei.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-04 19:13:01.000000 netteikei-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-04 19:13:16.047735 netteikei-0.4.2/setup.cfg
```

### Comparing `netteikei-0.4.1/LICENSE` & `netteikei-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netteikei-0.4.1/PKG-INFO` & `netteikei-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.4.1
+Version: 0.4.2
 Summary: Utility for making concurrent HTTP requests with aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
```

### Comparing `netteikei-0.4.1/netteikei/contrib/download.py` & `netteikei-0.4.2/netteikei/contrib/download.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,87 @@
 import asyncio
 from contextvars import ContextVar
 from pathlib import Path
 from typing import NamedTuple, Self, Unpack
 
 import aiofiles
 from aiohttp import ClientResponse, ClientSession
+from aiohttp.typedefs import LooseHeaders, StrOrURL
+import pyrfc6266
 import tqdm
 
 from .. import Client, Request
-from ..typedefs import SessionKwargs, StrOrURL
-from .utils import isfile, parse_name, parse_length, get_start_byte
+from ..typedefs import SessionKwargs
+from .utils import getsize, isfile
 
 
-__all__ = ["download"]
-
 download_dir: ContextVar[Path] = ContextVar("dir")
 
 
-class DownloadAlreadyExists(Exception):
+class DuplicateDownloadError(Exception):
     
     def __init__(self, path: Path) -> None:
         self.path = path
 
     def __str__(self) -> str:
         return f"Download has already been saved in {self.path}."
 
+        
+def _parse_name(res: ClientResponse, default: str) -> str:
+    if (s := res.headers.get("Content-Disposition")) is None:
+        return res.url.name
+    else:
+        if (name := pyrfc6266.parse_filename(s)) is None:
+            return default
+        return name
+
+
+def _parse_length(headers: LooseHeaders) -> int | None:
+    if (s := headers.get("Content-Length")) is not None:
+        return int(s)
+    return
+
+
+async def _get_start_offset(headers: LooseHeaders, file: Path) -> int:
+    if headers.get("Accept-Ranges") == "bytes" and await isfile(file):
+        return await getsize(file)
+    return 0
+
 
-class DownloadInfo(NamedTuple):
+class Properties(NamedTuple):
     url: StrOrURL
     path: Path
     length: int | None
-    start: int
+    offset: int
 
     @classmethod
-    async def find(cls, session: ClientSession, url: StrOrURL, /) -> Self:
-        async with session.head(url, allow_redirects=True) as resp:
-            name = parse_name(resp, "untitled")
-            length = parse_length(resp.headers)
+    async def fetch(cls, session: ClientSession, url: StrOrURL) -> Self:
+        async with session.head(url, allow_redirects=True) as res:
+            name = _parse_name(res, "untitled")
+            length = _parse_length(res.headers)
             path = download_dir.get() / name
-            start = await get_start_byte(resp.headers, path)
+            offset = await _get_start_offset(res.headers, path)
 
             # Throw an error if the file already exists and isn't empty.
-            if await isfile(path) and 0 < start == length:
-                raise DownloadAlreadyExists(path)
+            if await isfile(path) and 0 < offset == length:
+                raise DuplicateDownloadError(path)
 
-            return cls(url, path, length, start)
+            return cls(url, path, length, offset)
 
 
-async def handle_req(info: DownloadInfo) -> Request:
-    # Do not send redundant headers when starting a download from the
-    # beginning of a file.
-    headers = {} if info.start == 0 else {"Range": f"bytes={info.start}-"} 
-    return Request.new(url=info.url, headers=headers)
+async def handle_req(prop: Properties) -> Request:
+    # Do not send redundant headers when starting a new download.
+    headers = {} if prop.offset == 0 else {"Range": f"bytes={prop.offset}-"}
+    return Request.new(url=prop.url, headers=headers)
 
-async def handle_res(info: DownloadInfo, res: ClientResponse) -> None:
-    async with res, aiofiles.open(info.path, "ab") as fp:
+async def handle_res(prop: Properties, res: ClientResponse) -> None:
+    async with res, aiofiles.open(prop.path, "ab") as fp:
         with tqdm.tqdm(
-            total=info.length,
-            initial=info.start,
+            total=prop.length,
+            initial=prop.offset,
             unit="B",
             unit_scale=True,
             unit_divisor=1024
         ) as bar:
             async for chunk in res.content.iter_any():
                 progress = await fp.write(chunk)
                 bar.update(progress)
@@ -79,22 +99,22 @@
     Parameters
     ----------
     dir
         Directory where downloads will be stored.
     *urls
         URLs to download from.
     **opts
-        Initialization options for the underlying `aiohttp.ClientSession`.
+        Init options for the underlying `aiohttp.ClientSession`.
 
     Raises
     ------
-    DownloadAlreadyExists
+    DuplicateDownloadError
         Raised when the file has already been downloaded.
     """
     token = download_dir.set(dir)
     async with ClientSession(**kwargs) as session:
-        info = await asyncio.gather(
-            *(DownloadInfo.find(session, url) for url in urls)
+        props: list[Properties] = await asyncio.gather(
+            *(Properties.fetch(session, url) for url in urls)
         )
-        client = Client(handlers=(handle_req, handle_res), max_workers=limit)
-        await client.run(session, info)
+        client = Client(handlers=(handle_req, handle_res), limit=limit)
+        await client.run(session, props, return_exceptions=True)
     download_dir.reset(token)
```

### Comparing `netteikei-0.4.1/netteikei/core.py` & `netteikei-0.4.2/netteikei/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from collections.abc import Iterable
-from typing import Generic, final, overload
+from typing import Generic, Literal, final, overload
 
 from aiohttp import ClientSession
 
-from .typedefs import ReqHandler, ResHandler, T, U
+from .typedefs import RequestHandler, ResponseHandler, T, U
 
 
 @final
 class Client(Generic[T, U]):
     """Utility for making concurrent HTTP requests.
 
     Parameters
@@ -23,62 +23,62 @@
         used underneath.
 
         The response handler receieves a `aiohttp.ClientResponse` as its
         second argument which is processed into relevant data.
 
         Both handlers are asynchronous, and are called before and after
         each request made respectively.
-    max_workers, default 5
-        Number of request workers that can run concurrently.
+    limit, default 10
+        Number of requests that can run concurrently.
 
     Methods
     -------
     run(session, objs, return_exceptions=False)
     """
     def __init__(
         self,
         *,
-        handlers: tuple[ReqHandler[T], ResHandler[T, U]],
-        max_workers: int = 5
+        handlers: tuple[RequestHandler[T], ResponseHandler[T, U]],
+        limit: int = 10
     ) -> None:
-        self._semaphore = asyncio.Semaphore(max_workers)
+        self._semaphore = asyncio.Semaphore(limit)
         self._req_handler, self._res_handler = handlers
     
     async def _request(self, session: ClientSession, obj: T) -> U:
         async with self._semaphore:
             method, url, kwargs = await self._req_handler(obj)
             async with session.request(method, url, **kwargs) as res:
                 return await self._res_handler(obj, res)
 
     @overload
     async def run(
         self,
         session: ClientSession,
         objs: Iterable[T],
         /,
-        return_exceptions: bool = False
+        return_exceptions: Literal[False] = False
     ) -> list[U]:
         ...
 
     @overload
     async def run(
         self,
         session: ClientSession,
         objs: Iterable[T],
         /,
-        return_exceptions: bool = True
+        return_exceptions: Literal[True]
     ) -> list[U | BaseException]:
         ...
 
     async def run(
         self,
         session: ClientSession,
         objs: Iterable[T],
         /,
-        return_exceptions: bool = False
+        return_exceptions: Literal[True, False] = False
     ) -> list[U] | list[U | BaseException]:
         """Make concurrent HTTP requests.
 
         Processes the given objects into relevant data using the user
         provided handlers.
 
         Parameters
```

### Comparing `netteikei-0.4.1/netteikei/typedefs.py` & `netteikei-0.4.2/netteikei/typedefs.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 
 class RequestKwargs(TypedDict, total=False):
     params: Mapping[str, str]
     data: Any
     json: Any
     headers: LooseHeaders
+    cookies: LooseCookies
     skip_auto_headers: Iterable[str]
     auth: BasicAuth
     allow_redirects: bool
     max_redirects: int
     compress: bool
     # Docs are ambiguious for this keyword.
     # chunked: bool
@@ -91,9 +92,9 @@
         **kwargs: Unpack[RequestKwargs]
     ) -> Self:
         return cls(method, url, kwargs)
 
 
 T, U = TypeVar("T"), TypeVar("U")
 
-ReqHandler = Callable[[T], Awaitable[Request]]
-ResHandler = Callable[[T, ClientResponse], Awaitable[U]]
+RequestHandler = Callable[[T], Awaitable[Request]]
+ResponseHandler = Callable[[T, ClientResponse], Awaitable[U]]
```

### Comparing `netteikei-0.4.1/netteikei.egg-info/PKG-INFO` & `netteikei-0.4.2/netteikei.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netteikei
-Version: 0.4.1
+Version: 0.4.2
 Summary: Utility for making concurrent HTTP requests with aiohttp
 Home-page: https://github.com/fernofsigma/netteikei
 Author: FernOfSigma
 Author-email: fernofsigma@tuta.io
 License: MIT
 Project-URL: GitHub: issues, https://github.com/fernofsigma/netteikei/issues
 Project-URL: GitHub: repo, https://github.com/fernofsigma/netteikei
```

### Comparing `netteikei-0.4.1/setup.cfg` & `netteikei-0.4.2/setup.cfg`

 * *Files identical despite different names*

