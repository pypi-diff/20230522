# Comparing `tmp/autotraders-1.1.0.tar.gz` & `tmp/autotraders-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotraders-1.1.0.tar", last modified: Mon May 22 17:49:17 2023, max compression
+gzip compressed data, was "autotraders-1.1.1.tar", last modified: Mon May 22 18:59:49 2023, max compression
```

## Comparing `autotraders-1.1.0.tar` & `autotraders-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.369161 autotraders-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 17:49:03.000000 autotraders-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 17:49:17.369161 autotraders-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 17:49:03.000000 autotraders-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/faction/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/faction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/faction/contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/map/waypoint_types/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/jumpgate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/marketplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/map/waypoint_types/shipyard.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders/shared_models/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/shared_models/map_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/shared_models/trait.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.369161 autotraders-1.1.0/autotraders/ship/
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/ship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/ship/ship_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/ship/survey.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 17:49:03.000000 autotraders-1.1.0/autotraders/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.365161 autotraders-1.1.0/autotraders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 17:49:17.000000 autotraders-1.1.0/autotraders.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 17:49:03.000000 autotraders-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:49:17.369161 autotraders-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:17.369161 autotraders-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:49:03.000000 autotraders-1.1.0/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 17:49:03.000000 autotraders-1.1.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 17:49:03.000000 autotraders-1.1.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.153979 autotraders-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-22 18:59:35.000000 autotraders-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 18:59:49.153979 autotraders-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 18:59:35.000000 autotraders-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/faction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/faction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/faction/contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/map/waypoint_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/jumpgate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/marketplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/map/waypoint_types/shipyard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/shared_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/shared_models/map_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/shared_models/trait.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders/ship/
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/ship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/ship/ship_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/ship/survey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 18:59:35.000000 autotraders-1.1.1/autotraders/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.149979 autotraders-1.1.1/autotraders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 18:59:49.000000 autotraders-1.1.1/autotraders.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 18:59:35.000000 autotraders-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:59:49.153979 autotraders-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:49.153979 autotraders-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 18:59:35.000000 autotraders-1.1.1/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 18:59:35.000000 autotraders-1.1.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 18:59:35.000000 autotraders-1.1.1/tests/test_util.py
```

### Comparing `autotraders-1.1.0/LICENSE` & `autotraders-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/PKG-INFO` & `autotraders-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.0
+Version: 1.1.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.0/README.md` & `autotraders-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/__init__.py` & `autotraders-1.1.1/autotraders/map/waypoint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-"""A spacetraders api"""
-from datetime import datetime
-
-import requests
+import math
 
 from autotraders.session import AutoTradersSession
+from autotraders.shared_models.trait import Trait
+
+from autotraders.shared_models.map_symbol import MapSymbol
+
 
+class Waypoint:
+    def __init__(self, symbol, session: AutoTradersSession, update=True):
+        self.waypoint_type = None
+        self.faction = None
+        self.traits = None
+        self.marketplace = None
+        self.shipyard = None
+        self.session = session
+        self.symbol = MapSymbol(symbol)
+        self.x = math.nan
+        self.y = math.nan
 
-class Status:
-    status: str
-    version: str
-    reset_date: datetime
-    description: str
-    stats: dict[str, int]
-
-
-def get_status():  # TODO: Improve
-    """returns the API status, with reset dates, see the Status class for more info."""
-    r = requests.get("https://api.spacetraders.io/v2/")
-    j = r.json()
-    s = Status()
-    s.status = j["status"]
-    s.version = j["version"]
-    s.reset_date = j["resetDate"]
-    s.description = j["description"]
-    s.stats = j["stats"]
-
-
-class SpaceTradersEntity:
-    def __init__(self, session: AutoTradersSession, update, action_url):
-        self.session: AutoTradersSession = session
-        self.action_url = action_url
-        if self.action_url[-1] != "/":
-            self.action_url += "/"
         if update:
             self.update()
 
-    def get(self, action: str = "") -> dict:
-        if action == "":
-            r = self.session.get(self.action_url[0 : len(self.action_url) - 1])
+    def update(self, data=None):
+        if data is None:
+            data = self.session.get(
+                self.session.base_url
+                + "systems/"
+                + self.symbol.system
+                + "/waypoints/"
+                + self.symbol.waypoint
+                + "/?limit=20"
+            ).json()["data"]
+        self.waypoint_type = data["type"]
+        self.x = data["x"]
+        self.y = data["y"]
+        if "faction" in data:
+            self.faction = data["faction"]["symbol"]
         else:
-            r = self.session.get(
-                self.action_url + action,
-            )
-        j = r.json()
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        return j
-
-    def post(self, action: str, data=None) -> dict:
-        print(self.action_url + action)
-        print(data)
-        print(type(data))
-        self.session.headers["Content-Type"] = "application/json"
-        r = self.session.post(
-            self.action_url + action,
-            data=data,
+            self.faction = None
+        self.traits = []
+        if "traits" in data:
+            for trait in data["traits"]:
+                self.traits.append(Trait(trait))
+        self.marketplace = (
+            len([trait for trait in self.traits if trait.symbol == "MARKETPLACE"]) > 0
         )
-        j = r.json()
-        print(j)
-        if "error" in j:
-            raise IOError(j["error"]["message"])
-        return j
+        self.shipyard = (
+            len([trait for trait in self.traits if trait.symbol == "SHIPYARD"]) > 0
+        )
+
+    @staticmethod
+    def all(system, session):
+        r = session.get(session.base_url + "systems/" + system + "/waypoints")
+        data = r.json()["data"]
+        waypoints = []
+        for w in data:
+            waypoint = Waypoint(w["symbol"], session, False)
+            waypoint.update(w)
+            waypoints.append(waypoint)
+        return waypoints
+
 
-    def update(self):
-        pass
+def get_all_waypoints(system, session):
+    return Waypoint.all(system, session)
```

### Comparing `autotraders-1.1.0/autotraders/agent.py` & `autotraders-1.1.1/autotraders/agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         self.ships = None
         self.headquarters = None
         super().__init__(session, update, session.base_url + "my/agent")
 
     def update(self, data=None):
         """Uses 3 API requests to get all agent details"""
         if data is None:
-            print(self.get(""))
             data = self.get("")["data"]
         self.account_id = data["accountId"]
         self.symbol = data["symbol"]
         self.headquarters = data["headquarters"]
         self.credits = data["credits"]
         self.starting_faction = data["startingFaction"]
         self.ships = get_all_ships(self.session)
```

### Comparing `autotraders-1.1.0/autotraders/faction/__init__.py` & `autotraders-1.1.1/autotraders/faction/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/faction/contract.py` & `autotraders-1.1.1/autotraders/faction/contract.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/map/system.py` & `autotraders-1.1.1/autotraders/map/system.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/map/waypoint.py` & `autotraders-1.1.1/autotraders/map/waypoint_types/marketplace.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,46 @@
-import math
-
+from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
-from autotraders.shared_models.trait import Trait
-
-from autotraders.shared_models.map_symbol import MapSymbol
-
 
-class Waypoint:
-    def __init__(self, symbol, session: AutoTradersSession, update=True):
-        self.waypoint_type = None
-        self.faction = None
-        self.traits = None
-        self.marketplace = None
-        self.shipyard = None
-        self.session = session
-        self.symbol = MapSymbol(symbol)
-        self.x = math.nan
-        self.y = math.nan
 
-        if update:
-            self.update()
+class TradeGood:
+    def __init__(self, data):
+        self.symbol = data["symbol"]
+        self.trade_volume = data["tradeVolume"]
+        self.supply = data["supply"]
+        self.purchase_price = data["purchasePrice"]
+        self.sell_price = data["sellPrice"]
+
+
+class Marketplace(WaypointType):
+    def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
+        super().__init__(waypoint, "market", session, update)
+        self.imports = None
+        self.exports = None
+        self.exchange = None
+        self.trade_goods = None
 
-    def update(self, data=None):
+    def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
-                + self.symbol.system
+                + self.location.system
                 + "/waypoints/"
-                + self.symbol.waypoint
-                + "/?limit=20"
+                + self.location.waypoint
+                + "/market"
             ).json()["data"]
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
-    def all(system, session):
-        r = session.get(session.base_url + "systems/" + system + "/waypoints")
-        data = r.json()["data"]
-        waypoints = []
-        for w in data:
-            waypoint = Waypoint(w["symbol"], session, False)
-            waypoint.update(w)
-            waypoints.append(waypoint)
-        return waypoints
-
-
-def get_all_waypoints(system, session):
-    return Waypoint.all(system, session)
+        self.imports = []
+        for i in data["imports"]:
+            self.imports.append(i["symbol"])
+        self.exports = []
+        for i in data["exports"]:
+            self.exports.append(i["symbol"])
+        self.exchange = []
+        for i in data["exchange"]:
+            self.exchange.append(i["symbol"])
+
+        self.trade_goods = None
+        if "tradeGoods" in data:
+            self.trade_goods = []
+            for i in data["tradeGoods"]:
+                self.trade_goods.append(TradeGood(i))
```

### Comparing `autotraders-1.1.0/autotraders/map/waypoint_types/__init__.py` & `autotraders-1.1.1/autotraders/map/waypoint_types/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/map/waypoint_types/jumpgate.py` & `autotraders-1.1.1/autotraders/map/waypoint_types/jumpgate.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/map/waypoint_types/marketplace.py` & `autotraders-1.1.1/autotraders/map/waypoint_types/shipyard.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from autotraders.map.waypoint_types import WaypointType
 from autotraders.session import AutoTradersSession
