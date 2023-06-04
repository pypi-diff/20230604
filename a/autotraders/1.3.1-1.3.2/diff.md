# Comparing `tmp/autotraders-1.3.1.tar.gz` & `tmp/autotraders-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.3.1.tar", last modified: Sun Jun  4 07:05:10 2023, max compression
+gzip compressed data, was "autotraders-1.3.2.tar", last modified: Sun Jun  4 07:14:23 2023, max compression
```

## Comparing `autotraders-1.3.1.tar` & `autotraders-1.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.179640 autotraders-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-04 07:04:57.000000 autotraders-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 07:05:10.179640 autotraders-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-04 07:04:57.000000 autotraders-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.175640 autotraders-1.3.1/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.175640 autotraders-1.3.1/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.175640 autotraders-1.3.1/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.175640 autotraders-1.3.1/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.179640 autotraders-1.3.1/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.179640 autotraders-1.3.1/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 07:04:57.000000 autotraders-1.3.1/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.175640 autotraders-1.3.1/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 07:05:10.000000 autotraders-1.3.1/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 07:05:10.000000 autotraders-1.3.1/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:05:10.000000 autotraders-1.3.1/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 07:05:10.000000 autotraders-1.3.1/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 07:05:10.000000 autotraders-1.3.1/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 07:04:57.000000 autotraders-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 07:05:10.179640 autotraders-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:05:10.179640 autotraders-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 07:04:57.000000 autotraders-1.3.1/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 07:04:57.000000 autotraders-1.3.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-04 07:04:57.000000 autotraders-1.3.1/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-04 07:04:57.000000 autotraders-1.3.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.900708 autotraders-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-04 07:14:09.000000 autotraders-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 07:14:23.896708 autotraders-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-04 07:14:09.000000 autotraders-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 07:14:09.000000 autotraders-1.3.2/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 07:14:23.000000 autotraders-1.3.2/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 07:14:23.000000 autotraders-1.3.2/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:14:23.000000 autotraders-1.3.2/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 07:14:23.000000 autotraders-1.3.2/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 07:14:23.000000 autotraders-1.3.2/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 07:14:09.000000 autotraders-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 07:14:23.900708 autotraders-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:14:23.896708 autotraders-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 07:14:09.000000 autotraders-1.3.2/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 07:14:09.000000 autotraders-1.3.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-04 07:14:09.000000 autotraders-1.3.2/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-04 07:14:09.000000 autotraders-1.3.2/tests/test_util.py
```

### Comparing `autotraders-1.3.1/LICENSE` & `autotraders-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/PKG-INFO` & `autotraders-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.3.1
+Version: 1.3.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.3.1/README.md` & `autotraders-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/agent.py` & `autotraders-1.3.2/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/faction/__init__.py` & `autotraders-1.3.2/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/faction/contract.py` & `autotraders-1.3.2/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/map/system.py` & `autotraders-1.3.2/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/map/waypoint.py` & `autotraders-1.3.2/autotraders/map/waypoint.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.3.2/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.3.2/autotraders/map/waypoint_types/jumpgate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Optional
 
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
 
 
 class JumpGate(WaypointType):
-    def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
+    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
         self.faction_symbol: Optional[str] = ""
         self.jump_range: Optional[int] = None
-        super().__init__(waypoint, "jump-gate", session, update)
+        super().__init__(waypoint, "jump-gate", session, data)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.get()["data"]
         self.jump_range = data["jumpRange"]
         if "factionSymbol" in data:
             self.faction_symbol = data["factionSymbol"]
```

### Comparing `autotraders-1.3.1/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.3.2/autotraders/map/waypoint_types/marketplace.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,20 @@
         self.trade_volume: int = data["tradeVolume"]
         self.supply: str = data["supply"]
         self.purchase_price: int = data["purchasePrice"]
         self.sell_price: int = data["sellPrice"]
 
 
 class Marketplace(WaypointType):
-    def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
+    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
         self.imports: Optional[list[str]] = None
         self.exports: Optional[list[str]] = None
         self.exchange: Optional[list[str]] = None
         self.trade_goods: Optional[list[TradeGood]] = None
-        super().__init__(waypoint, "market", session, update)
+        super().__init__(waypoint, "market", session, data)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
                 + self.location.system
```

### Comparing `autotraders-1.3.1/autotraders/map/waypoint_types/shipyard.py` & `autotraders-1.3.2/autotraders/map/waypoint_types/shipyard.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         self.reactor = Reactor(data["reactor"])
         self.engine = Engine(data["engine"])
         self.modules = [Module(d) for d in data["modules"]]
         self.mounts = [Mount(d) for d in data["mounts"]]
 
 
 class Shipyard(WaypointType):
-    def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
+    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
         self.ship_types: Optional[list[str]] = None
         self.ships: Optional[list[ShipyardShip]] = None
-        super().__init__(waypoint, "shipyard", session, update)
+        super().__init__(waypoint, "shipyard", session, data)
 
     def update(self, data: dict = None):
         if data is None:
             data = self.get()["data"]
         self.ship_types = []
         for ship_type in data["shipTypes"]:
             self.ship_types.append(ship_type["type"])
```

### Comparing `autotraders-1.3.1/autotraders/session.py` & `autotraders-1.3.2/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/shared_models/map_symbol.py` & `autotraders-1.3.2/autotraders/shared_models/map_symbol.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/shared_models/transaction.py` & `autotraders-1.3.2/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/ship/__init__.py` & `autotraders-1.3.2/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/ship/ship_components.py` & `autotraders-1.3.2/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/space_traders_entity.py` & `autotraders-1.3.2/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/status.py` & `autotraders-1.3.2/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders/util.py` & `autotraders-1.3.2/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/autotraders.egg-info/PKG-INFO` & `autotraders-1.3.2/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.3.1
+Version: 1.3.2
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.3.1/autotraders.egg-info/SOURCES.txt` & `autotraders-1.3.2/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/pyproject.toml` & `autotraders-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.3.1/tests/test_init.py` & `autotraders-1.3.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/tests/test_ship.py` & `autotraders-1.3.2/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.1/tests/test_util.py` & `autotraders-1.3.2/tests/test_util.py`

 * *Files identical despite different names*

