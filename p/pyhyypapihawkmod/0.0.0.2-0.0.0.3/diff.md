# Comparing `tmp/pyhyypapihawkmod-0.0.0.2.tar.gz` & `tmp/pyhyypapihawkmod-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-0.0.0.2.tar", last modified: Mon May 22 11:38:47 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-0.0.0.3.tar", last modified: Mon May 22 13:10:13 2023, max compression
```

## Comparing `pyhyypapihawkmod-0.0.0.2.tar` & `pyhyypapihawkmod-0.0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/
--rw-rw-rw-   0        0        0    11357 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0       19 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      532 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-05-22 10:15:19.000000 pyhyypapihawkmod-0.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 11:38:47.862580 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      412 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      146 2023-05-22 10:16:52.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     4682 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2672 2023-05-22 11:34:21.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2825 2023-05-22 11:35:29.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    25351 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     3869 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      235 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0    57885 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    15720 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      532 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-05-22 11:37:56.000000 pyhyypapihawkmod-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:10:13.225230 pyhyypapihawkmod-0.0.0.3/
+-rw-rw-rw-   0        0        0    11357 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0       19 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      532 2023-05-22 13:10:13.225230 pyhyypapihawkmod-0.0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-05-22 10:15:19.000000 pyhyypapihawkmod-0.0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 13:10:13.193275 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      412 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      146 2023-05-22 10:16:52.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     4682 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2780 2023-05-22 13:06:09.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2825 2023-05-22 13:07:24.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    25351 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     3869 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      235 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7492 2023-05-22 13:06:09.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    15720 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:10:13.225230 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-05-22 13:10:13.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-22 13:10:13.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 13:10:13.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-22 13:10:13.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-22 13:10:13.000000 pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 13:10:13.225230 pyhyypapihawkmod-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-05-22 13:08:46.000000 pyhyypapihawkmod-0.0.0.3/setup.py
```

### Comparing `pyhyypapihawkmod-0.0.0.2/LICENSE.md` & `pyhyypapihawkmod-0.0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/PKG-INFO` & `pyhyypapihawkmod-0.0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/RenierM26/pyHyypApi/
 Author: Renier Moorcroft + Modified to update protobuf version
 Author-email: renierm26@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.2/README.md` & `pyhyypapihawkmod-0.0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61ndroid_checkin.proto\x12\rcheckin_proto\"~\n\x10\x43hromeBuildProto\x12)\n\x08platform\x18\x01 \x01(\x0e\x32\x17.checkin_proto.Platform\x12\x16\n\x0e\x63hrome_version\x18\x02 \x01(\t\x12\'\n\x07\x63hannel\x18\x03 \x01(\x0e\x32\x16.checkin_proto.Channel\"\xf6\x01\n\x13\x41ndroidCheckinProto\x12\x19\n\x11last_checkin_msec\x18\x02 \x01(\x03\x12\x15\n\rcell_operator\x18\x06 \x01(\t\x12\x14\n\x0csim_operator\x18\x07 \x01(\t\x12\x0f\n\x07roaming\x18\x08 \x01(\t\x12\x13\n\x0buser_number\x18\t \x01(\x05\x12:\n\x04type\x18\x0c \x01(\x0e\x32\x19.checkin_proto.DeviceType:\x11\x44\x45VICE_ANDROID_OS\x12\x35\n\x0c\x63hrome_build\x18\r \x01(\x0b\x32\x1f.checkin_proto.ChromeBuildProto*}\n\x08Platform\x12\x10\n\x0cPLATFORM_WIN\x10\x01\x12\x10\n\x0cPLATFORM_MAC\x10\x02\x12\x12\n\x0ePLATFORM_LINUX\x10\x03\x12\x11\n\rPLATFORM_CROS\x10\x04\x12\x10\n\x0cPLATFORM_IOS\x10\x05\x12\x14\n\x10PLATFORM_ANDROID\x10\x06*i\n\x07\x43hannel\x12\x12\n\x0e\x43HANNEL_STABLE\x10\x01\x12\x10\n\x0c\x43HANNEL_BETA\x10\x02\x12\x0f\n\x0b\x43HANNEL_DEV\x10\x03\x12\x12\n\x0e\x43HANNEL_CANARY\x10\x04\x12\x13\n\x0f\x43HANNEL_UNKNOWN\x10\x05*g\n\nDeviceType\x12\x15\n\x11\x44\x45VICE_ANDROID_OS\x10\x01\x12\x11\n\rDEVICE_IOS_OS\x10\x02\x12\x19\n\x15\x44\x45VICE_CHROME_BROWSER\x10\x03\x12\x14\n\x10\x44\x45VICE_CHROME_OS\x10\x04\x42\x02H\x03')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61ndroid_checkin.proto\x12\rcheckin_proto\"\x8a\x03\n\x10\x43hromeBuildProto\x12:\n\x08platform\x18\x01 \x01(\x0e\x32(.checkin_proto.ChromeBuildProto.Platform\x12\x16\n\x0e\x63hrome_version\x18\x02 \x01(\t\x12\x38\n\x07\x63hannel\x18\x03 \x01(\x0e\x32\'.checkin_proto.ChromeBuildProto.Channel\"}\n\x08Platform\x12\x10\n\x0cPLATFORM_WIN\x10\x01\x12\x10\n\x0cPLATFORM_MAC\x10\x02\x12\x12\n\x0ePLATFORM_LINUX\x10\x03\x12\x11\n\rPLATFORM_CROS\x10\x04\x12\x10\n\x0cPLATFORM_IOS\x10\x05\x12\x14\n\x10PLATFORM_ANDROID\x10\x06\"i\n\x07\x43hannel\x12\x12\n\x0e\x43HANNEL_STABLE\x10\x01\x12\x10\n\x0c\x43HANNEL_BETA\x10\x02\x12\x0f\n\x0b\x43HANNEL_DEV\x10\x03\x12\x12\n\x0e\x43HANNEL_CANARY\x10\x04\x12\x13\n\x0f\x43HANNEL_UNKNOWN\x10\x05\"\xf6\x01\n\x13\x41ndroidCheckinProto\x12\x19\n\x11last_checkin_msec\x18\x02 \x01(\x03\x12\x15\n\rcell_operator\x18\x06 \x01(\t\x12\x14\n\x0csim_operator\x18\x07 \x01(\t\x12\x0f\n\x07roaming\x18\x08 \x01(\t\x12\x13\n\x0buser_number\x18\t \x01(\x05\x12:\n\x04type\x18\x0c \x01(\x0e\x32\x19.checkin_proto.DeviceType:\x11\x44\x45VICE_ANDROID_OS\x12\x35\n\x0c\x63hrome_build\x18\r \x01(\x0b\x32\x1f.checkin_proto.ChromeBuildProto*g\n\nDeviceType\x12\x15\n\x11\x44\x45VICE_ANDROID_OS\x10\x01\x12\x11\n\rDEVICE_IOS_OS\x10\x02\x12\x19\n\x15\x44\x45VICE_CHROME_BROWSER\x10\x03\x12\x14\n\x10\x44\x45VICE_CHROME_OS\x10\x04\x42\x02H\x03')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_checkin_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_PLATFORM']._serialized_start=417
