# Comparing `tmp/nats-py-2.3.0.tar.gz` & `tmp/nats-py-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats-py-2.3.0.tar", last modified: Sat Jun  3 03:17:03 2023, max compression
+gzip compressed data, was "nats-py-2.3.1.tar", last modified: Sun Jun  4 07:06:34 2023, max compression
```

## Comparing `nats-py-2.3.0.tar` & `nats-py-2.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.448949 nats-py-2.3.0/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11357 2022-10-01 06:36:07.000000 nats-py-2.3.0/LICENSE
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    21002 2023-06-03 03:17:03.449064 nats-py-2.3.0/PKG-INFO
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7209 2023-06-03 03:16:18.000000 nats-py-2.3.0/README.md
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.442594 nats-py-2.3.0/nats/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1282 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/__init__.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.444033 nats-py-2.3.0/nats/aio/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/aio/__init__.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    77099 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/client.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4050 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/errors.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8450 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/msg.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    12256 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/subscription.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8164 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/aio/transport.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4269 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/errors.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.445350 nats-py-2.3.0/nats/js/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      765 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/__init__.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    19338 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/api.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    40535 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/client.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6913 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/errors.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    14722 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/kv.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11923 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/manager.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    17500 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/js/object_store.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2210 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/nuid.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.445878 nats-py-2.3.0/nats/protocol/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/protocol/__init__.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      825 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/protocol/command.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7401 2023-06-03 03:16:18.000000 nats-py-2.3.0/nats/protocol/parser.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats/py.typed
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.446976 nats-py-2.3.0/nats_py.egg-info/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    21002 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/PKG-INFO
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      808 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/SOURCES.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/dependency_links.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)       65 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/requires.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        5 2023-06-03 03:17:03.000000 nats-py-2.3.0/nats_py.egg-info/top_level.txt
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2022-10-01 06:36:07.000000 nats-py-2.3.0/nats_py.egg-info/zip-safe
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1816 2023-06-03 03:16:18.000000 nats-py-2.3.0/pyproject.toml
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)       70 2023-06-03 03:17:03.449296 nats-py-2.3.0/setup.cfg
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)      273 2023-06-03 03:16:18.000000 nats-py-2.3.0/setup.py
-drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-03 03:17:03.448817 nats-py-2.3.0/tests/
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)    84977 2023-06-03 03:16:18.000000 nats-py-2.3.0/tests/test_client.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6309 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_async_await.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     3944 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_nkeys.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2927 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_v2.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     3530 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_client_websocket.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)   106446 2023-06-03 03:16:18.000000 nats-py-2.3.0/tests/test_js.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2398 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_nuid.py
--rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6805 2022-10-01 06:36:07.000000 nats-py-2.3.0/tests/test_parser.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.470986 nats-py-2.3.1/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11357 2022-10-01 06:36:07.000000 nats-py-2.3.1/LICENSE
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    21053 2023-06-04 07:06:34.471077 nats-py-2.3.1/PKG-INFO
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7209 2023-06-03 03:16:18.000000 nats-py-2.3.1/README.md
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.465788 nats-py-2.3.1/nats/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1314 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/__init__.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.466832 nats-py-2.3.1/nats/aio/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.3.1/nats/aio/__init__.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    77393 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/aio/client.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4050 2023-06-03 03:16:18.000000 nats-py-2.3.1/nats/aio/errors.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8515 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/aio/msg.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    12292 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/aio/subscription.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     8241 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/aio/transport.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     4269 2022-10-01 06:36:07.000000 nats-py-2.3.1/nats/errors.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.467801 nats-py-2.3.1/nats/js/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      765 2023-06-03 03:16:18.000000 nats-py-2.3.1/nats/js/__init__.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    19647 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/js/api.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    40698 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/js/client.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6962 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/js/errors.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    14771 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/js/kv.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    11987 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/js/manager.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    17509 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/js/object_store.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2210 2023-06-03 03:16:18.000000 nats-py-2.3.1/nats/nuid.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.468283 nats-py-2.3.1/nats/protocol/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      581 2022-10-01 06:36:07.000000 nats-py-2.3.1/nats/protocol/__init__.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      825 2023-06-03 03:16:18.000000 nats-py-2.3.1/nats/protocol/command.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     7407 2023-06-04 07:06:27.000000 nats-py-2.3.1/nats/protocol/parser.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        0 2022-10-01 06:36:07.000000 nats-py-2.3.1/nats/py.typed
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.469095 nats-py-2.3.1/nats_py.egg-info/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    21053 2023-06-04 07:06:34.000000 nats-py-2.3.1/nats_py.egg-info/PKG-INFO
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      808 2023-06-04 07:06:34.000000 nats-py-2.3.1/nats_py.egg-info/SOURCES.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2023-06-04 07:06:34.000000 nats-py-2.3.1/nats_py.egg-info/dependency_links.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)       65 2023-06-04 07:06:34.000000 nats-py-2.3.1/nats_py.egg-info/requires.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        5 2023-06-04 07:06:34.000000 nats-py-2.3.1/nats_py.egg-info/top_level.txt
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)        1 2022-10-01 06:36:07.000000 nats-py-2.3.1/nats_py.egg-info/zip-safe
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     1862 2023-06-04 07:06:27.000000 nats-py-2.3.1/pyproject.toml
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)       70 2023-06-04 07:06:34.471299 nats-py-2.3.1/setup.cfg
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)      273 2023-06-03 03:16:18.000000 nats-py-2.3.1/setup.py
+drwxr-xr-x   0 waldemarquevedo   (501) staff       (20)        0 2023-06-04 07:06:34.470858 nats-py-2.3.1/tests/
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)    84977 2023-06-03 03:16:18.000000 nats-py-2.3.1/tests/test_client.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6309 2022-10-01 06:36:07.000000 nats-py-2.3.1/tests/test_client_async_await.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     3944 2022-10-01 06:36:07.000000 nats-py-2.3.1/tests/test_client_nkeys.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2927 2022-10-01 06:36:07.000000 nats-py-2.3.1/tests/test_client_v2.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     3992 2023-06-04 07:06:27.000000 nats-py-2.3.1/tests/test_client_websocket.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)   106617 2023-06-04 07:06:27.000000 nats-py-2.3.1/tests/test_js.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     2398 2022-10-01 06:36:07.000000 nats-py-2.3.1/tests/test_nuid.py
+-rw-r--r--   0 waldemarquevedo   (501) staff       (20)     6805 2022-10-01 06:36:07.000000 nats-py-2.3.1/tests/test_parser.py
```

### Comparing `nats-py-2.3.0/LICENSE` & `nats-py-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/PKG-INFO` & `nats-py-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py
-Version: 2.3.0
+Version: 2.3.1
 Summary: NATS client for Python
 Author-email: Waldemar Quevedo <wally@synadia.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,14 +211,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: nkeys
 Provides-Extra: aiohttp
 Provides-Extra: fast_parse
 License-File: LICENSE
```

### Comparing `nats-py-2.3.0/README.md` & `nats-py-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/__init__.py` & `nats-py-2.3.1/nats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from __future__ import annotations
 
