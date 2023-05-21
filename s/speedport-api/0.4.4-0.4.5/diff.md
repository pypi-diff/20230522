# Comparing `tmp/speedport-api-0.4.4.tar.gz` & `tmp/speedport-api-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedport-api-0.4.4.tar", last modified: Wed Feb  1 20:42:35 2023, max compression
+gzip compressed data, was "speedport-api-0.4.5.tar", last modified: Sun May 21 23:34:30 2023, max compression
```

## Comparing `speedport-api-0.4.4.tar` & `speedport-api-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:42:35.125563 speedport-api-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-01 20:42:18.000000 speedport-api-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-01 20:42:35.125563 speedport-api-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-02-01 20:42:18.000000 speedport-api-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 20:42:35.125563 speedport-api-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-01 20:42:18.000000 speedport-api-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:42:35.125563 speedport-api-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:42:35.125563 speedport-api-0.4.4/src/speedport/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-01 20:42:18.000000 speedport-api-0.4.4/src/speedport/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5844 2023-02-01 20:42:18.000000 speedport-api-0.4.4/src/speedport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-01 20:42:18.000000 speedport-api-0.4.4/src/speedport/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    10248 2023-02-01 20:42:18.000000 speedport-api-0.4.4/src/speedport/speedport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:42:35.125563 speedport-api-0.4.4/src/speedport_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-01 20:42:35.000000 speedport-api-0.4.4/src/speedport_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-01 20:42:35.000000 speedport-api-0.4.4/src/speedport_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:42:35.000000 speedport-api-0.4.4/src/speedport_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-01 20:42:35.000000 speedport-api-0.4.4/src/speedport_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-01 20:42:35.000000 speedport-api-0.4.4/src/speedport_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-01 20:42:35.000000 speedport-api-0.4.4/src/speedport_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.635834 speedport-api-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-21 23:34:19.000000 speedport-api-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 23:34:30.635834 speedport-api-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 23:34:19.000000 speedport-api-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:34:30.635834 speedport-api-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-21 23:34:19.000000 speedport-api-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.631833 speedport-api-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.635834 speedport-api-0.4.5/src/speedport/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5844 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-05-21 23:34:19.000000 speedport-api-0.4.5/src/speedport/speedport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:34:30.635834 speedport-api-0.4.5/src/speedport_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 23:34:30.000000 speedport-api-0.4.5/src/speedport_api.egg-info/top_level.txt
```

### Comparing `speedport-api-0.4.4/LICENSE` & `speedport-api-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.4/PKG-INFO` & `speedport-api-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedport-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: Control Telekom Speedport routers with Python
 Home-page: https://github.com/Andre0512/speedport-api
 Author: Andre Basche
 License: MIT
 Platform: any
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `speedport-api-0.4.4/README.md` & `speedport-api-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.4/setup.py` & `speedport-api-0.4.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="speedport-api",
-    version="0.4.4",
+    version="0.4.5",
     author="Andre Basche",
     description="Control Telekom Speedport routers with Python",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/Andre0512/speedport-api",
     license="MIT",
     platforms="any",
```

### Comparing `speedport-api-0.4.4/src/speedport/__main__.py` & `speedport-api-0.4.5/src/speedport/__main__.py`

 * *Files identical despite different names*

### Comparing `speedport-api-0.4.4/src/speedport/device.py` & `speedport-api-0.4.5/src/speedport/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     @property
     def slave(self):
         return bool(int(self._data.get("mdevice_slave") or "0"))
 
     @property
     def type(self):
-        return ["lan", "wlan", "wlan5"][int(self._data.get("mdevice_type"))]
+        return ["lan", "wlan", "wlan5"][int(self._data.get("mdevice_type", "0")) % 3]
 
     @property
     def ula_ipv6(self):
         return self._data.get("mdevice_ula_ipv6")
 
     @property
     def upspeed(self):
```

### Comparing `speedport-api-0.4.4/src/speedport/speedport.py` & `speedport-api-0.4.5/src/speedport/speedport.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,16 @@
     @property
     async def status(self):
         return await self.get("data/Status.json")
 
     @property
     async def devices(self):
         data = await self.get("data/DeviceList.json")
-        devices = data.get("addmlandevice", []) + data.get("addmwlan5device", []) + data.get("addmwlandevice", [])
+        devices = data.get("addmlandevice", []) + data.get("addmwlan5device", [])
+        devices += data.get("addmwlandevice", []) + data.get("addmdevice", [])
         devices = sorted(devices, key=lambda d: int(d["mdevice_ipv4"].split(".")[-1]))
         return [WlanDevice(device) for device in devices]
 
     @staticmethod
     def need_auth(func):
         @functools.wraps(func)
         async def inner(self):
```

### Comparing `speedport-api-0.4.4/src/speedport_api.egg-info/PKG-INFO` & `speedport-api-0.4.5/src/speedport_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedport-api
-Version: 0.4.4
+Version: 0.4.5
 Summary: Control Telekom Speedport routers with Python
 Home-page: https://github.com/Andre0512/speedport-api
 Author: Andre Basche
 License: MIT
 Platform: any
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

