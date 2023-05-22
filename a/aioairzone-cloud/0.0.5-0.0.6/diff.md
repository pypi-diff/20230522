# Comparing `tmp/aioairzone-cloud-0.0.5.tar.gz` & `tmp/aioairzone-cloud-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.0.5.tar", last modified: Sun May 21 08:37:26 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.0.6.tar", last modified: Mon May 22 13:44:31 2023, max compression
```

## Comparing `aioairzone-cloud-0.0.5.tar` & `aioairzone-cloud-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.5/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.5/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.5/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    15463 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     5888 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.5/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-21 08:37:26.000000 aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-21 08:35:30.000000 aioairzone-cloud-0.0.5/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.5/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-21 08:37:26.532835 aioairzone-cloud-0.0.5/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 13:44:31.361388 aioairzone-cloud-0.0.6/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.6/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.6/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 13:44:31.361388 aioairzone-cloud-0.0.6/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      320 2023-05-18 08:06:51.000000 aioairzone-cloud-0.0.6/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 13:44:31.361388 aioairzone-cloud-0.0.6/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16696 2023-05-22 13:41:38.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2022-04-06 15:45:16.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6167 2023-05-22 13:41:38.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3040 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1184 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      401 2022-04-06 19:37:08.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     3791 2023-05-19 11:19:38.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18130 2023-05-21 08:34:57.000000 aioairzone-cloud-0.0.6/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-22 13:44:31.361388 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1102 2023-05-22 13:44:31.000000 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      593 2023-05-22 13:44:31.000000 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 13:44:31.000000 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-22 13:44:31.000000 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-22 13:44:31.000000 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-22 13:44:31.000000 aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      963 2023-05-22 13:43:36.000000 aioairzone-cloud-0.0.6/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.0.6/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-22 13:44:31.365388 aioairzone-cloud-0.0.6/setup.cfg
```

### Comparing `aioairzone-cloud-0.0.5/LICENSE` & `aioairzone-cloud-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/PKG-INFO` & `aioairzone-cloud-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/cloudapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,20 @@
     AZD_INSTALLATIONS,
     AZD_SYSTEMS,
     AZD_WEBSERVERS,
     AZD_ZONES,
     HEADER_AUTHORIZATION,
     HEADER_BEARER,
     HTTP_CALL_TIMEOUT,