+from typing import List, Union
 from .aio.client import Client as NATS
 
 
 async def connect(
-    servers: str | list[str] = ["nats://localhost:4222"], **options
+    servers: Union[List[str]] = ["nats://localhost:4222"], **options
 ) -> NATS:
     """
     :param servers: List of servers to connect.
     :param options: NATS connect options.
 
     ::
```

### Comparing `nats-py-2.3.0/nats/aio/__init__.py` & `nats-py-2.3.1/nats/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/aio/client.py` & `nats-py-2.3.1/nats/aio/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 from secrets import token_hex
 from typing import (
     Any,
     Awaitable,
     Callable,
     Tuple,
     Union,
+    List,
+    Optional,
+    Dict,
 )
 from urllib.parse import ParseResult, urlparse
 
 try:
     from fast_mail_parser import parse_email
 except ImportError:
     parse_email = None
@@ -57,15 +60,15 @@
 from .subscription import (
     DEFAULT_SUB_PENDING_BYTES_LIMIT,
     DEFAULT_SUB_PENDING_MSGS_LIMIT,
     Subscription,
 )
 from .transport import TcpTransport, Transport, WebSocketTransport
 
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 __lang__ = 'python3'
 _logger = logging.getLogger(__name__)
 PROTOCOL = 1
 
 INFO_OP = b'INFO'
 CONNECT_OP = b'CONNECT'
 PING_OP = b'PING'
@@ -111,29 +114,29 @@
 @dataclass
 class Srv:
     """
     Srv is a helper data structure to hold state of a server.
     """
     uri: ParseResult
     reconnects: int = 0
-    last_attempt: float | None = None
+    last_attempt: Optional[float] = None
     did_connect: bool = False
     discovered: bool = False
-    tls_name: str | None = None
-    server_version: str | None = None
+    tls_name: Optional[str] = None
+    server_version: Optional[str] = None
 
 
 class ServerVersion:
 
     def __init__(self, server_version: str) -> None:
         self._server_version = server_version
-        self._major_version: int | None = None
-        self._minor_version: int | None = None
-        self._patch_version: int | None = None
-        self._dev_version: str | None = None
+        self._major_version: Optional[int] = None
+        self._minor_version: Optional[int] = None
+        self._patch_version: Optional[int] = None
+        self._dev_version: Optional[str] = None
 
     # TODO(@orsinium): use cached_property
     def parse_version(self) -> None:
         v = (self._server_version).split('-')
         if len(v) > 1:
             self._dev_version = v[1]
         tokens = v[0].split('.')
@@ -197,125 +200,125 @@
     DRAINING_SUBS = 5
     DRAINING_PUBS = 6
 
     def __repr__(self) -> str:
         return f"<nats client v{__version__}>"
 
     def __init__(self) -> None:
-        self._current_server: Srv | None = None
-        self._server_info: dict[str, Any] = {}
-        self._server_pool: list[Srv] = []
-        self._reading_task: asyncio.Task | None = None
-        self._ping_interval_task: asyncio.Task | None = None
+        self._current_server: Optional[Srv] = None
+        self._server_info: Dict[str, Any] = {}
+        self._server_pool: List[Srv] = []
+        self._reading_task: Optional[asyncio.Task] = None
+        self._ping_interval_task: Optional[asyncio.Task] = None
         self._pings_outstanding: int = 0
         self._pongs_received: int = 0
-        self._pongs: list[asyncio.Future] = []
-        self._transport: Transport | None = None
-        self._err: Exception | None = None
+        self._pongs: List[asyncio.Future] = []
+        self._transport: Optional[Transport] = None
+        self._err: Optional[Exception] = None
 
         # callbacks
         self._error_cb: ErrorCallback = _default_error_callback
-        self._disconnected_cb: Callback | None = None
-        self._closed_cb: Callback | None = None
-        self._discovered_server_cb: Callback | None = None
-        self._reconnected_cb: Callback | None = None
+        self._disconnected_cb: Optional[Callback] = None
+        self._closed_cb: Optional[Callback] = None
+        self._discovered_server_cb: Optional[Callback] = None
+        self._reconnected_cb: Optional[Callback] = None
 
-        self._reconnection_task: asyncio.Task[None] | None = None
-        self._reconnection_task_future: asyncio.Future | None = None
+        self._reconnection_task: Optional[asyncio.Task[None]] = None
+        self._reconnection_task_future: Optional[asyncio.Future] = None
         self._max_payload: int = DEFAULT_MAX_PAYLOAD_SIZE
 
         # client id that the NATS server knows about.
-        self._client_id: int | None = None
+        self._client_id: Optional[int] = None
         self._sid: int = 0
-        self._subs: dict[int, Subscription] = {}
+        self._subs: Dict[int, Subscription] = {}
         self._status: int = Client.DISCONNECTED
         self._ps: Parser = Parser(self)
 
         # pending queue of commands that will be flushed to the server.
-        self._pending: list[bytes] = []
+        self._pending: List[bytes] = []
 
         # current size of pending data in total.
         self._pending_data_size: int = 0
 
         # max pending size is the maximum size of the data that can be buffered.
         self._max_pending_size: int = 0
 
-        self._flush_queue: asyncio.Queue[asyncio.Future[Any]] | None = None
-        self._flusher_task: asyncio.Task | None = None
-        self._flush_timeout: float | None = 0
+        self._flush_queue: Optional[asyncio.Queue[asyncio.Future[Any]]] = None
+        self._flusher_task: Optional[asyncio.Task] = None
+        self._flush_timeout: Optional[float] = 0
         self._hdr_parser: BytesParser = BytesParser()
 
         # New style request/response
-        self._resp_map: dict[str, asyncio.Future] = {}
-        self._resp_sub_prefix: bytearray | None = None
+        self._resp_map: Dict[str, asyncio.Future] = {}
+        self._resp_sub_prefix: Optional[bytearray] = None
         self._nuid = NUID()
         self._inbox_prefix = bytearray(DEFAULT_INBOX_PREFIX)
         self._auth_configured: bool = False
 
         # NKEYS support
         #
         # user_jwt_cb is used to fetch and return the account
         # signed JWT for this user.
-        self._user_jwt_cb: JWTCallback | None = None
+        self._user_jwt_cb: Optional[JWTCallback] = None
 
         # signature_cb is used to sign a nonce from the server while
         # authenticating with nkeys. The user should sign the nonce and
         # return the base64 encoded signature.
-        self._signature_cb: SignatureCallback | None = None
+        self._signature_cb: Optional[SignatureCallback] = None
 
         # user credentials file can be a tuple or single file.
-        self._user_credentials: Credentials | None = None
+        self._user_credentials: Optional[Credentials] = None
 
         # file that contains the nkeys seed and its public key as a string.
-        self._nkeys_seed: str | None = None
-        self._public_nkey: str | None = None
+        self._nkeys_seed: Optional[str] = None
+        self._public_nkey: Optional[str] = None
 
-        self.options: dict[str, Any] = {}
+        self.options: Dict[str, Any] = {}
         self.stats = {
             'in_msgs': 0,
             'out_msgs': 0,
             'in_bytes': 0,
             'out_bytes': 0,
             'reconnects': 0,
             'errors_received': 0,
         }
 
     async def connect(
         self,
-        servers: str | list[str] = ["nats://localhost:4222"],
-        error_cb: ErrorCallback | None = None,
-        disconnected_cb: Callback | None = None,
-        closed_cb: Callback | None = None,
-        discovered_server_cb: Callback | None = None,
-        reconnected_cb: Callback | None = None,
-        name: str | None = None,
+        servers: Union[str, List[str]] = ["nats://localhost:4222"],
+        error_cb: Optional[ErrorCallback] = None,
+        disconnected_cb: Optional[Callback] = None,
+        closed_cb: Optional[Callback] = None,
+        discovered_server_cb: Optional[Callback] = None,
+        reconnected_cb: Optional[Callback] = None,
+        name: Optional[str] = None,
         pedantic: bool = False,
         verbose: bool = False,
         allow_reconnect: bool = True,
         connect_timeout: int = DEFAULT_CONNECT_TIMEOUT,
         reconnect_time_wait: int = DEFAULT_RECONNECT_TIME_WAIT,
         max_reconnect_attempts: int = DEFAULT_MAX_RECONNECT_ATTEMPTS,
         ping_interval: int = DEFAULT_PING_INTERVAL,
         max_outstanding_pings: int = DEFAULT_MAX_OUTSTANDING_PINGS,
         dont_randomize: bool = False,
         flusher_queue_size: int = DEFAULT_MAX_FLUSHER_QUEUE_SIZE,
         no_echo: bool = False,
-        tls: ssl.SSLContext | None = None,
-        tls_hostname: str | None = None,
-        user: str | None = None,
-        password: str | None = None,
-        token: str | None = None,
+        tls: Optional[ssl.SSLContext] = None,
+        tls_hostname: Optional[str] = None,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        token: Optional[str] = None,
         drain_timeout: int = DEFAULT_DRAIN_TIMEOUT,
-        signature_cb: SignatureCallback | None = None,
-        user_jwt_cb: JWTCallback | None = None,
-        user_credentials: Credentials | None = None,
-        nkeys_seed: str | None = None,
-        inbox_prefix: str | bytes = DEFAULT_INBOX_PREFIX,
+        signature_cb: Optional[SignatureCallback] = None,
+        user_jwt_cb: Optional[JWTCallback] = None,
+        user_credentials: Optional[Credentials] = None,
+        nkeys_seed: Optional[str] = None,
+        inbox_prefix: Union[str, bytes] = DEFAULT_INBOX_PREFIX,
         pending_size: int = DEFAULT_PENDING_SIZE,
-        flush_timeout: float | None = None,
+        flush_timeout: Optional[float] = None,
     ) -> None:
         """
         Establishes a connection to NATS.
 
         :param servers: NATS Connection
         :param name: Label the connection with name (shown in NATS monitoring)
         :param error_cb: Callback to report errors.
@@ -753,15 +756,15 @@
             await self._close(Client.CLOSED)
 
     async def publish(
         self,
         subject: str,
         payload: bytes = b'',
         reply: str = '',
-        headers: dict[str, str] | None = None
+        headers: Optional[Dict[str, str]] = None
     ) -> None:
         """
         Publishes a NATS message.
 
         :param subject: Subject to which the message will be published.
         :param payload: Message data.
         :param reply: Inbox to which a responder can respond.
@@ -824,15 +827,15 @@
 
     async def _send_publish(
         self,
         subject: str,
         reply: str,
         payload: bytes,
         payload_size: int,
-        headers: dict[str, Any] | None,
+        headers: Optional[Dict[str, Any]],
     ) -> None:
         """
         Sends PUB command to the NATS server.
         """
         if subject == "":
             # Avoid sending messages with empty replies.
             raise errors.BadSubjectError
@@ -863,16 +866,16 @@
         if self._flush_queue is not None and self._flush_queue.empty():
             await self._flush_pending()
 
     async def subscribe(
         self,
         subject: str,
         queue: str = "",
-        cb: Callable[[Msg], Awaitable[None]] | None = None,
-        future: asyncio.Future | None = None,
+        cb: Optional[Callable[[Msg], Awaitable[None]]] = None,
+        future: Optional[asyncio.Future] = None,
         max_msgs: int = 0,
         pending_msgs_limit: int = DEFAULT_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_SUB_PENDING_BYTES_LIMIT,
     ) -> Subscription:
         """
         subscribe registers interest in a given subject.
 
@@ -952,15 +955,15 @@
 
     async def request(
         self,
         subject: str,
         payload: bytes = b'',
         timeout: float = 0.5,
         old_style: bool = False,
-        headers: dict[str, Any] | None = None,
+        headers: Optional[Dict[str, Any]] = None,
     ) -> Msg:
         """
         Implements the request/response pattern via pub/sub
         using a single wildcard subscription that handles
         the responses.
 
         """
@@ -979,15 +982,15 @@
         return msg
 
     async def _request_new_style(
         self,
         subject: str,
         payload: bytes,
         timeout: float = 1,
-        headers: dict[str, Any] | None = None,
+        headers: Optional[Dict[str, Any]] = None,
     ) -> Msg:
         if self.is_draining_pubs:
             raise errors.ConnectionDrainingError
 
         if not self._resp_sub_prefix:
             await self._init_request_sub()
         assert self._resp_sub_prefix
@@ -1089,50 +1092,50 @@
             await self._send_ping(future)
             await asyncio.wait_for(future, timeout)
         except asyncio.TimeoutError:
             future.cancel()
             raise errors.FlushTimeoutError
 
     @property
-    def connected_url(self) -> ParseResult | None:
+    def connected_url(self) -> Optional[ParseResult]:
         if self._current_server and self.is_connected:
             return self._current_server.uri
         return None
 
     @property
-    def servers(self) -> list[ParseResult]:
+    def servers(self) -> List[ParseResult]:
         servers = []
         for srv in self._server_pool:
             servers.append(srv.uri)
         return servers
 
     @property
-    def discovered_servers(self) -> list[ParseResult]:
+    def discovered_servers(self) -> List[ParseResult]:
         servers = []
         for srv in self._server_pool:
             if srv.discovered:
                 servers.append(srv.uri)
         return servers
 
     @property
     def max_payload(self) -> int:
         """
         Returns the max payload which we received from the servers INFO
         """
         return self._max_payload
 
     @property
-    def client_id(self) -> int | None:
+    def client_id(self) -> Optional[int]:
         """
         Returns the client id which we received from the servers INFO
         """
         return self._client_id
 
     @property
-    def last_error(self) -> Exception | None:
+    def last_error(self) -> Optional[Exception]:
         """
         Returns the last error which may have occurred.
         """
         return self._err
 
     @property
     def pending_data_size(self) -> int:
