# Comparing `tmp/pyhyypapihawkmod-0.0.0.1.tar.gz` & `tmp/pyhyypapihawkmod-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-0.0.0.1.tar", last modified: Mon May 22 10:47:06 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-0.0.0.2.tar", last modified: Mon May 22 11:38:47 2023, max compression
```

## Comparing `pyhyypapihawkmod-0.0.0.1.tar` & `pyhyypapihawkmod-0.0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:47:06.152795 pyhyypapihawkmod-0.0.0.1/
--rw-rw-rw-   0        0        0    11357 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       19 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      532 2023-05-22 10:47:06.152795 pyhyypapihawkmod-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-05-22 10:15:19.000000 pyhyypapihawkmod-0.0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 10:47:06.135063 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      412 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      146 2023-05-22 10:16:52.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     4682 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2672 2023-05-22 09:40:35.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-22 10:01:11.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    25351 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     3869 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      235 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0    57885 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    15720 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:47:06.152795 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      532 2023-05-22 10:47:06.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-22 10:47:06.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:47:06.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-22 10:47:06.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 10:47:06.000000 pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:47:06.152795 pyhyypapihawkmod-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-05-22 10:46:19.000000 pyhyypapihawkmod-0.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/
+-rw-rw-rw-   0        0        0    11357 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/LICENSE.md
+-rw-rw-rw-   0        0        0       19 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      532 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-05-22 10:15:19.000000 pyhyypapihawkmod-0.0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 11:38:47.862580 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      412 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      146 2023-05-22 10:16:52.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     4682 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2672 2023-05-22 11:34:21.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2825 2023-05-22 11:35:29.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    25351 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     3869 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      235 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0    57885 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    15720 2022-10-01 05:44:28.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-22 11:38:47.000000 pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 11:38:47.878636 pyhyypapihawkmod-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-05-22 11:37:56.000000 pyhyypapihawkmod-0.0.0.2/setup.py
```

### Comparing `pyhyypapihawkmod-0.0.0.1/LICENSE.md` & `pyhyypapihawkmod-0.0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/PKG-INFO` & `pyhyypapihawkmod-0.0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/RenierM26/pyHyypApi/
 Author: Renier Moorcroft + Modified to update protobuf version
 Author-email: renierm26@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.1/README.md` & `pyhyypapihawkmod-0.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/checkin_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,18 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import android_checkin_pb2 as android__checkin__pb2
+from . import android_checkin_pb2 as android__checkin__pb2
 
