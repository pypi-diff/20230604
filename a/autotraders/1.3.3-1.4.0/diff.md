# Comparing `tmp/autotraders-1.3.3.tar.gz` & `tmp/autotraders-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.3.3.tar", last modified: Sun Jun  4 07:18:36 2023, max compression
+gzip compressed data, was "autotraders-1.4.0.tar", last modified: Sun Jun  4 20:26:26 2023, max compression
```

## Comparing `autotraders-1.3.3.tar` & `autotraders-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.982493 autotraders-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-04 07:18:20.000000 autotraders-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 07:18:36.978493 autotraders-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-04 07:18:20.000000 autotraders-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.974493 autotraders-1.3.3/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.974493 autotraders-1.3.3/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.978493 autotraders-1.3.3/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.978493 autotraders-1.3.3/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.978493 autotraders-1.3.3/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/shared_models/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/shared_models/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/shared_models/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.978493 autotraders-1.3.3/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/space_traders_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 07:18:20.000000 autotraders-1.3.3/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.974493 autotraders-1.3.3/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 07:18:36.000000 autotraders-1.3.3/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-04 07:18:36.000000 autotraders-1.3.3/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 07:18:36.000000 autotraders-1.3.3/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 07:18:36.000000 autotraders-1.3.3/autotraders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 07:18:36.000000 autotraders-1.3.3/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-04 07:18:20.000000 autotraders-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 07:18:36.982493 autotraders-1.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 07:18:36.978493 autotraders-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 07:18:20.000000 autotraders-1.3.3/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 07:18:20.000000 autotraders-1.3.3/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-04 07:18:20.000000 autotraders-1.3.3/tests/test_ship.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-04 07:18:20.000000 autotraders-1.3.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-04 20:26:14.000000 autotraders-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 20:26:26.955747 autotraders-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-04 20:26:14.000000 autotraders-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.951747 autotraders-1.4.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/shared_models/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/shared_models/trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/shared_models/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/space_traders_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-04 20:26:14.000000 autotraders-1.4.0/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.951747 autotraders-1.4.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-04 20:26:26.000000 autotraders-1.4.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-04 20:26:26.000000 autotraders-1.4.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 20:26:26.000000 autotraders-1.4.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 20:26:26.000000 autotraders-1.4.0/autotraders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 20:26:26.000000 autotraders-1.4.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-04 20:26:14.000000 autotraders-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 20:26:26.955747 autotraders-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 20:26:26.955747 autotraders-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-04 20:26:14.000000 autotraders-1.4.0/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-04 20:26:14.000000 autotraders-1.4.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-04 20:26:14.000000 autotraders-1.4.0/tests/test_ship.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-04 20:26:14.000000 autotraders-1.4.0/tests/test_util.py
```

### Comparing `autotraders-1.3.3/LICENSE` & `autotraders-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/PKG-INFO` & `autotraders-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.3.3
+Version: 1.4.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.3.3/README.md` & `autotraders-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/agent.py` & `autotraders-1.4.0/autotraders/agent.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/faction/__init__.py` & `autotraders-1.4.0/autotraders/map/system.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,54 @@
-from typing import Optional
+from typing import Optional, Union
 
+from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
+from autotraders.map.waypoint import Waypoint
 from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.shared_models.trait import Trait
 
 