+from autotraders.ship import Frame, Reactor, Engine, Module, Mount
 
 
-class TradeGood:
+class ShipyardShip:
     def __init__(self, data):
-        self.symbol = data["symbol"]
-        self.trade_volume = data["tradeVolume"]
-        self.supply = data["supply"]
+        self.ship_type = data["type"]
+        self.name = data["name"]
+        self.description = data["description"]
         self.purchase_price = data["purchasePrice"]
-        self.sell_price = data["sellPrice"]
+        self.frame = Frame(data["frame"])
+        self.reactor = Reactor(data["reactor"])
+        self.engine = Engine(data["engine"])
+        self.modules = [Module(d) for d in data["modules"]]
+        self.mounts = [Mount(d) for d in data["mounts"]]
 
 
-class Marketplace(WaypointType):
+class Shipyard(WaypointType):
     def __init__(self, waypoint: str, session: AutoTradersSession, update=True):
-        super().__init__(waypoint, "market", session, update)
-        self.imports = None
-        self.exports = None
-        self.exchange = None
-        self.trade_goods = None
+        super().__init__(waypoint, "shipyard", session, update)
+        self.ship_types = None
+        self.ships = None
 
     def update(self, data: dict = None):
         if data is None:
             data = self.session.get(
                 self.session.base_url
                 + "systems/"
                 + self.location.system
                 + "/waypoints/"
                 + self.location.waypoint
-                + "/market"
+                + "/shipyard"
             ).json()["data"]
-        self.imports = []
-        for i in data["imports"]:
-            self.imports.append(i["symbol"])
-        self.exports = []
-        for i in data["exports"]:
-            self.exports.append(i["symbol"])
-        self.exchange = []
-        for i in data["exchange"]:
-            self.exchange.append(i["symbol"])
-
-        self.trade_goods = None
-        if "tradeGoods" in data:
-            self.trade_goods = []
-            for i in data["tradeGoods"]:
-                self.trade_goods.append(TradeGood(i))
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

### Comparing `autotraders-1.1.0/autotraders/session.py` & `autotraders-1.1.1/autotraders/session.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/shared_models/map_symbol.py` & `autotraders-1.1.1/autotraders/shared_models/map_symbol.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
         """Your input must be a valid symbol for a sector, system, or waypoint. or a value error might be raised.
         :param s: The symbol
         """
         if type(s) is MapSymbol:
             s = str(s)
         split = s.split("-")
         self.sector = split[0]
-        if len(split) > 1:
-            self.system = split[0] + "-" + split[1]
         if len(split) == 2:
+            self.system = split[0] + "-" + split[1]
+        if len(split) == 3:
             self.waypoint = split[0] + "-" + split[1] + "-" + split[2]
-        if len(split) > 2:
+        if len(split) > 3:
             raise ValueError("Invalid map symbol")
         self.raw = s
 
     def __str__(self):
         """Returns the input that was passed as a string."""
         return self.raw
```

### Comparing `autotraders-1.1.0/autotraders/ship/__init__.py` & `autotraders-1.1.1/autotraders/ship/__init__.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders/ship/ship_components.py` & `autotraders-1.1.1/autotraders/ship/ship_components.py`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/autotraders.egg-info/PKG-INFO` & `autotraders-1.1.1/autotraders.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotraders
-Version: 1.1.0
+Version: 1.1.1
 Summary: A powerful spacetraders API
 Author-email: Ashwin Naren <arihant2math@gmail.com>
 Project-URL: Homepage, https://arihant2math.github.io/autotraders/
 Project-URL: Documentation, https://arihant2math.github.io/autotraders/
 Project-URL: Bug Tracker, https://github.com/arihant2math/autotraders/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `autotraders-1.1.0/autotraders.egg-info/SOURCES.txt` & `autotraders-1.1.1/autotraders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autotraders-1.1.0/pyproject.toml` & `autotraders-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autotraders"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Ashwin Naren", email="arihant2math@gmail.com" },
 ]
 description = "A powerful spacetraders API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `autotraders-1.1.0/tests/test_init.py` & `autotraders-1.1.1/tests/test_init.py`

 * *Files identical despite different names*

