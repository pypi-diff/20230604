# Comparing `tmp/d2y-0.2.18.tar.gz` & `tmp/d2y-0.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d2y-0.2.18.tar", last modified: Sat May 13 18:52:25 2023, max compression
+gzip compressed data, was "d2y-0.2.24.tar", last modified: Fri Jun  2 15:43:59 2023, max compression
```

## Comparing `d2y-0.2.18.tar` & `d2y-0.2.24.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-05-13 18:52:25.266013 d2y-0.2.18/
--rw-r--r--   0 amenon     (501) staff       (20)      566 2023-05-13 18:52:25.265906 d2y-0.2.18/PKG-INFO
--rw-r--r--   0 amenon     (501) staff       (20)     3570 2023-05-10 13:17:04.000000 d2y-0.2.18/README.md
-drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-05-13 18:52:25.264040 d2y-0.2.18/d2y/
--rw-r--r--   0 amenon     (501) staff       (20)        0 2023-04-28 17:37:27.000000 d2y-0.2.18/d2y/__init__.py
--rw-r--r--   0 amenon     (501) staff       (20)     1879 2023-05-13 18:51:26.000000 d2y-0.2.18/d2y/enums.py
--rw-r--r--   0 amenon     (501) staff       (20)     5891 2023-05-13 17:07:52.000000 d2y-0.2.18/d2y/formulas.py
-drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-05-13 18:52:25.265464 d2y-0.2.18/d2y/models/
--rw-r--r--   0 amenon     (501) staff       (20)      172 2023-05-10 19:28:29.000000 d2y-0.2.18/d2y/models/__init__.py
--rw-r--r--   0 amenon     (501) staff       (20)     1297 2023-05-10 13:16:03.000000 d2y-0.2.18/d2y/models/asset.py
--rw-r--r--   0 amenon     (501) staff       (20)     3433 2023-05-13 17:07:52.000000 d2y-0.2.18/d2y/models/option.py
--rw-r--r--   0 amenon     (501) staff       (20)     1458 2023-05-10 13:16:03.000000 d2y-0.2.18/d2y/models/order.py
--rw-r--r--   0 amenon     (501) staff       (20)      887 2023-05-10 13:16:03.000000 d2y-0.2.18/d2y/models/position.py
--rw-r--r--   0 amenon     (501) staff       (20)      857 2023-05-10 13:16:03.000000 d2y-0.2.18/d2y/models/simple_option.py
--rw-r--r--   0 amenon     (501) staff       (20)      934 2023-05-10 19:38:01.000000 d2y-0.2.18/d2y/models/trade.py
--rw-r--r--   0 amenon     (501) staff       (20)     1247 2023-05-10 13:16:03.000000 d2y-0.2.18/d2y/models/user.py
--rw-r--r--   0 amenon     (501) staff       (20)     9434 2023-05-13 17:09:04.000000 d2y-0.2.18/d2y/sdk.py
-drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-05-13 18:52:25.264598 d2y-0.2.18/d2y.egg-info/
--rw-r--r--   0 amenon     (501) staff       (20)      566 2023-05-13 18:52:25.000000 d2y-0.2.18/d2y.egg-info/PKG-INFO
--rw-r--r--   0 amenon     (501) staff       (20)      441 2023-05-13 18:52:25.000000 d2y-0.2.18/d2y.egg-info/SOURCES.txt
--rw-r--r--   0 amenon     (501) staff       (20)        1 2023-05-13 18:52:25.000000 d2y-0.2.18/d2y.egg-info/dependency_links.txt
--rw-r--r--   0 amenon     (501) staff       (20)        9 2023-05-13 18:52:25.000000 d2y-0.2.18/d2y.egg-info/requires.txt
--rw-r--r--   0 amenon     (501) staff       (20)       10 2023-05-13 18:52:25.000000 d2y-0.2.18/d2y.egg-info/top_level.txt
--rw-r--r--   0 amenon     (501) staff       (20)       38 2023-05-13 18:52:25.266047 d2y-0.2.18/setup.cfg
--rw-r--r--   0 amenon     (501) staff       (20)      747 2023-05-13 18:51:58.000000 d2y-0.2.18/setup.py
-drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-05-13 18:52:25.265745 d2y-0.2.18/tests/
--rw-r--r--   0 amenon     (501) staff       (20)        0 2023-04-28 17:37:27.000000 d2y-0.2.18/tests/__init__.py
--rw-r--r--   0 amenon     (501) staff       (20)     2658 2023-05-10 13:16:03.000000 d2y-0.2.18/tests/test_formulas.py
--rw-r--r--   0 amenon     (501) staff       (20)     5318 2023-05-13 17:07:52.000000 d2y-0.2.18/tests/test_sdk.py
+drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-06-02 15:43:59.062594 d2y-0.2.24/
+-rw-r--r--   0 amenon     (501) staff       (20)     4177 2023-06-02 15:43:59.062474 d2y-0.2.24/PKG-INFO
+-rw-r--r--   0 amenon     (501) staff       (20)     3570 2023-05-10 13:17:04.000000 d2y-0.2.24/README.md
+drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-06-02 15:43:59.061436 d2y-0.2.24/d2y/
+-rw-r--r--   0 amenon     (501) staff       (20)        0 2023-04-28 17:37:27.000000 d2y-0.2.24/d2y/__init__.py
+-rw-r--r--   0 amenon     (501) staff       (20)     1302 2023-06-01 18:23:59.000000 d2y-0.2.24/d2y/enums.py
+-rw-r--r--   0 amenon     (501) staff       (20)     8742 2023-06-01 18:30:58.000000 d2y-0.2.24/d2y/formulas.py
+-rw-r--r--   0 amenon     (501) staff       (20)    12002 2023-06-02 09:47:29.000000 d2y-0.2.24/d2y/models.py
+-rw-r--r--   0 amenon     (501) staff       (20)    26320 2023-06-02 12:20:21.000000 d2y-0.2.24/d2y/sdk.py
+drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-06-02 15:43:59.062018 d2y-0.2.24/d2y.egg-info/
+-rw-r--r--   0 amenon     (501) staff       (20)     4177 2023-06-02 15:43:59.000000 d2y-0.2.24/d2y.egg-info/PKG-INFO
+-rw-r--r--   0 amenon     (501) staff       (20)      281 2023-06-02 15:43:59.000000 d2y-0.2.24/d2y.egg-info/SOURCES.txt
+-rw-r--r--   0 amenon     (501) staff       (20)        1 2023-06-02 15:43:59.000000 d2y-0.2.24/d2y.egg-info/dependency_links.txt
+-rw-r--r--   0 amenon     (501) staff       (20)        9 2023-06-02 15:43:59.000000 d2y-0.2.24/d2y.egg-info/requires.txt
+-rw-r--r--   0 amenon     (501) staff       (20)       10 2023-06-02 15:43:59.000000 d2y-0.2.24/d2y.egg-info/top_level.txt
+-rw-r--r--   0 amenon     (501) staff       (20)       38 2023-06-02 15:43:59.062632 d2y-0.2.24/setup.cfg
+-rw-r--r--   0 amenon     (501) staff       (20)     1024 2023-06-01 10:16:09.000000 d2y-0.2.24/setup.py
+drwxr-xr-x   0 amenon     (501) staff       (20)        0 2023-06-02 15:43:59.062321 d2y-0.2.24/tests/
+-rw-r--r--   0 amenon     (501) staff       (20)        0 2023-05-29 22:20:39.000000 d2y-0.2.24/tests/__init__.py
+-rw-r--r--   0 amenon     (501) staff       (20)     2658 2023-05-10 13:16:03.000000 d2y-0.2.24/tests/test_formulas.py
+-rw-r--r--   0 amenon     (501) staff       (20)     6335 2023-05-30 15:18:09.000000 d2y-0.2.24/tests/test_sdk.py
```

### Comparing `d2y-0.2.18/README.md` & `d2y-0.2.24/README.md`

 * *Files identical despite different names*

### Comparing `d2y-0.2.18/setup.py` & `d2y-0.2.24/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # setup.py
-
 from setuptools import setup, find_packages