-class Faction(SpaceTradersEntity):
-    def __init__(self, symbol, session: AutoTradersSession, data=None):
-        self.is_recruiting: Optional[bool] = None
-        self.traits: Optional[list[Trait]] = None
-        self.headquarters: Optional[MapSymbol] = None
-        self.description: Optional[str] = None
-        self.name: Optional[str] = None
-        self.symbol: str = symbol
-        super().__init__(session, "factions/" + self.symbol, data)
+class System(SpaceTradersEntity):
+    def __init__(
+        self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
+    ):
+        self.symbol: MapSymbol = MapSymbol(symbol)
+        self.x: Optional[int] = None
+        self.y: Optional[int] = None
+        self.waypoints: Optional[list[Waypoint]] = None
+        self.factions: Optional[list[str]] = None
+        self.star_type: Optional[str] = None
+        super().__init__(session, "systems/" + str(self.symbol) + "/", data)
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
-        self.name = data["name"]
-        self.description = data["description"]
-        self.headquarters = MapSymbol(data["headquarters"])
-        self.traits = []
-        for trait in data["traits"]:
-            self.traits.append(Trait(trait))
-        self.is_recruiting = data["isRecruiting"]
+        self.waypoints = []
+        self.x = data["x"]
+        self.y = data["y"]
+        self.factions = data["factions"]
+        self.star_type = data["type"]
+        for w in data["waypoints"]:
+            waypoint = Waypoint(w["symbol"], self.session, w)
+            self.waypoints.append(waypoint)
 
     @staticmethod
-    def all(session):
-        r = session.get(session.base_url + "factions")
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        factions = []
-        for f in j["data"]:
-            faction = Faction(f["symbol"], session, f)
-            factions.append(faction)
-        return factions
+    def all(session, page: int = 1) -> PaginatedList:
+        def paginated_func(p, num_per_page):
+            r = session.get(
+                session.base_url
+                + "systems?limit="
+                + str(num_per_page)
+                + "&page="
+                + str(p)
+            )
+            j = r.json()["data"]
+            systems = []
+            for system in j:
+                s = System(system["symbol"], session, system)
+                systems.append(s)
+            return systems, r.json()["meta"]["total"]
 
+        return PaginatedList(paginated_func, page)
 
-def get_all_factions(session):
-    return Faction.all(session)
+    def __eq__(self, other):
+        return self.symbol == other.symbol
```

### Comparing `autotraders-1.3.3/autotraders/faction/contract.py` & `autotraders-1.4.0/autotraders/faction/contract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from typing import Optional
 
+from autotraders.paginated_list import PaginatedList
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.util import parse_time
 
 
 class Deliver:
@@ -64,14 +65,25 @@
 
     def fulfill(self):
         j = self.post("fulfill")
         self.update(j["data"]["contract"])
 
     @staticmethod
     def all(session, page: int = 1):
-        r = session.get(session.base_url + "my/contracts?limit=20&page=" + str(page))
-        j = r.json()
-        contracts = []
-        for contract in j["data"]:
-            c = Contract(contract["id"], session, contract)
-            contracts.append(c)
-        return contracts, r.json()["meta"]["total"]
+        def paginated_func(p, num_per_page):
+            r = session.get(
+                session.base_url
+                + "my/contracts?limit="
+                + str(num_per_page)
+                + "&page="
+                + str(p)
+            )
+            j = r.json()
+            if "error" in j:
+                raise IOError(j["error"]["message"])
+            contracts = []
+            for contract in j["data"]:
+                c = Contract(contract["id"], session, contract)
+                contracts.append(c)
+            return contracts, r.json()["meta"]["total"]
+
+        return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.3.3/autotraders/map/system.py` & `autotraders-1.4.0/autotraders/map/waypoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,69 @@
 from typing import Optional, Union
 
-from autotraders.space_traders_entity import SpaceTradersEntity
+from autotraders.paginated_list import PaginatedList
 from autotraders.session import AutoTradersSession
-from autotraders.map.waypoint import Waypoint
+from autotraders.shared_models.trait import Trait
+
 from autotraders.shared_models.map_symbol import MapSymbol
+from autotraders.space_traders_entity import SpaceTradersEntity
 
 
-class System(SpaceTradersEntity):
+class Waypoint(SpaceTradersEntity):
     def __init__(
         self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
     ):
-        self.symbol: MapSymbol = MapSymbol(symbol)
+        self.waypoint_type: Optional[str] = None
+        self.faction: Optional[str] = None
+        self.traits: Optional[list[Trait]] = []
+        self.marketplace: Optional[bool] = None
+        self.shipyard: Optional[bool] = None
+        self.symbol = MapSymbol(symbol)
         self.x: Optional[int] = None
         self.y: Optional[int] = None