@@ -1173,15 +1176,15 @@
         """
         if self._current_server and self._current_server.server_version:
             return ServerVersion(self._current_server.server_version)
         return ServerVersion("0.0.0-unknown")
 
     @property
     def ssl_context(self) -> ssl.SSLContext:
-        ssl_context: ssl.SSLContext | None = None
+        ssl_context: Optional[ssl.SSLContext] = None
         if "tls" in self.options:
             ssl_context = self.options.get('tls')
         else:
             ssl_context = ssl.create_default_context()
         if ssl_context is None:
             raise errors.Error('nats: no ssl context provided')
         return ssl_context
@@ -1216,15 +1219,15 @@
                 except asyncio.TimeoutError:
                     # Report to the async callback that there was a timeout.
                     await self._error_cb(errors.FlushTimeoutError())
 
         except asyncio.CancelledError:
             pass
 
-    def _setup_server_pool(self, connect_url: str | list[str]) -> None:
+    def _setup_server_pool(self, connect_url: Union[List[str]]) -> None:
         if isinstance(connect_url, str):
             try:
                 if "nats://" in connect_url or "tls://" in connect_url:
                     # Closer to how the Go client handles this.
                     # e.g. nats://localhost:4222
                     uri = urlparse(connect_url)
                 elif "ws://" in connect_url or "wss://" in connect_url:
@@ -1553,27 +1556,28 @@
         """
         if len(self._pongs) > 0:
             future = self._pongs.pop(0)
             future.set_result(True)
             self._pongs_received += 1
             self._pings_outstanding = 0
 
-    def _is_control_message(self, data, header: dict[str, str]) -> str | None:
+    def _is_control_message(self, data, header: Dict[str,
+                                                     str]) -> Optional[str]:
         if len(data) > 0:
             return None
         status = header.get(nats.js.api.Header.STATUS)
         if status == CTRL_STATUS:
             return header.get(nats.js.api.Header.DESCRIPTION)
         return None
 
-    async def _process_headers(self, headers) -> dict[str, str] | None:
+    async def _process_headers(self, headers) -> Optional[Dict[str, str]]:
         if not headers:
             return None
 
-        hdr: dict[str, str] | None = None
+        hdr: Optional[Dict[str, str]] = None
         raw_headers = headers[NATS_HDR_LINE_SIZE:]
 
         # If the first character is an empty space, then this is
         # an inline status message sent by the server.
         #
         # NATS/1.0 404\r\n\r\n
         # NATS/1.0 503\r\n\r\n
@@ -1786,15 +1790,15 @@
 
     def _build_message(
         self,
         sid: int,
         subject: bytes,
         reply: bytes,
         data: bytes,
-        headers: dict[str, str] | None,
+        headers: Optional[Dict[str, str]],
     ):
         return self.msg_class(
             subject=subject.decode(),
             reply=reply.decode(),
             data=data,
             headers=headers,
             _client=self,
@@ -1805,15 +1809,15 @@
         """
         Process disconnection from the server and set client status
         to DISCONNECTED.
         """
         self._status = Client.DISCONNECTED
 
     def _process_info(
-        self, info: dict[str, Any], initial_connection: bool = False
+        self, info: Dict[str, Any], initial_connection: bool = False
     ) -> None:
         """
         Process INFO lines sent by the server to reconfigure client
         with latest updates from cluster to enable server discovery.
         """
         assert self._current_server, "Client.connect must be called first"
         if 'connect_urls' in info:
@@ -1847,15 +1851,15 @@
                     shuffle(connect_urls)
                 for srv in connect_urls:
                     self._server_pool.append(srv)
 
                 if not initial_connection and connect_urls and self._discovered_server_cb:
                     self._discovered_server_cb()
 
-    def _host_is_ip(self, connect_url: str | None) -> bool:
+    def _host_is_ip(self, connect_url: Optional[str]) -> bool:
         if connect_url is None:
             return False
         try:
             ipaddress.ip_address(connect_url)
             return True
         except Exception:
             return False
@@ -1981,15 +1985,17 @@
         )
 
         # Task for kicking the flusher queue
         self._flusher_task = asyncio.get_running_loop().create_task(
             self._flusher()
         )
 
-    async def _send_ping(self, future: asyncio.Future | None = None) -> None:
+    async def _send_ping(
+        self, future: Optional[asyncio.Future] = None
+    ) -> None:
         assert self._transport, "Client.connect must be called first"
         if future is None:
             future = asyncio.Future()
         self._pongs.append(future)
         self._transport.write(PING_PROTO)
         self._pending_data_size += len(PING_PROTO)
         await self._flush_pending()
```

### Comparing `nats-py-2.3.0/nats/aio/errors.py` & `nats-py-2.3.1/nats/aio/errors.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/aio/msg.py` & `nats-py-2.3.1/nats/aio/msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # limitations under the License.
 #
 from __future__ import annotations
 
 import datetime
 import json
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List, Optional, Dict, Union
 
 from nats.errors import Error, MsgAlreadyAckdError, NotJSMessageError
 
 if TYPE_CHECKING:
     from nats import NATS
 
 # Subject without domain:
@@ -40,19 +40,19 @@
     """
     Msg represents a message delivered by NATS.
     """
     _client: NATS
     subject: str = ''
     reply: str = ''
     data: bytes = b''
-    headers: dict[str, str] | None = None
+    headers: Optional[Dict[str, str]] = None
 
-    _metadata: Metadata | None = None
+    _metadata: Optional[Metadata] = None
     _ackd: bool = False
-    _sid: int | None = None
+    _sid: Optional[int] = None
 
     class Ack:
         Ack = b"+ACK"
         Nak = b"-NAK"
         Progress = b"+WPI"
         Term = b"+TERM"
 
@@ -66,15 +66,15 @@
         NumDelivered = 6
         StreamSeq = 7
         ConsumerSeq = 8
         Timestamp = 9
         NumPending = 10
 
     @property
-    def header(self) -> dict | None:
+    def header(self) -> Optional[Dict[str, str]]:
         """
         header returns the headers from a message.
         """
         return self.headers
 
     @property
     def sid(self) -> int:
@@ -109,15 +109,15 @@
         ack_sync waits for the acknowledgement to be processed by the server.
         """
         self._check_reply()
         resp = await self._client.request(self.reply, timeout=timeout)
         self._ackd = True
         return resp
 
-    async def nak(self, delay: int | float | None = None) -> None:
+    async def nak(self, delay: Union[int, float, None] = None) -> None:
         """
         nak negatively acknowledges a message delivered by JetStream triggering a redelivery.
         if `delay` is provided, redelivery is delayed for `delay` seconds
         """
         self._check_reply()
         payload = Msg.Ack.Nak
         json_args = dict()
@@ -157,15 +157,15 @@
         metadata = self._metadata
         if metadata is not None:
             return metadata
         metadata = Msg.Metadata._from_reply(self.reply)
         self._metadata = metadata
         return metadata
 
-    def _get_metadata_fields(self, reply: str | None) -> list[str]:
+    def _get_metadata_fields(self, reply: Optional[str]) -> List[str]:
         return Msg.Metadata._get_metadata_fields(reply)
 
     def _check_reply(self) -> None:
         if self.reply is None or self.reply == '':
             raise NotJSMessageError
         if self._ackd:
             raise MsgAlreadyAckdError(self)
@@ -186,26 +186,26 @@
         """
         sequence: SequencePair
         num_pending: int
         num_delivered: int
         timestamp: datetime.datetime
         stream: str
         consumer: str
-        domain: str | None = None
+        domain: Optional[str] = None
 
         @dataclass(frozen=True)
         class SequencePair:
             """
             SequencePair represents a pair of consumer and stream sequence.
             """
             consumer: int
             stream: int
 
         @classmethod
-        def _get_metadata_fields(cls, reply: str | None) -> list[str]:
+        def _get_metadata_fields(cls, reply: Optional[str]) -> List[str]:
             if not reply:
                 raise NotJSMessageError
             tokens = reply.split('.')
             if (len(tokens) == _V1_TOKEN_COUNT or
                     len(tokens) >= _V2_TOKEN_COUNT-1) and \
                     tokens[0] == Msg.Ack.Prefix0 and \
                     tokens[1] == Msg.Ack.Prefix1:
```

### Comparing `nats-py-2.3.0/nats/aio/subscription.py` & `nats-py-2.3.1/nats/aio/subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 import asyncio
 from typing import (
     TYPE_CHECKING,
     AsyncIterator,
     Awaitable,
     Callable,
+    List,
+    Optional,
 )
 
 from nats import errors
 # Default Pending Limits of Subscriptions
 from nats.aio.msg import Msg
 
 if TYPE_CHECKING:
@@ -58,16 +60,16 @@
 
     def __init__(
         self,
         conn,
         id: int = 0,
         subject: str = '',
         queue: str = '',
-        cb: Callable[[Msg], Awaitable[None]] | None = None,
-        future: asyncio.Future | None = None,
+        cb: Optional[Callable[[Msg], Awaitable[None]]] = None,
+        future: Optional[asyncio.Future] = None,
         max_msgs: int = 0,
         pending_msgs_limit: int = DEFAULT_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_SUB_PENDING_BYTES_LIMIT,
     ) -> None:
         self._conn = conn
         self._id = id
         self._subject = subject
@@ -91,15 +93,15 @@
         else:
             self._pending_next_msgs_calls = None
         self._pending_size = 0
         self._wait_for_msgs_task = None
         self._message_iterator = None
 
         # For JetStream enabled subscriptions.
-        self._jsi: JetStreamContext._JSI | None = None
+        self._jsi: Optional[JetStreamContext._JSI] = None
 
     @property
     def subject(self) -> str:
         """
         Returns the subject of the `Subscription`.
         """
         return self._subject
@@ -145,15 +147,15 @@
     @property
     def delivered(self) -> int:
         """
         Number of delivered messages to this subscription so far.
         """
         return self._received
 
