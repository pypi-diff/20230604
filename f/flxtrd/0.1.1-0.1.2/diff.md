# Comparing `tmp/flxtrd-0.1.1.tar.gz` & `tmp/flxtrd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.1.1.tar", max compression
+gzip compressed data, was "flxtrd-0.1.2.tar", max compression
```

## Comparing `flxtrd-0.1.1.tar` & `flxtrd-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     9136 2023-06-03 18:45:23.386447 flxtrd-0.1.1/LICENSE
--rw-r--r--   0        0        0     3999 2023-06-03 18:51:18.453728 flxtrd-0.1.1/README.md
--rw-r--r--   0        0        0     2117 2023-06-03 18:52:35.405572 flxtrd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      610 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.1/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     4769 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      581 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4405 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     2451 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/core/types.py
--rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.1/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0     8590 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-03 18:45:23.386447 flxtrd-0.1.1/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     4740 1970-01-01 00:00:00.000000 flxtrd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-03 18:45:23.386447 flxtrd-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5760 2023-06-04 18:58:26.939632 flxtrd-0.1.2/README.md
+-rw-r--r--   0        0        0     2158 2023-06-04 18:58:54.311757 flxtrd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-06-04 18:58:26.943632 flxtrd-0.1.2/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.2/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-04 18:58:26.947632 flxtrd-0.1.2/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      580 2023-06-04 18:58:26.947632 flxtrd-0.1.2/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-03 18:45:23.386447 flxtrd-0.1.2/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4426 2023-06-04 18:58:26.947632 flxtrd-0.1.2/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-03 18:45:23.386447 flxtrd-0.1.2/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-03 18:45:23.386447 flxtrd-0.1.2/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-03 18:45:23.386447 flxtrd-0.1.2/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     5150 2023-06-04 18:58:26.951632 flxtrd-0.1.2/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0     1552 2023-06-04 18:58:26.951632 flxtrd-0.1.2/src/flxtrd/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 10:23:00.709774 flxtrd-0.1.2/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0    10040 2023-06-04 18:58:26.951632 flxtrd-0.1.2/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-03 18:45:23.386447 flxtrd-0.1.2/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-03 18:45:23.386447 flxtrd-0.1.2/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     6501 1970-01-01 00:00:00.000000 flxtrd-0.1.2/PKG-INFO
```

### Comparing `flxtrd-0.1.1/LICENSE` & `flxtrd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.1/README.md` & `flxtrd-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -18,106 +18,157 @@
 
 
 Install GLocalFlexTrade Python package
 
 ```sh
 pip install flxtrd
 ```
