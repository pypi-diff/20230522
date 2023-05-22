# Comparing `tmp/pitop.common-0.30.0.post1.tar.gz` & `tmp/pitop.common-0.31.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pitop.common-0.30.0.post1.tar", last modified: Fri Dec 16 14:08:13 2022, max compression
+gzip compressed data, was "dist/pitop.common-0.31.0.post2.tar", last modified: Mon May 22 19:13:11 2023, max compression
```

## Comparing `pitop.common-0.30.0.post1.tar` & `pitop.common-0.31.0.post2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      945 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      111 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7239 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/bitwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     2717 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3618 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/common_ids.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/common_names.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/configuration_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/counter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2041 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/current_session_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1339 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)     5477 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/firmware_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (122)     7212 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/i2c_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/lock.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     3051 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/notifications.py
--rw-r--r--   0 runner    (1001) docker     (122)     2659 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/pt_os.py
--rw-r--r--   0 runner    (1001) docker     (122)    19828 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/ptdm.py
--rw-r--r--   0 runner    (1001) docker     (122)      326 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     5539 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/smbus_device.py
--rw-r--r--   0 runner    (1001) docker     (122)     2623 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/switch_user.py
--rw-r--r--   0 runner    (1001) docker     (122)     8202 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (122)      337 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/pitop/common/type_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      945 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      810 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/pitop.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-16 14:08:13.000000 pitop.common-0.30.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2201 2022-12-16 14:07:48.000000 pitop.common-0.30.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/pitop/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/pitop/common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7239 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/bitwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2717 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/common_ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/common_names.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/configuration_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/counter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/current_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1339 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5477 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/firmware_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7212 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/i2c_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3442 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3050 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2659 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/pt_os.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19828 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/ptdm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5539 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/smbus_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2623 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/switch_user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8308 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/pitop/common/type_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/pitop.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-05-22 19:13:10.000000 pitop.common-0.31.0.post2/pitop.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/pitop.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 19:13:10.000000 pitop.common-0.31.0.post2/pitop.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-05-22 19:13:10.000000 pitop.common-0.31.0.post2/pitop.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 19:13:10.000000 pitop.common-0.31.0.post2/pitop.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 19:13:11.000000 pitop.common-0.31.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-05-22 19:12:55.000000 pitop.common-0.31.0.post2/setup.py
```

### Comparing `pitop.common-0.30.0.post1/PKG-INFO` & `pitop.common-0.31.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.common
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Common
```

### Comparing `pitop.common-0.30.0.post1/pitop/common/bitwise_ops.py` & `pitop.common-0.31.0.post2/pitop/common/bitwise_ops.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/command_runner.py` & `pitop.common-0.31.0.post2/pitop/common/command_runner.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/common_ids.py` & `pitop.common-0.31.0.post2/pitop/common/common_ids.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/common_names.py` & `pitop.common-0.31.0.post2/pitop/common/common_names.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/configuration_file.py` & `pitop.common-0.31.0.post2/pitop/common/configuration_file.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/current_session_info.py` & `pitop.common-0.31.0.post2/pitop/common/current_session_info.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/file_ops.py` & `pitop.common-0.31.0.post2/pitop/common/file_ops.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/firmware_device.py` & `pitop.common-0.31.0.post2/pitop/common/firmware_device.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/formatting.py` & `pitop.common-0.31.0.post2/pitop/common/formatting.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/i2c_device.py` & `pitop.common-0.31.0.post2/pitop/common/i2c_device.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/lock.py` & `pitop.common-0.31.0.post2/pitop/common/lock.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/logger.py` & `pitop.common-0.31.0.post2/pitop/common/logger.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/notifications.py` & `pitop.common-0.31.0.post2/pitop/common/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     timeout: int = 0,
     app_name: str = "",
     notification_id: int = -1,
     actions_manager: NotificationActionManager = None,
     urgency_level: NotificationUrgencyLevel = None,
     capture_notification_id: bool = True,
 ) -> str:
-
     # Check that `notify-send-ng` is available, as it's not a hard dependency of the package
     try:
         run(["dpkg-query", "-l", "notify-send-ng"], capture_output=True, check=True)
     except CalledProcessError:
         raise Exception("notify-send-ng not installed")
 
     cmd = "/usr/bin/notify-send "
```

### Comparing `pitop.common-0.30.0.post1/pitop/common/pt_os.py` & `pitop.common-0.31.0.post2/pitop/common/pt_os.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/ptdm.py` & `pitop.common-0.31.0.post2/pitop/common/ptdm.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/smbus_device.py` & `pitop.common-0.31.0.post2/pitop/common/smbus_device.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/switch_user.py` & `pitop.common-0.31.0.post2/pitop/common/switch_user.py`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/pitop/common/sys_info.py` & `pitop.common-0.31.0.post2/pitop/common/sys_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from enum import Enum, auto
 from fractions import Fraction
 from ipaddress import IPv4Network, IPv6Network, ip_address, ip_network
 from os import path, uname
+from pathlib import Path
 from subprocess import DEVNULL, PIPE, CalledProcessError, Popen, check_output
 from typing import Dict, Union
 
 import netifaces
 from isc_dhcp_leases import IscDhcpLeases
 
 from pitop.common.command_runner import run_command
@@ -215,17 +216,18 @@
         try:
             run_command(cmd, timeout=timeout, check=True, log_errors=False)
             return True
         except Exception:
             return False
 
     try:
-        current_leases = (
-            IscDhcpLeases("/var/lib/dhcp/dhcpd.leases").get_current().values()
-        )
+        leases_file = "/var/lib/dhcp/dhcpd.leases"
+        current_leases = ""
+        if Path(leases_file).exists():
+            current_leases = IscDhcpLeases(leases_file).get_current().values()
     except Exception as e:
         logger.error(f"Error reading dhcpd leases: {e}")
         return ""
 
     current_leases = list(current_leases)
     current_leases.reverse()
```

### Comparing `pitop.common-0.30.0.post1/pitop.common.egg-info/PKG-INFO` & `pitop.common-0.31.0.post2/pitop.common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pitop.common
-Version: 0.30.0.post1
+Version: 0.31.0.post2
 Summary: pi-top Python SDK.
 Home-page: https://github.com/pi-top/pi-top-Python-SDK
 Author: pi-top
 Author-email: deb-maintainers@pi-top.com
 License: Apache Software License
 Description: ===========================
         pi-top Common
```

### Comparing `pitop.common-0.30.0.post1/pitop.common.egg-info/SOURCES.txt` & `pitop.common-0.31.0.post2/pitop.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pitop.common-0.30.0.post1/setup.py` & `pitop.common-0.31.0.post2/setup.py`

 * *Files identical despite different names*

