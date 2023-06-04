# Comparing `tmp/bitcoinrpc-0.6.0.tar.gz` & `tmp/bitcoinrpc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoinrpc-0.6.0.tar", last modified: Thu Jun  1 13:45:08 2023, max compression
+gzip compressed data, was "bitcoinrpc-0.6.1.tar", last modified: Sun Jun  4 20:48:03 2023, max compression
```

## Comparing `bitcoinrpc-0.6.0.tar` & `bitcoinrpc-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/
--rw-rw-r--   0 boi       (1000) boi       (1000)     1080 2023-05-21 10:38:52.000000 bitcoinrpc-0.6.0/LICENSE
--rw-rw-r--   0 boi       (1000) boi       (1000)     6810 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/PKG-INFO
--rw-rw-r--   0 boi       (1000) boi       (1000)     5920 2023-06-01 13:44:53.000000 bitcoinrpc-0.6.0/README.md
--rw-rw-r--   0 boi       (1000) boi       (1000)      576 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/setup.cfg
--rw-rw-r--   0 boi       (1000) boi       (1000)     2054 2023-06-01 13:44:53.000000 bitcoinrpc-0.6.0/setup.py
-drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.242614 bitcoinrpc-0.6.0/src/
-drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/src/bitcoinrpc/
--rw-rw-r--   0 boi       (1000) boi       (1000)      205 2023-06-01 13:38:04.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/__init__.py
--rw-rw-r--   0 boi       (1000) boi       (1000)       22 2023-06-01 13:44:53.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/__version__.py
--rw-rw-r--   0 boi       (1000) boi       (1000)      140 2023-06-01 13:38:04.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/_exceptions.py
--rw-rw-r--   0 boi       (1000) boi       (1000)     3953 2023-05-21 10:38:52.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/_types.py
--rw-rw-r--   0 boi       (1000) boi       (1000)     8280 2023-06-01 13:38:12.000000 bitcoinrpc-0.6.0/src/bitcoinrpc/bitcoin_rpc.py
-drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/
--rw-rw-r--   0 boi       (1000) boi       (1000)     6810 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/PKG-INFO
--rw-rw-r--   0 boi       (1000) boi       (1000)      420 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/SOURCES.txt
--rw-rw-r--   0 boi       (1000) boi       (1000)        1 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/dependency_links.txt
--rw-rw-r--   0 boi       (1000) boi       (1000)       45 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/requires.txt
--rw-rw-r--   0 boi       (1000) boi       (1000)       11 2023-06-01 13:45:08.000000 bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/top_level.txt
-drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-01 13:45:08.246614 bitcoinrpc-0.6.0/tests/
--rw-rw-r--   0 boi       (1000) boi       (1000)      800 2023-06-01 13:38:04.000000 bitcoinrpc-0.6.0/tests/test_client_config.py
--rw-rw-r--   0 boi       (1000) boi       (1000)     1603 2023-06-01 13:38:12.000000 bitcoinrpc-0.6.0/tests/test_connection.py
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-04 20:48:03.061155 bitcoinrpc-0.6.1/
+-rw-rw-r--   0 boi       (1000) boi       (1000)     1080 2023-05-21 10:38:52.000000 bitcoinrpc-0.6.1/LICENSE
+-rw-rw-r--   0 boi       (1000) boi       (1000)     7136 2023-06-04 20:48:03.061155 bitcoinrpc-0.6.1/PKG-INFO
+-rw-rw-r--   0 boi       (1000) boi       (1000)     6246 2023-06-04 20:46:58.000000 bitcoinrpc-0.6.1/README.md
+-rw-rw-r--   0 boi       (1000) boi       (1000)      576 2023-06-04 20:48:03.061155 bitcoinrpc-0.6.1/setup.cfg
+-rw-rw-r--   0 boi       (1000) boi       (1000)     2054 2023-06-01 13:46:31.000000 bitcoinrpc-0.6.1/setup.py
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-04 20:48:03.057155 bitcoinrpc-0.6.1/src/
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-04 20:48:03.057155 bitcoinrpc-0.6.1/src/bitcoinrpc/
+-rw-rw-r--   0 boi       (1000) boi       (1000)      205 2023-06-01 13:46:31.000000 bitcoinrpc-0.6.1/src/bitcoinrpc/__init__.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)       22 2023-06-04 20:46:58.000000 bitcoinrpc-0.6.1/src/bitcoinrpc/__version__.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)      140 2023-06-01 13:46:31.000000 bitcoinrpc-0.6.1/src/bitcoinrpc/_exceptions.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)     4799 2023-06-04 20:46:58.000000 bitcoinrpc-0.6.1/src/bitcoinrpc/_types.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)    11385 2023-06-04 20:46:58.000000 bitcoinrpc-0.6.1/src/bitcoinrpc/bitcoin_rpc.py
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-04 20:48:03.061155 bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/
+-rw-rw-r--   0 boi       (1000) boi       (1000)     7136 2023-06-04 20:48:03.000000 bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/PKG-INFO
+-rw-rw-r--   0 boi       (1000) boi       (1000)      420 2023-06-04 20:48:03.000000 bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/SOURCES.txt
+-rw-rw-r--   0 boi       (1000) boi       (1000)        1 2023-06-04 20:48:03.000000 bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/dependency_links.txt
+-rw-rw-r--   0 boi       (1000) boi       (1000)       45 2023-06-04 20:48:03.000000 bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/requires.txt
+-rw-rw-r--   0 boi       (1000) boi       (1000)       11 2023-06-04 20:48:03.000000 bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/top_level.txt
+drwxrwxr-x   0 boi       (1000) boi       (1000)        0 2023-06-04 20:48:03.061155 bitcoinrpc-0.6.1/tests/
+-rw-rw-r--   0 boi       (1000) boi       (1000)      800 2023-06-01 13:46:31.000000 bitcoinrpc-0.6.1/tests/test_client_config.py
+-rw-rw-r--   0 boi       (1000) boi       (1000)     1603 2023-06-01 13:46:31.000000 bitcoinrpc-0.6.1/tests/test_connection.py
```

### Comparing `bitcoinrpc-0.6.0/LICENSE` & `bitcoinrpc-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoinrpc-0.6.0/PKG-INFO` & `bitcoinrpc-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoinrpc
-Version: 0.6.0
+Version: 0.6.1
 Summary: Lightweight Bitcoin JSON-RPC Python asynchronous client
 Home-page: https://github.com/bibajz/bitcoin-python-async-rpc
 Author: Libor Martinek
 Author-email: libasmartinek@protonmail.com
 License: MIT
 Keywords: bitcoin async json-rpc
 Classifier: Development Status :: 4 - Beta
