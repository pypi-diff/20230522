# Comparing `tmp/async_adbc-1.0.7.tar.gz` & `tmp/async_adbc-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_adbc-1.0.7.tar", max compression
+gzip compressed data, was "async_adbc-1.0.8.tar", max compression
```

## Comparing `async_adbc-1.0.7.tar` & `async_adbc-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,51 @@
--rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.7/async_adbc/__init__.py
--rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.7/async_adbc/adbclient.py
--rw-r--r--   0        0        0     3276 2023-05-19 07:56:58.086917 async_adbc-1.0.7/async_adbc/device.py
--rw-r--r--   0        0        0      187 2023-05-22 01:24:42.225886 async_adbc-1.0.7/async_adbc/exceptions.py
--rw-r--r--   0        0        0      601 2023-05-16 06:51:45.869292 async_adbc-1.0.7/async_adbc/plugins/__init__.py
--rw-r--r--   0        0        0      411 2023-05-18 08:06:58.438375 async_adbc-1.0.7/async_adbc/plugins/am.py
--rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.7/async_adbc/plugins/battery.py
--rw-r--r--   0        0        0    11610 2023-05-22 01:25:37.176656 async_adbc-1.0.7/async_adbc/plugins/cpu.py
--rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.7/async_adbc/plugins/forward.py
--rw-r--r--   0        0        0     3974 2023-05-22 01:24:42.228877 async_adbc-1.0.7/async_adbc/plugins/fps.py
--rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.7/async_adbc/plugins/gpu.py
--rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.7/async_adbc/plugins/input.py
--rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.7/async_adbc/plugins/logcat.py
--rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.7/async_adbc/plugins/mem.py
--rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.7/async_adbc/plugins/pm.py
--rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.7/async_adbc/plugins/prop.py
--rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.7/async_adbc/plugins/temp.py
--rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.7/async_adbc/plugins/traffic.py
--rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.7/async_adbc/plugins/utils.py
--rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.7/async_adbc/protocol.py
--rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.7/async_adbc/service/__init__.py
--rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.7/async_adbc/service/host.py
--rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.7/async_adbc/service/local.py
--rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.7/LICENSE
--rw-r--r--   0        0        0      482 2023-05-22 01:28:39.957454 async_adbc-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.7/README.md
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-16 06:58:01.167502 async_adbc-1.0.8/async_adbc/__init__.py
+-rw-r--r--   0        0        0      998 2023-05-16 06:58:27.465793 async_adbc-1.0.8/async_adbc/adbclient.py
+-rw-r--r--   0        0        0     3746 2023-05-22 09:52:07.908716 async_adbc-1.0.8/async_adbc/device.py
+-rw-r--r--   0        0        0      187 2023-05-22 01:24:42.225886 async_adbc-1.0.8/async_adbc/exceptions.py
+-rw-r--r--   0        0        0      663 2023-05-22 09:51:54.864677 async_adbc-1.0.8/async_adbc/plugins/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-18 08:06:58.438375 async_adbc-1.0.8/async_adbc/plugins/am.py
+-rw-r--r--   0        0        0     2657 2023-05-16 02:32:10.948830 async_adbc-1.0.8/async_adbc/plugins/battery.py
+-rw-r--r--   0        0        0    11610 2023-05-22 01:25:37.176656 async_adbc-1.0.8/async_adbc/plugins/cpu.py
+-rw-r--r--   0        0        0     1242 2023-05-16 06:51:45.797292 async_adbc-1.0.8/async_adbc/plugins/forward.py
+-rw-r--r--   0        0        0     3974 2023-05-22 01:24:42.228877 async_adbc-1.0.8/async_adbc/plugins/fps.py
+-rw-r--r--   0        0        0      614 2023-05-15 12:07:09.349059 async_adbc-1.0.8/async_adbc/plugins/gpu.py
+-rw-r--r--   0        0        0      393 2023-05-15 12:13:38.890420 async_adbc-1.0.8/async_adbc/plugins/input.py
+-rw-r--r--   0        0        0      895 2023-05-16 03:18:01.857216 async_adbc-1.0.8/async_adbc/plugins/logcat.py
+-rw-r--r--   0        0        0     2209 2023-05-16 03:26:42.422860 async_adbc-1.0.8/async_adbc/plugins/mem.py
+-rw-r--r--   0        0        0     1988 2023-05-22 10:18:29.986438 async_adbc-1.0.8/async_adbc/plugins/minicap.py
+-rw-r--r--   0        0        0     5597 2023-05-16 06:51:45.819291 async_adbc-1.0.8/async_adbc/plugins/pm.py
+-rw-r--r--   0        0        0      510 2023-05-15 11:29:29.910308 async_adbc-1.0.8/async_adbc/plugins/prop.py
+-rw-r--r--   0        0        0     4615 2023-05-16 04:20:29.957697 async_adbc-1.0.8/async_adbc/plugins/temp.py
+-rw-r--r--   0        0        0     2216 2023-05-16 06:51:45.868298 async_adbc-1.0.8/async_adbc/plugins/traffic.py
+-rw-r--r--   0        0        0      807 2023-05-15 11:29:32.496380 async_adbc-1.0.8/async_adbc/plugins/utils.py
+-rw-r--r--   0        0        0      686 2023-05-22 10:06:35.912810 async_adbc-1.0.8/async_adbc/plugins/wm.py
+-rw-r--r--   0        0        0     4481 2023-05-16 07:19:17.701385 async_adbc-1.0.8/async_adbc/protocol.py
+-rw-r--r--   0        0        0      796 2023-05-16 06:51:45.874292 async_adbc-1.0.8/async_adbc/service/__init__.py
+-rw-r--r--   0        0        0    10228 2023-05-16 06:51:45.939291 async_adbc-1.0.8/async_adbc/service/host.py
+-rw-r--r--   0        0        0    10086 2023-05-16 06:51:45.937291 async_adbc-1.0.8/async_adbc/service/local.py
+-rw-r--r--   0        0        0   722896 2023-05-22 08:50:56.899996 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minicap
+-rw-r--r--   0        0        0   722896 2023-05-22 08:50:56.904875 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minicap-nopie
+-rw-r--r--   0        0        0    38464 2023-05-22 08:50:56.906827 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minitouch
+-rw-r--r--   0        0        0    38464 2023-05-22 08:50:56.906827 async_adbc-1.0.8/async_adbc/vendor/minicap/arm64-v8a/minitouch-nopie
+-rw-r--r--   0        0        0    34060 2023-05-22 08:50:56.925390 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi/minitouch
+-rw-r--r--   0        0        0    29964 2023-05-22 08:50:56.926347 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi/minitouch-nopie
+-rw-r--r--   0        0        0   562792 2023-05-22 08:50:56.913660 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minicap
+-rw-r--r--   0        0        0   550504 2023-05-22 08:50:56.919515 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minicap-nopie
+-rw-r--r--   0        0        0    29972 2023-05-22 08:50:56.922442 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minitouch
+-rw-r--r--   0        0        0    29972 2023-05-22 08:50:56.923419 async_adbc-1.0.8/async_adbc/vendor/minicap/armeabi-v7a/minitouch-nopie
+-rw-r--r--   0        0        0    71328 2023-05-22 08:50:57.009974 async_adbc-1.0.8/async_adbc/vendor/minicap/mips/minitouch
+-rw-r--r--   0        0        0    71280 2023-05-22 08:50:57.012902 async_adbc-1.0.8/async_adbc/vendor/minicap/mips/minitouch-nopie
+-rw-r--r--   0        0        0    59992 2023-05-22 08:50:57.014854 async_adbc-1.0.8/async_adbc/vendor/minicap/mips64/minitouch
+-rw-r--r--   0        0        0    59992 2023-05-22 08:50:57.015829 async_adbc-1.0.8/async_adbc/vendor/minicap/mips64/minitouch-nopie
+-rw-r--r--   0        0        0   992920 2023-05-22 08:50:57.025589 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minicap
+-rw-r--r--   0        0        0   976536 2023-05-22 08:50:57.034373 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minicap-nopie
+-rw-r--r--   0        0        0    38108 2023-05-22 08:50:57.035349 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minitouch
+-rw-r--r--   0        0        0    38108 2023-05-22 08:50:57.036325 async_adbc-1.0.8/async_adbc/vendor/minicap/x86/minitouch-nopie
+-rw-r--r--   0        0        0   915840 2023-05-22 08:50:57.047007 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minicap
+-rw-r--r--   0        0        0   915840 2023-05-22 08:50:57.051886 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minicap-nopie
+-rw-r--r--   0        0        0    38728 2023-05-22 08:50:57.053838 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minitouch
+-rw-r--r--   0        0        0    38728 2023-05-22 08:50:57.054814 async_adbc-1.0.8/async_adbc/vendor/minicap/x86_64/minitouch-nopie
+-rw-r--r--   0        0        0     1090 2023-05-16 05:23:42.403245 async_adbc-1.0.8/LICENSE
+-rw-r--r--   0        0        0      482 2023-05-22 10:19:11.577795 async_adbc-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      423 2023-05-15 02:24:29.723099 async_adbc-1.0.8/README.md
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 async_adbc-1.0.8/PKG-INFO
```

### Comparing `async_adbc-1.0.7/async_adbc/adbclient.py` & `async_adbc-1.0.8/async_adbc/adbclient.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/device.py` & `async_adbc-1.0.8/async_adbc/device.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     MemPlugin,
     TempPlugin,
     UtilsPlugin,
     TrafficPlugin,
     ForwardPlugin,
     ActivityManagerPlugin,
     LogcatPlugin,
