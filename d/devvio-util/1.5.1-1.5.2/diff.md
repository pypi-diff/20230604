# Comparing `tmp/devvio_util-1.5.1.tar.gz` & `tmp/devvio_util-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.1.tar", last modified: Wed May 24 18:10:55 2023, max compression
+gzip compressed data, was "devvio_util-1.5.2.tar", last modified: Sun Jun  4 00:43:36 2023, max compression
```

## Comparing `devvio_util-1.5.1.tar` & `devvio_util-1.5.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:55.555533 devvio_util-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 18:10:55.555533 devvio_util-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:46.000000 devvio_util-1.5.1/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:55.551533 devvio_util-1.5.1/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:55.555533 devvio_util-1.5.1/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-05-24 18:10:46.000000 devvio_util-1.5.1/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:10:55.551533 devvio_util-1.5.1/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-24 18:10:55.000000 devvio_util-1.5.1/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-24 18:10:55.000000 devvio_util-1.5.1/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:10:55.000000 devvio_util-1.5.1/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:10:55.000000 devvio_util-1.5.1/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 18:10:55.000000 devvio_util-1.5.1/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 18:10:55.555533 devvio_util-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-24 18:10:46.000000 devvio_util-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.421477 devvio_util-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-04 00:43:36.421477 devvio_util-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:29.000000 devvio_util-1.5.2/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.417477 devvio_util-1.5.2/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/lib_creds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.421477 devvio_util-1.5.2/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-04 00:43:29.000000 devvio_util-1.5.2/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 00:43:36.417477 devvio_util-1.5.2/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-04 00:43:36.000000 devvio_util-1.5.2/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-04 00:43:36.421477 devvio_util-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-04 00:43:29.000000 devvio_util-1.5.2/setup.py
```

### Comparing `devvio_util-1.5.1/devvio_util/config.py` & `devvio_util-1.5.2/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.1/devvio_util/lib_creds.py` & `devvio_util-1.5.2/devvio_util/lib_creds.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Loader(ABC):
     def __init__(self, *args, **kwargs):
         """
         :param credentials: AWS credentials (AWS_ACCESS_KEY_ID, AWS_REGION, AWS_SECRET_ACCESS_KEY)
         """
         self._credentials = kwargs.get("credentials", {})
 
-    def get_secrets(self):
+    def get_secrets(self, secret_name):
         pass
 
 
 class FileLoader(Loader):
     def get_secrets(self, secret_name):
         try:
             with open(secret_name) as file:
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/address.py` & `devvio_util-1.5.2/devvio_util/primitives/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             raise Exception(f"Invalid Address: cannot initialize from type {type(addr)}")
         if not addr_bin:
             return None
         self._size = len(addr_bin)
         if self._size == kWALLET_ADDR_SIZE or self._size == kNODE_ADDR_SIZE:
             self._canonical = bytes([self._size]) + addr_bin
         elif self._size != (prefix_size := addr_bin[0] + 1):
-            raise Exception(f"Invalid Address: prefix != num bytes given ({prefix_size} != {self._size}")
+            raise Exception(f"Invalid Address: prefix != num bytes given ({prefix_size} != {self._size})")
         elif self._size == kWALLET_ADDR_BUF_SIZE or self._size == kNODE_ADDR_BUF_SIZE:
             self._canonical = addr_bin
             self._size -= 1
         else:
             raise Exception(f"Invalid Address: invalid size {self._size}")
 
     # compare addresses
@@ -41,14 +41,17 @@
     def __bool__(self) -> bool:
         return self._canonical is not None
 
     # get formatted address
     def __str__(self) -> str:
         return self.get_hex_str()
 
+    def __len__(self) -> int:
+        return self.get_size()
+
     # get address size (without buffer)
     def get_size(self) -> int:
         return self._size
 
     # get address bytes
     def get_canonical(self) -> bytes:
         return self._canonical
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/chainstate.py` & `devvio_util-1.5.2/devvio_util/primitives/chainstate.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.1/devvio_util/primitives/devv_constants.py` & `devvio_util-1.5.2/devvio_util/primitives/devv_constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 kLEGACY_ENVELOPE_SIZE = 17
 kSIGNER_LENGTH_OFFSET = 34
 kMIN_PAYLOAD_SIZE = 8
 kFLAGS_OFFSET = 24
 kOPERATION_OFFSET = 25
 kLEGACY_OPERATION_OFFSET = 16
 
