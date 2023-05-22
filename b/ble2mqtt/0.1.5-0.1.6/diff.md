# Comparing `tmp/ble2mqtt-0.1.5.tar.gz` & `tmp/ble2mqtt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ble2mqtt-0.1.5.tar", last modified: Sat Oct 22 17:50:36 2022, max compression
+gzip compressed data, was "ble2mqtt-0.1.6.tar", last modified: Mon May 22 09:19:07 2023, max compression
```

## Comparing `ble2mqtt-0.1.5.tar` & `ble2mqtt-0.1.6.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-10-22 17:50:36.395908 ble2mqtt-0.1.5/
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1086 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/LICENSE
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)       55 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/MANIFEST.in
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     9699 2022-10-22 17:50:36.395975 ble2mqtt-0.1.5/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     9119 2022-10-09 10:05:09.000000 ble2mqtt-0.1.5/README.md
-drwxr-xr-x   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-10-22 17:50:36.388728 ble2mqtt-0.1.5/ble2mqtt/
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     4599 2022-10-09 09:21:40.000000 ble2mqtt-0.1.5/ble2mqtt/__main__.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)       18 2022-10-22 17:39:16.000000 ble2mqtt-0.1.5/ble2mqtt/__version__.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)    39758 2022-10-22 17:35:56.000000 ble2mqtt-0.1.5/ble2mqtt/ble2mqtt.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)      574 2022-10-22 17:35:41.000000 ble2mqtt-0.1.5/ble2mqtt/compat.py
-drwxr-xr-x   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-10-22 17:50:36.393645 ble2mqtt-0.1.5/ble2mqtt/devices/
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)      787 2022-05-23 06:17:20.000000 ble2mqtt-0.1.5/ble2mqtt/devices/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1895 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/atom_fast.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)    27165 2022-10-09 10:03:09.000000 ble2mqtt-0.1.5/ble2mqtt/devices/base.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     4834 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/bulb_avea.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)    11419 2022-09-18 16:16:55.000000 ble2mqtt-0.1.5/ble2mqtt/devices/cooker_redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     4603 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/cover_am43.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     7158 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/cover_soma.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)    11248 2022-09-18 16:17:08.000000 ble2mqtt-0.1.5/ble2mqtt/devices/kettle_redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     6571 2022-09-18 16:15:15.000000 ble2mqtt-0.1.5/ble2mqtt/devices/kettle_xiaomi.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     2579 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/devices/presence.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     7154 2022-10-01 15:18:55.000000 ble2mqtt-0.1.5/ble2mqtt/devices/thermostat_ensto.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)      349 2022-05-23 06:17:20.000000 ble2mqtt-0.1.5/ble2mqtt/devices/uuids.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     3438 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/vson_air_wp6003.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1434 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_base.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     2562 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_ht.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1076 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_lywsd03.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     2273 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_lywsd03_atc.py
-drwxr-xr-x   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-10-22 17:50:36.395596 ble2mqtt-0.1.5/ble2mqtt/protocols/
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     4624 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/am43.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     5266 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/avea.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     3819 2022-05-23 07:22:42.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/base.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     6596 2022-09-26 13:59:55.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/ensto.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)    16297 2022-10-06 08:04:08.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     6441 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/soma.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     2618 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/wp6003.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)    10322 2022-08-26 05:17:39.000000 ble2mqtt-0.1.5/ble2mqtt/protocols/xiaomi.py
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1692 2022-02-14 18:17:17.000000 ble2mqtt-0.1.5/ble2mqtt/utils.py
-drwxr-xr-x   0 ivan.belokobylskiy   (502) staff       (20)        0 2022-10-22 17:50:36.389411 ble2mqtt-0.1.5/ble2mqtt.egg-info/
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     9699 2022-10-22 17:50:36.000000 ble2mqtt-0.1.5/ble2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1165 2022-10-22 17:50:36.000000 ble2mqtt-0.1.5/ble2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)        1 2022-10-22 17:50:36.000000 ble2mqtt-0.1.5/ble2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)       52 2022-10-22 17:50:36.000000 ble2mqtt-0.1.5/ble2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)       34 2022-10-22 17:50:36.000000 ble2mqtt-0.1.5/ble2mqtt.egg-info/requires.txt
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)        9 2022-10-22 17:50:36.000000 ble2mqtt-0.1.5/ble2mqtt.egg-info/top_level.txt
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)       99 2022-10-22 17:50:36.396218 ble2mqtt-0.1.5/setup.cfg
--rw-r--r--   0 ivan.belokobylskiy   (502) staff       (20)     1028 2022-05-07 19:01:30.000000 ble2mqtt-0.1.5/setup.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.948243 ble2mqtt-0.1.6/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1086 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/LICENSE
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/MANIFEST.in
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-22 09:19:07.948306 ble2mqtt-0.1.6/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9346 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/README.md
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.944147 ble2mqtt-0.1.6/ble2mqtt/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4599 2023-05-21 11:18:54.000000 ble2mqtt-0.1.6/ble2mqtt/__main__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       18 2023-05-22 09:12:57.000000 ble2mqtt-0.1.6/ble2mqtt/__version__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    39758 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/ble2mqtt.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      574 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/compat.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.947111 ble2mqtt-0.1.6/ble2mqtt/devices/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      911 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1901 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/atom_fast.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    27177 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4834 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/bulb_avea.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11419 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/cooker_redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4603 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/cover_am43.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7158 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/cover_soma.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11248 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/kettle_redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6571 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/kettle_xiaomi.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2579 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/presence.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1526 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/qingping_cgdk2.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7154 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/thermostat_ensto.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      349 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/uuids.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1571 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/voltage_bm2.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3438 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/vson_air_wp6003.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1434 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2568 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_ht.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1076 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2273 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03_atc.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.948128 ble2mqtt-0.1.6/ble2mqtt/protocols/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4624 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/am43.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5266 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/avea.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3819 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6596 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/ensto.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    16297 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6441 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/soma.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2618 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/wp6003.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10322 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/xiaomi.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1692 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/utils.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.944849 ble2mqtt-0.1.6/ble2mqtt.egg-info/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1232 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       52 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/requires.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       99 2023-05-22 09:19:07.948546 ble2mqtt-0.1.6/setup.cfg
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1089 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/setup.py
```

### Comparing `ble2mqtt-0.1.5/LICENSE` & `ble2mqtt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/PKG-INFO` & `ble2mqtt-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ble2mqtt
-Version: 0.1.5
+Version: 0.1.6
 Summary: BLE to MQTT bridge
 Home-page: https://github.com/devbis/ble2mqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE
 
 # BLE2MQTT
 ### Control your Bluetooth devices with smart home
 
 ![ble2mqtt devices](./ble2mqtt.png)
 