-  _globals['_PLATFORM']._serialized_end=542
-  _globals['_CHANNEL']._serialized_start=544
-  _globals['_CHANNEL']._serialized_end=649
-  _globals['_DEVICETYPE']._serialized_start=651
-  _globals['_DEVICETYPE']._serialized_end=754
-  _globals['_CHROMEBUILDPROTO']._serialized_start=40
-  _globals['_CHROMEBUILDPROTO']._serialized_end=166
-  _globals['_ANDROIDCHECKINPROTO']._serialized_start=169
-  _globals['_ANDROIDCHECKINPROTO']._serialized_end=415
+  _globals['_DEVICETYPE']._serialized_start=686
+  _globals['_DEVICETYPE']._serialized_end=789
+  _globals['_CHROMEBUILDPROTO']._serialized_start=41
+  _globals['_CHROMEBUILDPROTO']._serialized_end=435
+  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_start=203
+  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_end=328
+  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_start=330
+  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_end=435
+  _globals['_ANDROIDCHECKINPROTO']._serialized_start=438
+  _globals['_ANDROIDCHECKINPROTO']._serialized_end=684
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.2
+Version: 0.0.0.3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/RenierM26/pyHyypApi/
 Author: Renier Moorcroft + Modified to update protobuf version
 Author-email: renierm26@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-0.0.0.3/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.2/setup.py` & `pyhyypapihawkmod-0.0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="0.0.0.2",
+    version="0.0.0.3",
     license='Apache Software License 2.0',
     author='Renier Moorcroft + Modified to update protobuf version',
     author_email='renierm26@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/RenierM26/pyHyypApi/',
     packages=setuptools.find_packages(),
```