-kSECONDUINT64_SIZE = 8+8
 kTRANSFER_NONADDR_DATA_SIZE = kUINT64_SIZE*3
 kMERKLE_SIZE = 32
 kPREV_HASH_SIZE = 32
 
+kPEM_PREFIX = '-----BEGIN ENCRYPTED PRIVATE KEY-----\n'
+kPEM_SUFFIX = '\n-----END ENCRYPTED PRIVATE KEY-----'
+kPEM_PREFIX_SIZE = len(kPEM_PREFIX)
+kPEM_SUFFIX_SIZE = len(kPEM_SUFFIX)
+
 
 class OpType:
     CREATE = 0
     MODIFY = 1
     SEND = 2
     DELETE = 3
     REVERT = 4
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/final_block.py` & `devvio_util-1.5.2/devvio_util/primitives/final_block.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,101 @@
 from devvio_util.primitives.summary import Summary
 from devvio_util.primitives.transaction import Transaction
 from devvio_util.primitives.utils import InputBuffer
 from devvio_util.primitives.validation import Validation
 from devvio_util.primitives.chainstate import Chainstate
 
+
 class FinalBlock:
     def __init__(self,
-                 raw_blk: InputBuffer = None,
+                 final_blk: InputBuffer or str = None,
                  prior: Chainstate = None,
                  keys=None,
                  is_legacy: bool = False,
                  do_validate: bool = False):
+        self._canonical = None
+        if isinstance(final_blk, str):
+            # TODO: fetch attributes on request, clean up InputBuffer object on request
+            self._canonical = InputBuffer(final_blk)
         self._shard_index = None
         self._block_height = None
         self._block_time = None
         self._prev_hash = None
         self._merkle = None
         self._summary = None
         self._tx_size = None
         self._sum_size = None
         self._val_count = None
         self._vals = None
         self._is_legacy = is_legacy
         self._txs = []
-        if not isinstance(raw_blk, InputBuffer):
-            raise Exception(f"Invalid FinalBlock input type {type(raw_blk)}")
-        if raw_blk and isinstance(raw_blk, InputBuffer):
-            self.from_buffer(raw_blk, prior, keys, is_legacy, do_validate)
 
-    def from_buffer(self, raw_blk: InputBuffer, prior: Chainstate = None, keys=None,
-                    is_legacy: bool = False, do_validate: bool = False):
-        # Back to begin
-        raw_blk.seek(0)
-        self._is_legacy = is_legacy
+        if final_blk and isinstance(final_blk, InputBuffer):
+            self.from_buffer(final_blk, prior, keys, is_legacy, do_validate)
+        elif self._canonical:
+            self.from_buffer(self._canonical, prior, keys, is_legacy, do_validate)
+        else:
+            raise Exception(f"Invalid FinalBlock input type {type(final_blk)}")
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self._canonical:
+            self._canonical.__exit__()
 
-        version_ = raw_blk.get_next_uint8()
+    def get_indexes(self, buffer: InputBuffer):
+        version_ = buffer.get_next_uint8()
         if not version_:
             raise Exception("Invalid serialized FinalBlock, buffer empty!")
 
         if version_ > 1:
             raise Exception(f"Invalid FinalBlock.version: {version_}")
 
-        num_bytes_ = raw_blk.get_next_uint64()
+        num_bytes_ = buffer.get_next_uint64()
         if not num_bytes_:
             raise Exception("Invalid serialized FinalBlock, wrong size!")
 
         if not self._is_legacy:
-            self._shard_index = raw_blk.get_next_uint64()
-            self._block_height = raw_blk.get_next_uint64()
+            self._shard_index = buffer.get_next_uint64()
+            self._block_height = buffer.get_next_uint64()
 
-        self._block_time = raw_blk.get_next_uint64()
-        self._prev_hash = raw_blk.get_next_prev_hash()
-        self._merkle = raw_blk.get_next_merkle()
+        self._block_time = buffer.get_next_uint64()
+        self._prev_hash = buffer.get_next_prev_hash()
+        self._merkle = buffer.get_next_merkle()
+
+        self._tx_size = buffer.get_next_uint64()
+        self._sum_size = buffer.get_next_uint64()
+        self._val_count = buffer.get_next_uint32()
 
