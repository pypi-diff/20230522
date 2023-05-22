# Comparing `tmp/zwave_me_ws-0.4.2.tar.gz` & `tmp/zwave_me_ws-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zwave_me_ws-0.4.2.tar", max compression
+gzip compressed data, was "zwave_me_ws-0.4.3.tar", max compression
```

## Comparing `zwave_me_ws-0.4.2.tar` & `zwave_me_ws-0.4.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      536 2023-04-08 08:17:24.212857 zwave_me_ws-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1718 2023-02-02 09:31:19.285701 zwave_me_ws-0.4.2/README.md
--rw-r--r--   0        0        0       87 2023-04-08 08:17:24.223138 zwave_me_ws-0.4.2/zwave_me_ws/__init__.py
--rw-r--r--   0        0        0     8783 2023-04-08 08:17:16.692577 zwave_me_ws-0.4.2/zwave_me_ws/helpers.py
--rw-r--r--   0        0        0     1679 2023-02-02 09:31:19.286697 zwave_me_ws-0.4.2/zwave_me_ws/WebsocketListener.py
--rw-r--r--   0        0        0     8077 2023-04-08 07:24:35.214015 zwave_me_ws-0.4.2/zwave_me_ws/ZWaveMe.py
--rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 zwave_me_ws-0.4.2/setup.py
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 zwave_me_ws-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      536 2023-05-22 09:47:49.289056 zwave_me_ws-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1718 2023-05-16 10:02:16.858312 zwave_me_ws-0.4.3/README.md
+-rw-r--r--   0        0        0       87 2023-05-22 09:47:49.266634 zwave_me_ws-0.4.3/zwave_me_ws/__init__.py
+-rw-r--r--   0        0        0     9206 2023-05-22 09:47:23.599938 zwave_me_ws-0.4.3/zwave_me_ws/helpers.py
+-rw-r--r--   0        0        0     1679 2023-05-16 10:02:16.860377 zwave_me_ws-0.4.3/zwave_me_ws/WebsocketListener.py
+-rw-r--r--   0        0        0     8077 2023-05-16 10:02:16.860377 zwave_me_ws-0.4.3/zwave_me_ws/ZWaveMe.py
+-rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 zwave_me_ws-0.4.3/PKG-INFO
```

### Comparing `zwave_me_ws-0.4.2/pyproject.toml` & `zwave_me_ws-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zwave_me_ws"
-version = "0.4.2"
+version = "0.4.3"
 description = "Library, implementing websocket connection to ZWave-Me"
 authors = ["Dmitry Vlasov <kerbalspacema@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/Z-Wave-Me/zwave-me-ws"
 readme = 'README.md'
 
 [tool.poetry.dependencies]
```

### Comparing `zwave_me_ws-0.4.2/README.md` & `zwave_me_ws-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `zwave_me_ws-0.4.2/zwave_me_ws/helpers.py` & `zwave_me_ws-0.4.3/zwave_me_ws/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,24 @@
                 prepared_device = set_value_by_device_type(prepared_device)
                 return prepared_device
     if prepared_device["probeType"] == "motor":
         prepared_device["deviceType"] = "motor"
     elif prepared_device["probeType"] == "fan":
         prepared_device["deviceType"] = "fan"
     elif prepared_device['deviceType'] == 'sensorMultilevel':
-        prepared_device['deviceType'] = 'lightMultilivel'
+        if prepared_device["probeType"] == "light":
+            prepared_device['deviceType'] = 'lightMultilevel'
+            prepared_device = set_light_level(prepared_device)
+    elif prepared_device['deviceType'] == 'switchMultilevel':
+        prepared_device['deviceType'] = 'lightMultilevel'
         prepared_device = set_light_level(prepared_device)
+    elif 'alarm' in prepared_device["probeType"]:
+        prepared_device["deviceType"] = "sensorBinary"
+        prepared_device = set_value_by_device_type(prepared_device)
+
     return prepared_device
 
 
 def set_value_by_device_type(prepared_device) -> dict:
     if prepared_device['deviceType'] == "sensorBinary":
         if prepared_device['level'] in ('on', 'off'):
             return prepared_device
@@ -217,8 +225,8 @@
             }
         elif prepared_device['level'] == 'off':
             prepared_device["color"] = {
                 "r": 0,
                 "g": 0,
                 "b": 0,
             }
-    return prepared_device
+    return prepared_device
```

### Comparing `zwave_me_ws-0.4.2/zwave_me_ws/WebsocketListener.py` & `zwave_me_ws-0.4.3/zwave_me_ws/WebsocketListener.py`

 * *Files identical despite different names*

### Comparing `zwave_me_ws-0.4.2/zwave_me_ws/ZWaveMe.py` & `zwave_me_ws-0.4.3/zwave_me_ws/ZWaveMe.py`

 * *Files identical despite different names*

### Comparing `zwave_me_ws-0.4.2/setup.py` & `zwave_me_ws-0.4.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,86 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: zwave-me-ws
+Version: 0.4.3
+Summary: Library, implementing websocket connection to ZWave-Me
+Home-page: https://github.com/Z-Wave-Me/zwave-me-ws
+License: MIT
+Author: Dmitry Vlasov
+Author-email: kerbalspacema@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: websocket-client (>=1.2.1,<2.0.0)
+Project-URL: Repository, https://github.com/Z-Wave-Me/zwave-me-ws
+Description-Content-Type: text/markdown
+
+ZWave-Me-WS is a websocket connection library for [Z-Wave.Me Z-Way](https://z-wave.me/z-way/) controllers
+
+**Installing**
+
+To install this package use:
+
+`pip install zwave-me-ws`
+
+**Usage**
+
+To use the connector initialize the API using:
+
+```
+from zwave_me_ws import ZWaveMe, ZWaveMeData
+
+zwave_api = ZWaveMe(
+  on_device_create=on_device_func
+  on_device_update=on_device_update_func,
+  on_new_device=on_device_add_func,
+  token="....", # Z-Way access token in the form .../... (remote) of /... (local)
+  url="...", # wss://find.z-wave.me or ws://IP:8083
+  platforms=[...]
+)
+
+def on_device_add_func(self, device: ZWaveMeData)
+
+def on_device_create_func(self, devices: list[ZWaveMeData])
+
+def on_device_update_func(self, new_info: ZWaveMeData)
+```
+
+Here `platforms` is the list of deviceType fields to handle. Used to filter only types supported by your application. For example, 
+`["sensorBinary", "lightMultilevel", "toggleButton", "thermostat", "motor", "fan", "doorlock", "switchMultilevel", "switchBinary", "sensorMultilevel", "siren", "switchRGBW", "switchRGB"]`.
+
+Available functions:
+```
+devices = zwave_api.get_devices()
+
+zwave_api.send_command(device_id, command) # command can be "on", "off", "exact?level=..", "open", "close"
+
+is_connected = zwave_api.get_connection()
+
+zwave_api.close_ws()
+```
+
+Device (ZWaveMeData) has the following fields:
+```
+  id: str
+  deviceType: str
+  title: str
+  level: Union[str, int, float]
+  deviceIdentifier: str
+  probeType: str
+  scaleTitle: str
+  min: str
+  max: str
+  color: dict
+  isFailed: bool
+  locationName: str
+  manufacturer: str
+  firmware: str
+  tags: list[str]
+  nodeId: str
+  creatorId: str
+```
 
-packages = \
-['zwave_me_ws']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.28.1,<3.0.0', 'websocket-client>=1.2.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'zwave-me-ws',
-    'version': '0.4.2',
-    'description': 'Library, implementing websocket connection to ZWave-Me',
-    'long_description': 'ZWave-Me-WS is a websocket connection library for [Z-Wave.Me Z-Way](https://z-wave.me/z-way/) controllers\n\n**Installing**\n\nTo install this package use:\n\n`pip install zwave-me-ws`\n\n**Usage**\n\nTo use the connector initialize the API using:\n\n```\nfrom zwave_me_ws import ZWaveMe, ZWaveMeData\n\nzwave_api = ZWaveMe(\n  on_device_create=on_device_func\n  on_device_update=on_device_update_func,\n  on_new_device=on_device_add_func,\n  token="....", # Z-Way access token in the form .../... (remote) of /... (local)\n  url="...", # wss://find.z-wave.me or ws://IP:8083\n  platforms=[...]\n)\n\ndef on_device_add_func(self, device: ZWaveMeData)\n\ndef on_device_create_func(self, devices: list[ZWaveMeData])\n\ndef on_device_update_func(self, new_info: ZWaveMeData)\n```\n\nHere `platforms` is the list of deviceType fields to handle. Used to filter only types supported by your application. For example, \n`["sensorBinary", "lightMultilevel", "toggleButton", "thermostat", "motor", "fan", "doorlock", "switchMultilevel", "switchBinary", "sensorMultilevel", "siren", "switchRGBW", "switchRGB"]`.\n\nAvailable functions:\n```\ndevices = zwave_api.get_devices()\n\nzwave_api.send_command(device_id, command) # command can be "on", "off", "exact?level=..", "open", "close"\n\nis_connected = zwave_api.get_connection()\n\nzwave_api.close_ws()\n```\n\nDevice (ZWaveMeData) has the following fields:\n```\n  id: str\n  deviceType: str\n  title: str\n  level: Union[str, int, float]\n  deviceIdentifier: str\n  probeType: str\n  scaleTitle: str\n  min: str\n  max: str\n  color: dict\n  isFailed: bool\n  locationName: str\n  manufacturer: str\n  firmware: str\n  tags: list[str]\n  nodeId: str\n  creatorId: str\n```\n',
-    'author': 'Dmitry Vlasov',
-    'author_email': 'kerbalspacema@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Z-Wave-Me/zwave-me-ws',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

