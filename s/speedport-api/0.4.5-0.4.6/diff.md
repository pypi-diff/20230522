# Comparing `tmp/speedport-api-0.4.5.tar.gz` & `tmp/speedport-api-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedport-api-0.4.5.tar", last modified: Sun May 21 23:34:30 2023, max compression
+gzip compressed data, was "speedport-api-0.4.6.tar", last modified: Sun May 21 23:56:23 2023, max compression
```

## Comparing `speedport-api-0.4.5.tar` & `speedport-api-0.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.635834 speedport-api-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-21 23:34:19.000000 speedport-api-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 23:34:30.635834 speedport-api-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 23:34:19.000000 speedport-api-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:34:30.635834 speedport-api-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-21 23:34:19.000000 speedport-api-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.631833 speedport-api-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.635834 speedport-api-0.4.5/src/speedport/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5844 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/speedport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.635834 speedport-api-0.4.5/src/speedport_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:23.591475 speedport-api-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-21 23:56:10.000000 speedport-api-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 23:56:23.591475 speedport-api-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 23:56:10.000000 speedport-api-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:56:23.591475 speedport-api-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-21 23:56:10.000000 speedport-api-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:23.587475 speedport-api-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:23.587475 speedport-api-0.4.6/src/speedport/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 23:56:10.000000 speedport-api-0.4.6/src/speedport/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5844 2023-05-21 23:56:10.000000 speedport-api-0.4.6/src/speedport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-21 23:56:10.000000 speedport-api-0.4.6/src/speedport/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-05-21 23:56:10.000000 speedport-api-0.4.6/src/speedport/speedport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:56:23.591475 speedport-api-0.4.6/src/speedport_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 23:56:23.000000 speedport-api-0.4.6/src/speedport_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-21 23:56:23.000000 speedport-api-0.4.6/src/speedport_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:56:23.000000 speedport-api-0.4.6/src/speedport_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 23:56:23.000000 speedport-api-0.4.6/src/speedport_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 23:56:23.000000 speedport-api-0.4.6/src/speedport_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 23:56:23.000000 speedport-api-0.4.6/src/speedport_api.egg-info/top_level.txt
```

### Comparing `speedport-api-0.4.5/LICENSE` & `speedport-api-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.5/PKG-INFO` & `speedport-api-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedport-api
-Version: 0.4.5
+Version: 0.4.6
 Summary: Control Telekom Speedport routers with Python
 Home-page: https://github.com/Andre0512/speedport-api
 Author: Andre Basche
 License: MIT
 Platform: any
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `speedport-api-0.4.5/README.md` & `speedport-api-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.5/setup.py` & `speedport-api-0.4.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="speedport-api",
-    version="0.4.5",
+    version="0.4.6",
     author="Andre Basche",
     description="Control Telekom Speedport routers with Python",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/Andre0512/speedport-api",
     license="MIT",
     platforms="any",
```

### Comparing `speedport-api-0.4.5/src/speedport/__main__.py` & `speedport-api-0.4.6/src/speedport/__main__.py`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.5/src/speedport/device.py` & `speedport-api-0.4.6/src/speedport/device.py`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.5/src/speedport/speedport.py` & `speedport-api-0.4.6/src/speedport/speedport.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,25 @@
 
 from .device import WlanDevice
 
 _LOGGER = logging.getLogger(__name__)
 _LOGGER.setLevel(logging.WARNING)
 
 
+def need_auth(func):
+    @functools.wraps(func)
+    async def inner(self):
+        if not self._login_key:
+            _LOGGER.error("You need to login!")
+            raise PermissionError("You need to login!")
+        return await func(self)
+
+    return inner
+
+
 class Speedport:
     def __init__(self, host="speedport.ip", https=False):
         # Is this the default key for everyone or should we parse it?
         self._default_key = "cdc0cac1280b516e674f0057e4929bca84447cca8425007e33a88a5cf598a190"
         self._login_password = ""
         self._login_key = ""
         self._cookies = {}
@@ -110,25 +121,14 @@
     async def devices(self):
         data = await self.get("data/DeviceList.json")
         devices = data.get("addmlandevice", []) + data.get("addmwlan5device", [])
         devices += data.get("addmwlandevice", []) + data.get("addmdevice", [])
         devices = sorted(devices, key=lambda d: int(d["mdevice_ipv4"].split(".")[-1]))
         return [WlanDevice(device) for device in devices]
 
-    @staticmethod
-    def need_auth(func):
-        @functools.wraps(func)
-        async def inner(self):
-            if not self._login_key:
-                _LOGGER.error("You need to login!")
-                raise PermissionError("You need to login!")
-            return await func(self)
-
-        return inner
-
     @property
     @need_auth
     async def ip_data(self):
         referer = "html/content/internet/con_ipdata.html"
         return await self.get(f"data/IPData.json", referer=referer, auth=True)
 
     @property
```

### Comparing `speedport-api-0.4.5/src/speedport_api.egg-info/PKG-INFO` & `speedport-api-0.4.6/src/speedport_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedport-api
-Version: 0.4.5
+Version: 0.4.6
 Summary: Control Telekom Speedport routers with Python
 Home-page: https://github.com/Andre0512/speedport-api
 Author: Andre Basche
 License: MIT
 Platform: any
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

