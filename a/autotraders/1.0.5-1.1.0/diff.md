# Comparing `tmp/autotraders-1.0.5.tar.gz` & `tmp/autotraders-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.0.5.tar", last modified: Fri May 19 00:43:06 2023, max compression
+gzip compressed data, was "autotraders-1.1.0.tar", last modified: Mon May 22 17:49:17 2023, max compression
```

## Comparing `autotraders-1.0.5.tar` & `autotraders-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-19 00:42:53.000000 autotraders-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-19 00:43:06.461463 autotraders-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-19 00:42:53.000000 autotraders-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.457463 autotraders-1.0.5/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)    11176 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/trait.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/autotraders/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-19 00:42:53.000000 autotraders-1.0.5/autotraders/waypoint_types/shipyard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 00:43:06.000000 autotraders-1.0.5/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-19 00:42:53.000000 autotraders-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 00:43:06.461463 autotraders-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 00:43:06.461463 autotraders-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-19 00:42:53.000000 autotraders-1.0.5/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.369161 autotraders-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 17:49:03.000000 autotraders-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 17:49:17.369161 autotraders-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 17:49:03.000000 autotraders-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.369161 autotraders-1.1.0/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 17:49:03.000000 autotraders-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:49:17.369161 autotraders-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.369161 autotraders-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:03.000000 autotraders-1.1.0/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 17:49:03.000000 autotraders-1.1.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 17:49:03.000000 autotraders-1.1.0/tests/test_util.py
```

### Comparing `autotraders-1.0.5/LICENSE` & `autotraders-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.5/PKG-INFO` & `autotraders-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.0.5
+Version: 1.1.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.0.5/README.md` & `autotraders-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.5/autotraders/agent.py` & `autotraders-1.1.0/autotraders/map/waypoint_types/shipyard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,48 @@
-import math
+from autotraders.map.waypoint_types import WaypointType
+from autotraders.session import AutoTradersSession
+from autotraders.ship import Frame, Reactor, Engine, Module, Mount
 
-import requests
 
-from autotraders.ship import get_all_ships
-from autotraders.contract import get_all_contracts
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
 
 
-class Agent:
-    def __init__(self, session: requests.Session, update=True):
-        self.session = session
-        self.credits = math.nan
-        if update:
-            self.update()
+class Shipyard(WaypointType):
+    def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
+        super().__init__(waypoint, "shipyard", session, update)
+        self.ship_types = None
+        self.ships = None
 
-    def update(self, data=None):
-        """Uses 3 API requests to get all agent details"""
+    def update(self, data: dict = None):
         if data is None:
-            r = self.session.get("https://api.spacetraders.io/v2/my/agent")
-            j = r.json()
-            if "error" in j:
-                raise IOError(j["error"]["message"])
-            data = j["data"]
-        self.account_id = data["accountId"]
-        self.symbol = data["symbol"]
-        self.headquarters = data["headquarters"]
-        self.credits = data["credits"]
-        self.ships = get_all_ships(self.session)
-        self.contracts = get_all_contracts(self.session)
+            data = self.session.get(
+                self.session.base_url
+                + "systems/"
+                + self.location.system
+                + "/waypoints/"
+                + self.location.waypoint
+                + "/shipyard"
+            ).json()["data"]
+        self.ship_types = []
+        for ship_type in data["shipTypes"]:
+            self.ship_types.append(ship_type["type"])
+        self.ships = None
+        if "ships" in data:
+            self.ships = []
+            for ship in data["ships"]:
+                ShipyardShip(ship)
+
+    def purchase(self, ship_type: str):
+        self.session.post(
+            self.session.base_url + "my/ships",
+            data={"shipType": ship_type, "waypointSymbol": self.location},
+        )
```

### Comparing `autotraders-1.0.5/autotraders/contract.py` & `autotraders-1.1.0/autotraders/faction/contract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,83 @@
-import requests
+import math
 
+from autotraders import SpaceTradersEntity
+from autotraders.session import AutoTradersSession
+from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.util import parse_time
 
 
 class Deliver:
     def __init__(self, data):