-### Basic Example
+
+### Basic trading client example
 
 ```py
 """Example usage of the trading client using AMPQ protocol"""
-import sys
-import time
 from logging import ERROR, INFO
-from pprint import pformat
-from random import random
 
 from flxtrd import (
-    Broker,
+    ASK,
+    BID,
+    FlexBroker,
     FlexAPIClient,
-    Flexibility,
-    Market,
+    FlexResource,
+    FlexMarket,
     MarketOrder,
-    OrderType,
-    User,
+    FlexUser,
     log,
+    utils,
 )
 
 
 def main() -> None:
-    GFLEX_API_URL = "localhost"
+    GLOCALFLEX_MARKET_URL = "localhost"
 
-    user = User(
-        name="<your_email>",
-        password="<your_password>",
-        accessToken="<your_device_access_token>",
-    )
-
-    market = Market(ip=GFLEX_API_URL, broker=Broker(ip=GFLEX_API_URL))
-
-    # Define the tradable flexibility to sell or buy
-    flexResource = Flexibility(
-        wattage=random() * 100,
-        starttime=int((time.time() + (60 * 60 * random() * 10)) / 60) * 60 * 1000,
-        duration=int(((round(random()) * 14 + 1) / 60.0) * 60 * 60 * 1000),
-        expirationtime=int(time.time() / (60 * 1000) + random() * 20) * 60 * 1000,
-    )
+    user = FlexUser(name="<your_email>",
+                    password="<your_password>",
+                    access_token="<your_device_access_token>",
+                    )
 
-    # Create a market order to sell or buy flexibility
-    market_order = MarketOrder(type=OrderType.ASK, price=100, flexibility=flexResource)
+    market = FlexMarket(market_url=GLOCALFLEX_MARKET_URL)
 
     # Create a AMPQ client that connects to the message broker
-    trading_client = FlexAPIClient(base_url=GFLEX_API_URL, user=user, market=market)
+    trading_client = FlexAPIClient(base_url=GLOCALFLEX_MARKET_URL,
+                                   user=user,
+                                   market=market
+                                   )
+
+    # Define a flexibility resource that will be traded
+    # The resource is a 100W power for 60 minutes starting in 5 minutes
+    flex_resource = FlexResource(power_w=100,
+                                 start_time_epoch_s=utils.utc_timestamp_s() + utils.min_to_s(5), 
+                                 duration_min=60,  
+                                 order_expiration_min=50)
+
+    # Create a market ask order to sell flexibility
+    market_order = MarketOrder(order_type=ASK,
+                               price_eur=100,
+                               resource=flex_resource)
+
+    # Send the market order to the message broker
+    # The connection to the broker will be initiated automatically
+    _, err = trading_client.send_order(market_order=market_order,
+                                       verify_ssl=False)
+    
+    if err: log(ERROR, err)
+
+    # Create a market bid order to buy flexibility
+    market_order = MarketOrder(order_type=BID,
+                               price_eur=100,
+                               resource=flex_resource)
+
+    _, err = trading_client.send_order(market_order=market_order,
+                                       verify_ssl=False)
+    
+    if err: log(ERROR, err); sys.exit(1)
+
+    # Check the market responses for closed_deals, price tick messages
+    # from the message broker for 60 seconds and exit
+    wait_sec = 0
+    expected_responses = 3
+    log(INFO, f"Waiting for messages from market broker")
+
+    try:
+        while wait_sec < 60:
+            market_responses = trading_client.check_market_responses()
+            if market_responses is not None:
+                log(INFO, f"Received {len(market_responses)} responses from market broker")
+                # Close the connection to the market message broker
+                if len(market_responses) == expected_responses:
+                    break
+                
+            time.sleep(1)
+            wait_sec += 1
+
+    except KeyboardInterrupt:
+        log(INFO, "Keyboard interrupt received. Closing connection to the market broker")
+    finally:
+        trading_client.trade_protocol.close_connection()
 
-    # Send a request to the GLocalFlex with REST API
-    response, err = trading_client.make_request(
-        method="POST",
-        endpoint="/users/login",
-        data={"email": user.name, "password": user.password},
-    )
 
-    if err:
-        log(ERROR, err)
-        sys.exit(1)
+if __name__ == "__main__":
+    main()
 
-    log(INFO, pformat(response.request_response.json()))
-    log(INFO, response.request_response.status_code)
+```
 
-    # Send the market order to the message broker with AMPQ protocol
-    # The connection to the market message broker will be initiated automatically
-    response, err = trading_client.send_order(
-        method="",
-        verify_ssl=False,
-        order=market_order,
-    )
 
-    if err:
-        log(ERROR, err)
-        sys.exit(1)
+### Basic REST API client example
+
+```py
+"""Example usage of the REST API client"""
+from logging import ERROR, INFO
+from pprint import pformat
 
-    log(INFO, "Received response from message broker")
-    log(INFO, response.order_response)
+from flxtrd import (
+    ASK,
+    BID,
+    FlexBroker,
+    FlexAPIClient,
+    FlexResource,
+    FlexMarket,
+    MarketOrder,
+    FlexUser,
+    log,
+    utils,
+)
+
+
+def main() -> None:
+    GLOCALFLEX_MARKET_URL = "localhost"
 
-    # Send the market order to the message broker with AMPQ protocol
-    # The connection to the market message broker will be initiated automatically
-    response, err = trading_client.send_order(
-        method="",
-        verify_ssl=False,
-        order=market_order,
-    )
+    user = FlexUser(name="<your_email>",
+                    password="<your_password>",
+                    access_token="<your_device_access_token>"
+                    )
 
+    
+    market = FlexMarket(market_url=GLOCALFLEX_MARKET_URL)
+
+    # Create a AMPQ client that connects to the message broker
+    trading_client = FlexAPIClient(base_url=GLOCALFLEX_MARKET_URL,
+                                   user=user,
+                                   market=market
+                                   )
+
+    # Send a request to the GLocalFlex with REST API
+    response, err = trading_client.make_request(method="POST",
+                                                endpoint="/users/login",
+                                                data={"email": user.name, "password": user.password},
+                                                )
     if err:
         log(ERROR, err)
-        sys.exit(1)
 
-    log(INFO, "Received response from message broker")
-    log(INFO, response.order_response)
-
-    # Close the connection to the market message broker
-    trading_client.trade_protocol.close_connection()
+    log(INFO, pformat(response.request_response.json()))
+    log(INFO, response.request_response.status_code)
 
 
 if __name__ == "__main__":
     main()
 
-```
+```
```