-    async def next_msg(self, timeout: float | None = 1.0) -> Msg:
+    async def next_msg(self, timeout: Optional[float] = 1.0) -> Msg:
         """
         :params timeout: Time in seconds to wait for next message before timing out.
         :raises nats.errors.TimeoutError:
 
         next_msg can be used to retrieve the next message from a stream of messages using
         await syntax, this only works when not passing a callback on `subscribe`::
 
@@ -339,15 +341,15 @@
             self._unsubscribed_future.set_result(True)
 
     def __aiter__(self) -> _SubscriptionMessageIterator:
         return self
 
     async def __anext__(self) -> Msg:
         get_task = asyncio.get_running_loop().create_task(self._queue.get())
-        tasks: list[asyncio.Future] = [get_task, self._unsubscribed_future]
+        tasks: List[asyncio.Future] = [get_task, self._unsubscribed_future]
         finished, _ = await asyncio.wait(
             tasks, return_when=asyncio.FIRST_COMPLETED
         )
         sub = self._sub
 
         if get_task in finished:
             self._queue.task_done()
```

### Comparing `nats-py-2.3.0/nats/aio/transport.py` & `nats-py-2.3.1/nats/aio/transport.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import abc
 import asyncio
 import ssl
 from urllib.parse import ParseResult
+from typing import List, Union, Optional
 
 try:
     import aiohttp
 except ImportError:
     aiohttp = None  # type: ignore[assignment]
 
 from nats.errors import ProtocolError
@@ -24,15 +25,15 @@
         obtained calling urllib.parse.urlparse.
         """
         pass
 
     @abc.abstractmethod
     async def connect_tls(
         self,
-        uri: str | ParseResult,
+        uri: Union[str, ParseResult],
         ssl_context: ssl.SSLContext,
         buffer_size: int,
         connect_timeout: int,
     ):
         """
         connect_tls is similar to connect except it tries to connect to a secure endpoint, using the provided ssl
         context. The uri can be provided as string in case the hostname differs from the uri hostname, in case it
@@ -44,15 +45,15 @@
     def write(self, payload: bytes):
         """
         Write bytes to underlying transport. Needs a call to drain() to be successfully written.
         """
         pass
 
     @abc.abstractmethod
-    def writelines(self, payload: list[bytes]):
+    def writelines(self, payload: List[bytes]):
         """
         Writes a list of bytes, one by one, to the underlying transport. Needs a call to drain() to be successfully
         written.
         """
         pass
 
     @abc.abstractmethod
@@ -105,18 +106,18 @@
         """
         pass
 
 
 class TcpTransport(Transport):
 
     def __init__(self):
-        self._bare_io_reader: asyncio.StreamReader | None = None
-        self._io_reader: asyncio.StreamReader | None = None
-        self._bare_io_writer: asyncio.StreamWriter | None = None
-        self._io_writer: asyncio.StreamWriter | None = None
+        self._bare_io_reader: Optional[asyncio.StreamReader] = None
+        self._io_reader: Optional[asyncio.StreamReader] = None
+        self._bare_io_writer: Optional[asyncio.StreamWriter] = None
+        self._io_writer: Optional[asyncio.StreamWriter] = None
 
     async def connect(
         self, uri: ParseResult, buffer_size: int, connect_timeout: int
     ):
         r, w = await asyncio.wait_for(
             asyncio.open_connection(
                 host=uri.hostname,
@@ -132,15 +133,15 @@
         #
         # See https://github.com/nats-io/asyncio-nats/issues/43
         self._bare_io_reader = self._io_reader = r
         self._bare_io_writer = self._io_writer = w
 
     async def connect_tls(
         self,
-        uri: str | ParseResult,
+        uri: Union[str, ParseResult],
         ssl_context: ssl.SSLContext,
         buffer_size: int,
         connect_timeout: int,
     ) -> None:
         assert self._io_writer, f'{type(self).__name__}.connect must be called first'
 
         # manually recreate the stream reader/writer with a tls upgraded transport
@@ -191,32 +192,32 @@
 class WebSocketTransport(Transport):
 
     def __init__(self):
         if not aiohttp:
             raise ImportError(
                 "Could not import aiohttp transport, please install it with `pip install aiohttp`"
             )
-        self._ws: aiohttp.ClientWebSocketResponse | None = None
+        self._ws: Optional[aiohttp.ClientWebSocketResponse] = None
         self._client: aiohttp.ClientSession = aiohttp.ClientSession()
         self._pending = asyncio.Queue()
         self._close_task = asyncio.Future()
-        self._using_tls: bool | None = None
+        self._using_tls: Optional[bool] = None
 
     async def connect(
         self, uri: ParseResult, buffer_size: int, connect_timeout: int
     ):
         # for websocket library, the uri must contain the scheme already
         self._ws = await self._client.ws_connect(
             uri.geturl(), timeout=connect_timeout
         )
         self._using_tls = False
 
     async def connect_tls(
         self,
-        uri: str | ParseResult,
+        uri: Union[str, ParseResult],
         ssl_context: ssl.SSLContext,
         buffer_size: int,
         connect_timeout: int,
     ):
         if self._ws and not self._ws.closed:
             if self._using_tls:
                 return
```

### Comparing `nats-py-2.3.0/nats/errors.py` & `nats-py-2.3.1/nats/errors.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/js/__init__.py` & `nats-py-2.3.1/nats/js/__init__.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/js/api.py` & `nats-py-2.3.1/nats/js/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # limitations under the License.
 #
 
 from __future__ import annotations
 
 from dataclasses import dataclass, fields, replace
 from enum import Enum
-from typing import Any, Dict, Optional, TypeVar
+from typing import Any, Dict, Optional, TypeVar, List
 
 _NANOSECOND = 10**9
 
 
 class Header(str, Enum):
     CONSUMER_STALLED = "Nats-Consumer-Stalled"
     DESCRIPTION = "Description"
@@ -53,45 +53,45 @@
 @dataclass
 class Base:
     """
     Helper dataclass to filter unknown fields from the API.
     """
 
     @staticmethod
-    def _convert(resp: dict[str, Any], field: str, type: type[Base]) -> None:
+    def _convert(resp: Dict[str, Any], field: str, type: type[Base]) -> None:
         """Convert the field into the given type in place.
         """
         data = resp.get(field, None)
         if data is None:
             resp[field] = None
         elif isinstance(data, list):
             resp[field] = [type.from_response(item) for item in data]
         else:
             resp[field] = type.from_response(data)
 
     @staticmethod
-    def _convert_nanoseconds(resp: dict[str, Any], field: str) -> None:
+    def _convert_nanoseconds(resp: Dict[str, Any], field: str) -> None:
         """Convert the given field from nanoseconds to seconds in place.
         """
         val = resp.get(field, None)
         if val is not None:
             val = val / _NANOSECOND
         resp[field] = val
 
     @staticmethod
-    def _to_nanoseconds(val: float | None) -> int | None:
+    def _to_nanoseconds(val: Optional[float]) -> Optional[int]:
         """Convert the value from seconds to nanoseconds.
         """
         if val is None:
             # We use 0 to avoid sending null to Go servers.
             return 0
         return int(val * _NANOSECOND)
 
     @classmethod
-    def from_response(cls: type[_B], resp: dict[str, Any]) -> _B:
+    def from_response(cls: type[_B], resp: Dict[str, Any]) -> _B:
         """Read the class instance from a server response.
 
         Unknown fields are ignored ("open-world assumption").
         """
         params = {}
         for field in fields(cls):
             if field.name in resp:
@@ -99,15 +99,15 @@
         return cls(**params)
 
     def evolve(self: _B, **params) -> _B:
         """Return a copy of the instance with the passed values replaced.
         """
         return replace(self, **params)
 
-    def as_dict(self) -> dict[str, object]:
+    def as_dict(self) -> Dict[str, object]:
         """Return the object converted into an API-friendly dict.
         """
         result = {}
         for field in fields(self):
             val = getattr(self, field.name)
             if val is None:
                 continue
@@ -120,74 +120,74 @@
 @dataclass
 class PubAck(Base):
     """
     PubAck is the response of publishing a message to JetStream.
     """
     stream: str
     seq: int
-    domain: str | None = None
-    duplicate: bool | None = None
+    domain: Optional[str] = None
+    duplicate: Optional[bool] = None
 
 
 @dataclass
 class Placement(Base):
     """Placement directives to consider when placing replicas of this stream"""
 
-    cluster: str | None = None
-    tags: list[str] | None = None
+    cluster: Optional[str] = None
+    tags: Optional[List[str]] = None
 
 
 @dataclass
 class ExternalStream(Base):
     api: str
-    deliver: str | None = None
+    deliver: Optional[str] = None
 
 
 @dataclass
 class StreamSource(Base):
     name: str
-    opt_start_seq: int | None = None
+    opt_start_seq: Optional[int] = None
     # FIXME: Handle time type, omit for now.
     # opt_start_time: Optional[str] = None
-    filter_subject: str | None = None
-    external: ExternalStream | None = None
+    filter_subject: Optional[str] = None
+    external: Optional[ExternalStream] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'external', ExternalStream)
         return super().from_response(resp)
 
 
 @dataclass
 class StreamSourceInfo(Base):
     name: str
-    lag: int | None = None
-    active: int | None = None
-    error: dict[str, Any] | None = None
+    lag: Optional[int] = None
+    active: Optional[int] = None
+    error: Optional[Dict[str, Any]] = None
 
 
 @dataclass
 class LostStreamData(Base):
-    msgs: list[int] | None = None
-    bytes: int | None = None
+    msgs: Optional[List[int]] = None
+    bytes: Optional[int] = None
 
 
 @dataclass
 class StreamState(Base):
     messages: int
     bytes: int
     first_seq: int
     last_seq: int
     consumer_count: int
-    deleted: list[int] | None = None
-    num_deleted: int | None = None
-    lost: LostStreamData | None = None
+    deleted: Optional[List[int]] = None
+    num_deleted: Optional[int] = None
+    lost: Optional[LostStreamData] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'lost', LostStreamData)
         return super().from_response(resp)
 
 
 class RetentionPolicy(str, Enum):
     """How message retention is considered"""
 
@@ -212,111 +212,111 @@
 
 @dataclass
 class RePublish(Base):
     """
     RePublish is for republishing messages once committed to a stream. The original
     subject cis remapped from the subject pattern to the destination pattern.
     """
-    src: str | None = None
-    dest: str | None = None
-    headers_only: bool | None = None
+    src: Optional[str] = None
+    dest: Optional[str] = None
+    headers_only: Optional[bool] = None
 
 
 @dataclass
 class StreamConfig(Base):
     """
     StreamConfig represents the configuration of a stream.
     """
-    name: str | None = None
-    description: str | None = None
-    subjects: list[str] | None = None
-    retention: RetentionPolicy | None = None
-    max_consumers: int | None = None
-    max_msgs: int | None = None
-    max_bytes: int | None = None
-    discard: DiscardPolicy | None = DiscardPolicy.OLD
-    max_age: float | None = None  # in seconds
+    name: Optional[str] = None
+    description: Optional[str] = None
+    subjects: Optional[List[str]] = None
+    retention: Optional[RetentionPolicy] = None
+    max_consumers: Optional[int] = None
+    max_msgs: Optional[int] = None
+    max_bytes: Optional[int] = None
+    discard: Optional[DiscardPolicy] = DiscardPolicy.OLD
+    max_age: Optional[float] = None  # in seconds
     max_msgs_per_subject: int = -1