@@ -57,14 +56,15 @@
 - **Xiaomi MJ_HT_V1 (type: xiaomihtv1)**
 - **Xiaomi LYWSD02MMC (type: xiaomihtv1)**
 - **Xiaomi LYWSD03MMC (type: xiaomilywsd)** (due to the connection to the device on 
   every data fetch, it consumes more battery power. Flashing to the custom
   firmware is recommended)
 - **Xiaomi LYWSD03MMC with custom ATC firmware (xiaomilywsd_atc)**
   - supported both atc1441 and pvvx formats
+- **Qingping CGDK2 (type: qingpingCGDK2)**
 
 ### Air sensors
 - **Vson WP6003 (type: wp6003)**
 
 ### Shades and Blinds
 - **Generic AM43 (type: am43)**
 
@@ -83,14 +83,18 @@
   These devices require [manual pairing](#manual-pairing-in-linux).
   After the device is paired on the host device, see the logs for the `key` and 
   put it to the config.
 
   The adapter uses holiday mode to control temperature as thermostat. You cannot 
   use this feature in the official app while ble2mqtt is working.
 
+### Battery voltage meters
+
+- **BM2 car battery voltage meter (type: voltage_bm2)**
+
 
 By default, a device works in the passive mode without connection by 
 listening to advertisement packets from a device.
 To use connection to the device provide `"passive": false` parameter.
 
 **Supported devices in passive mode:**
 - Xiaomi MJ_HT_V1 (xiaomihtv1)
@@ -204,14 +208,18 @@
         {
             "address": "11:22:33:aa:bb:ff",
             "type": "xiaomilywsd_atc"
         },
         {
             "address": "11:22:33:aa:aa:aa",
             "type": "atomfast"
+        },
+        {
+            "address": "11:22:33:aa:aa:bb",
+            "type": "voltage_bm2"
         }
     ]
 }
 ```
 
 You can omit a line, then default value will be used.
 
@@ -385,9 +393,7 @@
       - NET_ADMIN
 
 ```
 
 You do not need sharing `/var/run/dbus`, because `dbus` will start in the container.
 
 NOTE: `--net=host` and `--cap-add=NET_ADMIN` is required as it needs to use and control the bluetooth interface