-        self._tx_size = raw_blk.get_next_uint64()
-        self._sum_size = raw_blk.get_next_uint64()
-        self._val_count = raw_blk.get_next_uint32()
+    def from_buffer(self, buffer: InputBuffer, prior: Chainstate = None, keys=None,
+                    is_legacy: bool = False, do_validate: bool = False):
+        # Back to begin
+        buffer.seek(0)
+        self._is_legacy = is_legacy
+        self.get_indexes(buffer)
 
-        tx_start = raw_blk.tell()
+        tx_start = buffer.tell()
 
-        while raw_blk.tell() < tx_start + self._tx_size:
-            one_tx = Transaction(raw_blk, self._is_legacy)
+        while buffer.tell() < tx_start + self._tx_size:
+            one_tx = Transaction(buffer, self._is_legacy)
             self._txs.append(one_tx)
 
         # if (do_validate):
         #     summary = Summary()
         #     for tx in self._txs:
         #         tx.isValid(None, keys, summary)
 
-        self._summary = Summary(raw_blk)
+        self._summary = Summary(buffer)
         if prior:
             prior.update(self._summary)
-        self._vals = Validation(raw_blk)
+        self._vals = Validation(buffer)
 
     def __bool__(self):
-        return bool(self._txs)
+        return self._block_height is not None
 
     def get_shard_index(self) -> int:
         return self._shard_index
 
     def get_block_height(self) -> int:
         return self._block_height
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/signature.py` & `devvio_util-1.5.2/devvio_util/primitives/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,17 @@
     def __bool__(self) -> bool:
         return self._canonical is not None
 
     # get formatted signature
     def __str__(self) -> str:
         return self.get_hex_str()
 
+    def __len__(self) -> int:
+        return self.get_size()
+
     # get sig length (without prefix)
     def get_size(self) -> int:
         return self._size
 
     # get raw sig
     def get_canonical(self) -> bytes:
         return self._canonical
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/smart_coin.py` & `devvio_util-1.5.2/devvio_util/primitives/smart_coin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.1/devvio_util/primitives/summary.py` & `devvio_util-1.5.2/devvio_util/primitives/summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from devvio_util.primitives.transfer import Transfer
 from devvio_util.primitives.address import Address
-from devvio_util.primitives.devv_constants import kUINT32_SIZE
 from devvio_util.primitives.utils import InputBuffer, set_uint64, set_int64, set_uint32
 
 
 class DelayedItem:
     """
      * Constructor
      * @param delay
      * @param delta
      """
 
     def __init__(self, delay_val: int = 0, delta_val: int = 0):
         self.delay = delay_val
         self.delta = delta_val
 
+    def get_delay(self):
+        return self.delay
+
+    def get_delta(self):
+        return self.delta
+
 
 class Summary:
 
     def __init__(self, buffer: InputBuffer):
         self._summaryMap = {}
 
         addr_count = buffer.get_next_uint32()
@@ -50,15 +55,15 @@
         if not self._summaryMap:
             return False
         coin_total = 0
         for addr, summaryPair in self._summaryMap.items():
             delayed_map = summaryPair[0]
             delta_map = summaryPair[1]
             for coin_id, delayPair in delayed_map.items():
-                coin_total += delayPair[1]
+                coin_total += delayPair.get_delta()
             for coin_id, delta in delta_map.items():
                 coin_total += delta
         if coin_total != 0:
             print(f"Summary state invalid: {self.get_map()}")
             return False
         return True
 