+    RAW_DEVICES_CONFIG,
+    RAW_DEVICES_STATUS,
+    RAW_INSTALLATIONS,
+    RAW_INSTALLATIONS_LIST,
+    RAW_USER,
+    RAW_WEBSERVERS,
     TOKEN_REFRESH_PERIOD,
 )
 from .device import Device
 from .exceptions import (
     AirzoneCloudError,
     APIError,
     AuthError,
@@ -65,14 +71,20 @@
 
     def __init__(
         self,
         aiohttp_session: ClientSession,
         options: ConnectionOptions,
     ):
         """Airzone Cloud API init."""
+        self._api_raw_data: dict[str, Any] = {
+            RAW_DEVICES_CONFIG: {},
+            RAW_DEVICES_STATUS: {},
+            RAW_INSTALLATIONS: {},
+            RAW_WEBSERVERS: {},
+        }
         self.aiohttp_session = aiohttp_session
         self.installations: list[Installation] = []
         self.options = options
         self.refresh_time: datetime
         self.refresh_token: str | None = None
         self.systems: list[System] = []
         self.token: str | None = None
@@ -118,79 +130,102 @@
         resp_json = await resp.json(content_type=None)
         _LOGGER.debug("aiohttp response: %s", resp_json)
 
         return cast(dict[str, Any], resp_json)
 
     async def api_get_device_config(self, device: Device) -> dict[str, Any]:
         """Request API device config data."""
-        dev_id = urllib.parse.quote(device.get_id())
+        dev_id = device.get_id()
+        url_id = urllib.parse.quote(dev_id)
 
         params = {
             API_INSTALLATION_ID: device.get_installation(),
         }
         dev_params = urllib.parse.urlencode(params)
 
-        return await self.api_request(
+        res = await self.api_request(
             "GET",
-            f"{API_V1}/{API_DEVICES}/{dev_id}/{API_CONFIG}?{dev_params}",
+            f"{API_V1}/{API_DEVICES}/{url_id}/{API_CONFIG}?{dev_params}",
         )
+        self._api_raw_data[RAW_DEVICES_CONFIG][dev_id] = res
+
+        return res
 
     async def api_get_device_status(self, device: Device) -> dict[str, Any]:
         """Request API device status data."""
-        dev_id = urllib.parse.quote(device.get_id())
+        dev_id = device.get_id()
+        url_id = urllib.parse.quote(dev_id)
 
         params = {
             API_INSTALLATION_ID: device.get_installation(),
         }
         dev_params = urllib.parse.urlencode(params)
 
-        return await self.api_request(
+        res = await self.api_request(
             "GET",
-            f"{API_V1}/{API_DEVICES}/{dev_id}/{API_STATUS}?{dev_params}",
+            f"{API_V1}/{API_DEVICES}/{url_id}/{API_STATUS}?{dev_params}",
         )
+        self._api_raw_data[RAW_DEVICES_STATUS][dev_id] = res
+
+        return res
 
     async def api_get_installation(self, installation: Installation) -> dict[str, Any]:
         """Request API installation data."""
-        inst_id = urllib.parse.quote(installation.get_id())
-        return await self.api_request(
+        inst_id = installation.get_id()
+        url_id = urllib.parse.quote(inst_id)
+
+        res = await self.api_request(
             "GET",
-            f"{API_V1}/{API_INSTALLATIONS}/{inst_id}",
+            f"{API_V1}/{API_INSTALLATIONS}/{url_id}",
         )
+        self._api_raw_data[RAW_INSTALLATIONS][inst_id] = res
+
+        return res
 
     async def api_get_installations(self) -> dict[str, Any]:
         """Request API installations data."""
-        return await self.api_request(
+        res = await self.api_request(
             "GET",
             f"{API_V1}/{API_INSTALLATIONS}",
         )
+        self._api_raw_data[RAW_INSTALLATIONS_LIST] = res
+
+        return res
 
     async def api_get_user(self) -> dict[str, Any]:
         """Request API user data."""
-        return await self.api_request(
+        res = await self.api_request(
             "GET",
             f"{API_V1}/{API_USER}",
         )
+        self._api_raw_data[RAW_USER] = res
+
+        return res
 
     async def api_get_webserver(
         self, webserver: WebServer, devices: bool
     ) -> dict[str, Any]:
         """Request API webserver data."""
-        ws_id = urllib.parse.quote(webserver.get_id())
+        ws_id = webserver.get_id()
+        url_id = urllib.parse.quote(ws_id)
 
         params: dict[str, Any] = {
             API_INSTALLATION_ID: webserver.get_installation(),
         }
         if devices:
             params[API_DEVICES] = 1
         ws_params = urllib.parse.urlencode(params)
 
-        return await self.api_request(
+        res = await self.api_request(
             "GET",
-            f"{API_V1}/{API_DEVICES}/{API_WS}/{ws_id}/{API_STATUS}?{ws_params}",
+            f"{API_V1}/{API_DEVICES}/{API_WS}/{url_id}/{API_STATUS}?{ws_params}",
         )
+        self._api_raw_data[RAW_WEBSERVERS][ws_id] = res
+
+        return res
 
     async def login(self) -> None:
         """Perform Airzone Cloud API login."""
         if self.token:
             await self.logout()
         resp = await self.api_request(
             "POST",
@@ -231,14 +266,18 @@
             )
             _LOGGER.debug("refresh resp: %s", resp)
             if resp.keys() < {API_TOKEN, API_REFRESH_TOKEN}:
                 raise TokenRefreshError("Invalid API response")
             self.token = resp[API_TOKEN]
             self.refresh_token = resp[API_REFRESH_TOKEN]
 
+    def raw_data(self) -> dict[str, Any]:
+        """Return raw Airzone Cloud API data."""
+        return self._api_raw_data
+
     def data(self) -> dict[str, Any]:
         """Return Airzone Cloud data."""
         data: dict[str, Any] = {}
 
         if self.installations:
             installations: dict[str, Any] = {}
             for installation in self.installations:
@@ -368,16 +407,21 @@
         """Update Airzone Cloud System by ID."""
         system = self.get_system_id(sys_id)
         if system:
             await self.update_system(system)
 
     async def update_systems(self) -> None:
         """Update all Airzone Cloud Systems."""
+        tasks = []
+
         for system in self.systems:
-            await self.update_system(system)
+            tasks += [self.update_system(system)]
+
+        for task in tasks:
+            await task
 
     async def update_webserver(self, ws: WebServer, devices: bool) -> None:
         """Update Airzone Cloud WebServer from API."""
         ws_data = await self.api_get_webserver(ws, devices)
         ws.update(ws_data)
         if devices:
             for device_data in ws_data[API_DEVICES]:
@@ -396,32 +440,42 @@
         """Update Airzone Cloud WebServer by ID."""
         ws = self.get_webserver_id(ws_id)
         if ws:
             await self.update_webserver(ws, devices)
 
     async def update_webservers(self, devices: bool) -> None:
         """Update all Airzone Cloud WebServers."""
+        tasks = []
+
         for ws in self.webservers:
-            await self.update_webserver(ws, devices)
+            tasks += [self.update_webserver(ws, devices)]
+
+        for task in tasks:
+            await task
 
     async def update_zone(self, zone: Zone) -> None:
         """Update Airzone Cloud Zone from API."""
         device_data = await self.api_get_device_status(zone)
         zone.update(device_data)
 
     async def update_zone_id(self, zone_id: str) -> None:
         """Update Airzone Cloud Zone by ID."""
         zone = self.get_zone_id(zone_id)
         if zone:
             await self.update_zone(zone)
 
     async def update_zones(self) -> None:
         """Update all Airzone Cloud Zones."""
+        tasks = []
+
         for zone in self.zones:
-            await self.update_zone(zone)
+            tasks += [self.update_zone(zone)]
+
+        for task in tasks:
+            await task
 
         for system in self.systems:
             self.set_system_zones_data(system)
 
     async def _update(self) -> None:
         tasks = [
             self.update_webservers(False),
```

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/common.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/const.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,8 +127,15 @@
 AZD_ZONES: Final[str] = "zones"
 
 HEADER_AUTHORIZATION: Final[str] = "Authorization"
 HEADER_BEARER: Final[str] = "Bearer"
 
 HTTP_CALL_TIMEOUT: Final[int] = 10
 
+RAW_DEVICES_CONFIG: Final[str] = "devices-config"
+RAW_DEVICES_STATUS: Final[str] = "devices-status"
+RAW_INSTALLATIONS: Final[str] = "installations"
+RAW_INSTALLATIONS_LIST: Final[str] = "installations-list"
+RAW_USER: Final[str] = "user"
+RAW_WEBSERVERS: Final[str] = "webservers"
+
 TOKEN_REFRESH_PERIOD: Final[timedelta] = timedelta(hours=12)
```

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/device.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/device.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/webserver.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.0.6/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.0.5/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.0.6/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.0.5/pyproject.toml` & `aioairzone-cloud-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.0.5"
+version = "0.0.6"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