-
-
```

### Comparing `ble2mqtt-0.1.5/README.md` & `ble2mqtt-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 - **Xiaomi MJ_HT_V1 (type: xiaomihtv1)**
 - **Xiaomi LYWSD02MMC (type: xiaomihtv1)**
 - **Xiaomi LYWSD03MMC (type: xiaomilywsd)** (due to the connection to the device on 
   every data fetch, it consumes more battery power. Flashing to the custom
   firmware is recommended)
 - **Xiaomi LYWSD03MMC with custom ATC firmware (xiaomilywsd_atc)**
   - supported both atc1441 and pvvx formats
+- **Qingping CGDK2 (type: qingpingCGDK2)**
 
 ### Air sensors
 - **Vson WP6003 (type: wp6003)**
 
 ### Shades and Blinds
 - **Generic AM43 (type: am43)**
 
@@ -65,14 +66,18 @@
   These devices require [manual pairing](#manual-pairing-in-linux).
   After the device is paired on the host device, see the logs for the `key` and 
   put it to the config.
 
   The adapter uses holiday mode to control temperature as thermostat. You cannot 
   use this feature in the official app while ble2mqtt is working.
 
+### Battery voltage meters
+
+- **BM2 car battery voltage meter (type: voltage_bm2)**
+
 
 By default, a device works in the passive mode without connection by 
 listening to advertisement packets from a device.
 To use connection to the device provide `"passive": false` parameter.
 
 **Supported devices in passive mode:**
 - Xiaomi MJ_HT_V1 (xiaomihtv1)
@@ -186,14 +191,18 @@
         {
             "address": "11:22:33:aa:bb:ff",
             "type": "xiaomilywsd_atc"
         },
         {
             "address": "11:22:33:aa:aa:aa",
             "type": "atomfast"
+        },
+        {
+            "address": "11:22:33:aa:aa:bb",
+            "type": "voltage_bm2"
         }
     ]
 }
 ```
 
 You can omit a line, then default value will be used.
```

### Comparing `ble2mqtt-0.1.5/ble2mqtt/__main__.py` & `ble2mqtt-0.1.6/ble2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/ble2mqtt.py` & `ble2mqtt-0.1.6/ble2mqtt/ble2mqtt.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/compat.py` & `ble2mqtt-0.1.6/ble2mqtt/compat.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/__init__.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,12 +3,14 @@
 from .bulb_avea import AveaBulb  # noqa: F401
 from .cooker_redmond import RedmondCooker  # noqa: F401
 from .cover_am43 import AM43Cover  # noqa: F401
 from .cover_soma import SomaCover  # noqa: F401
 from .kettle_redmond import RedmondKettle  # noqa: F401
 from .kettle_xiaomi import XiaomiKettle  # noqa: F401
 from .presence import Presence  # noqa: F401