-        self.trade_symbol = data["tradeSymbol"]
-        self.destination_symbol = data["destinationSymbol"]
+        self.trade_symbol = MapSymbol(data["tradeSymbol"])
+        self.destination_symbol = MapSymbol(data["destinationSymbol"])
         self.units_required = data["unitsRequired"]
         self.units_fulfilled = data["unitsFulfilled"]
 
 
-class Contract:
-    def __init__(self, contract_id, session: requests.Session, update=True):
+class Contract(SpaceTradersEntity):
+    def __init__(self, contract_id, session: AutoTradersSession, update=True):
+        self.contract_data = None
+        self.accepted = None
+        self.fulfilled = None
+        self.deadline = None
+        self.accept_deadline = None
+        self.contract_type = None
+        self.on_fulfilled = math.nan
+        self.on_accepted = math.nan
         self.contract_id = contract_id
-        self.session = session
-        if update:
-            self.update()
+        super().__init__(session, update, session.base_url + "my/contracts/" + self.contract_id)
 
     def update(self, data=None):
         if data is None:
-            r = self.session.get(
-                "https://api.spacetraders.io/v2/my/contracts/" + self.contract_id
-            )
-            data = r.json()["data"]
+            data = self.get()["data"]
         self.on_accepted = data["terms"]["payment"]["onAccepted"]
         self.on_fulfilled = data["terms"]["payment"]["onFulfilled"]
         self.accepted = data["accepted"]
         self.fulfilled = data["fulfilled"]
         self.deadline = parse_time(data["terms"]["deadline"])
-        if "deliver" in data:
-            self.contract_type = "deliver"
-            self.contract_data = [Deliver(d) for d in data["deliver"]]
+        self.accept_deadline = parse_time(data["deadlineToAccept"])
+        self.contract_type = data["type"]
+        if "deliver" in data["terms"]:
+            self.contract_data = [Deliver(d) for d in data["terms"]["deliver"]]
 
     def accept(self):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/contracts/"
-            + self.contract_id
-            + "/accept"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("accept")
+        self.update(j["data"]["contract"])
 
     def deliver(self, symbol, cargo_symbol, amount):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/contracts/"
-            + self.contract_id
-            + "/deliver",
-            data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
+        j = self.post("deliver",
+                      data={"shipSymbol": symbol, "tradeSymbol": cargo_symbol, "units": amount},
+                      )
+        self.update(j["data"]["contract"])
+
+    def negotiate(self, ship_symbol, session):
+        j = session.post(
+            self.session.base_url + "my/ships/" + ship_symbol + "/negotiate/contract"
         ).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
-        self.update()
+        c = Contract(j["data"]["id"], self.session, False)
+        c.update(j["data"])
+        return c
 
     def fulfill(self):
         j = self.session.post(
-            "https://api.spacetraders.io/v2/my/contracts/"
-            + self.contract_id
-            + "/fulfill"
+            self.session.base_url + "my/contracts/" + self.contract_id + "/fulfill"
         ).json()
         if "error" in j:
             raise IOError(j["error"]["message"])
 
     @staticmethod
-    def all(session):
-        r = session.get("https://api.spacetraders.io/v2/my/contracts")
+    def all(session, page: int = 1):
+        r = session.get(session.base_url + "my/contracts?page=" + str(page))
         j = r.json()
         contracts = []
         for contract in j["data"]:
             c = Contract(contract["id"], session, False)
             c.update(contract)
             contracts.append(c)
-        return contracts
+        return contracts, r.json()["meta"]["total"]
 
 
 def get_all_contracts(session):
-    return Contract.all(session)
+    return Contract.all(session)[0]
```

### Comparing `autotraders-1.0.5/autotraders/faction.py` & `autotraders-1.1.0/autotraders/faction/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-import requests
+from autotraders import SpaceTradersEntity
+from autotraders.session import AutoTradersSession
+from autotraders.shared_models.map_symbol import MapSymbol
+from autotraders.shared_models.trait import Trait
 
-from autotraders.trait import Trait
 
-
-class Faction:
-    def __init__(self, symbol, session: requests.Session, update=True):
+class Faction(SpaceTradersEntity):
+    def __init__(self, symbol, session: AutoTradersSession, update=True):
+        self.is_recruting = None
+        self.traits = None
+        self.headquarters = None
+        self.description = None
+        self.name = None
         self.symbol = symbol
