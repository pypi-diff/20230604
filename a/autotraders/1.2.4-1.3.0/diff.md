# Comparing `tmp/autotraders-1.2.4.tar.gz` & `tmp/autotraders-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.2.4.tar", last modified: Fri May 26 21:53:51 2023, max compression
+gzip compressed data, was "autotraders-1.3.0.tar", last modified: Sun Jun  4 06:58:32 2023, max compression
```

## Comparing `autotraders-1.2.4.tar` & `autotraders-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 21:53:37.000000 autotraders-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:53:51.442672 autotraders-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 21:53:37.000000 autotraders-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-26 21:53:37.000000 autotraders-1.2.4/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 21:53:51.000000 autotraders-1.2.4/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 21:53:37.000000 autotraders-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:53:51.442672 autotraders-1.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:53:51.442672 autotraders-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 21:53:37.000000 autotraders-1.2.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.128195 autotraders-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-04 06:58:18.000000 autotraders-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 06:58:32.128195 autotraders-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-04 06:58:18.000000 autotraders-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.124195 autotraders-1.3.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.124195 autotraders-1.3.0/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.124195 autotraders-1.3.0/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.128195 autotraders-1.3.0/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.128195 autotraders-1.3.0/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.128195 autotraders-1.3.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 06:58:18.000000 autotraders-1.3.0/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.124195 autotraders-1.3.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 06:58:32.000000 autotraders-1.3.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 06:58:32.000000 autotraders-1.3.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:58:32.000000 autotraders-1.3.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 06:58:32.000000 autotraders-1.3.0/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 06:58:32.000000 autotraders-1.3.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 06:58:18.000000 autotraders-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 06:58:32.128195 autotraders-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:58:32.128195 autotraders-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 06:58:18.000000 autotraders-1.3.0/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 06:58:18.000000 autotraders-1.3.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-04 06:58:18.000000 autotraders-1.3.0/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-04 06:58:18.000000 autotraders-1.3.0/tests/test_util.py
```

### Comparing `autotraders-1.2.4/LICENSE` & `autotraders-1.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 ASHWIN NAREN
+Copyright 2023 pytraders
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `autotraders-1.2.4/PKG-INFO` & `autotraders-1.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.4
+Version: 1.3.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autotraders
+[![Downloads](https://static.pepy.tech/badge/autotraders)](https://pepy.tech/project/autotraders)
+[![Python package](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml/badge.svg)](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml)
+
 A spacetraders API focused on automation and ease of use
 ## Usage
 First you need a client, which can be generated 
 ```python
 from autotraders import session
 s = session.get_session("YOUR_TOKEN_HERE")
 ```
@@ -34,15 +37,15 @@
 ship.dock()
 ship.refuel()
 ship.orbit()  # All these functions make API calls (one each), but the line below doesn't
 print(ship.fuel.current + "/" + ship.fuel.total)
 ```
 ## Contract
 ```python
-from autotraders.contract import Contract, get_all_contracts
+from autotraders.faction.contract import Contract, get_all_contracts
 # create a session here
 contract = Contract("id-here", session)
 contracts = get_all_contracts(session)
 contract.accept()
 print(contract.accepted) # True
 contract.deliver("SHIP_SYMBOL", "ALUMINUM_ORE", 30)
 contract.fulfill()
```

### Comparing `autotraders-1.2.4/autotraders/agent.py` & `autotraders-1.3.0/autotraders/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import Optional
 
+from autotraders.faction.contract import Contract
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
-from autotraders.faction.contract import get_all_contracts, Contract
 from autotraders.session import AutoTradersSession
-from autotraders.ship import get_all_ships, Ship
+from autotraders.ship import Ship
 
 
 class Agent(SpaceTradersEntity):
-    def __init__(self, session: AutoTradersSession, update=True):
+    def __init__(self, session: AutoTradersSession, data=None):
         self.contracts: Optional[list[Contract]] = None
         self.starting_faction: Optional[str] = None
         self.symbol: Optional[str] = None
         self.account_id: Optional[str] = None
         self.credits: Optional[int] = None
         self.ships: Optional[Ship] = None
         self.headquarters: Optional[MapSymbol] = None
