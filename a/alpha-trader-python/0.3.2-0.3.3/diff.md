# Comparing `tmp/alpha_trader_python-0.3.2.tar.gz` & `tmp/alpha_trader_python-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_trader_python-0.3.2.tar", max compression
+gzip compressed data, was "alpha_trader_python-0.3.3.tar", max compression
```

## Comparing `alpha_trader_python-0.3.2.tar` & `alpha_trader_python-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      255 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/README.md
--rw-r--r--   0        0        0       22 2023-05-21 19:00:18.011173 alpha_trader_python-0.3.2/alpha_trader/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/achievement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/authentication/__init__.py
--rw-r--r--   0        0        0      961 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/bank_account/__init__.py
--rw-r--r--   0        0        0     5117 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/bonds/__init__.py
--rw-r--r--   0        0        0     9225 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/client/__init__.py
--rw-r--r--   0        0        0     3352 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/company/__init__.py
--rw-r--r--   0        0        0      776 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/filter/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/listing/__init__.py
--rw-r--r--   0        0        0      387 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/logging/__init__.py
--rw-r--r--   0        0        0     4276 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/miner/__init__.py
--rw-r--r--   0        0        0     6091 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/order/__init__.py
--rw-r--r--   0        0        0      470 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/owner/__init__.py
--rw-r--r--   0        0        0       71 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/partner/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/portfolio/position.py
--rw-r--r--   0        0        0        0 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/price/__init__.py
--rw-r--r--   0        0        0      405 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/price/price.py
--rw-r--r--   0        0        0     2790 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/price/price_spread.py
--rw-r--r--   0        0        0     2771 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/securities_account/__init__.py
--rw-r--r--   0        0        0     8216 2023-05-21 19:00:17.239180 alpha_trader_python-0.3.2/alpha_trader/user/__init__.py
--rw-r--r--   0        0        0      929 2023-05-21 19:00:18.011173 alpha_trader_python-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/README.md
+-rw-r--r--   0        0        0       22 2023-06-04 10:59:03.491278 alpha_trader_python-0.3.3/alpha_trader/__init__.py
+-rw-r--r--   0        0        0     2074 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/achievement/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/authentication/__init__.py
+-rw-r--r--   0        0        0      961 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/bank_account/__init__.py
+-rw-r--r--   0        0        0     5117 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/bonds/__init__.py
+-rw-r--r--   0        0        0     9225 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/client/__init__.py
+-rw-r--r--   0        0        0     3352 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/company/__init__.py
+-rw-r--r--   0        0        0      776 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/filter/__init__.py
+-rw-r--r--   0        0        0     1155 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/listing/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/logging/__init__.py
+-rw-r--r--   0        0        0     4281 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/miner/__init__.py
+-rw-r--r--   0        0        0     6091 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/order/__init__.py
+-rw-r--r--   0        0        0      470 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/owner/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/partner/__init__.py
+-rw-r--r--   0        0        0     1629 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     1977 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/portfolio/position.py
+-rw-r--r--   0        0        0        0 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/price/__init__.py
+-rw-r--r--   0        0        0      405 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/price/price.py
+-rw-r--r--   0        0        0     2790 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/price/price_spread.py
+-rw-r--r--   0        0        0     2771 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/securities_account/__init__.py
+-rw-r--r--   0        0        0     8216 2023-06-04 10:59:02.667268 alpha_trader_python-0.3.3/alpha_trader/user/__init__.py
+-rw-r--r--   0        0        0      929 2023-06-04 10:59:03.491278 alpha_trader_python-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.3.3/PKG-INFO
```

### Comparing `alpha_trader_python-0.3.2/alpha_trader/achievement/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/achievement/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/bank_account/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/bank_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/bonds/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/bonds/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/client/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/client/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/company/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/company/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/filter/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/listing/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/listing/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/miner/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/miner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,7 +119,8 @@
             next_level_amortization_hours
         } (or {
             next_level_amortization_hours / 24
         } days)"""
         )
 
         return next_level_amortization_hours
+
```

### Comparing `alpha_trader_python-0.3.2/alpha_trader/order/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/order/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/portfolio/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/portfolio/position.py` & `alpha_trader_python-0.3.3/alpha_trader/portfolio/position.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from pydantic import BaseModel
-from typing import Dict
+from typing import Dict, Union
 
 from alpha_trader.listing import Listing
 from alpha_trader.price.price import Price
 from alpha_trader.client import Client
 
 
 class Position(BaseModel):
-    average_buying_price: int
+    average_buying_price: float
     committed_shares: int
-    current_ask_price: int
-    current_ask_size: int
-    current_bid_price: int
-    current_bid_size: int
-    last_buying_price: int
+    current_ask_price: Union[float, None]
+    current_ask_size: Union[int, None]
+    current_bid_price: Union[float, None]
+    current_bid_size: Union[int, None]
+    last_buying_price: Union[float, None]
     last_price: Price
     last_price_update: int
     listing: Listing
     number_of_shares: int
     security_identifier: str
     type: str
-    volume: int
+    volume: float
     client: Client
 
     @staticmethod
     def initialize_from_api_response(api_response: Dict, client: Client):
         return Position(
             average_buying_price=api_response["averageBuyingPrice"],
             committed_shares=api_response["committedShares"],
```

### Comparing `alpha_trader_python-0.3.2/alpha_trader/price/price_spread.py` & `alpha_trader_python-0.3.3/alpha_trader/price/price_spread.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/securities_account/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/securities_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/alpha_trader/user/__init__.py` & `alpha_trader_python-0.3.3/alpha_trader/user/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.3.2/pyproject.toml` & `alpha_trader_python-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-trader-python"
-version = "0.3.2"
+version = "0.3.3"
 description = "Python SDK for https://alpha-trader.com"
 authors = ["maltemelzer"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alpha_trader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `alpha_trader_python-0.3.2/PKG-INFO` & `alpha_trader_python-0.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpha-trader-python
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python SDK for https://alpha-trader.com
 License: MIT
 Author: maltemelzer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