-    max_msg_size: int | None = -1
-    storage: StorageType | None = None
-    num_replicas: int | None = None
+    max_msg_size: Optional[int] = -1
+    storage: Optional[StorageType] = None
+    num_replicas: Optional[int] = None
     no_ack: bool = False
-    template_owner: str | None = None
+    template_owner: Optional[str] = None
     duplicate_window: float = 0
-    placement: Placement | None = None
-    mirror: StreamSource | None = None
-    sources: list[StreamSource] | None = None
+    placement: Optional[Placement] = None
+    mirror: Optional[StreamSource] = None
+    sources: Optional[List[StreamSource]] = None
     sealed: bool = False
     deny_delete: bool = False
     deny_purge: bool = False
     allow_rollup_hdrs: bool = False
 
     # Allow republish of the message after being sequenced and stored.
-    republish: RePublish | None = None
+    republish: Optional[RePublish] = None
 
     # Allow higher performance, direct access to get individual messages. E.g. KeyValue
-    allow_direct: bool | None = None
+    allow_direct: Optional[bool] = None
 
     # Allow higher performance and unified direct access for mirrors as well.
-    mirror_direct: bool | None = None
+    mirror_direct: Optional[bool] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert_nanoseconds(resp, 'max_age')
         cls._convert_nanoseconds(resp, 'duplicate_window')
         cls._convert(resp, 'placement', Placement)
         cls._convert(resp, 'mirror', StreamSource)
         cls._convert(resp, 'sources', StreamSource)
         cls._convert(resp, 'republish', RePublish)
         return super().from_response(resp)
 
-    def as_dict(self) -> dict[str, object]:
+    def as_dict(self) -> Dict[str, object]:
         result = super().as_dict()
         result['duplicate_window'] = self._to_nanoseconds(
             self.duplicate_window
         )
         result['max_age'] = self._to_nanoseconds(self.max_age)
         return result
 
 
 @dataclass
 class PeerInfo(Base):
-    name: str | None = None
-    current: bool | None = None
-    offline: bool | None = None
-    active: int | None = None
-    lag: int | None = None
+    name: Optional[str] = None
+    current: Optional[bool] = None
+    offline: Optional[bool] = None
+    active: Optional[int] = None
+    lag: Optional[int] = None
 
 
 @dataclass
 class ClusterInfo(Base):
-    leader: str | None = None
-    name: str | None = None
-    replicas: list[PeerInfo] | None = None
+    leader: Optional[str] = None
+    name: Optional[str] = None
+    replicas: Optional[List[PeerInfo]] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'replicas', PeerInfo)
         return super().from_response(resp)
 
 
 @dataclass
 class StreamInfo(Base):
     """
     StreamInfo is the latest information about a stream from JetStream.
     """
     config: StreamConfig
     state: StreamState
-    mirror: StreamSourceInfo | None = None
-    sources: list[StreamSourceInfo] | None = None
-    cluster: ClusterInfo | None = None
-    did_create: bool | None = None
+    mirror: Optional[StreamSourceInfo] = None
+    sources: Optional[List[StreamSourceInfo]] = None
+    cluster: Optional[ClusterInfo] = None
+    did_create: Optional[bool] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'config', StreamConfig)
         cls._convert(resp, 'state', StreamState)
         cls._convert(resp, 'mirror', StreamSourceInfo)
         cls._convert(resp, 'sources', StreamSourceInfo)
         cls._convert(resp, 'cluster', ClusterInfo)
         return super().from_response(resp)
 
@@ -370,55 +370,55 @@
 @dataclass
 class ConsumerConfig(Base):
     """Consumer configuration.
 
     References:
         * `Consumers <https://docs.nats.io/jetstream/concepts/consumers>`_
     """
-    name: str | None = None
-    durable_name: str | None = None
-    description: str | None = None
-    deliver_policy: DeliverPolicy | None = DeliverPolicy.ALL
-    opt_start_seq: int | None = None
-    opt_start_time: int | None = None
-    ack_policy: AckPolicy | None = AckPolicy.EXPLICIT
-    ack_wait: float | None = None  # in seconds
-    max_deliver: int | None = None
-    filter_subject: str | None = None
-    replay_policy: ReplayPolicy | None = ReplayPolicy.INSTANT
-    rate_limit_bps: int | None = None
-    sample_freq: str | None = None
-    max_waiting: int | None = None
-    max_ack_pending: int | None = None
-    flow_control: bool | None = None
-    idle_heartbeat: float | None = None
-    headers_only: bool | None = None
+    name: Optional[str] = None
+    durable_name: Optional[str] = None
+    description: Optional[str] = None
+    deliver_policy: Optional[DeliverPolicy] = DeliverPolicy.ALL
+    opt_start_seq: Optional[int] = None
+    opt_start_time: Optional[int] = None
+    ack_policy: Optional[AckPolicy] = AckPolicy.EXPLICIT
+    ack_wait: Optional[float] = None  # in seconds
+    max_deliver: Optional[int] = None
+    filter_subject: Optional[str] = None
+    replay_policy: Optional[ReplayPolicy] = ReplayPolicy.INSTANT
+    rate_limit_bps: Optional[int] = None
+    sample_freq: Optional[str] = None
+    max_waiting: Optional[int] = None
+    max_ack_pending: Optional[int] = None
+    flow_control: Optional[bool] = None
+    idle_heartbeat: Optional[float] = None
+    headers_only: Optional[bool] = None
 
     # Push based consumers.
-    deliver_subject: str | None = None
-    deliver_group: str | None = None
+    deliver_subject: Optional[str] = None
+    deliver_group: Optional[str] = None
 
     # Ephemeral inactivity threshold
-    inactive_threshold: float | None = None  # in seconds
+    inactive_threshold: Optional[float] = None  # in seconds
 
     # Generally inherited by parent stream and other markers, now can
     # be configured directly.
-    num_replicas: int | None = None
+    num_replicas: Optional[int] = None
 
     # Force memory storage.
-    mem_storage: bool | None = None
+    mem_storage: Optional[bool] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert_nanoseconds(resp, 'ack_wait')
         cls._convert_nanoseconds(resp, 'idle_heartbeat')
         cls._convert_nanoseconds(resp, 'inactive_threshold')
         return super().from_response(resp)
 
-    def as_dict(self) -> dict[str, object]:
+    def as_dict(self) -> Dict[str, object]:
         result = super().as_dict()
         result['ack_wait'] = self._to_nanoseconds(self.ack_wait)
         result['idle_heartbeat'] = self._to_nanoseconds(self.idle_heartbeat)
         result['inactive_threshold'] = self._to_nanoseconds(
             self.inactive_threshold
         )
         return result
@@ -438,25 +438,25 @@
     ConsumerInfo represents the info about the consumer.
     """
     name: str
     stream_name: str
     config: ConsumerConfig
     # FIXME: Do not handle dates for now.
     # created: datetime
-    delivered: SequenceInfo | None = None
-    ack_floor: SequenceInfo | None = None
-    num_ack_pending: int | None = None
-    num_redelivered: int | None = None
-    num_waiting: int | None = None
-    num_pending: int | None = None
-    cluster: ClusterInfo | None = None
-    push_bound: bool | None = None
+    delivered: Optional[SequenceInfo] = None
+    ack_floor: Optional[SequenceInfo] = None
+    num_ack_pending: Optional[int] = None
+    num_redelivered: Optional[int] = None
+    num_waiting: Optional[int] = None
+    num_pending: Optional[int] = None
+    cluster: Optional[ClusterInfo] = None
+    push_bound: Optional[bool] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'delivered', SequenceInfo)
         cls._convert(resp, 'ack_floor', SequenceInfo)
         cls._convert(resp, 'config', ConsumerConfig)
         cls._convert(resp, 'cluster', ClusterInfo)
         return super().from_response(resp)
 
 
@@ -483,15 +483,15 @@
     memory: int
     storage: int
     streams: int
     consumers: int
     limits: AccountLimits
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'limits', AccountLimits)
         return super().from_response(resp)
 
 
 @dataclass
 class APIStats(Base):
     """API stats"""
@@ -511,71 +511,71 @@
     memory: int
     storage: int
     streams: int
     consumers: int
     limits: AccountLimits
 
     api: APIStats
-    domain: str | None = None
-    tiers: dict[str, Tier] | None = None
+    domain: Optional[str] = None
+    tiers: Optional[Dict[str, Tier]] = None
 
     @classmethod
-    def from_response(cls, resp: dict[str, Any]):
+    def from_response(cls, resp: Dict[str, Any]):
         cls._convert(resp, 'limits', AccountLimits)
         cls._convert(resp, 'api', APIStats)
         info = super().from_response(resp)
         tiers = resp.get('tiers', None)
         if tiers:
             result = {}
             for k, v in tiers.items():
                 result[k] = Tier.from_response(v)
             info.tiers = result
         return info
 
 
 @dataclass
 class RawStreamMsg(Base):
-    subject: str | None = None
-    seq: int | None = None
-    data: bytes | None = None
-    hdrs: bytes | None = None
-    headers: dict | None = None
-    stream: str | None = None
+    subject: Optional[str] = None
+    seq: Optional[int] = None
+    data: Optional[bytes] = None
+    hdrs: Optional[bytes] = None
+    headers: Optional[Dict] = None
+    stream: Optional[str] = None
     # TODO: Add 'time'
 
     @property
-    def sequence(self) -> int | None:
+    def sequence(self) -> Optional[int]:
         return self.seq
 
     @property
-    def header(self) -> dict | None:
+    def header(self) -> Optional[Dict]:
         """
         header returns the headers from a message.
         """
         return self.headers
 
 
 @dataclass
 class KeyValueConfig(Base):
     """
     KeyValueConfig is the configuration of a KeyValue store.
     """
     bucket: str
-    description: str | None = None
-    max_value_size: int | None = None
+    description: Optional[str] = None
+    max_value_size: Optional[int] = None
     history: int = 1
-    ttl: float | None = None  # in seconds
-    max_bytes: int | None = None
-    storage: StorageType | None = None
+    ttl: Optional[float] = None  # in seconds
+    max_bytes: Optional[int] = None
+    storage: Optional[StorageType] = None
     replicas: int = 1
-    placement: Placement | None = None
-    republish: RePublish | None = None
-    direct: bool | None = None
+    placement: Optional[Placement] = None
+    republish: Optional[RePublish] = None
+    direct: Optional[bool] = None
 
-    def as_dict(self) -> dict[str, object]:
+    def as_dict(self) -> Dict[str, object]:
         result = super().as_dict()
         result['ttl'] = self._to_nanoseconds(self.ttl)
         return result
 
 
 @dataclass
 class StreamPurgeRequest(Base):
```

### Comparing `nats-py-2.3.0/nats/js/client.py` & `nats-py-2.3.1/nats/js/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from __future__ import annotations
 
 import asyncio
 import json
 import time
 from email.parser import BytesParser
-from typing import TYPE_CHECKING, Awaitable, Callable, Optional
+from typing import TYPE_CHECKING, Awaitable, Callable, Optional, List, Dict
 
 import nats.errors
 import nats.js.errors
 from nats.aio.msg import Msg
 from nats.aio.subscription import Subscription
 from nats.js import api
 from nats.js.errors import BadBucketError, BucketNotFoundError, InvalidBucketNameError, NotFoundError
@@ -81,15 +81,15 @@
 
     """
 
     def __init__(
         self,
         conn: NATS,
         prefix: str = api.DEFAULT_PREFIX,
-        domain: str | None = None,
+        domain: Optional[str] = None,
         timeout: float = 5,
     ) -> None:
         self._prefix = prefix
         if domain is not None:
             self._prefix = f"$JS.{domain}.API"
         self._nc = conn
         self._timeout = timeout