@@ -68,25 +68,37 @@
 | `getconnectioncount` | ✔ |
 | `getnetworkinfo` | ✔ |
 
 ### Raw transactions
 
 |   Method   |   Supported?     |
 |------------|:----------------:|
+| `analyzepsbt` | ✔ |
+| `combinepsbt` | ✔ |
+| `decodepsbt` | ✔ |
+| `finalizepsbt` | ✔ |
 | `getrawtransaction` | ✔ |
+| `joinpsbts` | ✔ |
+| `utxoupdatepsbt` | ✔ |
+
+### Wallet
+
+|   Method   |   Supported?     |
+|------------|:----------------:|
+| `walletprocesspsbt` | ✔ |
 
 ## Usage
 Minimal illustration (assuming Python 3.8+, where you can run `async` code in console)
 
 ```
 $ python -m asyncio
 >>> import asyncio
 >>>
 >>> from bitcoinrpc import BitcoinRPC
->>> rpc = BitcoinRPC.from_config("http://localhost:18443" ("rpc_user", "rpc_passwd"))
+>>> rpc = BitcoinRPC.from_config("http://localhost:18443", ("rpc_user", "rpc_passwd"))
 >>> await rpc.getconnectioncount()
 10
 >>> await rpc.aclose()  # Clean-up resource
 ```
 
 You can also use the `BitcoinRPC` as an asynchronous context manager, which does
 all the resource clean-up automatically, as the following example shows:
@@ -236,15 +248,16 @@
 ```
 (your-venv-with-tox) $ tox run -e py311 -- -m 'not integration'
 ```
 
 
 ## Changelog
 
+- **2023/06/04 - 0.6.1**: Add RPC methods, mainly concerned with PSBTs
 - **2023/06/01 - 0.6.0**:
   * `BitcoinRPC` is now instantiated with a `httpx.AsyncClient` directly and an optional `counter` argument, which is a callable that may be used for distinguishing
     the JSON-RPC requests. Old-style instantiation, with `url` and optional user/password tuple, is kept within `BitcoinRPC.from_config` method.
-  
+
 - **2021/12/28 - 0.5.0** change the signature of `BitcoinRPC` from `host, port, ...` to `url, ...`, delegating the creation of the node url to the caller.
 
 ## License
 MIT