### Comparing `flxtrd-0.1.1/pyproject.toml` & `flxtrd-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.1.1"
+version = "0.1.2"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
@@ -33,20 +33,21 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # [tool.poetry.scripts]
 # gflex-trading-bot = "gflex.client:main"
 
 [tool.flake8]
-max-line-length = 90
+max-line-length = 100
 max-complexity = 18
 ignore = "F401 E501"
 
 [tool.black]
-line-length = 90
+line-length = 100
+multiline = "VERTICAL_HANGING_INDENT"
 target-version = ['py310']
 preview = true
 
 [tool.mypy]
 files = ["flxtrd"]
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
@@ -57,15 +58,15 @@
 show_error_codes = "True"
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 target-version = "py37"
-line-length = 90
+line-length = 100
 fix = false
 select = [
     # flake8-2020
     "YTT",
     # flake8-bandit
     "S",
     # flake8-bugbear
```

### Comparing `flxtrd-0.1.1/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.1.2/src/flxtrd/core/plugins/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from logging import DEBUG, ERROR, INFO
 
 import requests
 
 from flxtrd.core.logger import log
 from flxtrd.core.plugins.base import BasePlugin
-from flxtrd.core.types import APIResponse, User
+from flxtrd.core.types import FlexResponse, FlexUser
 
 
 @dataclass
 class AuthResponse:
     """Container for the Auth response"""
 
     userId: str
@@ -19,15 +19,15 @@
 
 
 class AuthPlugin(BasePlugin):
     """Plugin for authentication"""
 
     plugin_name = "AuthPlugin"
 
-    def __init__(self, user: User, authServer: str, verify_ssl: bool = True) -> None:
+    def __init__(self, user: FlexUser, authServer: str, verify_ssl: bool = True) -> None:
         self.authServer = authServer
         self.user = user
         self.verify_ssl = verify_ssl
         self.ssl_context = self._creat_ssl_context()
 
     def _creat_ssl_context(self) -> ssl.SSLContext:
         context = ssl.create_default_context()
@@ -40,22 +40,22 @@
         self,
         method: str = None,
         url: str = None,
         headers: dict = None,
         params: dict = None,
         data: dict = None,
     ) -> None:
-        if self.user.accessToken is not None:
+        if self.user.access_token is not None:
             self.validateApplicationToken(
                 authServer=self.authServer,
-                accessToken=self.user.accessToken,
+                accessToken=self.user.access_token,
                 verify_ssl=self.verify_ssl,
             )
 
-    def after_request(self, response: APIResponse) -> None:
+    def after_request(self, response: FlexResponse) -> None:
         pass
 
     def auth_client(
         authServer: str, username: str, password: str, appKey: str
     ) -> AuthResponse:
         AuthResponse(userId="", appKey="", appToken=appKey)
 
@@ -72,25 +72,25 @@
             "email": self.user.username,
             "password": self.user.password,
         }
         response = requests.post(userauthurl, data=authdata)
         if response.status_code == 200:
             log(INFO, "USER AUTH SUCCESFULL")
             json_response = response.json()
-            self.user.userId = json_response["userId"]
+            self.user.user_id = json_response["userId"]
             if "locations" in json_response:
                 for locs in json_response["locations"]:
-                    if self.user.appKey:
-                        if self.user.appKey == locs["_id"]:
-                            self.user.accessToken = locs["token"]
+                    if self.user.app_key:
+                        if self.user.app_key == locs["_id"]:
+                            self.user.access_token = locs["token"]
                             break
                     else:
                         # Pick first application/Metering point