+    MinicapPlugin,
+    WMPlugin,
 )
 
 if typing.TYPE_CHECKING:
     from async_adbc.adbclient import ADBClient
 
 
 class Status(enum.Enum):
@@ -45,14 +47,16 @@
         self.battery = BatteryPlugin(self)
         self.temp = TempPlugin(self)
         self.utils = UtilsPlugin(self)
         self.traffic = TrafficPlugin(self)
         self.am = ActivityManagerPlugin(self)
         self.forward = ForwardPlugin(self)
         self.logcat = LogcatPlugin(self)
+        self.minicap = MinicapPlugin(self)
+        self.wm = WMPlugin(self)
 
     async def create_connection(self) -> Connection:
         conn = await self.adbc.create_connection()
         await conn.transport_mode(self.serialno)
         return conn
 
     async def wait_boot_complete(
@@ -110,7 +114,19 @@
             process_list = [(seq[1], seq[7]) for seq in lines]
             process_list.sort(key=lambda v: v[1], reverse=False)
 
             return process_list[0][0]
 
         else:
             raise ValueError(f"{package_name} 应用没有运行")
+
+    async def file_exists(self, file_path: str) -> bool:
+        """判断设备存在这个文件路径
+
+        Args:
+            file_path (str): 文件路径
+
+        Returns:
+            bool: true 存在， false不存在
+        """
+        res = await self.shell("ls", file_path)
+        return not ("No such file or directory" in res)
```

### Comparing `async_adbc-1.0.7/async_adbc/plugins/__init__.py` & `async_adbc-1.0.8/async_adbc/plugins/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,7 +18,9 @@
 from .utils import UtilsPlugin
 from .battery import BatteryPlugin
 from .am import ActivityManagerPlugin
 from .temp import TempPlugin
 from .traffic import TrafficPlugin
 from .forward import ForwardPlugin
 from .logcat import LogcatPlugin
+from .minicap import MinicapPlugin
+from .wm import WMPlugin
```

### Comparing `async_adbc-1.0.7/async_adbc/plugins/battery.py` & `async_adbc-1.0.8/async_adbc/plugins/battery.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/cpu.py` & `async_adbc-1.0.8/async_adbc/plugins/cpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/forward.py` & `async_adbc-1.0.8/async_adbc/plugins/forward.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/fps.py` & `async_adbc-1.0.8/async_adbc/plugins/fps.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/gpu.py` & `async_adbc-1.0.8/async_adbc/plugins/gpu.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/logcat.py` & `async_adbc-1.0.8/async_adbc/plugins/logcat.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/mem.py` & `async_adbc-1.0.8/async_adbc/plugins/mem.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/pm.py` & `async_adbc-1.0.8/async_adbc/plugins/pm.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/temp.py` & `async_adbc-1.0.8/async_adbc/plugins/temp.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/traffic.py` & `async_adbc-1.0.8/async_adbc/plugins/traffic.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/plugins/utils.py` & `async_adbc-1.0.8/async_adbc/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/protocol.py` & `async_adbc-1.0.8/async_adbc/protocol.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/service/__init__.py` & `async_adbc-1.0.8/async_adbc/service/__init__.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/service/host.py` & `async_adbc-1.0.8/async_adbc/service/host.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/async_adbc/service/local.py` & `async_adbc-1.0.8/async_adbc/service/local.py`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/LICENSE` & `async_adbc-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `async_adbc-1.0.7/PKG-INFO` & `async_adbc-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-adbc
-Version: 1.0.7
+Version: 1.0.8
 Summary: 
 Author: kaluluosi
 Author-email: kaluluosi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