-        self.waypoints: Optional[list[Waypoint]] = None
-        self.factions: Optional[list[str]] = None
-        self.star_type: Optional[str] = None
-        super().__init__(session, "systems/" + str(self.symbol) + "/", data)
+        super().__init__(
+            session,
+            "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
+            data,
+        )
 
     def update(self, data=None):
         if data is None:
             data = self.get()["data"]
-        self.waypoints = []
+        self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
-        self.factions = data["factions"]
-        self.star_type = data["type"]
-        for w in data["waypoints"]:
-            waypoint = Waypoint(w["symbol"], self.session, w)
-            self.waypoints.append(waypoint)
+        if "faction" in data:
+            self.faction = data["faction"]["symbol"]
+        else:
+            self.faction = None
+        self.traits = []
+        if "traits" in data:
+            for trait in data["traits"]:
+                self.traits.append(Trait(trait))
+        self.marketplace = (
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+        )
+        self.shipyard = (
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        )
 
     @staticmethod
-    def all(session, page=1) -> (list, int):
-        r = session.get(session.base_url + "systems?limit=20&page=" + str(page))
-        j = r.json()["data"]
-        systems = []
-        for system in j:
-            s = System(system["symbol"], session, system)
-            systems.append(s)
-        return systems, r.json()["meta"]["total"]
+    def all(session, page: int = 1) -> PaginatedList:
+        def paginated_func(p, num_per_page):
+            r = session.get(
+                session.base_url
+                + "systems/waypoints?limit="
+                + str(num_per_page)
+                + "&page="
+                + str(p)
+            )
+            data = r.json()["data"]
+            waypoints = []
+            for w in data:
+                waypoint = Waypoint(w["symbol"], session, w)
+                waypoints.append(waypoint)
+
+        return PaginatedList(paginated_func, page)
 
     def __eq__(self, other):
         return self.symbol == other.symbol
```

### Comparing `autotraders-1.3.3/autotraders/map/waypoint.py` & `autotraders-1.4.0/autotraders/map/waypoint_types/shipyard.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,45 @@
-from typing import Optional, Union
+from typing import Optional
 
+from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
-from autotraders.shared_models.trait import Trait
+from autotraders.shared_models.transaction import ShipyardTransaction
+from autotraders.ship import Frame, Reactor, Engine, Module, Mount, Ship
 
-from autotraders.shared_models.map_symbol import MapSymbol
-from autotraders.space_traders_entity import SpaceTradersEntity
 
+class ShipyardShip:
+    def __init__(self, data):
+        self.ship_type = data["type"]
+        self.name = data["name"]
+        self.description = data["description"]
+        self.purchase_price = data["purchasePrice"]
+        self.frame = Frame(data["frame"])
+        self.reactor = Reactor(data["reactor"])
+        self.engine = Engine(data["engine"])
+        self.modules = [Module(d) for d in data["modules"]]
+        self.mounts = [Mount(d) for d in data["mounts"]]
+
+
+class Shipyard(WaypointType):
+    def __init__(self, waypoint: str, session: AutoTradersSession, data=None):
+        self.ship_types: Optional[list[str]] = None
+        self.ships: Optional[list[ShipyardShip]] = None
+        super().__init__(waypoint, "shipyard", session, data)
 
-class Waypoint(SpaceTradersEntity):
-    def __init__(
-        self, symbol: Union[str, MapSymbol], session: AutoTradersSession, data=None
-    ):
-        self.waypoint_type: Optional[str] = None
-        self.faction: Optional[str] = None
-        self.traits: Optional[list[Trait]] = []
-        self.marketplace: Optional[bool] = None
-        self.shipyard: Optional[bool] = None
-        self.symbol = MapSymbol(symbol)
-        self.x: Optional[int] = None
-        self.y: Optional[int] = None
-        super().__init__(
-            session,
-            "systems/" + self.symbol.system + "/waypoints/" + self.symbol.waypoint,
-            data,
-        )
-
-    def update(self, data=None):
+    def update(self, data: dict = None):
         if data is None:
             data = self.get()["data"]