```

### Comparing `bitcoinrpc-0.6.0/README.md` & `bitcoinrpc-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -45,25 +45,37 @@
 | `getconnectioncount` | ✔ |
 | `getnetworkinfo` | ✔ |
 
 ### Raw transactions
 
 |   Method   |   Supported?     |
 |------------|:----------------:|
+| `analyzepsbt` | ✔ |
+| `combinepsbt` | ✔ |
+| `decodepsbt` | ✔ |
+| `finalizepsbt` | ✔ |
 | `getrawtransaction` | ✔ |
+| `joinpsbts` | ✔ |
+| `utxoupdatepsbt` | ✔ |
+
+### Wallet
+
+|   Method   |   Supported?     |
+|------------|:----------------:|
+| `walletprocesspsbt` | ✔ |
 
 ## Usage
 Minimal illustration (assuming Python 3.8+, where you can run `async` code in console)
 
 ```
 $ python -m asyncio
 >>> import asyncio
 >>>
 >>> from bitcoinrpc import BitcoinRPC
->>> rpc = BitcoinRPC.from_config("http://localhost:18443" ("rpc_user", "rpc_passwd"))
+>>> rpc = BitcoinRPC.from_config("http://localhost:18443", ("rpc_user", "rpc_passwd"))
 >>> await rpc.getconnectioncount()
 10
 >>> await rpc.aclose()  # Clean-up resource
 ```
 
 You can also use the `BitcoinRPC` as an asynchronous context manager, which does
 all the resource clean-up automatically, as the following example shows:
@@ -213,15 +225,16 @@
 ```
 (your-venv-with-tox) $ tox run -e py311 -- -m 'not integration'
 ```
 
 
 ## Changelog
 
+- **2023/06/04 - 0.6.1**: Add RPC methods, mainly concerned with PSBTs
 - **2023/06/01 - 0.6.0**:
   * `BitcoinRPC` is now instantiated with a `httpx.AsyncClient` directly and an optional `counter` argument, which is a callable that may be used for distinguishing
     the JSON-RPC requests. Old-style instantiation, with `url` and optional user/password tuple, is kept within `BitcoinRPC.from_config` method.
-  
+
 - **2021/12/28 - 0.5.0** change the signature of `BitcoinRPC` from `host, port, ...` to `url, ...`, delegating the creation of the node url to the caller.
 
 ## License
 MIT
```

### Comparing `bitcoinrpc-0.6.0/setup.cfg` & `bitcoinrpc-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bitcoinrpc-0.6.0/setup.py` & `bitcoinrpc-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `bitcoinrpc-0.6.0/src/bitcoinrpc/_types.py` & `bitcoinrpc-0.6.1/src/bitcoinrpc/_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from typing import Any, Dict, List, TypeVar, Union
 
-from typing_extensions import Literal, TypedDict
+from typing_extensions import Literal, NotRequired, TypedDict
+
+JSONType = Union[None, bool, int, float, str, List["JSONType"], Dict[str, "JSONType"]]
 
 # Type aliases for 1-to-1 match of RPC method and its return type
 ConnectionCount = int
 Difficulty = float
 BestBlockHash = str
 BlockHash = str
 BlockCount = int
 NetworkHashps = float
+CombinePSBT = str
+JoinPSBTs = str
+UtxoUpdatePSBT = str
 
 
 class MempoolInfo(TypedDict):
     loaded: bool
     size: int
     bytes: int
     usage: int
@@ -172,14 +177,44 @@
     difficulty: float
     networkhashps: float
     pooledtx: int
     chain: Literal["main", "test", "regtest"]
     warnings: str
 
 
+class AnalyzePSBT(TypedDict):
+    inputs: List[Dict[str, Any]]  # TODO: Complete
+    next: str
+
+    fee: NotRequired[float]
+    estimated_vsize: NotRequired[float]
+    estimated_feerate: NotRequired[float]
+    error: NotRequired[str]
+
+
+class DecodePSBT(TypedDict):
+    tx: Dict[str, Any]
+    unknown: Dict[str, Any]
+    inputs: List[Dict[str, Any]]
+    outputs: List[Dict[str, Any]]
+
+    fee: NotRequired[float]
+
+
+class FinalizePSBT(TypedDict):
+    psbt: str
+    hex: str
+    complete: bool
+
+
+class WalletProcessPSBT(TypedDict):
+    psbt: str
+    complete: bool
+
+
 BitcoinRPCResponse = TypeVar(
     "BitcoinRPCResponse",
     ConnectionCount,
     Difficulty,
     BestBlockHash,
     BlockHash,
     BlockCount,
@@ -189,8 +224,15 @@
     BlockchainInfo,
     NetworkInfo,
     ChainTips,
     BlockHeader,
     BlockStats,
     Block,
     RawTransaction,
+    CombinePSBT,
+    JoinPSBTs,
+    UtxoUpdatePSBT,
+    AnalyzePSBT,
+    DecodePSBT,
+    FinalizePSBT,
+    WalletProcessPSBT,
 )
```

