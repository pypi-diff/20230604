# Comparing `tmp/flightgear_python-1.2.2.tar.gz` & `tmp/flightgear_python-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightgear_python-1.2.2.tar", max compression
+gzip compressed data, was "flightgear_python-1.3.0.tar", max compression
```

## Comparing `flightgear_python-1.2.2.tar` & `flightgear_python-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1083 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/LICENSE
--rw-r--r--   0        0        0     3159 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/__init__.py
--rw-r--r--   0        0        0     3784 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/ctrls_v27.py
--rw-r--r--   0        0        0     2890 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/fdm_v24.py
--rw-r--r--   0        0        0     3181 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/fdm_v25.py
--rwxr-xr-x   0        0        0    13516 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/fg_if.py
--rw-r--r--   0        0        0     1704 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/fg_util.py
--rw-r--r--   0        0        0     2294 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/flightgear_python/general_util.py
--rw-r--r--   0        0        0     1046 2023-03-13 18:11:33.838048 flightgear_python-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3906 2023-03-13 18:11:46.408953 flightgear_python-1.2.2/setup.py
--rw-r--r--   0        0        0     4096 2023-03-13 18:11:46.409374 flightgear_python-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3159 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/__init__.py
+-rw-r--r--   0        0        0     3784 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/ctrls_v27.py
+-rw-r--r--   0        0        0     2890 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/fdm_v24.py
+-rw-r--r--   0        0        0     3181 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/fdm_v25.py
+-rwxr-xr-x   0        0        0    14040 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/fg_if.py
+-rw-r--r--   0        0        0     1704 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/fg_util.py
+-rw-r--r--   0        0        0     2294 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/general_util.py
+-rw-r--r--   0        0        0     1630 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/flightgear_python/gui_v8.py
+-rw-r--r--   0        0        0     1046 2023-06-04 16:35:10.362326 flightgear_python-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3906 2023-06-04 16:35:24.169587 flightgear_python-1.3.0/setup.py
+-rw-r--r--   0        0        0     4096 2023-06-04 16:35:24.170080 flightgear_python-1.3.0/PKG-INFO
```

### Comparing `flightgear_python-1.2.2/LICENSE` & `flightgear_python-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.2.2/README.md` & `flightgear_python-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,11 +46,11 @@
         time.sleep(0.5)
 ```
 
 Supported interfaces:
 - [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)
   - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))
   - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))
-  - [ ] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))
+  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))
 - [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)
 - [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)
 - [ ] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)
```

### Comparing `flightgear_python-1.2.2/flightgear_python/ctrls_v27.py` & `flightgear_python-1.3.0/flightgear_python/ctrls_v27.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.2.2/flightgear_python/fdm_v24.py` & `flightgear_python-1.3.0/flightgear_python/fdm_v24.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.2.2/flightgear_python/fdm_v25.py` & `flightgear_python-1.3.0/flightgear_python/fdm_v25.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.2.2/flightgear_python/fg_if.py` & `flightgear_python-1.3.0/flightgear_python/fg_if.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         try:
             rx_msg, _ = self.fg_rx_sock.recvfrom(1024)
         except socket.timeout as e:
             raise FGConnectionError(f'Timeout waiting for data, waited {self.rx_timeout_s} seconds') from e
         try:
             s: Container = self.fg_net_struct.parse(rx_msg)
         except ConstError as e:
-            raise FGCommunicationError(f'Could not decode FG stream. Is this the right FDM version?\n{e}') from e
+            raise FGCommunicationError(f'Could not decode FG stream. Did you set the right version?\n{e}') from e
 
         if isinstance(self, FDMConnection):
             # Fix FG's radian parsing error :(
             s = fix_fg_radian_parsing(s)
 
         # Call user method
         s = self.fg_rx_cb(s, self.event_pipe)
@@ -160,14 +160,32 @@
             from .ctrls_v27 import ctrls_struct
         else:
             raise NotImplementedError(f'Controls version {ctrls_version} not supported yet')
         # Create Struct from Dict
         self.fg_net_struct = Struct(*[k / v for k, v in ctrls_struct.items()])
 
 
