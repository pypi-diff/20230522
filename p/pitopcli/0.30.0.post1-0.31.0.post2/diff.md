# Comparing `tmp/pitopcli-0.30.0.post1.tar.gz` & `tmp/pitopcli-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitopcli-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:08 2022, max compression
+gzip compressed data, was "dist/pitopcli-0.31.0.post2.tar", last modified: Mon May 22 19:13:10 2023, max compression
```

## Comparing `pitopcli-0.30.0.post1.tar` & `pitopcli-0.31.0.post2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      960 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      133 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2953 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/battery.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/cli_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/deprecated_cli_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4442 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)     5168 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/formatter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/imu.py
--rw-r--r--   0 runner    (1001) docker     (122)    14042 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/imu_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/oled.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/pitop.py
--rw-r--r--   0 runner    (1001) docker     (122)     2385 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli/support_core/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12012 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support_core/health_check.py
--rw-r--r--   0 runner    (1001) docker     (122)    11142 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support_core/hub_communication.py
--rw-r--r--   0 runner    (1001) docker     (122)     2974 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support_core/links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support_core/ptsoftware.py
--rw-r--r--   0 runner    (1001) docker     (122)     4569 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/pitopcli/support_core/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      960 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      249 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/pitopcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:08.000000 pitopcli-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2505 2022-12-16 14:07:48.000000 pitopcli-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/battery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/deprecated_cli_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4442 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5168 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2323 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/imu.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14042 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/imu_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/oled.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1774 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/pitop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2385 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli/support_core/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12012 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support_core/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11142 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support_core/hub_communication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2974 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support_core/links.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support_core/ptsoftware.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4568 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/pitopcli/support_core/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      726 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/pitopcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:10.000000 pitopcli-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2505 2023-05-22 19:12:55.000000 pitopcli-0.31.0.post2/setup.py
```

### Comparing `pitopcli-0.30.0.post1/PKG-INFO` & `pitopcli-0.31.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitopcli
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python CLI
```

### Comparing `pitopcli-0.30.0.post1/pitopcli/__main__.py` & `pitopcli-0.31.0.post2/pitopcli/__main__.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/battery.py` & `pitopcli-0.31.0.post2/pitopcli/battery.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,14 @@
                 if arg == "capacity":
                     print(capacity)
                 if arg == "time-remaining":
                     print(time_remaining)
                 if arg == "wattage":
                     print(wattage)
         else:
-
             if self.args.charging_state:
                 print(charging_state)
             elif self.args.capacity:
                 print(capacity)
             elif self.args.time_remaining:
                 print(time_remaining)
             elif self.args.wattage:
```

### Comparing `pitopcli-0.30.0.post1/pitopcli/cli_base.py` & `pitopcli-0.31.0.post2/pitopcli/cli_base.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/deprecated_cli_runner.py` & `pitopcli-0.31.0.post2/pitopcli/deprecated_cli_runner.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/devices.py` & `pitopcli-0.31.0.post2/pitopcli/devices.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/display.py` & `pitopcli-0.31.0.post2/pitopcli/display.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/formatter.py` & `pitopcli-0.31.0.post2/pitopcli/formatter.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/imu.py` & `pitopcli-0.31.0.post2/pitopcli/imu.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,14 @@
             imu_cal.plot_graphs(self.args.path)
         else:
             raise PitopCliInvalidArgument("oops")
         return 0
 
     @classmethod
     def add_parser_arguments(cls, parser) -> None:
-
         subparser = parser.add_subparsers(
             title="IMU utility", description=cls.parser_help, dest="imu_subcommand"
         )
 
         calibrate_parser = subparser.add_parser(
             "calibrate", help="Calibrate the magnetometer"
         )
```

### Comparing `pitopcli-0.30.0.post1/pitopcli/imu_calibration.py` & `pitopcli-0.31.0.post2/pitopcli/imu_calibration.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/oled.py` & `pitopcli-0.31.0.post2/pitopcli/oled.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/pitop.py` & `pitopcli-0.31.0.post2/pitopcli/pitop.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/support.py` & `pitopcli-0.31.0.post2/pitopcli/support.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/support_core/health_check.py` & `pitopcli-0.31.0.post2/pitopcli/support_core/health_check.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/support_core/hub_communication.py` & `pitopcli-0.31.0.post2/pitopcli/support_core/hub_communication.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/support_core/links.py` & `pitopcli-0.31.0.post2/pitopcli/support_core/links.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/support_core/ptsoftware.py` & `pitopcli-0.31.0.post2/pitopcli/support_core/ptsoftware.py`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/pitopcli/support_core/systemd_service.py` & `pitopcli-0.31.0.post2/pitopcli/support_core/systemd_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from ..formatter import StdoutFormat
 
 
 class SystemdService:
     def __init__(self):
-
         self._name = ""
         self._load_state = ""
         self._active_state = ""
         self._enabled = ""
         self._description = ""
         self._fragment_path = ""
         self._vendor_preset = ""
```

### Comparing `pitopcli-0.30.0.post1/pitopcli.egg-info/PKG-INFO` & `pitopcli-0.31.0.post2/pitopcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitopcli
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Python CLI
```

### Comparing `pitopcli-0.30.0.post1/pitopcli.egg-info/SOURCES.txt` & `pitopcli-0.31.0.post2/pitopcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitopcli-0.30.0.post1/setup.py` & `pitopcli-0.31.0.post2/setup.py`

 * *Files identical despite different names*