+from .qingping_cgdk2 import QingpingTempRHMonitorLite  # noqa: F401
 from .thermostat_ensto import EnstoThermostat  # noqa: F401
+from .voltage_bm2 import VoltageTesterBM2  # noqa: F401
 from .vson_air_wp6003 import VsonWP6003  # noqa: F401
 from .xiaomi_ht import XiaomiHumidityTemperatureV1  # noqa: F401
 from .xiaomi_lywsd03 import XiaomiHumidityTemperatureLYWSD  # noqa: F401
 from .xiaomi_lywsd03_atc import XiaomiHumidityTemperatureLYWSDATC  # noqa: F401
```

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/atom_fast.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/atom_fast.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,9 +62,9 @@
                     'device_class': 'battery',
                     'unit_of_measurement': '%',
                     'entity_category': 'diagnostic',
                 },
             ],
         }
 
-    def filter_notifications(self, sender):
+    def filter_notifications(self, sender, data):
         return sender == 0x24
```

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/base.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,27 +552,27 @@
         return await self.handle_active(*args, **kwargs)
 
 
 class SubscribeAndSetDataMixin:
     DATA_CHAR: uuid.UUID = None  # type: ignore
     SENSOR_CLASS: ty.Any = None  # type: ignore
 
-    def filter_notifications(self, sender):
+    def filter_notifications(self, sender, data):
         return True
 
     def process_data(self, data: bytearray):
         self._state = self.SENSOR_CLASS.from_data(data)
 
     def notification_handler(self, sender, data: bytearray):
         _LOGGER.debug("{0} notification: {1}: {2}".format(
             self,
             sender,
             format_binary(data),
         ))
-        if self.filter_notifications(sender):
+        if self.filter_notifications(sender, data):
             self.process_data(data)
 
     async def get_device_data(self):
         if self.DATA_CHAR:
             await self.client.start_notify(
                 self.DATA_CHAR,
                 self.notification_handler,
```

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/bulb_avea.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/bulb_avea.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/cooker_redmond.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/cooker_redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/cover_am43.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/cover_am43.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/cover_soma.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/cover_soma.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/kettle_redmond.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/kettle_redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/kettle_xiaomi.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/kettle_xiaomi.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/presence.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/presence.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/thermostat_ensto.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/thermostat_ensto.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/vson_air_wp6003.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/vson_air_wp6003.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_base.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_ht.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_ht.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     NAME = 'xiaomihtv1'
     DATA_CHAR = MJHT_DATA
     BATTERY_CHAR = BATTERY
     SENSOR_CLASS = SensorState
     SUPPORT_PASSIVE = True
     ACTIVE_CONNECTION_MODE = ConnectionMode.ACTIVE_POLL_WITH_DISCONNECT
 
-    def filter_notifications(self, sender):
+    def filter_notifications(self, sender, data):
         # sender is 0xd or several requests it becomes
         # /org/bluez/hci0/dev_58_2D_34_32_E0_69/service000c/char000d
         return (
             sender == 0xd or
             isinstance(sender, str) and sender.endswith('000d')
         )
```

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_lywsd03.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/devices/xiaomi_lywsd03_atc.py` & `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03_atc.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/am43.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/am43.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/avea.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/avea.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/base.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/ensto.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/ensto.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/redmond.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/soma.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/soma.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/wp6003.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/wp6003.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/protocols/xiaomi.py` & `ble2mqtt-0.1.6/ble2mqtt/protocols/xiaomi.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt/utils.py` & `ble2mqtt-0.1.6/ble2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.5/ble2mqtt.egg-info/PKG-INFO` & `ble2mqtt-0.1.6/ble2mqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: ble2mqtt
-Version: 0.1.5
+Version: 0.1.6
 Summary: BLE to MQTT bridge
 Home-page: https://github.com/devbis/ble2mqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+Provides-Extra: full
 License-File: LICENSE
 
 # BLE2MQTT
 ### Control your Bluetooth devices with smart home
 
 ![ble2mqtt devices](./ble2mqtt.png)
 
@@ -57,14 +56,15 @@
 - **Xiaomi MJ_HT_V1 (type: xiaomihtv1)**
 - **Xiaomi LYWSD02MMC (type: xiaomihtv1)**
 - **Xiaomi LYWSD03MMC (type: xiaomilywsd)** (due to the connection to the device on 
   every data fetch, it consumes more battery power. Flashing to the custom
   firmware is recommended)
 - **Xiaomi LYWSD03MMC with custom ATC firmware (xiaomilywsd_atc)**
   - supported both atc1441 and pvvx formats
+- **Qingping CGDK2 (type: qingpingCGDK2)**
 
 ### Air sensors
 - **Vson WP6003 (type: wp6003)**
 
 ### Shades and Blinds
 - **Generic AM43 (type: am43)**
 
@@ -83,14 +83,18 @@
   These devices require [manual pairing](#manual-pairing-in-linux).
   After the device is paired on the host device, see the logs for the `key` and 
   put it to the config.
 
   The adapter uses holiday mode to control temperature as thermostat. You cannot 
   use this feature in the official app while ble2mqtt is working.
 
+### Battery voltage meters
+
+- **BM2 car battery voltage meter (type: voltage_bm2)**
+
 
 By default, a device works in the passive mode without connection by 
 listening to advertisement packets from a device.
 To use connection to the device provide `"passive": false` parameter.
 
 **Supported devices in passive mode:**
 - Xiaomi MJ_HT_V1 (xiaomihtv1)
@@ -204,14 +208,18 @@
         {
             "address": "11:22:33:aa:bb:ff",
             "type": "xiaomilywsd_atc"
         },
         {
             "address": "11:22:33:aa:aa:aa",
             "type": "atomfast"
+        },
+        {
+            "address": "11:22:33:aa:aa:bb",
+            "type": "voltage_bm2"
         }
     ]
 }
 ```
 
 You can omit a line, then default value will be used.
 
@@ -385,9 +393,7 @@
       - NET_ADMIN
 
 ```
 
 You do not need sharing `/var/run/dbus`, because `dbus` will start in the container.
 
 NOTE: `--net=host` and `--cap-add=NET_ADMIN` is required as it needs to use and control the bluetooth interface
