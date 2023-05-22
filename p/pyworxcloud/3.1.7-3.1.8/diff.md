# Comparing `tmp/pyworxcloud-3.1.7.tar.gz` & `tmp/pyworxcloud-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.1.7.tar", max compression
+gzip compressed data, was "pyworxcloud-3.1.8.tar", max compression
```

## Comparing `pyworxcloud-3.1.7.tar` & `pyworxcloud-3.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/LICENSE
--rw-r--r--   0        0        0      929 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/README.md
--rw-r--r--   0        0        0      609 2023-05-17 09:07:59.121128 pyworxcloud-3.1.7/pyproject.toml
--rw-r--r--   0        0        0    29618 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     4804 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-05-17 09:07:41.993154 pyworxcloud-3.1.7/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/events.py
--rw-r--r--   0        0        0     2115 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3623 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     8300 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     3188 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6191 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1763 2023-05-17 09:07:41.997154 pyworxcloud-3.1.7/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 pyworxcloud-3.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/LICENSE
+-rw-r--r--   0        0        0      929 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/README.md
+-rw-r--r--   0        0        0      609 2023-05-22 06:38:59.128650 pyworxcloud-3.1.8/pyproject.toml
+-rw-r--r--   0        0        0    29688 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     4804 2023-05-22 06:38:43.036491 pyworxcloud-3.1.8/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/events.py
+-rw-r--r--   0        0        0     2115 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3623 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     8300 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     3188 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6191 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     2116 2023-05-22 06:38:43.040491 pyworxcloud-3.1.8/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1747 1970-01-01 00:00:00.000000 pyworxcloud-3.1.8/PKG-INFO
```

### Comparing `pyworxcloud-3.1.7/LICENSE` & `pyworxcloud-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/README.md` & `pyworxcloud-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyproject.toml` & `pyworxcloud-3.1.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.1.7"
+version = "v3.1.8"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pyworxcloud-3.1.7/pyworxcloud/__init__.py` & `pyworxcloud-3.1.8/pyworxcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,15 +513,17 @@
         self._mowers = self._api.get_mowers()
 
         for mower in self._mowers:
             device = DeviceHandler(self._api, mower)
             _LOGGER.debug("Mower '%s' data: %s", mower["name"], mower)
             self.devices.update({mower["name"]: device})
 
-            device.raw_data = mower["last_status"]["payload"]
+            if not isinstance(mower["last_status"], type(None)):
+                device.raw_data = mower["last_status"]["payload"]
+
             self._decode_data(device)
 
     def get_mower(self, serial_number: str) -> dict:
         """Get a specific mower."""
         for mower in self._mowers:
             if mower["serial_number"] == serial_number:
                 return mower
```

### Comparing `pyworxcloud-3.1.7/pyworxcloud/api.py` & `pyworxcloud-3.1.8/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/clouds.py` & `pyworxcloud-3.1.8/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/const.py` & `pyworxcloud-3.1.8/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/events.py` & `pyworxcloud-3.1.8/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/exceptions.py` & `pyworxcloud-3.1.8/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.1.8/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.1.8/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/battery.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/blades.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/capability.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/devices.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/product.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/requests.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/state.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.1.7/pyworxcloud/utils/zone.py` & `pyworxcloud-3.1.8/pyworxcloud/utils/zone.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,29 @@
         self["index"] = None
         self["indicies"] = [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
         self["starting_point"] = [0, 0, 0, 0]
 
         if not "last_status" in data:
             return
 
-        self["index"] = data["last_status"]["payload"]["dat"]["lz"]
-        self["indicies"] = data["last_status"]["payload"]["cfg"]["mzv"]
-        self["starting_point"] = data["last_status"]["payload"]["cfg"]["mz"]
+        self["index"] = (
+            data["last_status"]["payload"]["dat"]["lz"]
+            if "lz" in data["last_status"]["payload"]["dat"]
+            else 0
+        )
+        self["indicies"] = (
+            data["last_status"]["payload"]["cfg"]["mzv"]
+            if "mzv" in data["last_status"]["payload"]["dat"]
+            else [0, 0, 0, 0, 0, 0, 0, 0, 0, 0]
+        )
+        self["starting_point"] = (
+            data["last_status"]["payload"]["cfg"]["mz"]
+            if "mz" in data["last_status"]["payload"]["dat"]
+            else [0, 0, 0, 0]
+        )
         self["current"] = self["indicies"][self["index"]]
 
     @property
     def current(self) -> int:
         """Get current zone."""
         return self["current"]
```

### Comparing `pyworxcloud-3.1.7/PKG-INFO` & `pyworxcloud-3.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.1.7
+Version: 3.1.8
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.7 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.1.8 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Dist:
 paho-mqtt (>=1.6.1,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-
```