-        super().__init__(session, update, "my/agent")
+        super().__init__(session, "my/agent", data)
 
     def update(self, data=None):
         """Uses 3 API requests to get all agent details"""
         if data is None:
             data = self.get()["data"]
         self.account_id = data["accountId"]
         self.symbol = data["symbol"]
         self.headquarters = MapSymbol(data["headquarters"])
         self.credits = data["credits"]
         self.starting_faction = data["startingFaction"]
-        self.ships = get_all_ships(self.session)
-        self.contracts = get_all_contracts(self.session)
+        self.ships = Ship.all(self.session)
+        self.contracts = Contract.all(self.session)
```

### Comparing `autotraders-1.2.4/autotraders/faction/__init__.py` & `autotraders-1.3.0/autotraders/faction/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.shared_models.trait import Trait
 
 
 class Faction(SpaceTradersEntity):
-    def __init__(self, symbol, session: AutoTradersSession, update=True):
+    def __init__(self, symbol, session: AutoTradersSession, data=None):
         self.is_recruiting: Optional[bool] = None
         self.traits: Optional[list[Trait]] = None
         self.headquarters: Optional[MapSymbol] = None
         self.description: Optional[str] = None
         self.name: Optional[str] = None
         self.symbol: str = symbol
-        super().__init__(session, update, "factions/" + self.symbol)
+        super().__init__(session, "factions/" + self.symbol, data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.name = data["name"]
         self.description = data["description"]
         self.headquarters = MapSymbol(data["headquarters"])
@@ -31,15 +31,14 @@
     def all(session):
         r = session.get(session.base_url + "factions")
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         factions = []
         for f in j["data"]:
-            faction = Faction(f["symbol"], session, False)
-            faction.update(f)
+            faction = Faction(f["symbol"], session, f)
             factions.append(faction)
         return factions
 
 
 def get_all_factions(session):
     return Faction.all(session)
```

### Comparing `autotraders-1.2.4/autotraders/faction/contract.py` & `autotraders-1.3.0/autotraders/faction/contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
         self.trade_symbol = MapSymbol(data["tradeSymbol"])
         self.destination_symbol = MapSymbol(data["destinationSymbol"])
         self.units_required = data["unitsRequired"]
         self.units_fulfilled = data["unitsFulfilled"]
 
 
 class Contract(SpaceTradersEntity):
-    def __init__(self, contract_id: str, session: AutoTradersSession, update=True):
+    def __init__(self, contract_id: str, session: AutoTradersSession, data=None):
         self.contract_data = None
         self.accepted: Optional[bool] = None
         self.fulfilled: Optional[bool] = None
         self.deadline: Optional[datetime] = None
         self.accept_deadline: Optional[datetime] = None
         self.contract_type = None
         self.on_fulfilled: Optional[str] = None
         self.on_accepted: Optional[str] = None
         self.contract_id: str = contract_id
-        super().__init__(session, update, "my/contracts/" + self.contract_id)
+        super().__init__(session, "my/contracts/" + self.contract_id, data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
         self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
         self.accepted = data["accepted"]
@@ -55,30 +55,23 @@
     @staticmethod
     def negotiate(ship_symbol, session):
         j = session.post(
             session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
         ).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
-        print(j)
-        c = Contract(j["data"]["contract"]["id"], session, False)
-        c.update(j["data"]["contract"])
+        c = Contract(j["data"]["contract"]["id"], session, j["data"]["contract"])
         return c
 
     def fulfill(self):
         j = self.post("fulfill")
         self.update(j["data"]["contract"])
 
     @staticmethod
     def all(session, page: int = 1):
-        r = session.get(session.base_url + "my/contracts?page=" + str(page))
+        r = session.get(session.base_url + "my/contracts?limit=20&page=" + str(page))
         j = r.json()
         contracts = []
         for contract in j["data"]:
-            c = Contract(contract["id"], session, False)
-            c.update(contract)
+            c = Contract(contract["id"], session, contract)
             contracts.append(c)
         return contracts, r.json()["meta"]["total"]
-
-
-def get_all_contracts(session):
-    return Contract.all(session)[0]
```

### Comparing `autotraders-1.2.4/autotraders/map/system.py` & `autotraders-1.3.0/autotraders/map/system.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,44 @@
-from typing import Optional
+from typing import Optional, Union
 
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.map.waypoint import Waypoint
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class System(SpaceTradersEntity):
-    def __init__(self, symbol, session: AutoTradersSession, update=True):
+    def __init__(
+        self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
+    ):
         self.symbol: MapSymbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
         self.waypoints: Optional[list[Waypoint]] = None
         self.factions: Optional[list[str]] = None
         self.star_type: Optional[str] = None
-        super().__init__(session, update, "systems/" + str(self.symbol) + "/")
+        super().__init__(session, "systems/" + str(self.symbol) + "/", data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.waypoints = []
         self.x = data["x"]
         self.y = data["y"]
         self.factions = data["factions"]
         self.star_type = data["type"]
         for w in data["waypoints"]:
-            waypoint = Waypoint(w["symbol"], self.session, False)
-            waypoint.update(w)
+            waypoint = Waypoint(w["symbol"], self.session, w)
             self.waypoints.append(waypoint)
 
     @staticmethod
     def all(session, page=1) -> (list, int):
         r = session.get(session.base_url + "systems?limit=20&page=" + str(page))
         j = r.json()["data"]
         systems = []
         for system in j:
-            s = System(system["symbol"], session, False)
-            s.update(system)
+            s = System(system["symbol"], session, system)
             systems.append(s)
         return systems, r.json()["meta"]["total"]
 
     def __eq__(self, other):
         return self.symbol == other.symbol
-
-
-def list_systems(session, page=1) -> (list[System], int):
-    return System.all(session, page)
```

### Comparing `autotraders-1.2.4/autotraders/map/waypoint.py` & `autotraders-1.3.0/autotraders/map/waypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import Optional
+from typing import Optional, Union
 
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.trait import Trait
 
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.space_traders_entity import SpaceTradersEntity
 
 
 class Waypoint(SpaceTradersEntity):
-    def __init__(self, symbol, session: AutoTradersSession, update=True):
+    def __init__(
+        self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
+    ):
         self.waypoint_type: Optional[str] = None
         self.faction: Optional[str] = None
         self.traits: Optional[list[Trait]] = []
         self.marketplace: Optional[bool] = None
         self.shipyard: Optional[bool] = None
         self.symbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
         super().__init__(
             session,
-            update,
             "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
+            data,
         )
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
         self.waypoint_type = data["type"]
         self.x = data["x"]
@@ -41,23 +43,24 @@
             len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
         self.shipyard = (
             len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
         )
 
     @staticmethod
-    def all(system, session) -> (list, int):
-        r = session.get(session.base_url + "systems/" + system + "/waypoints?limit=20")
+    def all(system, session, page=1) -> (list, int):
+        r = session.get(
+            session.base_url
+            + "systems/"
+            + system
+            + "/waypoints?limit=20&page="
+            + str(page)
+        )
         data = r.json()["data"]
         waypoints = []
         for w in data:
-            waypoint = Waypoint(w["symbol"], session, False)
-            waypoint.update(w)
+            waypoint = Waypoint(w["symbol"], session, w)
             waypoints.append(waypoint)
         return waypoints, r.json()["meta"]["total"]
 
     def __eq__(self, other):
         return self.symbol == other.symbol
-
-
-def get_all_waypoints(system, session):
-    return Waypoint.all(system, session)
```

### Comparing `autotraders-1.2.4/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.3.0/autotraders/map/waypoint_types/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class WaypointType(SpaceTradersEntity):
     def __init__(
-        self, waypoint: str, trait: str, session: AutoTradersSession, update=True
+        self, waypoint: str, trait: str, session: AutoTradersSession, data=None
     ):
         self.location: MapSymbol = MapSymbol(waypoint)
         super().__init__(
             session,
-            update,
             "systems/"
             + self.location.system
             + "/waypoints/"
             + self.location.waypoint
             + "/"
             + trait
             + "/",
+            data,
         )
```

### Comparing `autotraders-1.2.4/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.3.0/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.4/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.3.0/autotraders/map/waypoint_types/marketplace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Optional
 
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
+from autotraders.shared_models.item import Item
 
 
-class TradeGood:
+class TradeGood(Item):
     def __init__(self, data):
-        self.symbol: str = data["symbol"]
+        super().__init__(data["symbol"], data["supply"], data["description"])
         self.trade_volume: int = data["tradeVolume"]
         self.supply: str = data["supply"]
         self.purchase_price: int = data["purchasePrice"]
         self.sell_price: int = data["sellPrice"]
 
 
 class Marketplace(WaypointType):
```

### Comparing `autotraders-1.2.4/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.3.0/autotraders/map/waypoint_types/shipyard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
+from autotraders.shared_models.transaction import ShipyardTransaction
 from autotraders.ship import Frame, Reactor, Engine, Module, Mount
 
 
 class ShipyardShip:
     def __init__(self, data):
         self.ship_type = data["type"]
         self.name = data["name"]
@@ -22,29 +23,23 @@
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
         self.ship_types: Optional[list[str]] = None
         self.ships: Optional[list[ShipyardShip]] = None
         super().__init__(waypoint, "shipyard", session, update)
 
     def update(self, data: dict = None):
         if data is None:
-            data = self.session.get(
-                self.session.base_url
-                + "systems/"
-                + self.location.system
-                + "/waypoints/"
-                + self.location.waypoint
-                + "/shipyard"
-            ).json()["data"]
+            data = self.get()["data"]
         self.ship_types = []
         for ship_type in data["shipTypes"]:
             self.ship_types.append(ship_type["type"])
         self.ships = None
         if "ships" in data:
             self.ships = []
             for ship in data["ships"]:
                 self.ships.append(ShipyardShip(ship))
 
     def purchase(self, ship_type: str):
-        self.session.post(
+        j = self.session.post(
             self.session.base_url + "my/ships",
             data={"shipType": ship_type, "waypointSymbol": self.location},
-        )
+        ).json()
+        return ShipyardTransaction(j["data"]["transaction"])
```

### Comparing `autotraders-1.2.4/autotraders/session.py` & `autotraders-1.3.0/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.4/autotraders/shared_models/map_symbol.py` & `autotraders-1.3.0/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.4/autotraders/ship/__init__.py` & `autotraders-1.3.0/autotraders/ship/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
 from datetime import datetime, timezone
 from typing import Union, Optional
 
+from autotraders.shared_models.item import Item
+from autotraders.shared_models.transaction import MarketTransaction
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
 from autotraders.ship.survey import Survey
 from autotraders.util import parse_time
@@ -21,18 +23,20 @@
         return str(self.current) + "/" + str(self.total)
 
 
 class Cargo:
     def __init__(self, j):
         self.capacity = j["capacity"]
         inventory = j["inventory"]
-        self.inventory = {}
+        self.inventory = []
         self.current = 0
         for symbol in inventory:
-            self.inventory[symbol["symbol"]] = symbol["units"]
+            self.inventory.append(
+                Item(symbol["symbol"], symbol["units"], symbol["description"])
+            )
             self.current += symbol["units"]
 
 
 class Route:
     def __init__(self, data):
         self.destination = MapSymbol(data["destination"]["symbol"])
         self.departure = MapSymbol(data["departure"]["symbol"])
@@ -56,74 +60,90 @@
         self.required = data["required"]
         self.capacity = data["capacity"]
         self.morale = data["morale"]
         self.wages = data["wages"]
 
 
 class Ship(SpaceTradersEntity):
-    def __init__(self, symbol, session: AutoTradersSession, update=True):
+    def __init__(self, symbol, session: AutoTradersSession, data=None):
         self.cargo: Optional[Cargo] = None
         self.fuel: Optional[Fuel] = None
         self.nav: Optional[Nav] = None
         self.symbol: str = symbol
         self.frame: Optional[Frame] = None
         self.reactor: Optional[Reactor] = None
         self.engine: Optional[Engine] = None
         self.modules: Optional[list[Module]] = None
         self.mounts: Optional[list[Mount]] = None
         self.crew: Optional[Crew] = None
-        super().__init__(session, update, "my/ships/" + self.symbol + "/")
+        super().__init__(session, "my/ships/" + self.symbol, data)
 
-    def update(self, data: dict = None, hard=False):
+    def update(self, data: dict = None, hard=False) -> None:  # TODO: Hard is deprecated
+        """
+        :param hard: deprecated does not do anything
+        """
         if data is None:
             data = self.get()["data"]
 
-        def go_for_update(d, s):
-            return s in data and (d is None or hard)
-
-        if go_for_update(self.crew, "crew"):
+        if "crew" in data:
             self.crew = Crew(data["crew"])
-        if go_for_update(self.frame, "frame"):
+        if "frame" in data:
             self.frame = Frame(data["frame"])
-        if go_for_update(self.reactor, "reactor"):
+        if "reactor" in data:
             self.reactor = Reactor(data["reactor"])
-        if go_for_update(self.engine, "engine"):
+        if "engine" in data:
             self.engine = Engine(data["engine"])
-        if go_for_update(self.modules, "modules"):
+        if "modules" in data:
             self.modules = [Module(d) for d in data["modules"]]
-        if go_for_update(self.mounts, "mounts"):
+        if "mounts" in data:
             self.mounts = [Mount(d) for d in data["mounts"]]
         if "nav" in data:
             self.nav = Nav(data["nav"])
         if "fuel" in data:
             self.fuel = Fuel(data["fuel"]["current"], data["fuel"]["capacity"])
         if "cargo" in data:
             self.cargo = Cargo(data["cargo"])
 
-    async def navigate_async(self, waypoint: Union[str, MapSymbol]):
+    async def navigate_async(self, waypoint: Union[str, MapSymbol], interval=1):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
-            :raise:
-                IOError: if a server error occurs
+        :param interval: Frequency of updates in seconds (default: 1)
         """
         j = self.post("navigate", data={"waypointSymbol": str(waypoint)})
         self.update(j["data"])
         while self.nav.status == "IN_TRANSIT":
-            await asyncio.sleep(5)
+            await asyncio.sleep(interval)
             self.update()
 
     def navigate(self, waypoint: Union[str, MapSymbol]):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function exits immediately, and does not wait the ship to arrive.
-            :raise:
-                IOError: if a server error occurs
         """
         j = self.post("navigate", data={"waypointSymbol": str(waypoint)})
         self.update(j["data"])
 
+    def jump(self, destination: Union[str, MapSymbol]):
+        j = self.post(
+            "jump",
+            data={
+                "systemSymbol": str(destination),
+            },
+        )
+        self.update(j["data"])
+        self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
+
+    def warp(self, destination: Union[str, MapSymbol]):
+        j = self.post(
+            "warp",
+            data={
+                "waypointSymbol": str(destination),
+            },
+        )
+        self.update(j["data"])
+
     def patch_navigation(self, new_flight_mode):
         r = self.session.patch(
             self.session.base_url + "my/ships/" + self.symbol + "/nav",
             data={"flightMode": new_flight_mode},
         )
         j = r.json()
         if "error" in j:
@@ -135,150 +155,129 @@
         self.update(j["data"])
 
     def orbit(self):
         j = self.post("orbit")
         self.update(j["data"])
 
     def extract(self):
-        j = self.session.post(
-            self.session.base_url + "my/ships/" + self.symbol + "/extract"
-        ).json()
-        if "error" in j:
-            if j["error"]["code"] == 4000:
-                raise IOError(
-                    "Ship is still in cooldown, "
-                    + str(j["error"]["data"]["cooldown"]["remainingSeconds"])
-                    + " seconds out of "
-                    + str(j["error"]["data"]["cooldown"]["totalSeconds"])
-                    + " seconds remaining"
-                )
-            else:
-                raise IOError(j["error"]["message"])
+        j = self.post("extract")
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
+        return Item(
+            j["data"]["extraction"]["yield"]["symbol"],
+            j["data"]["extraction"]["yield"]["units"],
+            "",
+        )
 
     def refuel(self):
         j = self.post("refuel")
         self.update(j["data"])
+        return MarketTransaction(j["data"]["transaction"])
 
     def sell(self, cargo_symbol: str, quantity: int):
         j = self.post("sell", data={"symbol": cargo_symbol, "units": quantity})
         self.update(j["data"])
+        return MarketTransaction(j["data"]["transaction"])
 
     def buy(self, cargo_symbol: str, quantity: int):
         j = self.post("purchase", data={"symbol": cargo_symbol, "units": quantity})
         self.update(j["data"])
+        return MarketTransaction(j["data"]["transaction"])
 
     def transfer(self, destination: str, cargo_symbol: str, quantity: int):
         j = self.post(
             "transfer",
             data={
                 "tradeSymbol": cargo_symbol,
                 "units": quantity,
                 "shipSymbol": destination,
             },
         )
         self.update(j["data"])
 
-    def jump(self, destination: Union[str, MapSymbol]):
-        j = self.post(
-            "jump",
-            data={
-                "systemSymbol": str(destination),
-            },
-        )
-        self.update(j["data"])
-        self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
-
-    def warp(self, destination: Union[str, MapSymbol]):
-        j = self.post(
-            "warp",
-            data={
-                "waypointSymbol": str(destination),
-            },
-        )
-        self.update(j["data"])
-
     def jettison(self, cargo_symbol: str, quantity: int):
         j = self.post(
             "jettison",
             data={"symbol": cargo_symbol, "units": quantity},
         )
         self.update(j["data"])
 
     def refine(self, output_symbol: str):
         j = self.post(
             "refine",
             data={"produce": output_symbol},
         )
-        print(j)
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
 
     def chart(self) -> Waypoint:
         """
         Charts the current waypoint
-        :return: The info about the waypoint that has been charted
+
+        :returns: The info about the waypoint that has been charted
         """
         j = self.post("chart")
-        w = Waypoint(j["data"]["waypoint"]["symbol"], self.session, False)
-        w.update(j["data"]["waypoint"])
+        w = Waypoint(
+            j["data"]["waypoint"]["symbol"], self.session, j["data"]["waypoint"]
+        )
         return w
 
     def survey(self) -> list[Survey]:
         j = self.post("survey")
         surveys = []
         for s in j["data"]["surveys"]:
             surveys.append(Survey(s))
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return surveys
 
-    def scan_systems(self):
+    def scan_systems(self) -> list[System]:
         j = self.post("scan/systems")
         systems = []
         for system in j["systems"]:
-            s = System(system["symbol"], self.session, False)
-            s.update(system)
+            s = System(system["symbol"], self.session, system)
             systems.append(s)
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return systems
 
-    def scan_waypoints(self):
+    def scan_waypoints(self) -> list[Waypoint]:
         j = self.post("scan/waypoints")
         waypoints = []
         for waypoint in j["waypoints"]:
-            s = Waypoint(waypoint["symbol"], self.session, False)
-            s.update(waypoint)
-            waypoints.append(s)
+            w = Waypoint(waypoint["symbol"], self.session, waypoint)
+            waypoints.append(w)
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return waypoints
 
-    def scan_ships(self):
+    def scan_ships(self) -> list:
         j = self.post("scan/ships")
         ships = []
         for ship in j["data"]["ships"]:
-            s = Ship(ship, self.session, False)
-            s.update(ship)
+            s = Ship(ship["symbol"], self.session, ship)
             ships.append(s)
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return ships
 
     def update_ship_cooldown(self):
         j = self.get("cooldown")
         self.reactor.cooldown = parse_time(j["data"]["expiration"])
 
+    def install_mount(self):
+        j = self.post("mounts/install")
+        self.update(j["data"])
+        return MarketTransaction(j["data"]["transaction"])
+
+    def remove_mount(self):
+        j = self.post("mounts/remove")
+        self.update(j["data"])
+        return MarketTransaction(j["data"]["transaction"])
+
     @staticmethod
     def all(session, page: int = 1) -> (str, int):
-        r = session.get(session.base_url + "my/ships?page=" + str(page))
+        r = session.get(session.base_url + "my/ships?limit=20&page=" + str(page))
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         ships = []
         for ship in j["data"]:
-            s = Ship(ship["symbol"], session, False)
-            s.update(ship)
+            s = Ship(ship["symbol"], session, ship)
             ships.append(s)
         return ships, r.json()["meta"]["total"]
-
-
-def get_all_ships(session):
-    return Ship.all(session)[0]
```

### Comparing `autotraders-1.2.4/autotraders/ship/ship_components.py` & `autotraders-1.3.0/autotraders/ship/ship_components.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
             self.slots = data["slots"]
 
 
 class ShipComponent:
     def __init__(self, data):
         self.symbol = data["symbol"]
         self.name = data["name"]
-        self.description = data["description"]
+        if "description" in data:
+            self.description = data["description"]
+        else:
+            self.description = None
         if "condition" in data:
             self.condition = data["condition"]
         else:
             self.condition = 100
         self.requirements = Requirements(data["requirements"])
```

### Comparing `autotraders-1.2.4/autotraders/status.py` & `autotraders-1.3.0/autotraders/status.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,27 @@
 
     def __init__(self, name: str, url: str):
         self.name = name
         self.url = url
 
 
 class Status:
+    """
+    :ivar status: User Readable description of the server status
+    :ivar version: The server version
+    :ivar reset_date: A datetime of the last reset date
+    :ivar description: A user-readable description of the server
+    :ivar stats: A dictionary of stats. The keys are agents, ships, systems, and waypoints
+    :ivar leaderboards:
+    :ivar next_reset: A datetime of the next reset
+    :ivar reset_frequency: A user-readable description of the server reset frequency
+    :ivar announcements: A list of announcements
+    :ivar links: A list of useful links
+    """
+
     status: str
     version: str
     reset_date: datetime
     description: str
     stats: dict[str, int]
     leaderboards: list[Leaderboard]
     next_reset: datetime
```

### Comparing `autotraders-1.2.4/autotraders.egg-info/PKG-INFO` & `autotraders-1.3.0/autotraders.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.2.4
+Version: 1.3.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autotraders
+[![Downloads](https://static.pepy.tech/badge/autotraders)](https://pepy.tech/project/autotraders)
+[![Python package](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml/badge.svg)](https://github.com/cosmictraders/autotraders/actions/workflows/python-package.yml)
+
 A spacetraders API focused on automation and ease of use
 ## Usage
 First you need a client, which can be generated 
 ```python
 from autotraders import session
 s = session.get_session("YOUR_TOKEN_HERE")
 ```
@@ -34,15 +37,15 @@
 ship.dock()
 ship.refuel()
 ship.orbit()  # All these functions make API calls (one each), but the line below doesn't
 print(ship.fuel.current + "/" + ship.fuel.total)
 ```
 ## Contract
 ```python
-from autotraders.contract import Contract, get_all_contracts
+from autotraders.faction.contract import Contract, get_all_contracts
 # create a session here
 contract = Contract("id-here", session)
 contracts = get_all_contracts(session)
 contract.accept()
 print(contract.accepted) # True
 contract.deliver("SHIP_SYMBOL", "ALUMINUM_ORE", 30)
 contract.fulfill()
```

### Comparing `autotraders-1.2.4/autotraders.egg-info/SOURCES.txt` & `autotraders-1.3.0/autotraders.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 pyproject.toml
 autotraders/__init__.py
 autotraders/agent.py
 autotraders/session.py
 autotraders/space_traders_entity.py
 autotraders/status.py
-autotraders/transaction.py
 autotraders/util.py
 autotraders.egg-info/PKG-INFO
 autotraders.egg-info/SOURCES.txt
 autotraders.egg-info/dependency_links.txt
 autotraders.egg-info/requires.txt
 autotraders.egg-info/top_level.txt
 autotraders/faction/__init__.py
@@ -18,16 +17,18 @@
 autotraders/map/__init__.py
 autotraders/map/system.py
 autotraders/map/waypoint.py
 autotraders/map/waypoint_types/__init__.py
 autotraders/map/waypoint_types/jumpgate.py
 autotraders/map/waypoint_types/marketplace.py
 autotraders/map/waypoint_types/shipyard.py
+autotraders/shared_models/item.py
 autotraders/shared_models/map_symbol.py
 autotraders/shared_models/trait.py
+autotraders/shared_models/transaction.py
 autotraders/ship/__init__.py
 autotraders/ship/ship_components.py
 autotraders/ship/survey.py
 tests/test_contract.py
 tests/test_init.py
 tests/test_ship.py
 tests/test_util.py
```

### Comparing `autotraders-1.2.4/pyproject.toml` & `autotraders-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.2.4"
+version = "1.3.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.2.4/tests/test_init.py` & `autotraders-1.3.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.2.4/tests/test_ship.py` & `autotraders-1.3.0/tests/test_ship.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,43 +30,39 @@
     s.transfer("TEST-2", "FUEL", 42)
     s.jettison("FUEL", 42)
 
 
 def test_ship_nav(session):
     start = datetime.now(timezone.utc) - timedelta(seconds=5)
     end = datetime.now(timezone.utc) + timedelta(seconds=5)
-    n = Nav({
-        "status": "IN_TRANSIT",
-        "waypointSymbol": "X1-TEST-TEST2",
-        "flightMode": "CRUISE",
-        "route": {
-            "destination": {
-                "symbol": "X1-TEST-TEST2"
+    n = Nav(
+        {
+            "status": "IN_TRANSIT",
+            "waypointSymbol": "X1-TEST-TEST2",
+            "flightMode": "CRUISE",
+            "route": {
+                "destination": {"symbol": "X1-TEST-TEST2"},
+                "departure": {"symbol": "X1-TEST-TEST"},
+                "departureTime": start.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                "arrival": end.strftime("%Y-%m-%dT%H:%M:%SZ"),
             },
-            "departure": {
-                "symbol": "X1-TEST-TEST"
-            },
-            "departureTime": start.strftime("%Y-%m-%dT%H:%M:%SZ"),
-            "arrival": end.strftime("%Y-%m-%dT%H:%M:%SZ")
         }
-    })
+    )
     assert n.status == "IN_TRANSIT"
     assert n.moving
     start2 = datetime.now(timezone.utc) - timedelta(seconds=10)
     end2 = datetime.now(timezone.utc) - timedelta(seconds=5)
-    n2 = Nav({
-        "status": "ORBIT",
-        "waypointSymbol": "X1-TEST-TEST2",
-        "flightMode": "CRUISE",
-        "route": {
-            "destination": {
-                "symbol": "X1-TEST-TEST2"
-            },
-            "departure": {
-                "symbol": "X1-TEST-TEST"
+    n2 = Nav(
+        {
+            "status": "ORBIT",
+            "waypointSymbol": "X1-TEST-TEST2",
+            "flightMode": "CRUISE",
+            "route": {
+                "destination": {"symbol": "X1-TEST-TEST2"},
+                "departure": {"symbol": "X1-TEST-TEST"},
+                "departureTime": start2.strftime("%Y-%m-%dT%H:%M:%SZ"),
+                "arrival": end2.strftime("%Y-%m-%dT%H:%M:%SZ"),
             },
-            "departureTime": start2.strftime("%Y-%m-%dT%H:%M:%SZ"),
-            "arrival": end2.strftime("%Y-%m-%dT%H:%M:%SZ")
         }
-    })
+    )
     assert n2.status == "ORBIT"
     assert not n2.moving
```

### Comparing `autotraders-1.2.4/tests/test_util.py` & `autotraders-1.3.0/tests/test_util.py`

 * *Files identical despite different names*