-from android_checkin_pb2 import *
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcheckin.proto\x12\rcheckin_proto\x1a\x15\x61ndroid_checkin.proto\"/\n\x10GservicesSetting\x12\x0c\n\x04name\x18\x01 \x02(\x0c\x12\r\n\x05value\x18\x02 \x02(\x0c\"\xcb\x03\n\x15\x41ndroidCheckinRequest\x12\x0c\n\x04imei\x18\x01 \x01(\t\x12\x0c\n\x04meid\x18\n \x01(\t\x12\x10\n\x08mac_addr\x18\t \x03(\t\x12\x15\n\rmac_addr_type\x18\x13 \x03(\t\x12\x15\n\rserial_number\x18\x10 \x01(\t\x12\x0b\n\x03\x65sn\x18\x11 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x12\n\nlogging_id\x18\x07 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x33\n\x07\x63heckin\x18\x04 \x02(\x0b\x32\".checkin_proto.AndroidCheckinProto\x12\x15\n\rdesired_build\x18\x05 \x01(\t\x12\x16\n\x0emarket_checkin\x18\x08 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_cookie\x18\x0b \x03(\t\x12\x11\n\ttime_zone\x18\x0c \x01(\t\x12\x16\n\x0esecurity_token\x18\r \x01(\x06\x12\x0f\n\x07version\x18\x0e \x01(\x05\x12\x10\n\x08ota_cert\x18\x0f \x03(\t\x12\x10\n\x08\x66ragment\x18\x14 \x01(\x05\x12\x11\n\tuser_name\x18\x15 \x01(\t\x12\x1a\n\x12user_serial_number\x18\x16 \x01(\x05\"\x83\x02\n\x16\x41ndroidCheckinResponse\x12\x10\n\x08stats_ok\x18\x01 \x02(\x08\x12\x11\n\ttime_msec\x18\x03 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x04 \x01(\t\x12\x15\n\rsettings_diff\x18\t \x01(\x08\x12\x16\n\x0e\x64\x65lete_setting\x18\n \x03(\t\x12\x30\n\x07setting\x18\x05 \x03(\x0b\x32\x1f.checkin_proto.GservicesSetting\x12\x11\n\tmarket_ok\x18\x06 \x01(\x08\x12\x12\n\nandroid_id\x18\x07 \x01(\x06\x12\x16\n\x0esecurity_token\x18\x08 \x01(\x06\x12\x14\n\x0cversion_info\x18\x0b \x01(\tB\x02H\x03P\x00')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcheckin.proto\x12\rcheckin_proto\x1a\x15\x61ndroid_checkin.proto\"/\n\x10GservicesSetting\x12\x0c\n\x04name\x18\x01 \x02(\x0c\x12\r\n\x05value\x18\x02 \x02(\x0c\"\xcb\x03\n\x15\x41ndroidCheckinRequest\x12\x0c\n\x04imei\x18\x01 \x01(\t\x12\x0c\n\x04meid\x18\n \x01(\t\x12\x10\n\x08mac_addr\x18\t \x03(\t\x12\x15\n\rmac_addr_type\x18\x13 \x03(\t\x12\x15\n\rserial_number\x18\x10 \x01(\t\x12\x0b\n\x03\x65sn\x18\x11 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x12\n\nlogging_id\x18\x07 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x33\n\x07\x63heckin\x18\x04 \x02(\x0b\x32\".checkin_proto.AndroidCheckinProto\x12\x15\n\rdesired_build\x18\x05 \x01(\t\x12\x16\n\x0emarket_checkin\x18\x08 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_cookie\x18\x0b \x03(\t\x12\x11\n\ttime_zone\x18\x0c \x01(\t\x12\x16\n\x0esecurity_token\x18\r \x01(\x06\x12\x0f\n\x07version\x18\x0e \x01(\x05\x12\x10\n\x08ota_cert\x18\x0f \x03(\t\x12\x10\n\x08\x66ragment\x18\x14 \x01(\x05\x12\x11\n\tuser_name\x18\x15 \x01(\t\x12\x1a\n\x12user_serial_number\x18\x16 \x01(\x05\"\x83\x02\n\x16\x41ndroidCheckinResponse\x12\x10\n\x08stats_ok\x18\x01 \x02(\x08\x12\x11\n\ttime_msec\x18\x03 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x04 \x01(\t\x12\x15\n\rsettings_diff\x18\t \x01(\x08\x12\x16\n\x0e\x64\x65lete_setting\x18\n \x03(\t\x12\x30\n\x07setting\x18\x05 \x03(\x0b\x32\x1f.checkin_proto.GservicesSetting\x12\x11\n\tmarket_ok\x18\x06 \x01(\x08\x12\x12\n\nandroid_id\x18\x07 \x01(\x06\x12\x16\n\x0esecurity_token\x18\x08 \x01(\x06\x12\x14\n\x0cversion_info\x18\x0b \x01(\tB\x02H\x03')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'checkin_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
```

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/RenierM26/pyHyypApi/
 Author: Renier Moorcroft + Modified to update protobuf version
 Author-email: renierm26@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.1/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-0.0.0.2/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.1/setup.py` & `pyhyypapihawkmod-0.0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="0.0.0.1",
+    version="0.0.0.2",
     license='Apache Software License 2.0',
     author='Renier Moorcroft + Modified to update protobuf version',
     author_email='renierm26@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/RenierM26/pyHyypApi/',
     packages=setuptools.find_packages(),
```

