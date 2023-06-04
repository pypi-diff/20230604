# Comparing `tmp/mon2pcap-1.0.2.tar.gz` & `tmp/mon2pcap-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mon2pcap-1.0.2.tar", max compression
+gzip compressed data, was "mon2pcap-1.0.3.tar", max compression
```

## Comparing `mon2pcap-1.0.2.tar` & `mon2pcap-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.2/LICENSE
--rw-r--r--   0        0        0     2328 2023-05-27 08:35:47.654469 mon2pcap-1.0.2/README.md
--rw-r--r--   0        0        0      204 2023-06-04 10:08:17.059955 mon2pcap-1.0.2/mon2pcap/__init__.py
--rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.2/mon2pcap/common.py
--rw-r--r--   0        0        0     2849 2023-06-04 11:18:28.078177 mon2pcap-1.0.2/mon2pcap/console.py
--rw-r--r--   0        0        0     3213 2023-06-04 10:03:27.795673 mon2pcap-1.0.2/mon2pcap/constants.py
--rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.2/mon2pcap/errors.py
--rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.2/mon2pcap/helpers.py
--rw-r--r--   0        0        0     7537 2023-06-04 10:13:54.030726 mon2pcap-1.0.2/mon2pcap/mon2pcap.py
--rw-r--r--   0        0        0    56507 2023-06-04 10:03:28.174218 mon2pcap-1.0.2/mon2pcap/packets.py
--rw-r--r--   0        0        0      877 2023-06-04 11:18:24.618178 mon2pcap-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 mon2pcap-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2338 2023-06-04 11:37:08.244034 mon2pcap-1.0.3/README.md
+-rw-r--r--   0        0        0      204 2023-06-04 10:08:17.059955 mon2pcap-1.0.3/mon2pcap/__init__.py
+-rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.3/mon2pcap/common.py
+-rw-r--r--   0        0        0     2850 2023-06-04 11:23:50.048354 mon2pcap-1.0.3/mon2pcap/console.py
+-rw-r--r--   0        0        0     3213 2023-06-04 10:03:27.795673 mon2pcap-1.0.3/mon2pcap/constants.py
+-rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.3/mon2pcap/errors.py
+-rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.3/mon2pcap/helpers.py
+-rw-r--r--   0        0        0     7537 2023-06-04 10:13:54.030726 mon2pcap-1.0.3/mon2pcap/mon2pcap.py
+-rw-r--r--   0        0        0    56507 2023-06-04 10:03:28.174218 mon2pcap-1.0.3/mon2pcap/packets.py
+-rw-r--r--   0        0        0     1017 2023-06-04 11:55:13.583598 mon2pcap-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3299 1970-01-01 00:00:00.000000 mon2pcap-1.0.3/PKG-INFO
```

### Comparing `mon2pcap-1.0.2/LICENSE` & `mon2pcap-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.2/README.md` & `mon2pcap-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ⚠️ All data-link layer protocols are generated, the MACs there are bogus.  
 ⚠️ All non-IP packets data-link, network and transport protocols are bogus.  
 ⚠️ If it's IP packet, the ports are correct (most of the time) but the transport level protocol is bogus.  
 The layers had to be generated for wireshark and other tools working with pcap file formats to properly dissect them.  
 
 ## Installation
 ### Prerequisites
-- [Python 3.6+](https://www.python.org/downloads/)  
+- [Python 3.8.1 or newer](https://www.python.org/downloads/)  
   ⚠️ Installers usually ask to add Python to `PATH`, do it now and you will avoid headaches later. 
 - [pip - The Python Package Installer](https://pip.pypa.io/en/stable/installation/)
 - _mon2pcap_ installation:
   ```
   $ pip install mon2pcap
   ```
```

### Comparing `mon2pcap-1.0.2/mon2pcap/console.py` & `mon2pcap-1.0.3/mon2pcap/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/python
 
 import sys
 import logging
 import argparse
-import jinja2
 
 from collections import OrderedDict
 import importlib.metadata
+import jinja2
 
 from .mon2pcap import Mon2Pcap
 from .packets import PARSERS
 from .constants import COLORS
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 
+
 def print_stats(stats: OrderedDict):
     """Print statistics nicely
     :param stats: Stats dict
 
     """
     total = sum(stats.values()) - (stats["Ignored"] + stats["Filtered"])
     environment = jinja2.Environment(autoescape=True)
```

### Comparing `mon2pcap-1.0.2/mon2pcap/constants.py` & `mon2pcap-1.0.3/mon2pcap/constants.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.2/mon2pcap/helpers.py` & `mon2pcap-1.0.3/mon2pcap/helpers.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.2/mon2pcap/mon2pcap.py` & `mon2pcap-1.0.3/mon2pcap/mon2pcap.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.2/mon2pcap/packets.py` & `mon2pcap-1.0.3/mon2pcap/packets.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.2/pyproject.toml` & `mon2pcap-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 [tool.poetry]
 name = "mon2pcap"
-version = "1.0.2"
+version = "1.0.3"
 description = "Convert StarOS \"monitor subscriber\" or \"monitor protocol\" ASCII dump to PCAP"
 authors = ["Artur Russu <arussu@cisco.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/arussu/mon2pcap"
 keywords = ["scapy", "mon2pcap"]
 classifiers = [
     "Intended Audience :: Telecommunications Industry",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: System :: Networking",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8.1"
 scapy = "^2.5.0"
 tqdm = "^4.65.0"
 Jinja2 = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
-flake8 = "^6.0.0"
 black = "23.3.0"
+flake8 = "^6.0.0"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.black]
 line-length = 88
```

### Comparing `mon2pcap-1.0.2/PKG-INFO` & `mon2pcap-1.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: mon2pcap
-Version: 1.0.2
+Version: 1.0.3
 Summary: Convert StarOS "monitor subscriber" or "monitor protocol" ASCII dump to PCAP
 Home-page: https://github.com/arussu/mon2pcap
 License: GPL-3.0-only
 Keywords: scapy,mon2pcap
 Author: Artur Russu
 Author-email: arussu@cisco.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Networking
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/arussu/mon2pcap
 Description-Content-Type: text/markdown
 
@@ -30,15 +33,15 @@
 ⚠️ All data-link layer protocols are generated, the MACs there are bogus.  
 ⚠️ All non-IP packets data-link, network and transport protocols are bogus.  
 ⚠️ If it's IP packet, the ports are correct (most of the time) but the transport level protocol is bogus.  
 The layers had to be generated for wireshark and other tools working with pcap file formats to properly dissect them.  
 
 ## Installation
 ### Prerequisites
-- [Python 3.6+](https://www.python.org/downloads/)  
+- [Python 3.8.1 or newer](https://www.python.org/downloads/)  
   ⚠️ Installers usually ask to add Python to `PATH`, do it now and you will avoid headaches later. 
 - [pip - The Python Package Installer](https://pip.pypa.io/en/stable/installation/)
 - _mon2pcap_ installation:
   ```
   $ pip install mon2pcap
   ```
```