### Comparing `bitcoinrpc-0.6.0/src/bitcoinrpc/bitcoin_rpc.py` & `bitcoinrpc-0.6.1/src/bitcoinrpc/bitcoin_rpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import itertools
 from types import TracebackType
-from typing import Any, Callable, List, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 import httpx
 import orjson
 from typing_extensions import Literal, Self
 
 from bitcoinrpc._exceptions import RPCError
 from bitcoinrpc._types import (
+    AnalyzePSBT,
     BestBlockHash,
     BitcoinRPCResponse,
     Block,
     BlockchainInfo,
     BlockCount,
     BlockHash,
     BlockHeader,
     BlockStats,
     ChainTips,
+    CombinePSBT,
     ConnectionCount,
+    DecodePSBT,
     Difficulty,
+    FinalizePSBT,
+    JoinPSBTs,
+    JSONType,
     MempoolInfo,
     MiningInfo,
     NetworkHashps,
     NetworkInfo,
     RawTransaction,
+    UtxoUpdatePSBT,
+    WalletProcessPSBT,
 )
 
 # Neat trick found in asyncio library for task enumeration
 # https://github.com/python/cpython/blob/3.8/Lib/asyncio/tasks.py#L31
 _next_rpc_id = itertools.count(1).__next__
 
 