-
-
```

### Comparing `ble2mqtt-0.1.5/ble2mqtt.egg-info/SOURCES.txt` & `ble2mqtt-0.1.6/ble2mqtt.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 ble2mqtt/devices/bulb_avea.py
 ble2mqtt/devices/cooker_redmond.py
 ble2mqtt/devices/cover_am43.py
 ble2mqtt/devices/cover_soma.py
 ble2mqtt/devices/kettle_redmond.py
 ble2mqtt/devices/kettle_xiaomi.py
 ble2mqtt/devices/presence.py
+ble2mqtt/devices/qingping_cgdk2.py
 ble2mqtt/devices/thermostat_ensto.py
 ble2mqtt/devices/uuids.py
+ble2mqtt/devices/voltage_bm2.py
 ble2mqtt/devices/vson_air_wp6003.py
 ble2mqtt/devices/xiaomi_base.py
 ble2mqtt/devices/xiaomi_ht.py
 ble2mqtt/devices/xiaomi_lywsd03.py
 ble2mqtt/devices/xiaomi_lywsd03_atc.py
 ble2mqtt/protocols/__init__.py
 ble2mqtt/protocols/am43.py
```

### Comparing `ble2mqtt-0.1.5/setup.py` & `ble2mqtt-0.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,17 @@
         'console_scripts': ['ble2mqtt=ble2mqtt.__main__:main']
     },
     packages=find_packages(include=['ble2mqtt', 'ble2mqtt.*']),
     install_requires=[
         'aio-mqtt-mod>=0.3.0',
         'bleak>=0.12.0',
     ],
+    extras_require={
+        'full': ['pycryptodome']
+    },
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Utilities',
```

