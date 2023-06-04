# Comparing `tmp/simple-websocket-0.8.1.tar.gz` & `tmp/simple-websocket-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-websocket-0.8.1.tar", last modified: Sun Sep 11 09:11:19 2022, max compression
+gzip compressed data, was "simple-websocket-0.9.0.tar", last modified: Thu Nov 17 10:29:59 2022, max compression
```

## Comparing `simple-websocket-0.8.1.tar` & `simple-websocket-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-09-11 09:11:19.192201 simple-websocket-0.8.1/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2021-04-17 13:46:40.000000 simple-websocket-0.8.1/LICENSE
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1263 2022-09-11 09:11:19.192448 simple-websocket-0.8.1/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      619 2021-06-13 23:24:21.000000 simple-websocket-0.8.1/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-04-17 13:42:13.000000 simple-websocket-0.8.1/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      821 2022-09-11 09:11:19.193314 simple-websocket-0.8.1/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-04-17 13:42:19.000000 simple-websocket-0.8.1/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-09-11 09:11:19.185242 simple-websocket-0.8.1/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-09-11 09:11:19.188546 simple-websocket-0.8.1/src/simple_websocket/
--rw-r--r--   0 mgrinberg   (502) staff       (20)       80 2021-06-07 14:10:16.000000 simple-websocket-0.8.1/src/simple_websocket/__init__.py
--rw-r--r--   0 mgrinberg   (502) staff       (20)    19867 2022-09-11 09:06:31.000000 simple-websocket-0.8.1/src/simple_websocket/ws.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-09-11 09:11:19.191829 simple-websocket-0.8.1/src/simple_websocket.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1263 2022-09-11 09:11:19.000000 simple-websocket-0.8.1/src/simple_websocket.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      373 2022-09-11 09:11:19.000000 simple-websocket-0.8.1/src/simple_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2022-09-11 09:11:19.000000 simple-websocket-0.8.1/src/simple_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-04-17 14:17:18.000000 simple-websocket-0.8.1/src/simple_websocket.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)        8 2022-09-11 09:11:19.000000 simple-websocket-0.8.1/src/simple_websocket.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       17 2022-09-11 09:11:19.000000 simple-websocket-0.8.1/src/simple_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-11-17 10:29:59.020191 simple-websocket-0.9.0/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1072 2022-11-16 23:28:57.000000 simple-websocket-0.9.0/LICENSE
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1263 2022-11-17 10:29:59.020339 simple-websocket-0.9.0/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      619 2022-11-16 23:28:57.000000 simple-websocket-0.9.0/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2022-11-16 23:28:57.000000 simple-websocket-0.9.0/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      821 2022-11-17 10:29:59.020940 simple-websocket-0.9.0/setup.cfg
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2022-11-16 23:28:57.000000 simple-websocket-0.9.0/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-11-17 10:29:59.012927 simple-websocket-0.9.0/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-11-17 10:29:59.016228 simple-websocket-0.9.0/src/simple_websocket/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       80 2022-11-16 23:28:57.000000 simple-websocket-0.9.0/src/simple_websocket/__init__.py
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    19914 2022-11-16 23:42:58.000000 simple-websocket-0.9.0/src/simple_websocket/ws.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-11-17 10:29:59.019849 simple-websocket-0.9.0/src/simple_websocket.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1263 2022-11-17 10:29:59.000000 simple-websocket-0.9.0/src/simple_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      373 2022-11-17 10:29:59.000000 simple-websocket-0.9.0/src/simple_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2022-11-17 10:29:59.000000 simple-websocket-0.9.0/src/simple_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-04-17 14:17:18.000000 simple-websocket-0.9.0/src/simple_websocket.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        8 2022-11-17 10:29:59.000000 simple-websocket-0.9.0/src/simple_websocket.egg-info/requires.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       17 2022-11-17 10:29:59.000000 simple-websocket-0.9.0/src/simple_websocket.egg-info/top_level.txt
```

### Comparing `simple-websocket-0.8.1/LICENSE` & `simple-websocket-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-websocket-0.8.1/PKG-INFO` & `simple-websocket-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-websocket
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple WebSocket server and client for Python
 Home-page: https://github.com/miguelgrinberg/simple-websocket
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/simple-websocket/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `simple-websocket-0.8.1/README.md` & `simple-websocket-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `simple-websocket-0.8.1/src/simple_websocket/ws.py` & `simple-websocket-0.9.0/src/simple_websocket/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,19 +59,17 @@
         if thread_class is None:
             import threading
             thread_class = threading.Thread
         if event_class is None:  # pragma: no branch
             import threading
             event_class = threading.Event
         if selector_class is None:
-            import selectors
             selector_class = selectors.DefaultSelector
-
+        self.selector_class = selector_class
         self.event = event_class()
-        self.selector = selector_class()
 
         self.ws = WSConnection(connection_type)
         self.handshake()
 
         if not self.connected:  # pragma: no cover
             raise ConnectionError()
         self.thread = thread_class(target=self._thread)
@@ -96,15 +94,15 @@
             out_data = self.ws.send(TextMessage(data=str(data)))
         self.sock.send(out_data)
 
     def receive(self, timeout=None):
         """Receive data over the WebSocket connection.
 
         :param timeout: Amount of time to wait for the data, in seconds. Set
-                        to ``None`` (the default) to wait undefinitely. Set
+                        to ``None`` (the default) to wait indefinitely. Set
                         to 0 to read without blocking.
 
         The data received is returned, as ``bytes`` or ``str``, depending on
         the type of the incoming message.
         """
         while self.connected and not self.input_buffer:
             if not self.event.wait(timeout=timeout):
@@ -114,15 +112,15 @@
             raise ConnectionClosed(self.close_reason, self.close_message)
         return self.input_buffer.pop(0)
 
     def close(self, reason=None, message=None):
         """Close the WebSocket connection.
 
         :param reason: A numeric status code indicating the reason of the
-                       closure, as defined by the WebSocket specifiation. The
+                       closure, as defined by the WebSocket specification. The
                        default is 1000 (normal closure).
         :param message: A text message to be sent to the other side.
         """
         if not self.connected:
             raise ConnectionClosed(self.close_reason, self.close_message)
         out_data = self.ws.send(CloseConnection(
             reason or CloseReason.NORMAL_CLOSURE, message))
@@ -138,15 +136,15 @@
         # the server-side of the WebSocket protocol.
         return None
 
     def _thread(self):
         sel = None
         if self.ping_interval:
             next_ping = time() + self.ping_interval
-            sel = self.selector
+            sel = self.selector_class()
             sel.register(self.sock, selectors.EVENT_READ, True)
 
         while self.connected:
             try:
                 if sel:
                     now = time()
                     if next_ping <= now or not sel.select(next_ping - now):
@@ -162,16 +160,19 @@
                 in_data = self.sock.recv(self.receive_bytes)
                 if len(in_data) == 0:
                     raise OSError()
             except (OSError, ConnectionResetError):  # pragma: no cover
                 self.connected = False
                 self.event.set()
                 break
+
             self.ws.receive_data(in_data)
             self.connected = self._handle_events()
+        sel.close() if sel else None
+        self.sock.close()
 
     def _handle_events(self):
         keep_going = True
         out_data = b''
         for event in self.ws.events():
             try:
                 if isinstance(event, Request):
```

### Comparing `simple-websocket-0.8.1/src/simple_websocket.egg-info/PKG-INFO` & `simple-websocket-0.9.0/src/simple_websocket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-websocket
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple WebSocket server and client for Python
 Home-page: https://github.com/miguelgrinberg/simple-websocket
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/simple-websocket/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

