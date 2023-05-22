# Comparing `tmp/akari-client-0.3.1.tar.gz` & `tmp/akari-client-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-client-0.3.1.tar", last modified: Mon Apr 10 15:04:27 2023, max compression
+gzip compressed data, was "akari-client-0.3.2.tar", last modified: Mon May 22 02:20:15 2023, max compression
```

## Comparing `akari-client-0.3.1.tar` & `akari-client-0.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-04-10 15:04:27.274032 akari-client-0.3.1/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      725 2023-04-10 14:34:37.000000 akari-client-0.3.1/README.md
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       87 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      920 2022-12-05 23:29:31.000000 akari-client-0.3.1/akari_client/akari_client.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2014 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/color.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3717 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/config.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client/grpc/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-client-0.3.1/akari_client/grpc/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      125 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/_error.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      656 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/channel_pool.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1434 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/factory.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4096 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/grpc/joints_controller.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4739 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/grpc/m5stack.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2478 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/joint_controller.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     8963 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/joint_manager.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    11435 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/m5stack_client.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      374 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/position.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-client-0.3.1/akari_client/py.typed
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client/serial/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-04-06 13:57:42.000000 akari-client-0.3.1/akari_client/serial/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6666 2022-12-05 23:08:44.000000 akari-client-0.3.1/akari_client/serial/dynamixel.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4538 2022-12-05 23:03:45.000000 akari-client-0.3.1/akari_client/serial/dynamixel_communicator.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1405 2022-12-05 23:07:56.000000 akari-client-0.3.1/akari_client/serial/factory.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4599 2023-03-16 13:20:21.000000 akari-client-0.3.1/akari_client/serial/m5stack.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4117 2022-12-05 21:46:13.000000 akari-client-0.3.1/akari_client/serial/m5stack_communicator.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-04-10 15:04:27.274032 akari-client-0.3.1/akari_client.egg-info/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      843 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      157 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       13 2023-04-10 15:04:27.000000 akari-client-0.3.1/akari_client.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-04-10 15:04:27.274032 akari-client-0.3.1/setup.cfg
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1316 2023-04-10 15:03:53.000000 akari-client-0.3.1/setup.py
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1461 2023-05-22 02:20:15.975682 akari-client-0.3.2/PKG-INFO
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      725 2023-05-22 00:31:41.000000 akari-client-0.3.2/README.md
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       87 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/__init__.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      920 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/akari_client.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2014 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/color.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3717 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/config.py
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client/grpc/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/__init__.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      125 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/_error.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      656 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/channel_pool.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1434 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/factory.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4096 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/joints_controller.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4739 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/grpc/m5stack.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2478 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/joint_controller.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     8960 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/joint_manager.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    11435 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/m5stack_client.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      374 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/position.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/py.typed
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client/serial/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/__init__.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     6666 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/dynamixel.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4538 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/dynamixel_communicator.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1405 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/factory.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4599 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/serial/m5stack.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4299 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/serial/m5stack_communicator.py
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client.egg-info/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1461 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      843 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        1 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      157 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       13 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       38 2023-05-22 02:20:15.975682 akari-client-0.3.2/setup.cfg
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1316 2023-05-22 00:31:41.000000 akari-client-0.3.2/setup.py
```

### Comparing `akari-client-0.3.1/PKG-INFO` & `akari-client-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: akari-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Akari Python package
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
-Description: # akari\_client
-        
-        [AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
-        
-        ## インストール
-        
-        ```sh
-        pip install akari_client
-        ```
-        
-        **注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
-        詳しくはオンラインドキュメントを参照してください。
-        
-        ## Getting Started: ディスプレイに文字を表示する
-        
-        ```py
-        with AkariClient() as akari:
-            m5 = akari.m5stack
-            m5.set_display_text("Hello, world!")
-        ```
-        
-        その他のサンプルや使い方はオンラインドキュメントを参照してください。
-        
-        ## ドキュメント
-        
-        [https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 Provides-Extra: grpc
 Provides-Extra: depthai
+
+# akari\_client
+
+[AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
+
+## インストール
+
+```sh
+pip install akari_client
+```
+
+**注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
+詳しくはオンラインドキュメントを参照してください。
+
+## Getting Started: ディスプレイに文字を表示する
+
+```py
+with AkariClient() as akari:
+    m5 = akari.m5stack
+    m5.set_display_text("Hello, world!")
+```
+
+その他のサンプルや使い方はオンラインドキュメントを参照してください。
+
+## ドキュメント
+
+[https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
+
```

### Comparing `akari-client-0.3.1/README.md` & `akari-client-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/akari_client.py` & `akari-client-0.3.2/akari_client/akari_client.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/color.py` & `akari-client-0.3.2/akari_client/color.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/config.py` & `akari-client-0.3.2/akari_client/config.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/grpc/channel_pool.py` & `akari-client-0.3.2/akari_client/grpc/channel_pool.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/grpc/factory.py` & `akari-client-0.3.2/akari_client/grpc/factory.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/grpc/joints_controller.py` & `akari-client-0.3.2/akari_client/grpc/joints_controller.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/grpc/m5stack.py` & `akari-client-0.3.2/akari_client/grpc/m5stack.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/joint_controller.py` & `akari-client-0.3.2/akari_client/joint_controller.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/joint_manager.py` & `akari-client-0.3.2/akari_client/joint_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         Returns:
             関節名と位置リミット(min,max)[rad]のDict
 
         Example:
             >>> from akari_client import AkariClient
             >>> akari = AkariClient()
             >>> joints = akari.joints
-            >>> print(joints.get_joint_positions())
+            >>> print(joints.get_joint_limits())
             # 各軸のリミット値が出力される
 
         """
         ret: Dict[str, PositionLimit] = {}
         for joint_name, controller in self._joints.items():
             ret[joint_name] = controller.get_position_limit()
         return ret
```

### Comparing `akari-client-0.3.1/akari_client/m5stack_client.py` & `akari-client-0.3.2/akari_client/m5stack_client.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/serial/dynamixel.py` & `akari-client-0.3.2/akari_client/serial/dynamixel.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/serial/dynamixel_communicator.py` & `akari-client-0.3.2/akari_client/serial/dynamixel_communicator.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/serial/factory.py` & `akari-client-0.3.2/akari_client/serial/factory.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/serial/m5stack.py` & `akari-client-0.3.2/akari_client/serial/m5stack.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/akari_client/serial/m5stack_communicator.py` & `akari-client-0.3.2/akari_client/serial/m5stack_communicator.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import serial
 
 from ..m5stack_client import M5ComDict
 
 BAUDRATE = 500000
 DEVICE_NAME = pathlib.Path("/dev/ttyUSB_M5Stack")
 TIMEOUT = 0.2
+RESPONSE_TIMEOUT = 1.0
 
 
 class M5SerialCommunicator:
     def __init__(
         self,
         baudrate: int = BAUDRATE,
         port: pathlib.Path = DEVICE_NAME,
@@ -112,16 +113,21 @@
         json_data = json.dumps(data, ensure_ascii=False)
         self.send(bytes(json_data, "UTF-8"))
 
         if sync:
             self._wait_response()
 
     def _wait_response(self) -> None:
+        called_time = self.current_time
+
         def _predicate() -> bool:
-            return self._latest_msg is not None and self._latest_msg["is_response"]
+            elapsed = self.current_time - called_time
+            return (
+                self._latest_msg is not None and self._latest_msg["is_response"]
+            ) or (elapsed > RESPONSE_TIMEOUT)
 
         with self._condition:
             while True:
                 self._condition.wait()
                 if _predicate():
                     break
```

### Comparing `akari-client-0.3.1/akari_client.egg-info/PKG-INFO` & `akari-client-0.3.2/akari_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: akari-client
-Version: 0.3.1
+Version: 0.3.2
 Summary: Akari Python package
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
-Description: # akari\_client
-        
-        [AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
-        
-        ## インストール
-        
-        ```sh
-        pip install akari_client
-        ```
-        
-        **注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
-        詳しくはオンラインドキュメントを参照してください。
-        
-        ## Getting Started: ディスプレイに文字を表示する
-        
-        ```py
-        with AkariClient() as akari:
-            m5 = akari.m5stack
-            m5.set_display_text("Hello, world!")
-        ```
-        
-        その他のサンプルや使い方はオンラインドキュメントを参照してください。
-        
-        ## ドキュメント
-        
-        [https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 Provides-Extra: grpc
 Provides-Extra: depthai
+
+# akari\_client
+
+[AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
+
+## インストール
+
+```sh
+pip install akari_client
+```
+
+**注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
+詳しくはオンラインドキュメントを参照してください。
+
+## Getting Started: ディスプレイに文字を表示する
+
+```py
+with AkariClient() as akari:
+    m5 = akari.m5stack
+    m5.set_display_text("Hello, world!")
+```
+
+その他のサンプルや使い方はオンラインドキュメントを参照してください。
+
+## ドキュメント
+
+[https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
+
```

### Comparing `akari-client-0.3.1/akari_client.egg-info/SOURCES.txt` & `akari-client-0.3.2/akari_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.1/setup.py` & `akari-client-0.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="akari-client",
-    version="0.3.1",
+    version="0.3.2",
     packages=find_packages(exclude=["tests"]),
     description="Akari Python package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="akari",
     author_email="akari.tmc@gmail.com",
     license="Apache License 2.0",
```

