# Comparing `tmp/growmax-1.2.0.tar.gz` & `tmp/growmax-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growmax-1.2.0.tar", last modified: Tue May  2 07:05:33 2023, max compression
+gzip compressed data, was "growmax-1.2.1.tar", last modified: Sun May 21 22:01:45 2023, max compression
```

## Comparing `growmax-1.2.0.tar` & `growmax-1.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.574210 growmax-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-02 07:05:21.000000 growmax-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-02 07:05:33.574210 growmax-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-02 07:05:21.000000 growmax-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 07:05:21.000000 growmax-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 07:05:33.574210 growmax-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.566210 growmax-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/atlas_ph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/import_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/set_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/atlas_ph/uart_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/displays/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/displays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/displays/sh1107.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/displays/ssd1327.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/moisture.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/ntpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/pump.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/routine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/sensors/adafruit_scd4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/sensors/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.574210 growmax-1.2.0/src/growmax/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/displays.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/water.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-02 07:05:21.000000 growmax-1.2.0/src/growmax/utils/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 07:05:33.570210 growmax-1.2.0/src/growmax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 07:05:33.000000 growmax-1.2.0/src/growmax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-21 22:01:34.000000 growmax-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-21 22:01:45.585334 growmax-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-21 22:01:34.000000 growmax-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-21 22:01:34.000000 growmax-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-21 22:01:45.585334 growmax-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.573334 growmax-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.577334 growmax-1.2.1/src/growmax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.577334 growmax-1.2.1/src/growmax/atlas_ph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/import_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/set_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/atlas_ph/uart_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/src/growmax/displays/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/displays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/displays/sh1107.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/displays/ssd1327.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/moisture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/ntpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/routine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/src/growmax/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/sensors/adafruit_scd4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/sensors/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.581334 growmax-1.2.1/src/growmax/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/displays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/water.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-21 22:01:34.000000 growmax-1.2.1/src/growmax/utils/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 22:01:45.577334 growmax-1.2.1/src/growmax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 22:01:45.000000 growmax-1.2.1/src/growmax.egg-info/top_level.txt
```

### Comparing `growmax-1.2.0/LICENSE` & `growmax-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/PKG-INFO` & `growmax-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.0
+Version: 1.2.1
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
@@ -19,15 +19,15 @@
 
 To purchase a Growmax board or four sourcing parts, visit https://opensensor.io
 
 ![Growmax Board install with screen and i2c CO2 sensor](https://github.com/opensensor/growmax/blob/main/images/growmax_install_with_screen.jpg)
 
 
 # Installation
-To install the ``growmax`` package on a Pico or Pico W, first install the appropriate firmware for Micropython that is for your device.
+To install the ``growmax`` package on a Pico or BananaPi Pico (ESP32S3), first install the appropriate firmware for Micropython that is for your device.
 * Pico: https://micropython.org/download/rp2-pico/
 * Pico W:  https://micropython.org/download/rp2-pico-w/
 
 Ensure that you have Thonny IDE installed; for more information visit:  https://thonny.org/
 
 Launch Thonny IDE with your device connected.
```

### Comparing `growmax-1.2.0/README.md` & `growmax-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 To purchase a Growmax board or four sourcing parts, visit https://opensensor.io
 
 ![Growmax Board install with screen and i2c CO2 sensor](https://github.com/opensensor/growmax/blob/main/images/growmax_install_with_screen.jpg)
 
 
 # Installation
-To install the ``growmax`` package on a Pico or Pico W, first install the appropriate firmware for Micropython that is for your device.
+To install the ``growmax`` package on a Pico or BananaPi Pico (ESP32S3), first install the appropriate firmware for Micropython that is for your device.
 * Pico: https://micropython.org/download/rp2-pico/
 * Pico W:  https://micropython.org/download/rp2-pico-w/
 
 Ensure that you have Thonny IDE installed; for more information visit:  https://thonny.org/
 
 Launch Thonny IDE with your device connected.
```

### Comparing `growmax-1.2.0/setup.cfg` & `growmax-1.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = growmax
-version = 1.2.0
+version = 1.2.1
 author = Matt Davis and OpenSensor.io
 author_email = matteius@gmail.com
 description = Micropython routines for automated plant watering and monitoring.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/opensensor/growmax
 project_urls =
```

### Comparing `growmax-1.2.0/src/growmax/atlas_ph/calibration.py` & `growmax-1.2.1/src/growmax/atlas_ph/calibration.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/atlas_ph/i2c.py` & `growmax-1.2.1/src/growmax/atlas_ph/i2c.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/config.py` & `growmax-1.2.1/src/growmax/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,7 +44,8 @@
 WIFI_SSID = "SSID"
 WIFI_PASSWORD = ""
 
 # Data collection w/ api.opensensor.io (early alpha testing)
 OPEN_SENSOR_COLLECT_DATA = False
 OPEN_SENSOR_API_KEY = None  # Register your device for a key at https://opensensor.io/members/profile
 DEVICE_NAME = ""
+OPEN_SENSOR_RETRIEVE_COMMANDS = False  # Experimental feature to retrieve commands from the cloud
```

### Comparing `growmax-1.2.0/src/growmax/constants.py` & `growmax-1.2.1/src/growmax/constants.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/displays/sh1107.py` & `growmax-1.2.1/src/growmax/displays/sh1107.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/displays/ssd1327.py` & `growmax-1.2.1/src/growmax/displays/ssd1327.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/moisture.py` & `growmax-1.2.1/src/growmax/moisture.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/ntpclient.py` & `growmax-1.2.1/src/growmax/ntpclient.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/pump.py` & `growmax-1.2.1/src/growmax/pump.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/routine.py` & `growmax-1.2.1/src/growmax/routine.py`

 * *Files 14% similar despite different names*

```diff
@@ -87,14 +87,21 @@
                 "readings": soil_moistures
             }
             if atlas_ph and ph_reading:
                 report_data["pH"] = {
                     "pH": ph_reading
                 }
             api.report_environment_data(report_data)
+        if config.OPEN_SENSOR_RETRIEVE_COMMANDS:
+            command_parts = api.retrieve_command()  # Experimental
+            if command_parts and len(command_parts) == 3 and command_parts[0] == "WATER":
+                print("WATER", command_parts[1], command_parts[2])
+                pos = int(command_parts[1]) - 1
+                duration = int(command_parts[2])
+                pumps[pos].dose(1, duration)
         if scd40x:
             display_scd4x_reading(temp, rh, ppm_carbon_dioxide)
             utime.sleep(3)
         if atlas_ph:
             display_ph_reading(ph_reading)
             utime.sleep(3)
```

### Comparing `growmax-1.2.0/src/growmax/sensors/adafruit_scd4x.py` & `growmax-1.2.1/src/growmax/sensors/adafruit_scd4x.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/sensors/motion.py` & `growmax-1.2.1/src/growmax/sensors/motion.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/utils/api.py` & `growmax-1.2.1/src/growmax/utils/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -49,7 +49,29 @@
             "https://api.opensensor.io/environment/",
             headers=headers,
             data=json.dumps(report_data))
         print(resp.status_code)
         resp.close()
     except Exception as e:
         print(e)
