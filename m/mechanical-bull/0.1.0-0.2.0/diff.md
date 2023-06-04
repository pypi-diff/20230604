# Comparing `tmp/mechanical_bull-0.1.0.tar.gz` & `tmp/mechanical_bull-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanical_bull-0.1.0.tar", max compression
+gzip compressed data, was "mechanical_bull-0.2.0.tar", max compression
```

## Comparing `mechanical_bull-0.1.0.tar` & `mechanical_bull-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     1062 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/LICENSE
--rw-r--r--   0        0        0     3110 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-24 16:56:15.604644 mechanical_bull-0.1.0/mechanical_bull/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 16:56:15.608644 mechanical_bull-0.1.0/mechanical_bull/actions/__init__.py
--rw-r--r--   0        0        0      196 2023-05-24 16:56:54.509035 mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1206 2023-05-24 16:56:54.509035 mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0      930 2023-05-24 16:56:54.525035 mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
--rw-r--r--   0        0        0     1236 2023-05-24 16:56:54.513035 mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0     1985 2023-05-24 16:56:54.509035 mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      491 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/actions/accept_follow_request.py
--rw-r--r--   0        0        0      225 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/actions/log_to_file.py
--rw-r--r--   0        0        0      521 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/actions/reject_follow_request.py
--rw-r--r--   0        0        0      847 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/actions/test_accept_reject_follow_request.py
--rw-r--r--   0        0        0     1813 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/add_user.py
--rw-r--r--   0        0        0     1132 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/event_loop.py
--rw-r--r--   0        0        0      335 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/handlers.py
--rw-r--r--   0        0        0      708 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/run.py
--rw-r--r--   0        0        0      542 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/test_event_loop.py
--rw-r--r--   0        0        0      484 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/mechanical_bull/test_handlers.py
--rw-r--r--   0        0        0      896 2023-05-24 16:56:15.524643 mechanical_bull-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mechanical_bull-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-04 13:25:25.548713 mechanical_bull-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3110 2023-06-04 13:25:25.548713 mechanical_bull-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-04 13:25:25.616713 mechanical_bull-0.2.0/mechanical_bull/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 13:25:25.616713 mechanical_bull-0.2.0/mechanical_bull/actions/__init__.py
+-rw-r--r--   0        0        0      196 2023-06-04 13:26:02.617086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1387 2023-06-04 13:26:02.621086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0     2430 2023-06-04 13:26:02.625086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/announce.cpython-311.pyc
+-rw-r--r--   0        0        0     1380 2023-06-04 13:26:02.637086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
+-rw-r--r--   0        0        0     1417 2023-06-04 13:26:02.621086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0     1985 2023-06-04 13:26:02.617086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3497 2023-06-04 13:26:02.625086 mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/test_announce.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      680 2023-06-04 13:25:25.548713 mechanical_bull-0.2.0/mechanical_bull/actions/accept_follow_request.py
+-rw-r--r--   0        0        0     1811 2023-06-04 13:25:25.548713 mechanical_bull-0.2.0/mechanical_bull/actions/announce.py
+-rw-r--r--   0        0        0      682 2023-06-04 13:25:25.548713 mechanical_bull-0.2.0/mechanical_bull/actions/log_to_file.py
+-rw-r--r--   0        0        0      710 2023-06-04 13:25:25.548713 mechanical_bull-0.2.0/mechanical_bull/actions/reject_follow_request.py
+-rw-r--r--   0        0        0      847 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/actions/test_accept_reject_follow_request.py
+-rw-r--r--   0        0        0     1377 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/actions/test_announce.py
+-rw-r--r--   0        0        0     1813 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/add_user.py
+-rw-r--r--   0        0        0     1873 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/event_loop.py
+-rw-r--r--   0        0        0      335 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/handlers.py
+-rw-r--r--   0        0        0      708 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/run.py
+-rw-r--r--   0        0        0      542 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/test_event_loop.py
+-rw-r--r--   0        0        0      484 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/mechanical_bull/test_handlers.py
+-rw-r--r--   0        0        0      896 2023-06-04 13:25:25.552713 mechanical_bull-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 mechanical_bull-0.2.0/PKG-INFO
```

### Comparing `mechanical_bull-0.1.0/LICENSE` & `mechanical_bull-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.1.0/README.md` & `mechanical_bull-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc` & `mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc`

 * *Files 25% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xaf416e64 (Wed May 24 16:56:15 2023 UTC)
-files sz: 491
+moddate:  0xc5907c64 (Sun Jun  4 13:25:25 2023 UTC)
+files sz: 680
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100020065006a0300
@@ -14,150 +14,151 @@
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
      3          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('BovineActor',))
+                12 LOAD_CONST               2 (('BovineClient',))
                 14 IMPORT_NAME              1 (bovine)
-                16 IMPORT_FROM              2 (BovineActor)
-                18 STORE_NAME               2 (BovineActor)
+                16 IMPORT_FROM              2 (BovineClient)
+                18 STORE_NAME               2 (BovineClient)
                 20 POP_TOP
    
      5          22 PUSH_NULL
                 24 LOAD_NAME                0 (logging)
                 26 LOAD_ATTR                3 (getLogger)
                 36 LOAD_NAME                4 (__name__)
                 38 PRECALL                  1
                 42 CALL                     1
                 52 STORE_NAME               5 (logger)
    
-     8          54 LOAD_CONST               3 ('actor')
-                56 LOAD_NAME                2 (BovineActor)
+     8          54 LOAD_CONST               3 ('client')
+                56 LOAD_NAME                2 (BovineClient)
                 58 LOAD_CONST               4 ('data')
                 60 LOAD_NAME                6 (dict)
                 62 BUILD_TUPLE              4
                 64 LOAD_CONST               5 (<code object handle, file "/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/accept_follow_request.py", line 8>)
                 66 MAKE_FUNCTION            4 (annotations)
                 68 STORE_NAME               7 (handle)
                 70 LOAD_CONST               1 (None)
                 72 RETURN_VALUE
    consts
       0
       None
-      ('BovineActor',)
-      'actor'
+      ('BovineClient',)
+      'client'
       'data'
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 131
          code
             0x4b00010097007c0164011900000000000000000064026b030000000072
-            02640053007c016403190000000000000000007d02740100000000000000
+            02640353007c016404190000000000000000007d02740100000000000000
             0000007c02740200000000000000000000a6020000ab0200000000000000
-            0072087c026404190000000000000000007d027404000000000000000000
-            00a003000000000000000000000000000000000000000064057c02a60200
+            0072087c026405190000000000000000007d027404000000000000000000
+            00a003000000000000000000000000000000000000000064067c02a60200
             00ab02000000000000000001007c006a040000000000000000a005000000
-            00000000000000000000000000000000007c016404190000000000000000
-            007c016403190000000000000000006801ac06a6020000ab020000000000
+            00000000000000000000000000000000007c016405190000000000000000
+            007c016404190000000000000000006801ac07a6020000ab020000000000
             000000a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000007d037c00a007000000000000000000000000000000
-            00000000007c03a6010000ab010000000000000000830064007b03560097
-            038604010064005300
+            00000000007c03a6010000ab010000000000000000830064037b03560097
+            038604010064035300
            8           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-           9           6 LOAD_FAST                1 (data)
+          16           6 LOAD_FAST                1 (data)
                        8 LOAD_CONST               1 ('type')
                       10 BINARY_SUBSCR
                       20 LOAD_CONST               2 ('Follow')
                       22 COMPARE_OP               3 (!=)
                       28 POP_JUMP_FORWARD_IF_FALSE     2 (to 34)
          
-          10          30 LOAD_CONST               0 (None)
+          17          30 LOAD_CONST               3 (None)
                       32 RETURN_VALUE
          
-          12     >>   34 LOAD_FAST                1 (data)
-                      36 LOAD_CONST               3 ('actor')
+          19     >>   34 LOAD_FAST                1 (data)
+                      36 LOAD_CONST               4 ('actor')
                       38 BINARY_SUBSCR
                       48 STORE_FAST               2 (follow_actor)
          
-          13          50 LOAD_GLOBAL              1 (NULL + isinstance)
+          20          50 LOAD_GLOBAL              1 (NULL + isinstance)
                       62 LOAD_FAST                2 (follow_actor)
                       64 LOAD_GLOBAL              2 (dict)
                       76 PRECALL                  2
                       80 CALL                     2
                       90 POP_JUMP_FORWARD_IF_FALSE     8 (to 108)
          
-          14          92 LOAD_FAST                2 (follow_actor)
-                      94 LOAD_CONST               4 ('id')
+          21          92 LOAD_FAST                2 (follow_actor)
+                      94 LOAD_CONST               5 ('id')
                       96 BINARY_SUBSCR
                      106 STORE_FAST               2 (follow_actor)
          
-          16     >>  108 LOAD_GLOBAL              4 (logger)
+          23     >>  108 LOAD_GLOBAL              4 (logger)
                      120 LOAD_METHOD              3 (info)
-                     142 LOAD_CONST               5 ('Accepting follow request from %s')
+                     142 LOAD_CONST               6 ('Accepting follow request from %s')
                      144 LOAD_FAST                2 (follow_actor)
                      146 PRECALL                  2
                      150 CALL                     2
                      160 POP_TOP
          
-          18         162 LOAD_FAST                0 (actor)
+          25         162 LOAD_FAST                0 (client)
                      164 LOAD_ATTR                4 (activity_factory)
                      174 LOAD_METHOD              5 (accept)
                      196 LOAD_FAST                1 (data)
-                     198 LOAD_CONST               4 ('id')
+                     198 LOAD_CONST               5 ('id')
                      200 BINARY_SUBSCR
                      210 LOAD_FAST                1 (data)
-                     212 LOAD_CONST               3 ('actor')
+                     212 LOAD_CONST               4 ('actor')
                      214 BINARY_SUBSCR
                      224 BUILD_SET                1
-                     226 KW_NAMES                 6
+                     226 KW_NAMES                 7
                      228 PRECALL                  2
                      232 CALL                     2
                      242 LOAD_METHOD              6 (build)
                      264 PRECALL                  0
                      268 CALL                     0
                      278 STORE_FAST               3 (accept)
          
-          20         280 LOAD_FAST                0 (actor)
+          27         280 LOAD_FAST                0 (client)
                      282 LOAD_METHOD              7 (send_to_outbox)
                      304 LOAD_FAST                3 (accept)
                      306 PRECALL                  1
                      310 CALL                     1
                      320 GET_AWAITABLE            0
-                     322 LOAD_CONST               0 (None)
+                     322 LOAD_CONST               3 (None)
                  >>  324 SEND                     3 (to 332)
                      326 YIELD_VALUE
                      328 RESUME                   3
                      330 JUMP_BACKWARD_NO_INTERRUPT     4 (to 324)
                  >>  332 POP_TOP
-                     334 LOAD_CONST               0 (None)
+                     334 LOAD_CONST               3 (None)
                      336 RETURN_VALUE
          consts
-            None
+            'Automatically accepts follow requests. Include via\n\n    .. code-block:: toml\n\n        [username.handlers]\n        "mechanical_bull.actions.accept_follow_request" = true\n    '
             'type'
             'Follow'
+            None
             'actor'
             'id'
             'Accepting follow request from %s'
             ('to',)
          names      ('isinstance', 'dict', 'logger', 'info', 'activity_factory', 'accept', 'build', 'send_to_outbox')
-         varnames   ('actor', 'data', 'follow_actor', 'accept')
+         varnames   ('client', 'data', 'follow_actor', 'accept')
          freevars   ()
          cellvars   ()
          filename   '/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/accept_follow_request.py'
          name       'handle'
          firstlineno 8
-         lnotab 0x06011801040210012a01100236027602
-   names      ('logging', 'bovine', 'BovineActor', 'getLogger', '__name__', 'logger', 'dict', 'handle')
+         lnotab 0x06081801040210012a01100236027602
+   names      ('logging', 'bovine', 'BovineClient', 'getLogger', '__name__', 'logger', 'dict', 'handle')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/accept_follow_request.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108020c022003
```