@@ -95,15 +103,15 @@
 
     async def aclose(self) -> None:
         await self.client.aclose()
 
     async def acall(
         self,
         method: str,
-        params: List[Union[str, int, List[str], None]],
+        params: List[JSONType],
         **kwargs: Any,
     ) -> BitcoinRPCResponse:
         """
         Pass keyword arguments to directly modify the constructed request -
             see `httpx.Request`.
         """
         response = await self.client.post(
@@ -243,7 +251,84 @@
             otherwise as an average over last provided number of blocks
         :param height: If not provided, get estimated hash power for the latest block
         :param timeout: If doing a lot of processing, no timeout may come in handy
         """
         return await self.acall(
             "getnetworkhashps", [nblocks, height], timeout=httpx.Timeout(timeout)
         )
+
+    async def analyzepsbt(self, psbt: str) -> AnalyzePSBT:
+        """
+        https://developer.bitcoin.org/reference/rpc/analyzepsbt.html
+
+        :param psbt: base64 string of a partially signed bitcoin transaction
+        """
+        return await self.acall("analyzepsbt", [psbt])
+
+    async def combinepsbt(self, *psbts: str) -> CombinePSBT:
+        """
+        https://developer.bitcoin.org/reference/rpc/combinepsbt.html
+
+        :param psbts: base64 strings, each representing a partially signed bitcoin transaction
+        """
+        return await self.acall("combinepsbt", list(psbts))
+
+    async def decodepsbt(self, psbt: str) -> DecodePSBT:
+        """
+        https://developer.bitcoin.org/reference/rpc/decodepsbt.html
+
+        :param psbt: base64 string of a partially signed bitcoin transaction
+        """
+        return await self.acall("decodepsbt", [psbt])
+
+    async def finalizepsbt(self, psbt: str, extract: bool = True) -> FinalizePSBT:
+        """
+        https://developer.bitcoin.org/reference/rpc/finalizepsbt.html
+
+        :param psbt: base64 string of a partially signed bitcoin transaction
+        :param extract: If set to true and the transaction is complete, return a hex-encoded network transaction
+        """
+        return await self.acall("finalizepsbt", [psbt, extract])
+
+    async def joinpsbts(self, *psbts: str) -> JoinPSBTs:
+        """
+        https://developer.bitcoin.org/reference/rpc/joinpsbts.html
+
+        :param psbts: base64 strings, each representing a partially signed bitcoin transaction
+        """
+        return await self.acall("joinpsbts", list(psbts))
+
+    async def utxoupdatepsbt(
+        self,
+        psbt: str,
+        descriptors: Optional[List[Union[str, Dict[str, Union[int, str]]]]] = None,
+    ) -> UtxoUpdatePSBT:
+        """
+        https://developer.bitcoin.org/reference/rpc/utxoupdatepsbt.html
+
+        :param psbt: base64 string of a partially signed bitcoin transaction
+        :param extract: If set to true and the transaction is complete, return a hex-encoded network transaction
+        """
+        if descriptors is not None:
+            params = [psbt, descriptors]
+        else:
+            params = [psbt]
+        return await self.acall("utxoupdatepsbt", params)  # type: ignore
+
+    async def walletprocesspsbt(
+        self,
+        psbt: str,
+        sign: bool = True,
+        sighashtype: str = "ALL",
+        bip32_derivs: bool = True,
+    ) -> WalletProcessPSBT:
+        """
+        https://developer.bitcoin.org/reference/rpc/walletprocesspsbt.html
+
+        :param psbt: base64 string of a partially signed bitcoin transaction
+        :param sign: Sign the transaction too when updating
+        :param sighashtype: signature hash type to sign, if it is not specified by PSBT.
+        :param bip32_derivs: include bip32 derivation paths for pubkeys if known
+        """
+        return await self.acall(
+            "walletprocesspsbt", [psbt, sign, sighashtype, bip32_derivs]
+        )
```

### Comparing `bitcoinrpc-0.6.0/src/bitcoinrpc.egg-info/PKG-INFO` & `bitcoinrpc-0.6.1/src/bitcoinrpc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoinrpc
-Version: 0.6.0
+Version: 0.6.1
 Summary: Lightweight Bitcoin JSON-RPC Python asynchronous client
 Home-page: https://github.com/bibajz/bitcoin-python-async-rpc
 Author: Libor Martinek
 Author-email: libasmartinek@protonmail.com
 License: MIT
 Keywords: bitcoin async json-rpc
 Classifier: Development Status :: 4 - Beta
@@ -68,25 +68,37 @@
 | `getconnectioncount` | ✔ |
 | `getnetworkinfo` | ✔ |
 
 ### Raw transactions
 
 |   Method   |   Supported?     |
 |------------|:----------------:|
+| `analyzepsbt` | ✔ |
+| `combinepsbt` | ✔ |
+| `decodepsbt` | ✔ |
+| `finalizepsbt` | ✔ |
 | `getrawtransaction` | ✔ |
+| `joinpsbts` | ✔ |
+| `utxoupdatepsbt` | ✔ |
+
+### Wallet
+
+|   Method   |   Supported?     |
+|------------|:----------------:|
+| `walletprocesspsbt` | ✔ |
 
 ## Usage
 Minimal illustration (assuming Python 3.8+, where you can run `async` code in console)
 
 ```
 $ python -m asyncio
 >>> import asyncio
 >>>
 >>> from bitcoinrpc import BitcoinRPC
->>> rpc = BitcoinRPC.from_config("http://localhost:18443" ("rpc_user", "rpc_passwd"))
+>>> rpc = BitcoinRPC.from_config("http://localhost:18443", ("rpc_user", "rpc_passwd"))
 >>> await rpc.getconnectioncount()
 10
 >>> await rpc.aclose()  # Clean-up resource
 ```
 
 You can also use the `BitcoinRPC` as an asynchronous context manager, which does
 all the resource clean-up automatically, as the following example shows:
@@ -236,15 +248,16 @@
 ```
 (your-venv-with-tox) $ tox run -e py311 -- -m 'not integration'
 ```
 
 
 ## Changelog
 
+- **2023/06/04 - 0.6.1**: Add RPC methods, mainly concerned with PSBTs
 - **2023/06/01 - 0.6.0**:
   * `BitcoinRPC` is now instantiated with a `httpx.AsyncClient` directly and an optional `counter` argument, which is a callable that may be used for distinguishing
     the JSON-RPC requests. Old-style instantiation, with `url` and optional user/password tuple, is kept within `BitcoinRPC.from_config` method.
-  
+
 - **2021/12/28 - 0.5.0** change the signature of `BitcoinRPC` from `host, port, ...` to `url, ...`, delegating the creation of the node url to the caller.
 
 ## License
 MIT
```

### Comparing `bitcoinrpc-0.6.0/tests/test_client_config.py` & `bitcoinrpc-0.6.1/tests/test_client_config.py`

 * *Files identical despite different names*

### Comparing `bitcoinrpc-0.6.0/tests/test_connection.py` & `bitcoinrpc-0.6.1/tests/test_connection.py`

 * *Files identical despite different names*