-                        self.user.appKey = locs["_id"]
-                        self.user.accessToken = locs["token"]
+                        self.user.app_key = locs["_id"]
+                        self.user.access_token = locs["token"]
                         break
         else:
             log(
                 INFO,
                 "Location/measurement point/application auth failed with"
                 f" response {response.status_code}",
             )
@@ -99,38 +99,38 @@
         self,
         authServer: str,
         accessToken: str,
         endpoint: str = "/users/mptoken/",
         verify_ssl: bool = True,
     ) -> None:
         if self._isUserValidated():
-            log(DEBUG, "User already validated")
+            log(INFO, "User already validated")
             return
 
         appAuthUrl = f"https://{authServer}{endpoint}{accessToken}"
         response = requests.get(appAuthUrl, verify=verify_ssl)
 
         if response.status_code != 200:
             log(
                 ERROR,
                 f"Response status code {response.status_code},"
                 f"failed to validate accessToken {accessToken}",
             )
             return "", ""
 
-        self.user.userId = response.json()["userId"]
+        self.user.user_id = response.json()["userId"]
         if "locations" in response.json():
             if len(response.json()["locations"]) > 0:
-                self.user.appKey = response.json()["locations"][0]["_id"]
+                self.user.app_key = response.json()["locations"][0]["_id"]
             else:
-                self.user.appKey = None
+                self.user.app_key = None
                 log(ERROR, f"Failed to validate accessToken {accessToken}")
                 return
 
         log(INFO, "Application token successfully received and validated")
         return
 
     def _isUserValidated(self) -> bool:
         """Check if the user is validated based on exising appKey"""
-        if self.user.appKey is None:
+        if self.user.app_key is None:
             return False
         return True
```

### Comparing `flxtrd-0.1.1/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.1.2/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.1/src/flxtrd/protocols/ampq.py` & `flxtrd-0.1.2/src/flxtrd/protocols/ampq.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,122 @@
 import json
 import ssl as _ssl
+import sys
 import time
 from logging import DEBUG, ERROR, INFO
+from pprint import pformat
 from typing import Optional
 
 import pika
 
 from flxtrd.core.logger import log
 from flxtrd.core.types import (
-    Broker,
+    FlexBroker,
     FlexError,
-    Flexibility,
-    Market,
+    FlexResource,
+    FlexMarket,
     MarketOrder,
     OrderType,
-    User,
+    FlexUser,
 )
 from flxtrd.protocols.base import BaseAPI
 
+    
+def create_line_message(
+    user: FlexUser, flexibility: FlexResource, marketOrder: MarketOrder
+):
+    """Create a line protocol message for InfluxDB that is the payload in the AMQP message
+
+    Format ask:
+    ask,applicationKey=64218f1adc42c714c1f08043,version=1 starttime=1685730000000i,wattage=19.556418841474642,runtime=60000i,totalenergy=0.32594031402457735,askingprice=7.933964367826437,expirationtime=1685730000000i
+
+    Bid:
+    bid,applicationKey=64218f1adc42c714c1f08043,version=1 starttime=1685732700000i,wattage=226.3288909510559,runtime=840000i,totalenergy=52.81007455524638,biddingprice=6.56704792164692,expirationtime=1685732700000i
+
+    """
+    lineordermsg = ""
+    if marketOrder.order_type == OrderType.ASK:
+        pricename = "askingprice"
+    elif marketOrder.order_type == OrderType.BID:
+        pricename = "biddingprice"
+    else:
+        raise FlexError(f"Order type {marketOrder.order_type} not supported")
+
+    order_type = marketOrder.order_type
+    application_key = user.app_key
+    wattage = flexibility.power_w
+    duration = flexibility.duration_min
+    starttime = flexibility.start_time_epoch_ms
+    totalenergy = flexibility.energy_wh
+    orderprice = marketOrder.price_eur
+    expirationtime = flexibility.expiration_time_epoch_ms
+
+    lineordermsg = (
+        f"{order_type.value},"
+        f"applicationKey={application_key},"
+        f"version=1 starttime={starttime}i,"
+        f"wattage={wattage},"
+        f"runtime={duration}i,"
+        f"totalenergy={totalenergy},"
+        f"{pricename}={orderprice},"
+        f"expirationtime={expirationtime}i"
+    )
+
+    return json.dumps(lineordermsg).strip('"')
+
 
 class AmpqAPI(BaseAPI):
     """Amqp API implementation that connects to public API"""
 