### Comparing `mechanical_bull-0.1.0/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc` & `mechanical_bull-0.2.0/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xaf416e64 (Wed May 24 16:56:15 2023 UTC)
+moddate:  0xc5907c64 (Sun Jun  4 13:25:25 2023 UTC)
 files sz: 847
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.1.0/mechanical_bull/actions/reject_follow_request.py` & `mechanical_bull-0.2.0/mechanical_bull/actions/accept_follow_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import logging
 
-from bovine import BovineActor
+from bovine import BovineClient
 
 logger = logging.getLogger(__name__)
 
 
-async def handle(actor: BovineActor, data: dict):
+async def handle(client: BovineClient, data: dict):
+    """Automatically accepts follow requests. Include via
+
+    .. code-block:: toml
+
+        [username.handlers]
+        "mechanical_bull.actions.accept_follow_request" = true
+    """
     if data["type"] != "Follow":
         return
 
     follow_actor = data["actor"]
     if isinstance(follow_actor, dict):
         follow_actor = follow_actor["id"]
 
-    logger.info("Rejecting follow request from %s", follow_actor)
+    logger.info("Accepting follow request from %s", follow_actor)
 
-    reject = actor.activity_factory.accept(data["id"], to={data["actor"]}).build()
-    reject["type"] = "Reject"
+    accept = client.activity_factory.accept(data["id"], to={data["actor"]}).build()
 
