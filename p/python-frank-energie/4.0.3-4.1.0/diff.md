# Comparing `tmp/python_frank_energie-4.0.3.tar.gz` & `tmp/python_frank_energie-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-4.0.3.tar", max compression
+gzip compressed data, was "python_frank_energie-4.1.0.tar", max compression
```

## Comparing `python_frank_energie-4.0.3.tar` & `python_frank_energie-4.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2023-05-04 13:23:35.186148 python_frank_energie-4.0.3/LICENSE
--rw-r--r--   0        0        0      325 2023-05-04 13:23:35.186148 python_frank_energie-4.0.3/README.md
--rw-r--r--   0        0        0     2353 2023-05-04 13:23:54.373767 python_frank_energie-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      175 2023-05-04 13:23:35.186148 python_frank_energie-4.0.3/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      378 2023-05-04 13:23:35.186148 python_frank_energie-4.0.3/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0     7092 2023-05-04 13:23:35.186148 python_frank_energie-4.0.3/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0    10387 2023-05-04 13:23:35.186148 python_frank_energie-4.0.3/python_frank_energie/models.py
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/LICENSE
+-rw-r--r--   0        0        0      325 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/README.md
+-rw-r--r--   0        0        0     2353 2023-05-22 09:35:02.079432 python_frank_energie-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      378 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0     8256 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0    11198 2023-05-22 09:34:41.962801 python_frank_energie-4.1.0/python_frank_energie/models.py
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 python_frank_energie-4.1.0/PKG-INFO
```

### Comparing `python_frank_energie-4.0.3/LICENSE` & `python_frank_energie-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-4.0.3/pyproject.toml` & `python_frank_energie-4.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "4.0.3"
+version = "4.1.0"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
```

### Comparing `python_frank_energie-4.0.3/python_frank_energie/frank_energie.py` & `python_frank_energie-4.1.0/python_frank_energie/frank_energie.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """FrankEnergie API implementation."""
 
 from __future__ import annotations
 
 import asyncio
-from datetime import datetime
+from datetime import date
 from typing import Any
 
 from aiohttp.client import ClientError, ClientSession
 
 from .exceptions import AuthRequiredException
 from .models import Authentication, Invoices, MarketPrices, MonthSummary, User
 
@@ -46,15 +46,15 @@
             )
 
             return await resp.json()
 
         except (asyncio.TimeoutError, ClientError, KeyError) as error:
             raise ValueError(f"Request failed: {error}") from error
 
-    async def login(self, username: str, password: str) -> str:
+    async def login(self, username: str, password: str) -> Authentication:
         """Login and get the authentication token."""
         query = {
             "query": """
                 mutation Login($email: String!, $password: String!) {
                     login(email: $email, password: $password) {
                         authToken
                         refreshToken
@@ -64,15 +64,15 @@
             "operationName": "Login",
             "variables": {"email": username, "password": password},
         }
 
         self._auth = Authentication.from_dict(await self._query(query))
         return self._auth
 
-    async def renewToken(self, authToken: str, refreshToken: str) -> str:
+    async def renewToken(self, authToken: str, refreshToken: str) -> Authentication:
         """Renew the authentication token."""
         query = {
             "query": """
                 mutation RenewToken($authToken: String!, $refreshToken: String!) {
                     renewToken(authToken: $authToken, refreshToken: $refreshToken) {
                         authToken
                         refreshToken
@@ -171,15 +171,15 @@
             "operationName": "Me",
             "variables": {},
         }
 
         return User.from_dict(await self._query(query))
 
     async def prices(
-        self, start_date: datetime, end_date: datetime | None = None
+        self, start_date: date, end_date: date | None = None
     ) -> MarketPrices:
         """Get market prices."""
         query_data = {
             "query": """
                 query MarketPrices($startDate: Date!, $endDate: Date!) {
                     marketPricesElectricity(startDate: $startDate, endDate: $endDate) {
                        from till marketPrice marketPriceTax sourcingMarkupPrice energyTaxPrice
@@ -191,14 +191,44 @@
             """,
             "variables": {"startDate": str(start_date), "endDate": str(end_date)},
             "operationName": "MarketPrices",
         }
 
         return MarketPrices.from_dict(await self._query(query_data))
 
+    async def userPrices(self, start_date: date) -> MarketPrices:
+        """Get customer market prices."""
+        if self._auth is None:
+            raise AuthRequiredException
+
+        query_data = {
+            "query": """
+                query CustomerMarketPrices($date: String!) {
+                    customerMarketPrices(date: $date) {
+                        electricityPrices {
+                            from till marketPrice marketPriceTax
+                            sourcingMarkupPrice: consumptionSourcingMarkupPrice
+                            energyTaxPrice: energyTax
+                        }
+                        gasPrices {
+                            from till marketPrice marketPriceTax
+                            sourcingMarkupPrice: consumptionSourcingMarkupPrice
+                            energyTaxPrice: energyTax
+                        }
+                    }
+                }
+            """,
+            "variables": {"date": str(start_date)},
+            "operationName": "CustomerMarketPrices",
+        }
+
+        result = await self._query(query_data)
+
+        return MarketPrices.from_userprices_dict(result)
+
     @property
     def is_authenticated(self) -> bool:
         """Return if client is authenticated.
 
         Does not actually check if the token is valid.
         """
         return self._auth is not None
```

### Comparing `python_frank_energie-4.0.3/python_frank_energie/models.py` & `python_frank_energie-4.1.0/python_frank_energie/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,7 +317,29 @@
         if not payload:
             raise RequestException("Unexpected response")
 
         return MarketPrices(
             electricity=PriceData(payload.get("marketPricesElectricity")),
             gas=PriceData(payload.get("marketPricesGas")),
         )
+
+    @staticmethod
+    def from_userprices_dict(data: dict[str, str]) -> MarketPrices:
+        """Parse the response from the marketPrices query."""
+        _LOGGER.debug("Prices %s", data)
+
+        if errors := data.get("errors"):
+            if errors[0]["message"].startswith("No marketprices found for segment"):
+                return MarketPrices(PriceData(), PriceData())
+
+            raise RequestException(errors[0]["message"])
+
+        payload = data.get("data")
+        if not payload:
+            raise RequestException("Unexpected response")
+
+        customerMarketPrices = payload.get("customerMarketPrices")
+
+        return MarketPrices(
+            electricity=PriceData(customerMarketPrices.get("electricityPrices")),
+            gas=PriceData(customerMarketPrices.get("gasPrices")),
+        )
```

### Comparing `python_frank_energie-4.0.3/PKG-INFO` & `python_frank_energie-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 4.0.3
+Version: 4.1.0
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