-        self.waypoint_type = data["type"]
-        self.x = data["x"]
-        self.y = data["y"]
-        if "faction" in data:
-            self.faction = data["faction"]["symbol"]
-        else:
-            self.faction = None
-        self.traits = []
-        if "traits" in data:
-            for trait in data["traits"]:
-                self.traits.append(Trait(trait))
-        self.marketplace = (
-            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
-        )
-        self.shipyard = (
-            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
-        )
-
-    @staticmethod
-    def all(system, session, page=1) -> (list, int):
-        r = session.get(
-            session.base_url
-            + "systems/"
-            + system
-            + "/waypoints?limit=20&page="
-            + str(page)
-        )
-        data = r.json()["data"]
-        waypoints = []
-        for w in data:
-            waypoint = Waypoint(w["symbol"], session, w)
-            waypoints.append(waypoint)
-        return waypoints, r.json()["meta"]["total"]
-
-    def __eq__(self, other):
-        return self.symbol == other.symbol
+        self.ship_types = []
+        for ship_type in data["shipTypes"]:
+            self.ship_types.append(ship_type["type"])
+        self.ships = None
+        if "ships" in data:
+            self.ships = []
+            for ship in data["ships"]:
+                self.ships.append(ShipyardShip(ship))
+
+    def purchase(self, ship_type: str):
+        j = self.session.post(
+            self.session.base_url + "my/ships",
+            data={"shipType": ship_type, "waypointSymbol": self.location},
+        ).json()
+        return Ship(j["data"]["ship"], self.session), ShipyardTransaction(j["data"]["transaction"])
```

### Comparing `autotraders-1.3.3/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.4.0/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.4.0/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.4.0/autotraders/map/waypoint_types/marketplace.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/session.py` & `autotraders-1.4.0/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/shared_models/map_symbol.py` & `autotraders-1.4.0/autotraders/shared_models/map_symbol.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,17 @@
             raise ValueError("Invalid map symbol")
         self.raw = s
 
     def __str__(self):
         """Returns the input that was passed as a string."""
         return self.raw
 
+    def __add__(self, other):
+        return self / other
+
     def __truediv__(self, other):
         """Concatenates with a '-'"""
         assert isinstance(other, str)
         if other[0] == "-":
             other = other[1:]
         return MapSymbol(str(self) + "-" + other)
```

### Comparing `autotraders-1.3.3/autotraders/shared_models/transaction.py` & `autotraders-1.4.0/autotraders/shared_models/transaction.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/ship/__init__.py` & `autotraders-1.4.0/autotraders/ship/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 from datetime import datetime, timezone
 from typing import Union, Optional
 
+from autotraders.paginated_list import PaginatedList
 from autotraders.shared_models.item import Item
 from autotraders.shared_models.transaction import MarketTransaction
 from autotraders.space_traders_entity import SpaceTradersEntity
 from autotraders.map.system import System
 from autotraders.session import AutoTradersSession
 from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
@@ -59,26 +60,34 @@
         self.current = data["current"]
         self.required = data["required"]
         self.capacity = data["capacity"]
         self.morale = data["morale"]
         self.wages = data["wages"]
 
 
+class Registration:
+    def __init__(self, data):
+        self.name = data["name"]
+        self.faction_symbol = data["factionSymbol"]
+        self.role = data["role"]
+
+
 class Ship(SpaceTradersEntity):
     def __init__(self, symbol, session: AutoTradersSession, data=None):
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
+        self.registration: Optional[Registration] = None
         super().__init__(session, "my/ships/" + self.symbol, data)
 
     def update(self, data: dict = None, hard=False) -> None:  # TODO: Hard is deprecated
         """
         :param hard: deprecated does not do anything
         """
         if data is None:
@@ -98,14 +107,16 @@
             self.mounts = [Mount(d) for d in data["mounts"]]
         if "nav" in data:
             self.nav = Nav(data["nav"])
         if "fuel" in data:
             self.fuel = Fuel(data["fuel"]["current"], data["fuel"]["capacity"])
         if "cargo" in data:
             self.cargo = Cargo(data["cargo"])