+class GuiConnection(FGConnection):
+    """
+    FlightGear GUI Connection
+
+    :param gui_version: Net GUI version (8)
+    """
+
+    def __init__(self, gui_version: int):
+        super().__init__()
+        # TODO: Support auto-version check
+        if gui_version == 8:
+            from .gui_v8 import gui_struct
+        else:
+            raise NotImplementedError(f'GUI version {gui_version} not supported yet')
+        # Create Struct from Dict
+        self.fg_net_struct = Struct(*[k / v for k, v in gui_struct.items()])
+
+
 class PropsConnection:
     """
     FlightGear Telnet Interface Connection (also known as the property interface).
     See https://wiki.flightgear.org/Telnet_usage for general details.
 
     :param host: IP address of FG (usually localhost)
     :param tcp_port: Port of the telnet socket (i.e. the ``5500`` from\
```

### Comparing `flightgear_python-1.2.2/flightgear_python/fg_util.py` & `flightgear_python-1.3.0/flightgear_python/fg_util.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.2.2/flightgear_python/general_util.py` & `flightgear_python-1.3.0/flightgear_python/general_util.py`

 * *Files identical despite different names*

### Comparing `flightgear_python-1.2.2/pyproject.toml` & `flightgear_python-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flightgear_python"
-version = "1.2.2"
+version = "1.3.0"
 description = "Interface for FlightGear network connections"
 authors = ["Julianne Swinoga <julianneswinoga@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `flightgear_python-1.2.2/setup.py` & `flightgear_python-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['construct>=2.10,<3.0', 'multiprocess==0.70.12.2']
 
 setup_kwargs = {
     'name': 'flightgear-python',
-    'version': '1.2.2',
+    'version': '1.3.0',
     'description': 'Interface for FlightGear network connections',
-    'long_description': '# FlightGear Python Interface\n[![Documentation Status](https://readthedocs.org/projects/flightgear-python/badge/?version=latest)](https://flightgear-python.readthedocs.io/en/latest/?badge=latest)\n[![CircleCI](https://circleci.com/gh/julianneswinoga/flightgear-python.svg?style=shield)](https://circleci.com/gh/julianneswinoga/flightgear-python)\n[![Coverage Status](https://coveralls.io/repos/github/julianneswinoga/flightgear-python/badge.svg?branch=master)](https://coveralls.io/github/julianneswinoga/flightgear-python?branch=master)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flightgear_python)](https://pypi.org/project/flightgear-python/)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/flightgear-python)\n\n`flightgear-python` is an interface package to the [FlightGear flight simulation software](https://www.flightgear.org/) aimed at simplicity.\n\nInstall: `pip3 install flightgear-python`\n\nDon\'t know where to begin? Check out the [quick-start](https://flightgear-python.readthedocs.io/en/latest/quickstart.html) documentation.\n\nFDM example, from `examples/simple_fdm.py`\n```python\n"""\nSimple Flight Dynamics Model (FDM) example that makes the altitude increase and the plane roll in the air.\n"""\nimport time\nfrom flightgear_python.fg_if import FDMConnection\n\ndef fdm_callback(fdm_data, event_pipe):\n    if event_pipe.child_poll():\n        phi_rad_child, = event_pipe.child_recv()  # unpack tuple\n        # set only the data that we need to\n        fdm_data[\'phi_rad\'] = phi_rad_child  # we can force our own values\n    fdm_data.alt_m = fdm_data.alt_m + 0.5  # or just make a relative change\n    return fdm_data  # return the whole structure\n\n"""\nStart FlightGear with `--native-fdm=socket,out,30,localhost,5501,udp --native-fdm=socket,in,30,localhost,5502,udp`\n(you probably also want `--fdm=null` and `--max-fps=30` to stop the simulation fighting with\nthese external commands)\n"""\nif __name__ == \'__main__\':  # NOTE: This is REQUIRED on Windows!\n    fdm_conn = FDMConnection(fdm_version=24)  # May need to change version from 24\n    fdm_event_pipe = fdm_conn.connect_rx(\'localhost\', 5501, fdm_callback)\n    fdm_conn.connect_tx(\'localhost\', 5502)\n    fdm_conn.start()  # Start the FDM RX/TX loop\n    \n    phi_rad_parent = 0.0\n    while True:\n        phi_rad_parent += 0.1\n        # could also do `fdm_conn.event_pipe.parent_send` so you just need to pass around `fdm_conn`\n        fdm_event_pipe.parent_send((phi_rad_parent,))  # send tuple\n        time.sleep(0.5)\n```\n\nSupported interfaces:\n- [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)\n  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))\n  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))\n  - [ ] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))\n- [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)\n- [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)\n- [ ] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)\n',
+    'long_description': '# FlightGear Python Interface\n[![Documentation Status](https://readthedocs.org/projects/flightgear-python/badge/?version=latest)](https://flightgear-python.readthedocs.io/en/latest/?badge=latest)\n[![CircleCI](https://circleci.com/gh/julianneswinoga/flightgear-python.svg?style=shield)](https://circleci.com/gh/julianneswinoga/flightgear-python)\n[![Coverage Status](https://coveralls.io/repos/github/julianneswinoga/flightgear-python/badge.svg?branch=master)](https://coveralls.io/github/julianneswinoga/flightgear-python?branch=master)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flightgear_python)](https://pypi.org/project/flightgear-python/)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/flightgear-python)\n\n`flightgear-python` is an interface package to the [FlightGear flight simulation software](https://www.flightgear.org/) aimed at simplicity.\n\nInstall: `pip3 install flightgear-python`\n\nDon\'t know where to begin? Check out the [quick-start](https://flightgear-python.readthedocs.io/en/latest/quickstart.html) documentation.\n\nFDM example, from `examples/simple_fdm.py`\n```python\n"""\nSimple Flight Dynamics Model (FDM) example that makes the altitude increase and the plane roll in the air.\n"""\nimport time\nfrom flightgear_python.fg_if import FDMConnection\n\ndef fdm_callback(fdm_data, event_pipe):\n    if event_pipe.child_poll():\n        phi_rad_child, = event_pipe.child_recv()  # unpack tuple\n        # set only the data that we need to\n        fdm_data[\'phi_rad\'] = phi_rad_child  # we can force our own values\n    fdm_data.alt_m = fdm_data.alt_m + 0.5  # or just make a relative change\n    return fdm_data  # return the whole structure\n\n"""\nStart FlightGear with `--native-fdm=socket,out,30,localhost,5501,udp --native-fdm=socket,in,30,localhost,5502,udp`\n(you probably also want `--fdm=null` and `--max-fps=30` to stop the simulation fighting with\nthese external commands)\n"""\nif __name__ == \'__main__\':  # NOTE: This is REQUIRED on Windows!\n    fdm_conn = FDMConnection(fdm_version=24)  # May need to change version from 24\n    fdm_event_pipe = fdm_conn.connect_rx(\'localhost\', 5501, fdm_callback)\n    fdm_conn.connect_tx(\'localhost\', 5502)\n    fdm_conn.start()  # Start the FDM RX/TX loop\n    \n    phi_rad_parent = 0.0\n    while True:\n        phi_rad_parent += 0.1\n        # could also do `fdm_conn.event_pipe.parent_send` so you just need to pass around `fdm_conn`\n        fdm_event_pipe.parent_send((phi_rad_parent,))  # send tuple\n        time.sleep(0.5)\n```\n\nSupported interfaces:\n- [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)\n  - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))\n  - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))\n  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))\n- [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)\n- [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)\n- [ ] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)\n',
     'author': 'Julianne Swinoga',
     'author_email': 'julianneswinoga@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `flightgear_python-1.2.2/PKG-INFO` & `flightgear_python-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightgear-python
-Version: 1.2.2
+Version: 1.3.0
 Summary: Interface for FlightGear network connections
 License: MIT
 Author: Julianne Swinoga
 Author-email: julianneswinoga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -68,12 +68,12 @@
         time.sleep(0.5)
 ```
 
 Supported interfaces:
 - [x] [Native Protocol](https://wiki.flightgear.org/Property_Tree/Sockets) (currently only UDP)
   - [x] Flight Dynamics Model ([`net_fdm.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_fdm.hxx))
   - [x] Controls ([`net_ctrls.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_ctrls.hxx))
-  - [ ] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))
+  - [x] GUI ([`net_gui.hxx`](https://github.com/FlightGear/flightgear/blob/next/src/Network/net_gui.hxx))
 - [ ] [Generic Protocol](https://wiki.flightgear.org/Generic_protocol)
 - [x] [Telnet](https://wiki.flightgear.org/Telnet_usage)
 - [ ] [HTTP](https://wiki.flightgear.org/Property_Tree_Servers)
```