@@ -103,17 +103,17 @@
             timeout=self._timeout,
         )
 
     async def publish(
         self,
         subject: str,
         payload: bytes = b'',
-        timeout: float | None = None,
-        stream: str | None = None,
-        headers: dict | None = None
+        timeout: Optional[float] = None,
+        stream: Optional[str] = None,
+        headers: Optional[Dict] = None
     ) -> api.PubAck:
         """
         publish emits a new message to JetStream.
         """
         hdr = headers
         if timeout is None:
             timeout = self._timeout
@@ -135,27 +135,27 @@
         if 'error' in resp:
             raise nats.js.errors.APIError.from_error(resp['error'])
         return api.PubAck.from_response(resp)
 
     async def subscribe(
         self,
         subject: str,
-        queue: str | None = None,
-        cb: Callback | None = None,
-        durable: str | None = None,
-        stream: str | None = None,
-        config: api.ConsumerConfig | None = None,
+        queue: Optional[str] = None,
+        cb: Optional[Callback] = None,
+        durable: Optional[str] = None,
+        stream: Optional[str] = None,
+        config: Optional[api.ConsumerConfig] = None,
         manual_ack: bool = False,
         ordered_consumer: bool = False,
-        idle_heartbeat: float | None = None,
+        idle_heartbeat: Optional[float] = None,
         flow_control: bool = False,
         pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-        deliver_policy: api.DeliverPolicy | None = None,
-        headers_only: bool | None = None,
+        deliver_policy: Optional[api.DeliverPolicy] = None,
+        headers_only: Optional[bool] = None,
     ) -> PushSubscription:
         """Create consumer if needed and push-subscribe to it.
 
         1. Check if consumer exists.
         2. Creates consumer if needed.
         3. Calls `subscribe_bind`.
 
@@ -317,15 +317,15 @@
         )
 
     async def subscribe_bind(
         self,
         stream: str,
         config: api.ConsumerConfig,
         consumer: str,
-        cb: Callback | None = None,
+        cb: Optional[Callback] = None,
         manual_ack: bool = False,
         ordered_consumer: bool = False,
         pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
     ) -> PushSubscription:
         """Push-subscribe to an existing consumer.
         """
@@ -372,16 +372,16 @@
 
         return new_callback
 
     async def pull_subscribe(
         self,
         subject: str,
         durable: str,
-        stream: str | None = None,
-        config: api.ConsumerConfig | None = None,
+        stream: Optional[str] = None,
+        config: Optional[api.ConsumerConfig] = None,
         pending_msgs_limit: int = DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
         pending_bytes_limit: int = DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
         inbox_prefix: bytes = api.INBOX_PREFIX,
     ) -> JetStreamContext.PullSubscription:
         """Create consumer and pull subscription.
 
         1. Find stream name by subject if `stream` is not passed.
@@ -478,78 +478,78 @@
             sub=sub,
             stream=stream,
             consumer=durable,
             deliver=deliver,
         )
 
     @classmethod
-    def is_status_msg(cls, msg: Msg | None) -> str | None:
+    def is_status_msg(cls, msg: Optional[Msg]) -> Optional[str]:
         if msg is None or msg.headers is None:
             return None
         return msg.headers.get(api.Header.STATUS)
 
     @classmethod
-    def _is_processable_msg(cls, status: str | None, msg: Msg) -> bool:
+    def _is_processable_msg(cls, status: Optional[str], msg: Msg) -> bool:
         if not status:
             return True
         # Skip most 4XX errors and do not raise exception.
         if JetStreamContext._is_temporary_error(status):
             return False
         raise nats.js.errors.APIError.from_msg(msg)
 
     @classmethod
-    def _is_temporary_error(cls, status: str | None) -> bool:
+    def _is_temporary_error(cls, status: Optional[str]) -> bool:
         if status == api.StatusCode.NO_MESSAGES or status == api.StatusCode.CONFLICT \
            or status == api.StatusCode.REQUEST_TIMEOUT:
             return True
         else:
             return False
 
     @classmethod
-    def _time_until(
-        cls, timeout: float | None, start_time: float
-    ) -> float | None:
+    def _time_until(cls, timeout: Optional[float],
+                    start_time: float) -> Optional[float]:
         if timeout is None:
             return None
         return timeout - (time.monotonic() - start_time)
 
     class _JSI():
 
         def __init__(
             self,
             js: JetStreamContext,
             conn: NATS,
             stream: str,
-            ordered: bool | None,
+            ordered: Optional[bool],
             psub: JetStreamContext.PushSubscription,
             sub: Subscription,
             ccreq: api.ConsumerConfig,
         ) -> None:
             self._conn = conn
             self._js = js
             self._stream = stream
             self._ordered = ordered
             self._psub = psub
             self._sub = sub
             self._ccreq = ccreq
 
             self._dseq = 1
             self._sseq = 0
-            self._cmeta: str | None = None
+            self._cmeta: Optional[str] = None
             self._fciseq = 0
-            self._active: bool | None = None
+            self._active: Optional[bool] = None
 
         def track_sequences(self, reply: str) -> None:
             self._fciseq += 1
             self._cmeta = reply
 
         def schedule_flow_control_response(self, reply: str) -> None:
             pass
 
-        async def check_for_sequence_mismatch(self, msg: Msg) -> bool | None:
+        async def check_for_sequence_mismatch(self,
+                                              msg: Msg) -> Optional[bool]:
             self._active = True
             if not self._cmeta:
                 return None
 
             tokens = msg._get_metadata_fields(self._cmeta)
             dseq = int(tokens[6])  # consumer sequence
             ldseq = None
@@ -571,15 +571,15 @@
                         stream_resume_sequence=sseq,
                         consumer_sequence=dseq,
                         last_consumer_sequence=ldseq,
                     )
                     await self._conn._error_cb(ecs)
             return did_reset
 
-        async def reset_ordered_consumer(self, sseq: int | None) -> bool:
+        async def reset_ordered_consumer(self, sseq: Optional[int]) -> bool:
             # FIXME: Handle AUTO_UNSUB called previously to this.
 
             # Replace current subscription.
             osid = self._sub._id
             self._conn._remove_sub(osid)
             new_deliver = self._conn.new_inbox()
 