+
+
+def retrieve_command():
+    """ This method requires installing urequests from pypi. """
+    try:
+        import urequests
+        import json
+        time.sleep(1.0)
+        metadata = get_device_metadata()
+        metadata["device_id"] = metadata["device_metadata"]["device_id"]
+        metadata["name"] = metadata["device_metadata"]["name"]
+        metadata["api_key"] = metadata["device_metadata"]["api_key"]
+        resp = urequests.post(
+            "https://api.opensensor.io/command/consume",
+            headers=headers,
+            data=json.dumps(metadata))
+        data = resp.json()
+        if data and data.get("command"):
+            parts = data["command"].split(",")
+            return parts
+    except Exception as e:
+        pass
```

### Comparing `growmax-1.2.0/src/growmax/utils/displays.py` & `growmax-1.2.1/src/growmax/utils/displays.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/utils/sensors.py` & `growmax-1.2.1/src/growmax/utils/sensors.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax/utils/wifi.py` & `growmax-1.2.1/src/growmax/utils/wifi.py`

 * *Files identical despite different names*

### Comparing `growmax-1.2.0/src/growmax.egg-info/PKG-INFO` & `growmax-1.2.1/src/growmax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: growmax
-Version: 1.2.0
+Version: 1.2.1
 Summary: Micropython routines for automated plant watering and monitoring.
 Home-page: https://github.com/opensensor/growmax
 Author: Matt Davis and OpenSensor.io
 Author-email: matteius@gmail.com
 Project-URL: Bug Tracker, https://github.com/opensensor/growmax/-/issues
 Project-URL: repository, https://github.com/opensensor/growmax
 Classifier: Programming Language :: Python :: Implementation :: MicroPython
@@ -19,15 +19,15 @@
 
 To purchase a Growmax board or four sourcing parts, visit https://opensensor.io
 
 ![Growmax Board install with screen and i2c CO2 sensor](https://github.com/opensensor/growmax/blob/main/images/growmax_install_with_screen.jpg)
 
 
 # Installation
-To install the ``growmax`` package on a Pico or Pico W, first install the appropriate firmware for Micropython that is for your device.
+To install the ``growmax`` package on a Pico or BananaPi Pico (ESP32S3), first install the appropriate firmware for Micropython that is for your device.
 * Pico: https://micropython.org/download/rp2-pico/
 * Pico W:  https://micropython.org/download/rp2-pico-w/
 
 Ensure that you have Thonny IDE installed; for more information visit:  https://thonny.org/
 
 Launch Thonny IDE with your device connected.
```

### Comparing `growmax-1.2.0/src/growmax.egg-info/SOURCES.txt` & `growmax-1.2.1/src/growmax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