+        if "registration" in data:
+            self.registration = Registration(data["registration"])
 
     async def navigate_async(self, waypoint: Union[str, MapSymbol], interval=1):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
         :param interval: Frequency of updates in seconds (default: 1)
         """
         j = self.post("navigate", data={"waypointSymbol": str(waypoint)})
@@ -161,15 +172,15 @@
     def extract(self):
         j = self.post("extract")
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
         return Item(
             j["data"]["extraction"]["yield"]["symbol"],
             j["data"]["extraction"]["yield"]["units"],
-            "",
+            None,
         )
 
     def refuel(self):
         j = self.post("refuel")
         self.update(j["data"])
         return MarketTransaction(j["data"]["transaction"])
 
@@ -204,14 +215,19 @@
     def refine(self, output_symbol: str):
         j = self.post(
             "refine",
             data={"produce": output_symbol},
         )
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
+        return Item(
+            j["data"]["produced"]["symbol"],
+            j["data"]["produced"]["units"],
+            None
+        )
 
     def chart(self) -> Waypoint:
         """
         Charts the current waypoint
 
         :returns: The info about the waypoint that has been charted
         """
@@ -267,17 +283,26 @@
 
     def remove_mount(self):
         j = self.post("mounts/remove")
         self.update(j["data"])
         return MarketTransaction(j["data"]["transaction"])
 
     @staticmethod
-    def all(session, page: int = 1) -> (str, int):
-        r = session.get(session.base_url + "my/ships?limit=20&page=" + str(page))
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        ships = []
-        for ship in j["data"]:
-            s = Ship(ship["symbol"], session, ship)
-            ships.append(s)
-        return ships, r.json()["meta"]["total"]
+    def all(session, page: int = 1) -> PaginatedList:
+        def paginated_func(p, num_per_page):
+            r = session.get(
+                session.base_url
+                + "my/ships?limit="
+                + str(num_per_page)
+                + "&page="
+                + str(p)
+            )
+            j = r.json()
+            if "error" in j:
+                raise IOError(j["error"]["message"])
+            ships = []
+            for ship in j["data"]:
+                s = Ship(ship["symbol"], session, ship)
+                ships.append(s)
+            return ships, r.json()["meta"]["total"]
+
+        return PaginatedList(paginated_func, page)
```

### Comparing `autotraders-1.3.3/autotraders/ship/ship_components.py` & `autotraders-1.4.0/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/space_traders_entity.py` & `autotraders-1.4.0/autotraders/space_traders_entity.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/status.py` & `autotraders-1.4.0/autotraders/status.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders/util.py` & `autotraders-1.4.0/autotraders/util.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/autotraders.egg-info/PKG-INFO` & `autotraders-1.4.0/autotraders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.3.3
+Version: 1.4.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.3.3/autotraders.egg-info/SOURCES.txt` & `autotraders-1.4.0/autotraders.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 autotraders/__init__.py
 autotraders/agent.py
+autotraders/paginated_list.py
 autotraders/session.py
 autotraders/space_traders_entity.py
 autotraders/status.py
 autotraders/util.py
 autotraders.egg-info/PKG-INFO
 autotraders.egg-info/SOURCES.txt
 autotraders.egg-info/dependency_links.txt
```

### Comparing `autotraders-1.3.3/pyproject.toml` & `autotraders-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.3.3"
+version = "1.4.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "requests>=2.20",
-    "requests-ratelimiter >=0.4"
+    "requests-ratelimiter>=0.4"
 ]
 
 [tool.setuptools.packages.find]
 include = ["autotraders*"]
 exclude = ["source*", "tests*", "venv*"]
 
 [project.urls]
```

### Comparing `autotraders-1.3.3/tests/test_init.py` & `autotraders-1.4.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/tests/test_ship.py` & `autotraders-1.4.0/tests/test_ship.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.3.3/tests/test_util.py` & `autotraders-1.4.0/tests/test_util.py`

 * *Files identical despite different names*

