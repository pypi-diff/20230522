# Comparing `tmp/aioairzone-cloud-0.0.7.tar.gz` & `tmp/aioairzone-cloud-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.0.7.tar", last modified: Mon May 22 14:18:34 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.0.tar", last modified: Mon May 22 17:29:23 2023, max compression
```

## Comparing `aioairzone-cloud-0.0.7.tar` & `aioairzone-cloud-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 14:18:34.499355 aioairzone-cloud-0.0.7/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.7/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.7/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 14:18:34.499355 aioairzone-cloud-0.0.7/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.7/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 14:18:34.499355 aioairzone-cloud-0.0.7/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16696 2023-05-22 13:41:38.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-22 13:41:38.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.7/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 14:18:34.499355 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 14:18:34.000000 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-22 14:18:34.000000 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 14:18:34.000000 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 14:18:34.000000 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-22 14:18:34.000000 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-22 14:18:34.000000 aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-22 14:17:47.000000 aioairzone-cloud-0.0.7/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.7/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-22 14:18:34.499355 aioairzone-cloud-0.0.7/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.0/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.0/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.1.0/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16659 2023-05-22 17:23:29.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-22 13:41:38.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.0/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      619 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-22 17:29:23.000000 aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-22 17:27:48.000000 aioairzone-cloud-0.1.0/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.0/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-22 17:29:23.858698 aioairzone-cloud-0.1.0/setup.cfg
```

### Comparing `aioairzone-cloud-0.0.7/LICENSE` & `aioairzone-cloud-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/PKG-INFO` & `aioairzone-cloud-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.7
+Version: 0.1.0
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/cloudapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Airzone Cloud API."""
 from __future__ import annotations
 
+import asyncio
 import logging
 import urllib.parse
 from datetime import datetime
 from typing import Any, cast
 
 from aiohttp import ClientConnectorError, ClientResponseError, ClientSession
 from aiohttp.client_reqrep import ClientResponse
@@ -412,16 +413,15 @@
     async def update_systems(self) -> None:
         """Update all Airzone Cloud Systems."""
         tasks = []
 
         for system in self.systems:
             tasks += [self.update_system(system)]
 
-        for task in tasks:
-            await task
+        await asyncio.gather(*tasks)
 
     async def update_webserver(self, ws: WebServer, devices: bool) -> None:
         """Update Airzone Cloud WebServer from API."""
         ws_data = await self.api_get_webserver(ws, devices)
         ws.update(ws_data)
         if devices:
             for device_data in ws_data[API_DEVICES]:
@@ -445,16 +445,15 @@
     async def update_webservers(self, devices: bool) -> None:
         """Update all Airzone Cloud WebServers."""
         tasks = []
 
         for ws in self.webservers:
             tasks += [self.update_webserver(ws, devices)]
 
-        for task in tasks:
-            await task
+        await asyncio.gather(*tasks)
 
     async def update_zone(self, zone: Zone) -> None:
         """Update Airzone Cloud Zone from API."""
         device_data = await self.api_get_device_status(zone)
         zone.update(device_data)
 
     async def update_zone_id(self, zone_id: str) -> None:
@@ -466,29 +465,27 @@
     async def update_zones(self) -> None:
         """Update all Airzone Cloud Zones."""
         tasks = []
 
         for zone in self.zones:
             tasks += [self.update_zone(zone)]
 
-        for task in tasks:
-            await task
+        await asyncio.gather(*tasks)
 
         for system in self.systems:
             self.set_system_zones_data(system)
 
     async def _update(self) -> None:
         tasks = [
             self.update_webservers(False),
             self.update_systems(),
             self.update_zones(),
         ]
 
-        for task in tasks:
-            await task
+        await asyncio.gather(*tasks)
 
     async def update(self) -> None:
         """Update all Airzone Cloud data."""
 
         if (datetime.now() - self.refresh_time) > TOKEN_REFRESH_PERIOD:
             try:
                 await self.token_refresh()
```

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.0/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.7
+Version: 0.1.0
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.7/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.0/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.7/pyproject.toml` & `aioairzone-cloud-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.0.7"
+version = "0.1.0"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