-        self.session = session
-        if update:
-            self.update()
+        super().__init__(session, update, session.base_url + "factions/" + self.symbol)
 
     def update(self, data=None):
         if data is None:
-            r = self.session.get(
-                "https://api.spacetraders.io/v2/factions/" + self.symbol
-            )
-            data = r.json()["data"]
+            data = self.get("")["data"]
         self.name = data["name"]
         self.description = data["description"]
-        self.headquarters = data["headquarters"]
+        self.headquarters = MapSymbol(data["headquarters"])
         self.traits = []
         for trait in data["traits"]:
             self.traits.append(Trait(trait))
+        self.is_recruting = data["isRecruiting"]
 
     @staticmethod
     def all(session):
-        r = session.get("https://api.spacetraders.io/v2/factions")
+        r = session.get(session.base_url + "factions")
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         factions = []
         for f in j["data"]:
             faction = Faction(f["symbol"], session, False)
             faction.update(f)
```

### Comparing `autotraders-1.0.5/autotraders/ship/__init__.py` & `autotraders-1.1.0/autotraders/ship/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import asyncio
 
-import requests
-
-from autotraders.ship.survey import Survey
-
+from autotraders import SpaceTradersEntity
+from autotraders.session import AutoTradersSession
+from autotraders.shared_models.map_symbol import MapSymbol
 from autotraders.ship.ship_components import Frame, Reactor, Engine, Module, Mount
+from autotraders.ship.survey import Survey
 from autotraders.util import parse_time
-from autotraders.waypoint import Waypoint
+from autotraders.map.waypoint import Waypoint
 
 
 class Fuel:
     def __init__(self, current, total):
         self.current = current
         self.total = total
 
@@ -27,50 +27,60 @@
         for symbol in inventory:
             self.inventory[symbol["symbol"]] = symbol["units"]
             self.current += symbol["units"]
 
 
 class Route:
     def __init__(self, data):
-        self.destination = data["destination"]
-        self.departure = data["departure"]["symbol"]
+        self.destination = MapSymbol(data["destination"]["symbol"])
+        self.departure = MapSymbol(data["departure"]["symbol"])
         self.moving = self.destination == self.departure
         if self.moving:
             self.depature_time = parse_time(data["departure_time"])
             self.arrival = parse_time(data["arrival"])
 
 
 class Nav:
     def __init__(self, data):
         self.status = data["status"]
-        self.location = data["waypointSymbol"]
+        self.location = MapSymbol(data["waypointSymbol"])
         self.flight_mode = data["flightMode"]
         self.route = Route(data["route"])
 
 
-class Ship:
-    def __init__(self, symbol, session: requests.Session, update=True):
+class Crew:
+    def __init__(self, data):
+        self.current = data["current"]
+        self.required = data["required"]
+        self.capacity = data["capacity"]
+        self.morale = data["morale"]
+        self.wages = data["wages"]
+
+
+class Ship(SpaceTradersEntity):
+    def __init__(self, symbol, session: AutoTradersSession, update=True):
+        self.cargo = None
+        self.fuel = None
+        self.nav = None
         self.symbol = symbol
-        self.session = session
         self.frame = None
         self.reactor = None
         self.engine = None
         self.modules = None
         self.mounts = None
-        if update:
-            self.update()
+        self.crew = None
+        super().__init__(
+            session, update, session.base_url + "my/ships/" + self.symbol + "/"
+        )
 
     def update(self, data: dict = None, hard=False):
         if data is None:
-            r = self.session.get(
-                "https://api.spacetraders.io/v2/my/ships/" + self.symbol
-            )
-            if "error" in r.json():
-                raise IOError(r.json()["error"]["message"])
-            data = r.json()["data"]
+            data = self.get("")["data"]  # TODO: This is a hack (sort of)
+        if self.crew is None and not hard:
+            self.crew = Crew(data["crew"])
         if self.frame is None and not hard:
             self.frame = Frame(data["frame"])
         if self.reactor is None and not hard:
             self.reactor = Reactor(data["reactor"])
         if self.engine is None and not hard:
             self.engine = Engine(data["engine"])
         if self.modules is None and not hard:
