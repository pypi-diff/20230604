# Comparing `tmp/mon2pcap-1.0.1.tar.gz` & `tmp/mon2pcap-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mon2pcap-1.0.1.tar", max compression
+gzip compressed data, was "mon2pcap-1.0.2.tar", max compression
```

## Comparing `mon2pcap-1.0.1.tar` & `mon2pcap-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.1/LICENSE
--rw-r--r--   0        0        0     2328 2023-05-27 08:35:47.654469 mon2pcap-1.0.1/README.md
--rw-r--r--   0        0        0      204 2023-06-04 10:08:17.059955 mon2pcap-1.0.1/mon2pcap/__init__.py
--rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.1/mon2pcap/common.py
--rw-r--r--   0        0        0     2770 2023-06-04 10:58:10.193486 mon2pcap-1.0.1/mon2pcap/console.py
--rw-r--r--   0        0        0     3213 2023-06-04 10:03:27.795673 mon2pcap-1.0.1/mon2pcap/constants.py
--rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.1/mon2pcap/errors.py
--rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.1/mon2pcap/helpers.py
--rw-r--r--   0        0        0     7537 2023-06-04 10:13:54.030726 mon2pcap-1.0.1/mon2pcap/mon2pcap.py
--rw-r--r--   0        0        0    56507 2023-06-04 10:03:28.174218 mon2pcap-1.0.1/mon2pcap/packets.py
--rw-r--r--   0        0        0      877 2023-06-04 11:00:19.518771 mon2pcap-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 mon2pcap-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-26 07:14:15.966359 mon2pcap-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2328 2023-05-27 08:35:47.654469 mon2pcap-1.0.2/README.md
+-rw-r--r--   0        0        0      204 2023-06-04 10:08:17.059955 mon2pcap-1.0.2/mon2pcap/__init__.py
+-rw-r--r--   0        0        0      428 2023-05-30 13:18:44.837375 mon2pcap-1.0.2/mon2pcap/common.py
+-rw-r--r--   0        0        0     2849 2023-06-04 11:18:28.078177 mon2pcap-1.0.2/mon2pcap/console.py
+-rw-r--r--   0        0        0     3213 2023-06-04 10:03:27.795673 mon2pcap-1.0.2/mon2pcap/constants.py
+-rw-r--r--   0        0        0      348 2023-06-04 10:03:27.778216 mon2pcap-1.0.2/mon2pcap/errors.py
+-rw-r--r--   0        0        0     1928 2023-06-04 10:03:27.787298 mon2pcap-1.0.2/mon2pcap/helpers.py
+-rw-r--r--   0        0        0     7537 2023-06-04 10:13:54.030726 mon2pcap-1.0.2/mon2pcap/mon2pcap.py
+-rw-r--r--   0        0        0    56507 2023-06-04 10:03:28.174218 mon2pcap-1.0.2/mon2pcap/packets.py
+-rw-r--r--   0        0        0      877 2023-06-04 11:18:24.618178 mon2pcap-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3135 1970-01-01 00:00:00.000000 mon2pcap-1.0.2/PKG-INFO
```

### Comparing `mon2pcap-1.0.1/LICENSE` & `mon2pcap-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.1/README.md` & `mon2pcap-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.1/mon2pcap/console.py` & `mon2pcap-1.0.2/mon2pcap/console.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import sys
 import logging
 import argparse
 import jinja2
 
 from collections import OrderedDict
+import importlib.metadata
 
-from .mon2pcap import Mon2Pcap, __version__
+from .mon2pcap import Mon2Pcap
 from .packets import PARSERS
 from .constants import COLORS
 
+__version__ = importlib.metadata.version(__package__ or __name__)
 
 def print_stats(stats: OrderedDict):
     """Print statistics nicely
     :param stats: Stats dict
 
     """
     total = sum(stats.values()) - (stats["Ignored"] + stats["Filtered"])
```

### Comparing `mon2pcap-1.0.1/mon2pcap/constants.py` & `mon2pcap-1.0.2/mon2pcap/constants.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.1/mon2pcap/helpers.py` & `mon2pcap-1.0.2/mon2pcap/helpers.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.1/mon2pcap/mon2pcap.py` & `mon2pcap-1.0.2/mon2pcap/mon2pcap.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.1/mon2pcap/packets.py` & `mon2pcap-1.0.2/mon2pcap/packets.py`

 * *Files identical despite different names*

### Comparing `mon2pcap-1.0.1/pyproject.toml` & `mon2pcap-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mon2pcap"
-version = "1.0.1"
+version = "1.0.2"
 description = "Convert StarOS \"monitor subscriber\" or \"monitor protocol\" ASCII dump to PCAP"
 authors = ["Artur Russu <arussu@cisco.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/arussu/mon2pcap"
 keywords = ["scapy", "mon2pcap"]
 classifiers = [
```

### Comparing `mon2pcap-1.0.1/PKG-INFO` & `mon2pcap-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mon2pcap
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert StarOS "monitor subscriber" or "monitor protocol" ASCII dump to PCAP
 Home-page: https://github.com/arussu/mon2pcap
 License: GPL-3.0-only
 Keywords: scapy,mon2pcap
 Author: Artur Russu
 Author-email: arussu@cisco.com
 Requires-Python: >=3.11,<4.0
```