-    await actor.send_to_outbox(reject)
+    await client.send_to_outbox(accept)
```

### Comparing `mechanical_bull-0.1.0/mechanical_bull/actions/test_accept_reject_follow_request.py` & `mechanical_bull-0.2.0/mechanical_bull/actions/test_accept_reject_follow_request.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.1.0/mechanical_bull/add_user.py` & `mechanical_bull-0.2.0/mechanical_bull/add_user.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.1.0/mechanical_bull/event_loop.py` & `mechanical_bull-0.2.0/mechanical_bull/event_loop.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,63 @@
 import json
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-async def handle_connection(client, handlers):
+async def handle_connection(client: bovine.BovineClient, handlers: list):
+    """Opens an event source and applies all handlers to captured events.
+
+    :param handlers:
+
+        list of methods taking at argument the BovineClient client and
+        a dictionary representing the ActivityPub activity."""
     event_source = await client.event_source()
     logger.info("Connected")
     async for event in event_source:
         if not event:
             return
         if event and event.data:
             data = json.loads(event.data)
             logger.debug(event.data)
 
             for handler in handlers:
                 await handler(client, data)
 
 
+async def handle_connection_with_reconnect(
+    client: bovine.BovineClient,
+    handlers: list,
+    client_name: str = "BovineClient",
+    wait_time: int = 10,
+):
+    """As handle_connection, but automatically recoonects after wait_time many seconds.
+
+    :param client_name:
+
+        Used for logging purpose
+
+    :param wait_time:
+
+        Time in seconds to wait between connection attempts."""
+    while True:
+        await handle_connection(client, handlers)
+        logger.info(
+            "Disconnected from server for %s, reconnecting in %d seconds",
+            client_name,
+            wait_time,
+        )
+        await asyncio.sleep(wait_time)
+
+
 async def loop(client_name, client_config, handlers):
     while True:
         try:
             async with bovine.BovineClient(client_config) as client:
-                while True:
-                    await handle_connection(client, handlers)
-                    logger.info(
-                        "Disconnected from server for %s, reconnecting in 10 seconds",
-                        client_name,
-                    )
-                    await asyncio.sleep(10)
+                await handle_connection_with_reconnect(
+                    client, handlers, client_name=client_name
+                )
         except Exception as e:
             logger.exception("Something went wrong for %s", client_name)
             logger.exception(e)
             await asyncio.sleep(60)
```

### Comparing `mechanical_bull-0.1.0/mechanical_bull/run.py` & `mechanical_bull-0.2.0/mechanical_bull/run.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.1.0/mechanical_bull/test_event_loop.py` & `mechanical_bull-0.2.0/mechanical_bull/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.1.0/pyproject.toml` & `mechanical_bull-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mechanical-bull"
-version = "0.1.0"
+version = "0.2.0"
 description = "A framework to automate reacting to ActivityStreams events."
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "mechanical_bull"}]
 repository = "https://codeberg.org/bovine/mechanical_bull"
 documentation = "https://mechanical-bull.readthedocs.io/en/latest/"
```

### Comparing `mechanical_bull-0.1.0/PKG-INFO` & `mechanical_bull-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanical-bull
-Version: 0.1.0
+Version: 0.2.0
 Summary: A framework to automate reacting to ActivityStreams events.
 Home-page: https://codeberg.org/bovine/mechanical_bull
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