@@ -747,15 +747,15 @@
             info = await self._js._jsm.consumer_info(
                 self._stream, self._consumer
             )
             return info
 
         async def fetch(self,
                         batch: int = 1,
-                        timeout: float | None = 5) -> list[Msg]:
+                        timeout: Optional[float] = 5) -> List[Msg]:
             """
             fetch makes a request to JetStream to be delivered a set of messages.
 
             :param batch: Number of messages to fetch from server.
             :param timeout: Max duration of the fetch request before it expires.
 
             ::
@@ -795,16 +795,16 @@
                 msg = await self._fetch_one(expires, timeout)
                 return [msg]
             msgs = await self._fetch_n(batch, expires, timeout)
             return msgs
 
         async def _fetch_one(
             self,
-            expires: int | None,
-            timeout: float | None,
+            expires: Optional[int],
+            timeout: Optional[float],
         ) -> Msg:
             queue = self._sub._pending_queue
 
             # Check the next message in case there are any.
             while not queue.empty():
                 try:
                     msg = queue.get_nowait()
@@ -845,24 +845,24 @@
                     # Any other type of status message is an error.
                     raise nats.js.errors.APIError.from_msg(msg)
             return msg
 
         async def _fetch_n(
             self,
             batch: int,
-            expires: int | None,
-            timeout: float | None,
-        ) -> list[Msg]:
+            expires: Optional[int],
+            timeout: Optional[float],
+        ) -> List[Msg]:
             msgs = []
             queue = self._sub._pending_queue
             start_time = time.monotonic()
             needed = batch
 
             # Fetch as many as needed from the internal pending queue.
-            msg: Msg | None
+            msg: Optional[Msg]
 
             while not queue.empty():
                 try:
                     msg = queue.get_nowait()
                     self._sub._pending_size -= len(msg.data)
                     status = JetStreamContext.is_status_msg(msg)
                     if status:
@@ -1017,15 +1017,15 @@
             pre=KV_PRE_TEMPLATE.format(bucket=bucket),
             js=self,
             direct=bool(si.config.allow_direct)
         )
 
     async def create_key_value(
         self,
-        config: api.KeyValueConfig | None = None,
+        config: Optional[api.KeyValueConfig] = None,
         **params,
     ) -> KeyValue:
         """
         create_key_value takes an api.KeyValueConfig and creates a KV in JetStream.
         """
         if config is None:
             config = api.KeyValueConfig(bucket=params["bucket"])
```

### Comparing `nats-py-2.3.0/nats/js/errors.py` & `nats-py-2.3.1/nats/js/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,56 +11,56 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, NoReturn
+from typing import TYPE_CHECKING, Any, NoReturn, Optional, Dict
 
 import nats.errors
 from nats.js import api
 
 if TYPE_CHECKING:
     from nats.aio.msg import Msg
 
 
 class Error(nats.errors.Error):
     """
     An Error raised by the NATS client when using JetStream.
     """
 
-    def __init__(self, description: str | None = None) -> None:
+    def __init__(self, description: Optional[str] = None) -> None:
         self.description = description
 
     def __str__(self) -> str:
         desc = ''
         if self.description:
             desc = self.description
         return f"nats: JetStream.{self.__class__.__name__} {desc}"
 
 
 @dataclass(repr=False, init=False)
 class APIError(Error):
     """
     An Error that is the result of interacting with NATS JetStream.
     """
-    code: int | None
-    err_code: int | None
-    description: str | None
-    stream: str | None
-    seq: int | None
+    code: Optional[int]
+    err_code: Optional[int]
+    description: Optional[str]
+    stream: Optional[str]
+    seq: Optional[int]
 
     def __init__(
         self,
-        code: int | None = None,
-        description: str | None = None,
-        err_code: int | None = None,
-        stream: str | None = None,
-        seq: int | None = None,
+        code: Optional[int] = None,
+        description: Optional[str] = None,
+        err_code: Optional[int] = None,
+        stream: Optional[str] = None,
+        seq: Optional[int] = None,
     ) -> None:
         self.code = code
         self.err_code = err_code
         self.description = description
         self.stream = stream
         self.seq = seq
 
@@ -72,15 +72,15 @@
         if code == api.StatusCode.SERVICE_UNAVAILABLE:
             raise ServiceUnavailableError
         else:
             desc = msg.header[api.Header.DESCRIPTION]
             raise APIError(code=int(code), description=desc)
 
     @classmethod
-    def from_error(cls, err: dict[str, Any]):
+    def from_error(cls, err: Dict[str, Any]):
         code = err['code']
         if code == 503:
             raise ServiceUnavailableError(**err)
         elif code == 500:
             raise ServerError(**err)
         elif code == 404:
             raise NotFoundError(**err)
```

### Comparing `nats-py-2.3.0/nats/js/kv.py` & `nats-py-2.3.1/nats/js/kv.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 
 from __future__ import annotations
 
 import asyncio
 import datetime
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List, Optional
 
 import nats.errors
 import nats.js.errors
 from nats.js import api
 
 if TYPE_CHECKING:
     from nats.js import JetStreamContext
@@ -67,19 +67,19 @@
     @dataclass
     class Entry:
         """
         An entry from a KeyValue store in JetStream.
         """
         bucket: str
         key: str
-        value: bytes | None
-        revision: int | None
-        delta: int | None
-        created: int | None
-        operation: str | None
+        value: Optional[bytes]
+        revision: Optional[int]
+        delta: Optional[int]
+        created: Optional[int]
+        operation: Optional[str]
 
     @dataclass(frozen=True)
     class BucketStatus:
         """
         BucketStatus is the status of a KeyValue bucket.
         """
         stream_info: api.StreamInfo
@@ -96,15 +96,15 @@
         def history(self) -> int:
             """
             history returns the max msgs per subject.
             """
             return self.stream_info.config.max_msgs_per_subject
 
         @property
-        def ttl(self) -> float | None:
+        def ttl(self) -> Optional[float]:
             """
             ttl returns the max age in seconds.
             """
             if self.stream_info.config.max_age is None:
                 return None
             return self.stream_info.config.max_age
 
@@ -118,26 +118,26 @@
     ) -> None:
         self._name = name
         self._stream = stream
         self._pre = pre
         self._js = js
         self._direct = direct
 
-    async def get(self, key: str, revision: int | None = None) -> Entry:
+    async def get(self, key: str, revision: Optional[int] = None) -> Entry:
         """
         get returns the latest value for the key.
         """
         entry = None
         try:
             entry = await self._get(key, revision)
         except nats.js.errors.KeyDeletedError as err:
             raise nats.js.errors.KeyNotFoundError(err.entry, err.op)
         return entry
 
-    async def _get(self, key: str, revision: int | None = None) -> Entry:
+    async def _get(self, key: str, revision: Optional[int] = None) -> Entry:
         msg = None
         subject = f"{self._pre}{key}"
         try:
             if revision:
                 msg = await self._js.get_msg(
                     self._stream,
                     seq=revision,
@@ -212,15 +212,15 @@
                 raise err
             except nats.js.errors.KeyDeletedError as err:
                 pa = await self.update(key, value, last=err.entry.revision)
 
         return pa
 
     async def update(
-        self, key: str, value: bytes, last: int | None = None
+        self, key: str, value: bytes, last: Optional[int] = None
     ) -> int:
         """
         update will update the value iff the latest revision matches.
         """
         hdrs = {}
         if not last:
             last = 0
@@ -237,15 +237,15 @@
                 raise nats.js.errors.KeyWrongLastSequenceError(
                     description=err.description
                 )
             else:
                 raise err
         return pa.seq
 
-    async def delete(self, key: str, last: int | None = None) -> bool:
+    async def delete(self, key: str, last: Optional[int] = None) -> bool:
         """
         delete will place a delete marker and remove all previous revisions.
         """
         hdrs = {}
         hdrs[KV_OP] = KV_DEL
 
         if last and last > 0:
@@ -296,15 +296,15 @@
 
     class KeyWatcher:
 
         def __init__(self, js):
             self._js = js
             self._updates = asyncio.Queue(maxsize=256)
             self._sub = None
-            self._pending: int | None = None
+            self._pending: Optional[int] = None
 
             # init done means that the nil marker has been sent,
             # once this is sent it won't be sent anymore.
             self._init_done = False
 
         async def stop(self):
             """
@@ -333,15 +333,15 @@
 
     async def watchall(self, **kwargs) -> KeyWatcher:
         """
         watchall returns a KeyValue watcher that matches all the keys.
         """
         return await self.watch(">", **kwargs)
 
-    async def keys(self, **kwargs) -> list[str]:
+    async def keys(self, **kwargs) -> List[str]:
         """
         keys will return a list of the keys from a KeyValue store.
         """
         watcher = await self.watchall(
             ignore_deletes=True,
             meta_only=True,
         )
@@ -355,15 +355,15 @@
         await watcher.stop()
 
         if not keys:
             raise nats.js.errors.NoKeysError
 
         return keys
 
-    async def history(self, key: str) -> list[Entry]:
+    async def history(self, key: str) -> List[Entry]:
         """
         history retrieves a list of the entries so far.
         """
         watcher = await self.watch(key, include_history=True)
 
         entries = []
```

### Comparing `nats-py-2.3.0/nats/js/manager.py` & `nats-py-2.3.1/nats/js/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 
 from __future__ import annotations
 
 import base64
 import json
 from email.parser import BytesParser
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, List, Optional, Dict
 
 from nats.errors import NoRespondersError
 from nats.js import api
 from nats.js.errors import APIError, NotFoundError, ServiceUnavailableError
 
 if TYPE_CHECKING:
     from nats import NATS
@@ -73,15 +73,15 @@
         resp = await self._api_request(
             f"{self._prefix}.STREAM.INFO.{name}", timeout=self._timeout
         )
         return api.StreamInfo.from_response(resp)
 
     async def add_stream(
         self,
-        config: api.StreamConfig | None = None,
+        config: Optional[api.StreamConfig] = None,
         **params
     ) -> api.StreamInfo:
         """
         add_stream creates a stream.
         """
         if config is None:
             config = api.StreamConfig()
@@ -95,15 +95,15 @@
             data.encode(),
             timeout=self._timeout,
         )
         return api.StreamInfo.from_response(resp)
 
     async def update_stream(
         self,
-        config: api.StreamConfig | None = None,
+        config: Optional[api.StreamConfig] = None,
         **params
     ) -> api.StreamInfo:
         """
         update_stream updates a stream.
         """
         if config is None:
             config = api.StreamConfig()
@@ -127,22 +127,22 @@
             f"{self._prefix}.STREAM.DELETE.{name}", timeout=self._timeout
         )
         return resp['success']
 
     async def purge_stream(
         self,
         name: str,
-        seq: int | None = None,
-        subject: str | None = None,
-        keep: int | None = None
+        seq: Optional[int] = None,
+        subject: Optional[str] = None,
+        keep: Optional[int] = None
     ) -> bool:
         """
         Purge a stream by name.
         """
-        stream_req: dict[str, Any] = {}
+        stream_req: Dict[str, Any] = {}
         if seq:
             stream_req['seq'] = seq
         if subject:
             stream_req['filter'] = subject
         if keep:
             stream_req['keep'] = keep
 
@@ -151,27 +151,27 @@
             f"{self._prefix}.STREAM.PURGE.{name}",
             req.encode(),
             timeout=self._timeout
         )
         return resp['success']
 
     async def consumer_info(
-        self, stream: str, consumer: str, timeout: float | None = None
+        self, stream: str, consumer: str, timeout: Optional[float] = None
     ):
         # TODO: Validate the stream and consumer names.
         if timeout is None:
             timeout = self._timeout
         resp = await self._api_request(
             f"{self._prefix}.CONSUMER.INFO.{stream}.{consumer}",
             b'',
             timeout=timeout
         )
         return api.ConsumerInfo.from_response(resp)
 