@@ -86,74 +96,51 @@
 
     async def navigate_async(self, waypoint):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function waits for the ship to arrive.
             :raise:
                 IOError: if a server error occurs
         """
-        r = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/navigate",
-            data={"waypointSymbol": waypoint},
-        )
-        j = r.json()
-        if "error" in j:
-            raise j["error"]["message"]
-        await asyncio.sleep(5)
-        self.update()
+        j = self.post("navigate", data={"waypointSymbol": waypoint})
+        self.update(j["data"])
         while self.nav.status == "IN_TRANSIT":
             await asyncio.sleep(5)
             self.update()
 
     def navigate(self, waypoint):
         """Attempts to move ship to the provided waypoint.
         If the request succeeds, this function exits immediately, and does not wait the ship to arrive.
             :raise:
                 IOError: if a server error occurs
         """
-        r = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/navigate",
-            data={"waypointSymbol": waypoint},
-        )
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("navigate", data={"waypointSymbol": waypoint})
         self.update(j["data"])
 
     def patch_navigation(self, new_flight_mode):
         r = self.session.patch(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/nav"
+            self.session.base_url + "my/ships/" + self.symbol + "/nav",
+            data={"flightMode": new_flight_mode},  # TODO: Test
         )
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         self.update({"nav": j["data"]})
 
     def dock(self):
-        r = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/dock"
-        )
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        self.update(j['data'])
+        j = self.post("dock")
+        self.update(j["data"])
 
     def orbit(self):
-        r = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/orbit"
-        )
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("orbit")
         self.update(j["data"])
 
     def extract(self):
-        r = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/extract"
-        )
-        j = r.json()
+        j = self.session.post(
+            self.session.base_url + "my/ships/" + self.symbol + "/extract"
+        ).json()
         if "error" in j:
             if j["error"]["code"] == 4000:
                 raise IOError(
                     "Ship is still in cooldown, "
                     + str(j["error"]["data"]["cooldown"]["remainingSeconds"])
                     + " seconds out of "
                     + str(j["error"]["data"]["cooldown"]["totalSeconds"])
@@ -161,167 +148,127 @@
                 )
             else:
                 raise IOError(j["error"]["message"])
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["data"]["cooldown"]["expiration"])
 
     def refuel(self):
-        r = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/refuel"
-        )
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("refuel")
         self.update(j["data"])
 
     def sell(self, cargo_symbol, quantity):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/sell",
-            data={"symbol": cargo_symbol, "units": quantity},
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        self.update()
+        j = self.post("sell", data={"symbol": cargo_symbol, "units": quantity})
+        self.update(j["data"])
 
     def buy(self, cargo_symbol, quantity):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/purchase",
-            data={"symbol": cargo_symbol, "units": quantity},
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("purchase", data={"symbol": cargo_symbol, "units": quantity})
         self.update(j["data"])
 
     def transfer(self, destination: str, cargo_symbol: str, quantity: int):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/transfer",
+        j = self.post(
+            "transfer",
             data={
                 "tradeSymbol": cargo_symbol,
                 "units": quantity,
                 "shipSymbol": destination,
             },
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        )
         self.update(j["data"])
 
     def jump(self, destination: str):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/jump",
+        j = self.post(
+            "jump",
             data={
                 "systemSymbol": destination,
             },
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        )
         self.update(j["data"])
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
 
     def warp(self, destination: str):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/warp",
+        j = self.post(
+            "warp",
             data={
                 "waypointSymbol": destination,
             },
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        )
         self.update(j["data"])
 
     def jettison(self, cargo_symbol: str, quantity: int):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/jettison",
+        j = self.post(
+            "jettison",
             data={"symbol": cargo_symbol, "units": quantity},
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        )
         self.update(j["data"])
 
     def refine(self, output_symbol: str):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/refine",
+        j = self.post(  # TODO: Fix
+            "refine",
             data={"produce": output_symbol},
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        self.update()
+        )
+        self.update(j["data"])
+        self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
 
-    def chart(self):
+    def chart(self) -> Waypoint:
         """
         Charts the current waypoint
         :return: The info about the waypoint that has been charted
         """
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/chart"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("chart")
         w = Waypoint(j["data"]["waypoint"]["symbol"], self.session, False)
         w.update(j["data"]["waypoint"])
-        self.update()
+        self.update()  # TODO: Fix
         return w
 
-    def survey(self):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/survey"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+    def survey(self) -> list[Survey]:
+        j = self.post("survey")
         surveys = []
-        for survey in j["data"]["surveys"]:
-            surveys.append(Survey(survey))
+        for s in j["data"]["surveys"]:
+            surveys.append(Survey(s))
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
         return surveys
 
     def scan_systems(self):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/scan/systems"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("scan/systems")
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
-        raise NotImplementedError
+        raise NotImplementedError  # TODO: Fix
 
     def scan_waypoints(self):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/scan/waypoints"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("scan/waypoints")
         waypoints = []
         for waypoint in j["systems"]:
             s = Waypoint(waypoint["symbol"], self.session, False)
             s.update(waypoint)
             waypoints.append(s)
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
         return waypoints
 
     def scan_ships(self):
-        j = self.session.post(
-            "https://api.spacetraders.io/v2/my/ships/" + self.symbol + "/scan/ships"
-        ).json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
+        j = self.post("scan/ships")
         ships = []
         for ship in j["data"]["ships"]:
             s = Ship(ship["data"], self.session, False)
             s.update(ship)
             ships.append(s)
         self.reactor.cooldown = parse_time(j["cooldown"]["expiration"])
         return ships
 
+    def update_ship_cooldown(self):
+        j = self.get("cooldown")
+        self.reactor.cooldown = parse_time(j["data"]["expiration"])
+
     @staticmethod
-    def all(session):
-        r = session.get("https://api.spacetraders.io/v2/my/ships")
+    def all(session, page: int = 1):
+        r = session.get(session.base_url + "my/ships?page=" + str(page))
         j = r.json()
         if "error" in j:
             raise IOError(j["error"]["message"])
         ships = []
         for ship in j["data"]:
             s = Ship(ship["symbol"], session, False)
             s.update(ship)
             ships.append(s)
-        return ships
+        return ships, r.json()["meta"]["total"]
 
 
 def get_all_ships(session):
-    return Ship.all(session)
+    return Ship.all(session)[0]
```

### Comparing `autotraders-1.0.5/autotraders/ship/ship_components.py` & `autotraders-1.1.0/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.0.5/autotraders/system.py` & `autotraders-1.1.0/autotraders/map/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import math
 
-import requests
+from autotraders import SpaceTradersEntity
+from autotraders.session import AutoTradersSession
+from autotraders.map.waypoint import Waypoint
+from autotraders.shared_models.map_symbol import MapSymbol
 
-from autotraders.waypoint import Waypoint
 
-
-class System:
-    def __init__(self, symbol, session: requests.Session, update=True):
-        self.session = session
-        self.symbol = symbol
+class System(SpaceTradersEntity):
+    def __init__(self, symbol, session: AutoTradersSession, update=True):
+        self.symbol = MapSymbol(symbol)
         self.x = math.nan
         self.y = math.nan
-        if update:
-            self.update()
+        self.waypoints = None
+        self.factions = None
+        self.star_type = None
+        super().__init__(
+            session, update, session.base_url + "systems/" + str(self.symbol) + "/"
+        )
 
     def update(self, data=None):
         if data is None:
-            r = self.session.get(
-                "https://api.spacetraders.io/v2/systems/" + self.symbol
-            )
-            data = r.json()["data"]
+            data = self.get("")["data"]
         self.waypoints = []
         self.x = data["x"]
         self.y = data["y"]
         self.factions = data["factions"]
         self.star_type = data["type"]
         for w in data["waypoints"]:
             waypoint = Waypoint(w["symbol"], self.session, False)
             waypoint.update(w)
             self.waypoints.append(waypoint)
 
     @staticmethod
-    def all(session, page=1):
-        r = session.get("https://api.spacetraders.io/v2/systems?limit=20&page=" + str(page))
+    def all(session, page=1) -> (list, int):
+        r = session.get(session.base_url + "systems?limit=20&page=" + str(page))
         j = r.json()["data"]
         systems = []
         for system in j:
             s = System(system["symbol"], session, False)
             s.update(system)
             systems.append(s)
         return systems, r.json()["meta"]["total"]
```

### Comparing `autotraders-1.0.5/autotraders/waypoint.py` & `autotraders-1.1.0/autotraders/map/waypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-import requests
+import math
 
-from autotraders.trait import Trait
+from autotraders.session import AutoTradersSession
+from autotraders.shared_models.trait import Trait
+
+from autotraders.shared_models.map_symbol import MapSymbol
 
 
 class Waypoint:
-    def __init__(self, symbol, session: requests.Session, update=True):
+    def __init__(self, symbol, session: AutoTradersSession, update=True):
+        self.waypoint_type = None
+        self.faction = None
+        self.traits = None
+        self.marketplace = None
+        self.shipyard = None
         self.session = session
-        self.symbol = symbol
+        self.symbol = MapSymbol(symbol)
+        self.x = math.nan
+        self.y = math.nan
+
         if update:
             self.update()
 
     def update(self, data=None):
         if data is None:
-            split = self.symbol.split("-")
-            self.sector = split[0]
-            self.system_symbol = split[0] + "-" + split[1]
-            waypoint_symbol = self.symbol
             data = self.session.get(
-                "https://api.spacetraders.io/v2/systems/"
-                + self.system_symbol
+                self.session.base_url
+                + "systems/"
+                + self.symbol.system
                 + "/waypoints/"
-                + waypoint_symbol
+                + self.symbol.waypoint
+                + "/?limit=20"
             ).json()["data"]
         self.waypoint_type = data["type"]
         self.x = data["x"]
         self.y = data["y"]
         if "faction" in data:
             self.faction = data["faction"]["symbol"]
         else:
             self.faction = None
         self.traits = []
         if "traits" in data:
             for trait in data["traits"]:
                 self.traits.append(Trait(trait))
         self.marketplace = (
-                len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
         self.shipyard = (
-                len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
         )
 
     @staticmethod
     def all(system, session):
-        r = session.get("https://api.spacetraders.io/v2/systems/" + system + "/waypoints")
+        r = session.get(session.base_url + "systems/" + system + "/waypoints")
         data = r.json()["data"]
         waypoints = []
         for w in data:
             waypoint = Waypoint(w["symbol"], session, False)
             waypoint.update(w)
             waypoints.append(waypoint)
         return waypoints
```

### Comparing `autotraders-1.0.5/autotraders/waypoint_types/marketplace.py` & `autotraders-1.1.0/autotraders/map/waypoint_types/marketplace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import requests
+from autotraders.map.waypoint_types import WaypointType
+from autotraders.session import AutoTradersSession
 
 
 class TradeGood:
     def __init__(self, data):
         self.symbol = data["symbol"]
         self.trade_volume = data["tradeVolume"]
         self.supply = data["supply"]
         self.purchase_price = data["purchasePrice"]
         self.sell_price = data["sellPrice"]
 
 
-class Marketplace:
-    def __init__(self, waypoint: str, session: requests.Session, update=True):
-        self.location = waypoint
-        self.session = session
-        if update:
-            self.update()
+class Marketplace(WaypointType):
+    def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
+        super().__init__(waypoint, "market", session, update)
+        self.imports = None
+        self.exports = None
+        self.exchange = None
+        self.trade_goods = None
 
     def update(self, data: dict = None):
         if data is None:
-            split = self.location.split("-")
-            system_symbol = split[0] + "-" + split[1]
-            waypoint_symbol = self.location
             data = self.session.get(
-                "https://api.spacetraders.io/v2/systems/"
-                + system_symbol
+                self.session.base_url
+                + "systems/"
+                + self.location.system
                 + "/waypoints/"
-                + waypoint_symbol
+                + self.location.waypoint
                 + "/market"
             ).json()["data"]
         self.imports = []
         for i in data["imports"]:
             self.imports.append(i["symbol"])
         self.exports = []
         for i in data["exports"]:
```

### Comparing `autotraders-1.0.5/autotraders.egg-info/PKG-INFO` & `autotraders-1.1.0/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.0.5
+Version: 1.1.0
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.0.5/pyproject.toml` & `autotraders-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.0.5"
+version = "1.1.0"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