+from os import path
 
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+    
 setup(
     name="d2y",
-    version="0.2.18",
+    version="0.2.24",
     description="A Python SDK for the D2Y Exchange API",
     author="d2y Core Team",
     author_email="admin@d2y.exchange",
     url="",
     packages=find_packages(),
     install_requires=[
         "requests",
@@ -20,8 +24,10 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.9",
+    long_description=long_description,
+    long_description_content_type='text/markdown'    
 )
```

### Comparing `d2y-0.2.18/tests/test_formulas.py` & `d2y-0.2.24/tests/test_formulas.py`

 * *Files identical despite different names*

### Comparing `d2y-0.2.18/tests/test_sdk.py` & `d2y-0.2.24/tests/test_sdk.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,176 @@
-# tests/test_sdk.py
 import unittest
-
-# from d2y.models import CreateOrder, OrderType, Side
-from d2y.sdk import TradingClient
 import os
 from dotenv import load_dotenv
-from d2y.sdk import TradingClient
-from d2y.formulas import *
-from d2y.enums import *
-from d2y.models.order import PlaceOrderArgs
+from sdk import Client
+from enums import *
+from models import *
 
 load_dotenv()
 
-API_KEY = os.environ["API_KEY"]
-API_SECRET = os.environ["API_SECRET"]
+API_KEY = 'cKVG7-0KTcGpBiCJ4Zb993zxZeX245eIGv4rc0JAskU'
+API_SECRET = 'fvTxXGpE8XLkDiJPFn_uSrXpo4cJI1RDaiHX3B8NNCY'
+
+# API_KEY = os.environ["API_KEY"]
+# API_SECRET = os.environ["API_SECRET"]
 BASE_URL = os.environ.get("API_BASE_URL", "https://api.dev.d2y.exchange")
 
-TEST_OPTION_ID = os.environ.get("TEST_OPTION_ID", 31617)
-TEST_OPTION_STRIKE_PRICE = float(os.environ.get("TEST_OPTION_STRIKE_PRICE", 2700))
+TEST_OPTION_ID = os.environ.get("TEST_OPTION_ID", 167704)
+TEST_OPTION_STRIKE_PRICE = float(os.environ.get("TEST_OPTION_STRIKE_PRICE", 1600))
 TEST_OPTION_EXPIRATION_TIMESTAMP = os.environ.get(
-    "TEST_OPTION_EXPIRATION_TIMESTAMP", "2023-06-30T08:00:00Z"
+    "TEST_OPTION_EXPIRATION_TIMESTAMP", "2023-06-02T08:00:00Z"
 )
 
 
 class TestTradingClient(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.sdk = TradingClient(API_KEY, API_SECRET, BASE_URL)
+        cls.sdk = TradingClient(api_key=API_KEY, api_secret=API_SECRET, base_url=BASE_URL)
+
+    def test_get_profile(self):
+        print("\n****** GETTING USER PROFILE ******\n")
+        profile = self.sdk.get_profile()
+        print("\n****** Profile:", profile)
+        for key, value in profile.__dict__.items():
+            print(f"{key}: {value}")
 
-    def test_get_user(self):
-        print("\n****** GETTING USER INFO ******\n")
-        user = self.sdk.get_user_info()
-        print("User:", user)
-        for key, value in user.__dict__.items():
+    def test_get_account(self):
+        print("\n****** GETTING ACCOUNT ******\n")
+        account = self.sdk.get_account()
+        print("Account:", account)
+        for key, value in account.__dict__.items():
+            print(f"{key}: {value}")
+
+    def test_get_transfers(self):
+        print("\n****** GETTING Transfers ******\n")
+        transfers = self.sdk.get_transfers()
+        print("Transfers:", transfers)
+        for transfer in transfers:
+            print("Transfer:", transfer)
+            for key, value in transfer.__dict__.items():
+                print(f"{key}: {value}")        
+
+    def test_portfolio(self):
+        print("\n****** GETTING PORTFOLIO ******\n")
+        portfolio = self.sdk.get_portfolio()
+        print("Portfolio:", portfolio)
+        for key, value in portfolio.__dict__.items():
             print(f"{key}: {value}")
 
     def test_get_assets(self):
         print("\n****** GETTING ASSETS ******\n")
         assets = self.sdk.get_assets()
         for asset in assets:
             print("Asset:", asset)
             for key, value in asset.__dict__.items():
                 print(f"{key}: {value}")
 
-    def test_get_options(self):
-        print("\n****** GETTING OPTIONS ******\n")
-        options = self.sdk.get_options(
+
+    def test_get_markets(self):
+        print("\n****** GETTING MARKETS ******\n")
+        markets = self.sdk.get_markets(
             expiration_timestamp=[TEST_OPTION_EXPIRATION_TIMESTAMP],
             option_type=OptionType.CALL,
-            ordering="strike_price",
             strike_price=[TEST_OPTION_STRIKE_PRICE],
+            instrument_type=InstrumentType.OPTION,
         )
-        for option in options:
-            print("Option:", option)
-            for key, value in option.__dict__.items():
+        for market in markets:
+            print("Market:", market)
+            for key, value in market.__dict__.items():
                 print(f"{key}: {value}")
 
     def test_get_orderbook(self):
         print("\n****** GETTING ORDERBOOK ******\n")
-        option_id = TEST_OPTION_ID
-        orderbook = self.sdk.get_orderbook(option_id)
+        orderbook = self.sdk.get_orderbook(instrument_id=TEST_OPTION_ID)
         print("Orderbook for option_id:", orderbook)
 
-    def test_get_orders_with_pagination(self):
+    def test_get_orders(self):
         print("\n****** GETTING ORDERS ******\n")
         orders = self.sdk.get_orders(status=[OrderStatus.OPEN], limit=3, offset=0)
         for order in orders[:3]:
             print("Order:", order)
             for key, value in order.__dict__.items():
                 print(f"{key}: {value}")
 
-    def test_positions(self):
+    def test_cancel_all_orders(self):
+        print("\n****** CANCELING ALL ORDERS ******\n")
+        cancellation_result = self.sdk.cancel_all_orders(
+            # expiration_timestamp=TEST_OPTION_EXPIRATION_TIMESTAMP,
+            # instrument_id=TEST_OPTION_ID,
+            # instrument_name=TEST_OPTION_NAME,
+            # instrument_type=InstrumentType.OPTION,
+            strike_price=1600
+        )
+        print("Cancellation Result:", cancellation_result)
+        for key, value in cancellation_result.items():
+            print(f"{key}: {value}")
+
+    def test_reduce_order(self):
+        print("\n****** REDUCING ORDER ******\n")
+        order_id = 187921  # Replace with the actual order ID
+        reduced_order_result = self.sdk.reduce_order(order_id=order_id, quantity=.5)
+        print("Reduced Order Result:", reduced_order_result)
+        for key, value in reduced_order_result.items():
+            print(f"{key}: {value}")
+
+
+    def test_get_positions(self):
         print("\n****** GETTING POSITIONS ******\n")
         positions = self.sdk.get_positions()
         for position in positions:
             print("Position:", position)
             for key, value in position.__dict__.items():
                 print(f"{key}: {value}")
 
-    def test_place_and_cancel_order(self):
-        print("\n****** PLACING ORDER ******\n")
-        order = self.sdk.place_order(
-            option=TEST_OPTION_ID,
+    def test_get_trades(self):
+        print("\n****** GETTING TRADES ******\n")
+        trades = self.sdk.get_trades()
+        for trade in trades:
+            print("Trade:", trade)
+            for key, value in trade.__dict__.items():
+                print(f"{key}: {value}")
+
+    def test_post_orders_and_cancel_order(self):
+        print("\n****** POSTING AND CANCELING ORDER ******\n")
+        new_order = self.sdk.place_order(
+            instrument_id=TEST_OPTION_ID,
             price=0.01,
             quantity=2,
             side=OrderSide.BUY,
-            order_type=OrderType.LIMIT,
+            order_type=OrderType.LIMIT
         )
-        print("Order:", order)
-        for key, value in order.__dict__.items():
+        print("Order:", new_order)
+        for key, value in new_order.__dict__.items():
             print(f"{key}: {value}")
 
         print("\n****** CANCELLING ORDER ******\n")
-        cancelled_order = self.sdk.cancel_order(order.id)
-        print("Cancelled order:", cancelled_order)
-        for key, value in cancelled_order.__dict__.items():
-            print(f"{key}: {value}")
-
-    def test_place_bulk_orders_and_get_trades(self):
-        print("\n****** PLACING BULK ORDERS ******\n")
-        orders = self.sdk.place_bulk_orders(
-            [
-                PlaceOrderArgs(
-                    option=TEST_OPTION_ID,
-                    price=0.01,
-                    quantity=1,
-                    side=OrderSide.BUY,
-                    order_type=OrderType.LIMIT,
-                ),
-                PlaceOrderArgs(
-                    option=TEST_OPTION_ID,
-                    quantity=1,
-                    side=OrderSide.SELL,
-                    order_type=OrderType.MARKET,
-                ),
-            ]
-        )
+        cancel_order = self.sdk.cancel_order(new_order.id)
+        print("Cancelled order:", cancel_order)
+        # for key, value in cancel_order.__dict__.items():
+        #     print(f"{key}: {value}")
+
+    def test_post_multi_orders_and_get_trades(self):
+        print("\n****** POSTING BULK ORDERS ******\n")
+        orders = self.sdk.place_bulk_order([
+            {
+                "instrument_id": TEST_OPTION_ID,
+                "price": 0.01,
+                "quantity": 1,
+                "side": OrderSide.BUY,
+                "order_type": OrderType.LIMIT,
+            },
+            {
+                "instrument_id": TEST_OPTION_ID,
+                "quantity": 1,
+                "side": OrderSide.SELL,
+                "order_type": OrderType.MARKET,
+            },
+        ])
         for order in orders:
             print("Order:", order)
             for key, value in order.__dict__.items():
                 print(f"{key}: {value}")
 
-        print("\n****** GETTING TRADES ******\n")
-        trades = self.sdk.get_trades()
-        for trade in trades:
-            print("Trade:", trade)
-            for key, value in trade.__dict__.items():
-                print(f"{key}: {value}")
-
-    def test_calculate_option_price(self):
-        print("\n****** TESTING CALCULATE_OPTION_PRICE ******\n")
-
-        # Define parameters for the function
-        S = 100.0  # Current stock price
-        K = 100.0  # Strike price of the option
-        T = datetime(2024, 1, 1).replace(tzinfo=pytz.UTC)  # Expiration date
-        r = 0.05  # Annual risk-free interest rate, expressed as a decimal
-        sigma = 0.2  # Annual volatility of the stock price, expressed as a decimal
-        option_type = OptionType.CALL  # Option type (CALL or PUT)
-
-        # Call the function with the parameters
-        option_price = calculate_option_price(S, K, T, r, sigma, option_type)
-
-        # Print the calculated option price
-        print(f"Calculated option price: {option_price}")
 
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