@@ -67,16 +72,16 @@
         for addr, summaryPair in self._summaryMap.items():
             delayed_map = summaryPair[0]
             delta_map = summaryPair[1]
             for coin_id, delayPair in delayed_map.items():
                 one_xfer = {
                     'address': addr,
                     'coin': coin_id,
-                    'amount': delayPair[1],
-                    'delay': delayPair[0]
+                    'amount': delayPair.get_delta(),
+                    'delay': delayPair.get_delay()
                 }
                 xfers.append(Transfer(one_xfer))
             for coin_id, delta in delta_map.items():
                 one_xfer = {
                     'address': addr,
                     'coin': coin_id,
                     'amount': delta,
@@ -92,13 +97,13 @@
         for addr, pair in self._summaryMap.items():
             out += Address(addr).get_canonical()
             delayed_map, coin_map = pair
             out += set_uint64(len(delayed_map))
             out += set_uint64(len(coin_map))
             for coin, xfer in delayed_map.items():
                 out += set_uint64(coin)
-                out += set_uint64(xfer['delay'])
-                out += set_int64(xfer['delta'])
+                out += set_uint64(xfer.get_delay())
+                out += set_int64(xfer.get_delta())
             for coin, delta in coin_map.items():
                 out += set_uint64(coin)
                 out += set_int64(delta)
         return out
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/transaction.py` & `devvio_util-1.5.2/devvio_util/primitives/transaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from devvio_util.primitives.address import Address
 from devvio_util.primitives.signature import Signature
-from devvio_util.primitives.utils import InputBuffer
+from devvio_util.primitives.utils import InputBuffer, set_uint64, set_uint8
+from devvio_util.primitives.devv_sign import sign_binary, DevvHash
 from devvio_util.primitives.transfer import Transfer
 from devvio_util.primitives.devv_constants import kLEGACY_ENVELOPE_SIZE, kNODE_SIG_BUF_SIZE, kNODE_ADDR_BUF_SIZE, \
     kSIGNER_LENGTH_OFFSET, kUINT_SIZE, kMIN_PAYLOAD_SIZE, kFLAGS_OFFSET, kOPERATION_OFFSET, kLEGACY_OPERATION_OFFSET, \
     kENVELOPE_SIZE, OpType
 
 
 class Transaction:
     def __init__(self, raw_blk: InputBuffer = None, is_legacy: bool = None):
         self._tx_offset = None
         self._tx_size = None
         self._payload_size = None
         self._xfer_size = None
         self._signer_size = None
+        self._signer = None
         self._is_legacy = None
         self._canonical = None
         self._sig = None
         if raw_blk:
             self.from_buffer(raw_blk, is_legacy)
 
     def from_buffer(self, buffer: InputBuffer, is_legacy: bool):
@@ -28,14 +30,15 @@
             self._tx_size = kLEGACY_ENVELOPE_SIZE + self._xfer_size + self._payload_size + kNODE_SIG_BUF_SIZE
             self._signer_size = kNODE_ADDR_BUF_SIZE
         else:
             self._tx_size = buffer.get_next_uint64()
             self._xfer_size = buffer.get_next_uint64()
             self._payload_size = buffer.get_next_uint64()
             self._signer_size = buffer.get_int(self._tx_offset + kSIGNER_LENGTH_OFFSET, kUINT_SIZE) + 1
+            self._signer = Address(buffer.get_bytes(self._tx_offset + kSIGNER_LENGTH_OFFSET, self._signer_size))
 
         if self._payload_size < kMIN_PAYLOAD_SIZE:
             raise Exception(f"Invalid Transaction: bad payload size {self._payload_size}")
 
         if not Address.is_valid_addr_size(self._signer_size):
             raise Exception(f"Invalid Transaction: bad signer size {self._signer_size}")
 
@@ -47,29 +50,29 @@
             if oper >= OpType.NUM_OPS:
                 raise Exception("Invalid Transaction: invalid operation")
         else:
             oper = buffer.get_int(self._tx_offset + kLEGACY_OPERATION_OFFSET, kUINT_SIZE)
             if oper >= OpType.NUM_OPS:
                 raise Exception("Invalid Transaction: invalid operation")
             self._is_legacy = True
-        self._sig = self.get_signature_from_raw_blk(buffer)
+        self._sig = self.get_sig_from_raw_blk(buffer)
         buffer.seek(self._tx_offset)
         self._canonical = buffer.get_next_bytes(self._tx_size)
         if not self._canonical:
             raise Exception(f"Invalid Transaction: buffer too small for tx (< {self._tx_size}")
 
-    def get_signature_from_raw_blk(self, buffer: InputBuffer) -> Signature:
+    def get_sig_from_raw_blk(self, buffer: InputBuffer) -> Signature:
         if self._is_legacy:
             offset = self._tx_offset + kLEGACY_ENVELOPE_SIZE + self._payload_size + self._xfer_size + 1
         else:
             offset = kENVELOPE_SIZE + self._payload_size + self._xfer_size + self._signer_size
         sig_len = self._tx_size - offset
         return Signature(buffer.get_bytes(self._tx_offset + offset, sig_len))
 
-    def get_signature(self) -> Signature:
+    def get_sig(self) -> Signature:
         if self._is_legacy:
             offset = kLEGACY_ENVELOPE_SIZE + self._payload_size + self._xfer_size + 1
         else:
             offset = kENVELOPE_SIZE + self._payload_size + self._xfer_size + self._signer_size
         return Signature(self._canonical[offset:])
 
     def get_payload(self) -> str:
@@ -78,31 +81,95 @@
         else:
             offset = kENVELOPE_SIZE + self._xfer_size + self._signer_size
         return self.get_canonical()[offset:offset + self._payload_size].decode('utf-8')
 
     def get_canonical(self) -> bytes:
         return self._canonical
 
-    def get_hex_str(self) -> str:
+    def get_hex_str(self) -> str or None:
         if not self._canonical:
             return None
         return self._canonical.hex()
 
     def __str__(self):
         return self.get_hex_str()
 
     def __bool__(self):
         return self._sig is not None
 
     def __eq__(self, other):
-        return self._sig == other.get_signature()
+        return self._sig == other.get_sig()
 
     def get_xfers_from_raw_blk(self, buffer: InputBuffer) -> list:
         if not self._is_legacy:
             start_offset = self._tx_offset + kENVELOPE_SIZE + self._signer_size
         else:
             start_offset = self._tx_offset + kLEGACY_ENVELOPE_SIZE
         return Transfer.get_xfers_from_buffer(buffer, start_offset, self._xfer_size)
 
     def get_xfers(self) -> list:
         buffer = InputBuffer(self._canonical)
         return Transfer.get_xfers_from_buffer(buffer, kENVELOPE_SIZE + self._signer_size, self._xfer_size)
+
+    def get_message_digest(self) -> bytes:
+        return self._canonical[:kENVELOPE_SIZE + self._signer_size + self._xfer_size + self._payload_size]
+
+    def pre_signature_init(self, oper, signer: Address, xfers: list, payload: bytes, flags, timestamp):
+        self._payload_size = len(payload)
+
+        if self._payload_size < kMIN_PAYLOAD_SIZE:
+            raise ValueError(f"Failed to serialize transaction, payload too small ({self._payload_size})")
+
+        self._canonical = bytes()
+        self._canonical += set_uint64(self._payload_size)
+
+        if set_uint8(oper) >= OpType.NUM_OPS:
+            raise ValueError(f"Invalid Transaction: bad OpType ({oper} >= {OpType.NUM_OPS})")
+        self._canonical += set_uint8(oper)
+        if flags != 0:
+            raise ValueError("Invalid Transaction: unknown flags")
+        self._canonical += set_uint8(flags)
+        self._canonical += set_uint64(timestamp)
+        self._canonical += signer.get_canonical()
+
+        self._xfer_size = 0
+        for xfer in xfers:
+            self._xfer_size += xfer.get_size()
+            self._canonical += xfer.get_canonical()
+
+        self._signer_size = signer.get_size()
+        self._tx_size = kENVELOPE_SIZE + self._signer_size + self._xfer_size + self._payload_size \
+                        + signer.get_corresponding_sig_size()
+
+        self._canonical = set_uint64(self._tx_size) + set_uint64(self._xfer_size) + self._canonical
+
+    def serialize(self, oper: int, signer: Address, xfers: list,
+                  payload: bytes, eckey, keys, flags: int, timestamp: int):
+        self.pre_signature_init(oper, signer, xfers, payload, eckey, keys, flags, timestamp)
+
+        # TODO: finish sign_binary()
+        self._sig = sign_binary(eckey, DevvHash(self._canonical))
+        self._canonical += self._sig
+
+    def get_signer(self) -> Address:
+        return self._signer
+
+
+'''
+Address Transaction::getSigner() const {
+  if (is_legacy_) {
+    uint8_t signer_length = kNODE_ADDR_BUF_SIZE;
+    std::vector<byte> signer_bin(canonical_.begin()
+        + kLEGACY_SIGNER_LENGTH_OFFSET
+        , canonical_.begin() + kLEGACY_SIGNER_LENGTH_OFFSET + signer_length);
+    Address signer(signer_bin);
+    return signer;
+  }
+  uint8_t signer_length = canonical_[kSIGNER_LENGTH_OFFSET];
+  std::vector<byte> signer_bin(canonical_.begin() + kSIGNER_LENGTH_OFFSET
+      , canonical_.begin() + kSIGNER_LENGTH_OFFSET + signer_length + 1);
+  Address signer(signer_bin);
+  return signer;
+}
+'''
+
+
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/transfer.py` & `devvio_util-1.5.2/devvio_util/primitives/transfer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from devvio_util.primitives.devv_constants import kUINT64_SIZE, kTRANSFER_NONADDR_DATA_SIZE
+from devvio_util.primitives.devv_constants import kTRANSFER_NONADDR_DATA_SIZE
 from devvio_util.primitives.address import Address
 from devvio_util.primitives.utils import InputBuffer, set_int64, set_uint64
 
 
 class Transfer:
     def __init__(self, xfer: dict or bytes or InputBuffer or None = None):
         self._addr = None
@@ -18,25 +18,16 @@
         elif isinstance(xfer, dict):
             self.from_dict(xfer)
         elif xfer is not None:
             raise Exception(f"Invalid Transfer: could not initialize from {type(xfer)}")
 
     def from_canonical(self, xfer_bin: bytes):
         self._canonical = None
-        try:
-            addr_size = int.from_bytes(xfer_bin[1], 'little') + 1
-            self._addr = Address(bytes(xfer_bin[:addr_size]))
-            self._coin_id = int.from_bytes(xfer_bin[addr_size: addr_size + kUINT64_SIZE], 'little')
-            self._amount = int.from_bytes(xfer_bin[addr_size + kUINT64_SIZE: addr_size + kUINT64_SIZE * 2], 'little',
-                                          signed=True)
-            self._delay = int.from_bytes(xfer_bin[addr_size + kUINT64_SIZE * 2: addr_size + kUINT64_SIZE * 3], 'little')
-            self._canonical = bytes(xfer_bin)
-            self._size = addr_size + kTRANSFER_NONADDR_DATA_SIZE
-        except IndexError:
-            raise Exception("Invalid Transfer: bytes index error")
+        buffer = InputBuffer(xfer_bin)
+        self.from_buffer(buffer)
 
     def from_buffer(self, buffer: InputBuffer):
         self._canonical = None
         buffer_index = buffer.tell()
         addr_size = buffer.get_next_uint8()
         addr_bin = buffer.get_next_bytes(addr_size)
         if not addr_bin:
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/utils.py` & `devvio_util-1.5.2/devvio_util/primitives/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,10 +110,7 @@
     return set_int(x, kUINT_SIZE, False)
 
 
 def set_int(x: int, num_bytes: int, signed: bool) -> bytes:
     return x.to_bytes(num_bytes, 'little', signed=signed)
 
 
-class DevvHash:
-    def __init__(self, raw_bin: bytes):
-        self._hash = None
```

### Comparing `devvio_util-1.5.1/devvio_util/primitives/validation.py` & `devvio_util-1.5.2/devvio_util/primitives/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self._raw_addrs = False
         self._sigs = {}
 
         remainder = count
         offset = buffer.tell()
 
         if remainder is not None:
-            if offset + remainder * self.pair_size() > len(buffer):
+            if offset + remainder * self.pair_size() > buffer.__sizeof__():
                 raise Exception(f"Invalid Validation: buffer too small for {remainder} node addr/sig pairs")
             while remainder > 0:
                 self.create_sig(buffer)
                 remainder = remainder - 1
         else:
             while self.create_sig(buffer):
                 pass
```

### Comparing `devvio_util-1.5.1/devvio_util/psql_mixin.py` & `devvio_util-1.5.2/devvio_util/psql_mixin.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.1/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.5.2/devvio_util.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 devvio_util.egg-info/not-zip-safe
 devvio_util.egg-info/top_level.txt
 devvio_util/primitives/__init__.py
 devvio_util/primitives/address.py
 devvio_util/primitives/atomic_transaction_set.py
 devvio_util/primitives/chainstate.py
 devvio_util/primitives/devv_constants.py
+devvio_util/primitives/devv_sign.py
 devvio_util/primitives/final_block.py
 devvio_util/primitives/signature.py
 devvio_util/primitives/smart_coin.py
 devvio_util/primitives/summary.py
 devvio_util/primitives/transaction.py
 devvio_util/primitives/transfer.py
 devvio_util/primitives/utils.py
```