-    def __init__(self, base_url: str, user: User, broker: Broker, callback_fn=None):
+    def __init__(self, base_url: str, user: FlexUser, broker: FlexBroker, callback_fn=None):
         super().__init__(base_url=base_url)
-        self.user: User = user
-        self.broker: Broker = broker
+        self.user: FlexUser = user
+        self.broker: FlexBroker = broker
         self.ssl_options: pika.SSLOptions = None
         self.connection = None
         self.channel = None
         self.callback_queue_id = None
         self.callback_fn = callback_fn
-        self.callback_response = None
+        self.callback_responses: list = []
 
     def send_request(
         self,
-        endpoint: str = None,
+        endpoint: Optional[str] = None,
         params: Optional[dict] = None,
         data: Optional[dict] = None,
         verifiy_ssl: Optional[bool] = False,
         **kwargs,
     ) -> dict:
         if "market" not in kwargs:
             raise FlexError("'market' not found arguments")
         if "user" not in kwargs:
             raise FlexError("'user' not found in arguments")
-        if "order" not in kwargs:
-            raise FlexError("'order' not found in arguments")
 
-        market: Market = kwargs["market"]
-
-        user: User = kwargs["user"]
+        market: FlexMarket = kwargs["market"]
+        user: FlexUser = kwargs["user"]
         order: MarketOrder = kwargs["order"]
-        flexibility = order.flexibility
-
-        routingkey = order.type.value
+        flexibility = order.resource
 
-        log(INFO, f"Using {routingkey} as routing key for message broker")
+        routingkey = order.order_type.value
 