-    async def streams_info(self) -> list[api.StreamInfo]:
+    async def streams_info(self) -> List[api.StreamInfo]:
         """
         streams_info retrieves a list of streams.
         """
         resp = await self._api_request(
             f"{self._prefix}.STREAM.LIST",
             b'',
             timeout=self._timeout,
@@ -181,16 +181,16 @@
             stream_info = api.StreamInfo.from_response(stream)
             streams.append(stream_info)
         return streams
 
     async def add_consumer(
         self,
         stream: str,
-        config: api.ConsumerConfig | None = None,
-        timeout: float | None = None,
+        config: Optional[api.ConsumerConfig] = None,
+        timeout: Optional[float] = None,
         **params,
     ) -> api.ConsumerInfo:
         if not timeout:
             timeout = self._timeout
         if config is None:
             config = api.ConsumerConfig()
         config = config.evolve(**params)
@@ -222,15 +222,15 @@
         resp = await self._api_request(
             f"{self._prefix}.CONSUMER.DELETE.{stream}.{consumer}",
             b'',
             timeout=self._timeout
         )
         return resp['success']
 
-    async def consumers_info(self, stream: str) -> list[api.ConsumerInfo]:
+    async def consumers_info(self, stream: str) -> List[api.ConsumerInfo]:
         """
         consumers_info retrieves a list of consumers.
         """
         resp = await self._api_request(
             f"{self._prefix}.CONSUMER.LIST.{stream}",
             b'',
             timeout=self._timeout,
@@ -240,24 +240,24 @@
             consumer_info = api.ConsumerInfo.from_response(consumer)
             consumers.append(consumer_info)
         return consumers
 
     async def get_msg(
         self,
         stream_name: str,
-        seq: int | None = None,
-        subject: str | None = None,
-        direct: bool | None = False,
-        next: bool | None = False,
+        seq: Optional[int] = None,
+        subject: Optional[str] = None,
+        direct: Optional[bool] = False,
+        next: Optional[bool] = False,
     ) -> api.RawStreamMsg:
         """
         get_msg retrieves a message from a stream.
         """
         req_subject = None
-        req: dict[str, Any] = {}
+        req: Dict[str, Any] = {}
         if seq:
             req['seq'] = seq
         if subject:
             req['seq'] = None
             req.pop('seq', None)
             req['last_by_subj'] = subject
         if next:
@@ -296,15 +296,15 @@
             headers = None
             if len(parsed_headers.items()) > 0:
                 headers = {}
                 for k, v in parsed_headers.items():
                     headers[k] = v
             raw_msg.headers = headers
 
-        msg_data: bytes | None = None
+        msg_data: Optional[bytes] = None
         if raw_msg.data:
             msg_data = base64.b64decode(raw_msg.data)
         raw_msg.data = msg_data
 
         return raw_msg
 
     @classmethod
@@ -340,27 +340,27 @@
         resp = await self._api_request(req_subject, data.encode())
         return resp['success']
 
     async def get_last_msg(
         self,
         stream_name: str,
         subject: str,
-        direct: bool | None = False,
+        direct: Optional[bool] = False,
     ) -> api.RawStreamMsg:
         """
         get_last_msg retrieves the last message from a stream.
         """
         return await self.get_msg(stream_name, subject=subject, direct=direct)
 
     async def _api_request(
         self,
         req_subject: str,
         req: bytes = b'',
         timeout: float = 5,
-    ) -> dict[str, Any]:
+    ) -> Dict[str, Any]:
         try:
             msg = await self._nc.request(req_subject, req, timeout=timeout)
             resp = json.loads(msg.data)
         except NoRespondersError:
             raise ServiceUnavailableError
 
         # Check for API errors.
```

### Comparing `nats-py-2.3.0/nats/js/object_store.py` & `nats-py-2.3.1/nats/js/object_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import re
 import io
 from datetime import datetime, timezone
 from hashlib import sha256
 from dataclasses import dataclass
 import json
 import asyncio
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Optional, Union, List
 
 import nats.errors
 from nats.js import api
 from nats.js.errors import (
     BadObjectMetaError, DigestMismatchError, ObjectAlreadyExists,
     ObjectDeletedError, ObjectNotFoundError, NotFoundError, LinkIsABucketError
 )
@@ -422,15 +422,15 @@
 
     class ObjectWatcher:
 
         def __init__(self, js):
             self._js = js
             self._updates = asyncio.Queue(maxsize=256)
             self._sub = None
-            self._pending: int | None = None
+            self._pending: Optional[int] = None
 
             # init done means that the nil marker has been sent,
             # once this is sent it won't be sent anymore.
             self._init_done = False
 
         async def stop(self):
             """
@@ -540,15 +540,15 @@
             )
         finally:
             await self._js.purge_stream(self._stream, subject=chunk_subj)
 
     async def list(
         self,
         ignore_deletes=False,
-    ) -> list[api.ObjectInfo]:
+    ) -> List[api.ObjectInfo]:
         """
         list will list all the objects in this store.
         """
         watcher = await self.watch(ignore_deletes=ignore_deletes)
         entries = []
 
         async for entry in watcher:
```

### Comparing `nats-py-2.3.0/nats/nuid.py` & `nats-py-2.3.1/nats/nuid.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/protocol/__init__.py` & `nats-py-2.3.1/nats/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/protocol/command.py` & `nats-py-2.3.1/nats/protocol/command.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/nats/protocol/parser.py` & `nats-py-2.3.1/nats/protocol/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 NATS network protocol parser.
 """
 
 from __future__ import annotations
 
 import json
 import re
-from typing import Any
+from typing import Any, Dict
 
 from nats.errors import ProtocolError
 
 MSG_RE = re.compile(
     b'\\AMSG\\s+([^\\s]+)\\s+([^\\s]+)\\s+(([^\\s]+)[^\\S\r\n]+)?(\\d+)\r\n'
 )
 HMSG_RE = re.compile(
@@ -81,15 +81,15 @@
         return f"<nats protocol parser state={self.state}>"
 
     def reset(self) -> None:
         self.buf = bytearray()
         self.state = AWAITING_CONTROL_LINE
         self.needed = 0
         self.header_needed = 0
-        self.msg_arg: dict[str, Any] = {}
+        self.msg_arg: Dict[str, Any] = {}
 
     async def parse(self, data: bytes = b''):
         """
         Parses the wire protocol from NATS for the client
         and dispatches the subscription callbacks.
         """
         self.buf.extend(data)
```

### Comparing `nats-py-2.3.0/nats_py.egg-info/PKG-INFO` & `nats-py-2.3.1/nats_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nats-py
-Version: 2.3.0
+Version: 2.3.1
 Summary: NATS client for Python
 Author-email: Waldemar Quevedo <wally@synadia.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,14 +211,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: nkeys
 Provides-Extra: aiohttp
 Provides-Extra: fast_parse
 License-File: LICENSE
```

### Comparing `nats-py-2.3.0/nats_py.egg-info/SOURCES.txt` & `nats-py-2.3.1/nats_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/pyproject.toml` & `nats-py-2.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     'License :: OSI Approved :: Apache Software License',
     'Intended Audience :: Developers',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10'
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11'
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/nats-io/nats.py"
 "Bug Tracker" = "https://github.com/nats-io/nats.py/issues"
 
 [tool.setuptools]
```

### Comparing `nats-py-2.3.0/tests/test_client.py` & `nats-py-2.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/tests/test_client_async_await.py` & `nats-py-2.3.1/tests/test_client_async_await.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/tests/test_client_nkeys.py` & `nats-py-2.3.1/tests/test_client_nkeys.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/tests/test_client_v2.py` & `nats-py-2.3.1/tests/test_client_v2.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/tests/test_client_websocket.py` & `nats-py-2.3.1/tests/test_client_websocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,34 @@
 import shutil
 import ssl
 import tempfile
 import time
 import unittest
 from unittest import mock
 
+import pytest
 import nats
 from nats.aio.client import Client as NATS, __version__
 from nats.aio.errors import *
 from tests.utils import *
 
+try:
+    import aiohttp
+    aiohttp_installed = True
+except ModuleNotFoundError:
+    aiohttp_installed = False
+
 
 class WebSocketTest(SingleWebSocketServerTestCase):
 
     @async_test
     async def test_simple_headers(self):
+        if not aiohttp_installed:
+            pytest.skip("aiohttp not installed")
+
         nc = await nats.connect("ws://localhost:8080")
 
         sub = await nc.subscribe("foo")
         await nc.flush()
         await nc.publish(
             "foo", b'hello world', headers={
                 'foo': 'bar',
@@ -36,14 +46,17 @@
         self.assertEqual(msg.headers['foo'], 'bar')
         self.assertEqual(msg.headers['hello'], 'world-1')
 
         await nc.close()
 
     @async_test
     async def test_request_with_headers(self):
+        if not aiohttp_installed:
+            pytest.skip("aiohttp not installed")
+
         nc = await nats.connect("ws://localhost:8080")
 
         async def service(msg):
             # Add another header
             msg.headers['quux'] = 'quuz'
             await msg.respond(b'OK!')
 
@@ -63,14 +76,17 @@
         self.assertEqual(msg.headers['quux'], 'quuz')
         self.assertEqual(msg.data, b'OK!')
 
         await nc.close()
 
     @async_test
     async def test_empty_headers(self):
+        if not aiohttp_installed:
+            pytest.skip("aiohttp not installed")
+
         nc = await nats.connect("ws://localhost:8080")
 
         sub = await nc.subscribe("foo")
         await nc.flush()
         await nc.publish("foo", b'hello world', headers={'': ''})
 
         msg = await sub.next_msg()
@@ -102,14 +118,17 @@
         await nc.close()
 
 
 class WebSocketTLSTest(SingleWebSocketTLSServerTestCase):
 
     @async_test
     async def test_pub_sub(self):
+        if not aiohttp_installed:
+            pytest.skip("aiohttp not installed")
+
         nc = await nats.connect("wss://localhost:8081", tls=self.ssl_ctx)
 
         sub = await nc.subscribe("foo")
         await nc.flush()
         await nc.publish("foo", b'hello world', headers={'foo': 'bar'})
 
         msg = await sub.next_msg()
```

### Comparing `nats-py-2.3.0/tests/test_js.py` & `nats-py-2.3.1/tests/test_js.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,19 @@
 from nats.aio.msg import Msg
 from nats.aio.client import Client as NATS, __version__
 from nats.aio.errors import *
 from nats.errors import *
 from nats.js.errors import *
 from tests.utils import *
 
+try:
+    from fast_mail_parser import parse_email
+except ImportError:
+    parse_email = None
+
 
 class PublishTest(SingleJetStreamServerTestCase):
 
     @async_test
     async def test_publish(self):
         nc = NATS()
         await nc.connect()
@@ -639,14 +644,18 @@
         assert msgs[0].header['AAA-AAA-AAA'] == 'a'
         assert msgs[0].header['AAA-BBB-AAA'] == ''
 
         msg = await js.get_msg("test-nats", 3)
         assert msg.header['AAA-AAA-AAA'] == 'a'
         assert msg.header['AAA-BBB-AAA'] == ''
 
+        if not parse_email:
+            await nc.close()
+            return
+
         await js.publish(
             "test.nats.1",
             b'third_msg',
             headers={
                 '  AAA AAA AAA  ': '     a          ',
                 '  AAA-BBB-AAA  ': '     b          ',
                 ' B B B ': '        a               '
```

### Comparing `nats-py-2.3.0/tests/test_nuid.py` & `nats-py-2.3.1/tests/test_nuid.py`

 * *Files identical despite different names*

### Comparing `nats-py-2.3.0/tests/test_parser.py` & `nats-py-2.3.1/tests/test_parser.py`

 * *Files identical despite different names*