-        log(INFO, f"Creating line protocol message for the order {order}")
-        msg = self.create_line_message(
+        log(DEBUG, f"Using {routingkey} as routing key for message broker")
+        log(
+            DEBUG,
+            f"Creating line protocol message for the  {order.order_type.name} order",
+        )
+        msg = create_line_message(
             user=user, flexibility=flexibility, marketOrder=order
         )
 
         log(INFO, f"Send market order {order}")
         log(DEBUG, f"Order message: {msg}")
 
         self.publish(
             message=msg,
-            userid=user.userId,
+            userid=user.user_id,
             routingkey=routingkey,
             exchangename=market.broker.exchangename,
         )
 
         replies = self.checkreplies()
 
         err = None
@@ -94,18 +138,23 @@
         #  appkey or accesskeys are available
         # based on what the user provided different methods
         #  to connect to the server can be selected
         ssl_options = self._ssl_context(verify_ssl)
         err = self._connecttobrokerWithAppToken(
             user=self.user,
             broker=self.broker,
-            ssl_options=ssl_options,
-            verify_ssl=verify_ssl,
+            ssl_options=ssl_options
         )
-        # TODO
+
+        if not err:
+            self.set_consumer(
+                callback=self.callback_on_response,
+                callback_queue=self.callback_queue_id,
+                channel=self.channel,
+            )
         return err
 
     def close_connection(self):
         """Close connection gracefully to message broker"""
         if self.connection is not None:
             self.connection.close()
             log(INFO, "Connection closed")
@@ -113,15 +162,15 @@
             log(INFO, "No connection to be closed")
 
     def publish(self, message: str, userid: str, routingkey: str, exchangename=str):
         """Send message to the broker"""
         props = pika.BasicProperties(
             user_id=userid,
             reply_to=self.callback_queue_id,
-            headers={"sendertimestamp_in_ms": getcurrenttimems()},
+            headers={"sendertimestamp_in_ms": get_current_time_ms()},
         )
         try:
             self.channel.basic_publish(
                 exchange=exchangename,
                 routing_key=routingkey,
                 properties=props,
                 body=message,
@@ -135,32 +184,27 @@
     def is_connected(self):
         if self.connection is None:
             return False
         return self.connection.is_open
 
     def _connecttobrokerWithAppToken(
         self,
-        user: User,
-        broker: Broker,
-        ssl_options: pika.SSLOptions,
-        verify_ssl: bool = True,
+        user: FlexUser,
+        broker: FlexBroker,
+        ssl_options: pika.SSLOptions
     ):
         """Connects to the broker with the application token"""
         err = None
-        brokerip = broker.ip
+        brokerip = broker.url
         brokerport = broker.port
-        accessToken = user.accessToken
+        accessToken = user.access_token
         tickeroutexname = broker.tickeroutexname
 
-        # userid, applicationKey = validateApplicationToken(authServer=authServer,
-        #                                                 accessTaken=accessToken,
-        #                                                 verify_ssl=verify_ssl)
-
-        userid = user.userId
-        applicationKey = user.appKey
+        userid = user.user_id
+        applicationKey = user.app_key
 
         if userid is None or applicationKey is None:
             raise FlexError("User or application key is None")
 
         credentials = pika.PlainCredentials(userid, accessToken)
         parameters = pika.ConnectionParameters(
             brokerip, brokerport, "/", credentials, ssl_options=ssl_options
@@ -174,61 +218,57 @@
                 self.channel, applicationKey, tickeroutexname
             )
         except Exception as excep:
             err = FlexError(str(excep))
             raise err
         return err
 
-    @staticmethod
-    def create_line_message(
-        user: User, flexibility: Flexibility, marketOrder: MarketOrder
-    ):
-        """Create a line protocol message for InfluxDB that is the payload in the AMQP message
 
-        Format ask:
-        ask,applicationKey=64218f1adc42c714c1f08043,version=1 starttime=1685730000000i,wattage=19.556418841474642,runtime=60000i,totalenergy=0.32594031402457735,askingprice=7.933964367826437,expirationtime=1685730000000i
+    def set_consumer(self, callback, callback_queue, channel):
+        channel.basic_consume(
+            queue=callback_queue, on_message_callback=callback, auto_ack=True
+        )
 
-        Bid:
-        bid,applicationKey=64218f1adc42c714c1f08043,version=1 starttime=1685732700000i,wattage=226.3288909510559,runtime=840000i,totalenergy=52.81007455524638,biddingprice=6.56704792164692,expirationtime=1685732700000i
+    def checkreplies(self):
+        if self.connection is None:
+            raise FlexError("No connection to broker established")
+        self.connection.process_data_events()
 
-        """
-        lineordermsg = ""
-        if marketOrder.type == OrderType.ASK:
-            pricename = "askingprice"
-        elif marketOrder.type == OrderType.BID:
-            pricename = "biddingprice"
-        else:
-            raise FlexError(f"Order type {marketOrder.type} not supported")
+    def callback_on_response(self, ch, method, props, body):
+        global tickprice
+        currTimeMs = int(time.time() * 1000)
+        # Tick message ex. {'msgtype': 'tick', 'last_price_time': 1559732378418422410, 'last_price': 7.529581909307273}
+        try:
+            msgBody = json.loads(body.decode("utf-8"))
+            self.callback_responses.append(msgBody)
+
+            log(INFO, f"Received message")
+            log(INFO, f"{pformat(msgBody)}")
+            # if 'msgtype' in msgBody.keys():
+            #     if msgBody['msgtype'] == 'cancel':
+            #             log(INFO,"--- Bohoo! My message got cancelled for ", msgBody['reason'])
+            #     if msgBody['msgtype'] == 'tick':
+            #         tickprice = msgBody['last_price']
+            #         log(INFO,"--- Tick ",tickprice)
+            #         if 'sendertimestamp_in_ms' in props.headers.keys():
+            #             log(INFO,f"----- Tick was received in {currTimeMs - props.headers['sendertimestamp_in_ms']} ms")
+            #     if msgBody['msgtype'] == 'bid_closed_order':
+            #         if "closed_order" in msgBody.keys():
+            #             log(INFO,"--- Wohoo! My bid order deal went through for ", msgBody['closed_order']['price'])
+            #     if msgBody['msgtype'] == 'ask_closed_order':
+            #         if "closed_order" in msgBody.keys():
+            #             log(INFO,"--- Wohoo! My ask order deal went through for ", msgBody['closed_order']['price'])
+
+            # sys.exit(0)
 
-        order_type = marketOrder.type
-        applicationKey = user.appKey
-        wattage = flexibility.wattage
-        duration = flexibility.duration
-        starttime = flexibility.starttime
-        totalenergy = flexibility.energy
-        orderprice = marketOrder.price
-        expirationtime = flexibility.expirationtime
-
-        lineordermsg = (
-            f"{order_type.value},"
-            f"applicationKey={applicationKey},"
-            f"version=1 starttime={starttime}i,"
-            f"wattage={wattage},"
-            f"runtime={duration}i,"
-            f"totalenergy={totalenergy},"
-            f"{pricename}={orderprice},"
-            f"expirationtime={expirationtime}i"
-        )
-
-        return json.dumps(lineordermsg).strip('"')
-        # linemsg = createLineMessage(user=user ,marketOrder=marketOrder, flexibility=flexibility)
-        # return json.dumps(linemsg).strip('"')
+        except ValueError:
+            log(ERROR, "RECEIVED A NON JSON MESSAGE:", body)
 
 
-def getcurrenttimems():
+def get_current_time_ms():
     return int(time.time() * 1000)
 
 
 def declareReplyToQueue(
     channel: pika.adapters.blocking_connection.BlockingChannel,
     applicationKey: str,
     tickeroutexname: str,
@@ -239,17 +279,7 @@
         dec_res = channel.queue_declare(applicationKey, exclusive=True)
         callback_queue_id: str = dec_res.method.queue
         channel.queue_bind(callback_queue_id, tickeroutexname)
         log(INFO, f"Created queue with ID {callback_queue_id}")
         return callback_queue_id
     except pika.exceptions.ChannelClosedByBroker:
         log(ERROR, "ReplyTo queue creation failed " + applicationKey)
-
-
-def setreceiver(callback, callback_queue, channel):
-    channel.basic_consume(
-        queue=callback_queue, on_message_callback=callback, auto_ack=True
-    )
-
-
-def checkreplies(connection):
-    connection.process_data_events()
```

### Comparing `flxtrd-0.1.1/src/flxtrd/protocols/restapi.py` & `flxtrd-0.1.2/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.1.1/PKG-INFO` & `flxtrd-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.1.1
+Version: 0.1.2
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/GLocalFlexTrade
 Author: glocalflex
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -36,107 +36,157 @@
 
 
 Install GLocalFlexTrade Python package
 
 ```sh
 pip install flxtrd
 ```
-### Basic Example
+
+### Basic trading client example
 
 ```py
 """Example usage of the trading client using AMPQ protocol"""
-import sys
-import time
 from logging import ERROR, INFO
-from pprint import pformat
-from random import random
 
 from flxtrd import (
-    Broker,
+    ASK,
+    BID,
+    FlexBroker,
     FlexAPIClient,
-    Flexibility,
-    Market,
+    FlexResource,
+    FlexMarket,
     MarketOrder,
-    OrderType,
-    User,
+    FlexUser,
     log,
+    utils,
 )
 
 
 def main() -> None:
-    GFLEX_API_URL = "localhost"
+    GLOCALFLEX_MARKET_URL = "localhost"
 
-    user = User(
-        name="<your_email>",
-        password="<your_password>",
-        accessToken="<your_device_access_token>",
-    )
-
-    market = Market(ip=GFLEX_API_URL, broker=Broker(ip=GFLEX_API_URL))
-
-    # Define the tradable flexibility to sell or buy
-    flexResource = Flexibility(
-        wattage=random() * 100,
-        starttime=int((time.time() + (60 * 60 * random() * 10)) / 60) * 60 * 1000,
-        duration=int(((round(random()) * 14 + 1) / 60.0) * 60 * 60 * 1000),
-        expirationtime=int(time.time() / (60 * 1000) + random() * 20) * 60 * 1000,
-    )
+    user = FlexUser(name="<your_email>",
+                    password="<your_password>",
+                    access_token="<your_device_access_token>",
+                    )
 
-    # Create a market order to sell or buy flexibility
-    market_order = MarketOrder(type=OrderType.ASK, price=100, flexibility=flexResource)
+    market = FlexMarket(market_url=GLOCALFLEX_MARKET_URL)
 
     # Create a AMPQ client that connects to the message broker
-    trading_client = FlexAPIClient(base_url=GFLEX_API_URL, user=user, market=market)
+    trading_client = FlexAPIClient(base_url=GLOCALFLEX_MARKET_URL,
+                                   user=user,
+                                   market=market
+                                   )
+
+    # Define a flexibility resource that will be traded
+    # The resource is a 100W power for 60 minutes starting in 5 minutes
+    flex_resource = FlexResource(power_w=100,
+                                 start_time_epoch_s=utils.utc_timestamp_s() + utils.min_to_s(5), 
+                                 duration_min=60,  
+                                 order_expiration_min=50)
+
+    # Create a market ask order to sell flexibility
+    market_order = MarketOrder(order_type=ASK,
+                               price_eur=100,
+                               resource=flex_resource)
+
+    # Send the market order to the message broker
+    # The connection to the broker will be initiated automatically
+    _, err = trading_client.send_order(market_order=market_order,
+                                       verify_ssl=False)
+    
+    if err: log(ERROR, err)
+
+    # Create a market bid order to buy flexibility
+    market_order = MarketOrder(order_type=BID,
+                               price_eur=100,
+                               resource=flex_resource)
+
+    _, err = trading_client.send_order(market_order=market_order,
+                                       verify_ssl=False)
+    
+    if err: log(ERROR, err); sys.exit(1)
+
+    # Check the market responses for closed_deals, price tick messages
+    # from the message broker for 60 seconds and exit
+    wait_sec = 0
+    expected_responses = 3
+    log(INFO, f"Waiting for messages from market broker")
+
+    try:
+        while wait_sec < 60:
+            market_responses = trading_client.check_market_responses()
+            if market_responses is not None:
+                log(INFO, f"Received {len(market_responses)} responses from market broker")
+                # Close the connection to the market message broker
+                if len(market_responses) == expected_responses:
+                    break
+                
+            time.sleep(1)
+            wait_sec += 1
+
+    except KeyboardInterrupt:
+        log(INFO, "Keyboard interrupt received. Closing connection to the market broker")
+    finally:
+        trading_client.trade_protocol.close_connection()
 
-    # Send a request to the GLocalFlex with REST API
-    response, err = trading_client.make_request(
-        method="POST",
-        endpoint="/users/login",
-        data={"email": user.name, "password": user.password},
-    )
 
-    if err:
-        log(ERROR, err)
-        sys.exit(1)
+if __name__ == "__main__":
+    main()
 
-    log(INFO, pformat(response.request_response.json()))
-    log(INFO, response.request_response.status_code)
+```
 
-    # Send the market order to the message broker with AMPQ protocol
-    # The connection to the market message broker will be initiated automatically
-    response, err = trading_client.send_order(
-        method="",
-        verify_ssl=False,
-        order=market_order,
-    )
 
-    if err:
-        log(ERROR, err)
-        sys.exit(1)
+### Basic REST API client example
+
+```py
+"""Example usage of the REST API client"""
+from logging import ERROR, INFO
+from pprint import pformat
 
-    log(INFO, "Received response from message broker")
-    log(INFO, response.order_response)
+from flxtrd import (
+    ASK,
+    BID,
+    FlexBroker,
+    FlexAPIClient,
+    FlexResource,
+    FlexMarket,
+    MarketOrder,
+    FlexUser,
+    log,
+    utils,
+)
+
+
+def main() -> None:
+    GLOCALFLEX_MARKET_URL = "localhost"
 
-    # Send the market order to the message broker with AMPQ protocol
-    # The connection to the market message broker will be initiated automatically
-    response, err = trading_client.send_order(
-        method="",
-        verify_ssl=False,
-        order=market_order,
-    )
+    user = FlexUser(name="<your_email>",
+                    password="<your_password>",
+                    access_token="<your_device_access_token>"
+                    )
 
+    
+    market = FlexMarket(market_url=GLOCALFLEX_MARKET_URL)
+
+    # Create a AMPQ client that connects to the message broker
+    trading_client = FlexAPIClient(base_url=GLOCALFLEX_MARKET_URL,
+                                   user=user,
+                                   market=market
+                                   )
+
+    # Send a request to the GLocalFlex with REST API
+    response, err = trading_client.make_request(method="POST",
+                                                endpoint="/users/login",
+                                                data={"email": user.name, "password": user.password},
+                                                )
     if err:
         log(ERROR, err)
-        sys.exit(1)
 
-    log(INFO, "Received response from message broker")
-    log(INFO, response.order_response)
-
-    # Close the connection to the market message broker
-    trading_client.trade_protocol.close_connection()
+    log(INFO, pformat(response.request_response.json()))
+    log(INFO, response.request_response.status_code)
 
 
 if __name__ == "__main__":
     main()
 
 ```
-
```

