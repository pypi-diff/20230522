# Comparing `tmp/pyhyypapihawkmod-0.0.0.5.tar.gz` & `tmp/pyhyypapihawkmod-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-0.0.0.5.tar", last modified: Mon May 22 14:35:55 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-0.0.0.6.tar", last modified: Mon May 22 15:01:42 2023, max compression
```

## Comparing `pyhyypapihawkmod-0.0.0.5.tar` & `pyhyypapihawkmod-0.0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:35:55.570649 pyhyypapihawkmod-0.0.0.5/
--rw-rw-rw-   0        0        0    11357 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/LICENSE.md
--rw-rw-rw-   0        0        0       19 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-05-22 14:35:55.570649 pyhyypapihawkmod-0.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1178 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 14:35:55.538154 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/
--rw-rw-rw-   0        0        0      412 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/__init__.py
--rw-rw-rw-   0        0        0      146 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/__main__.py
--rw-rw-rw-   0        0        0     4682 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2780 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2825 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    25351 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/client.py
--rw-rw-rw-   0        0        0     3869 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/constants.py
--rw-rw-rw-   0        0        0      235 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7492 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    15720 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:35:55.554754 pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-05-22 14:35:55.000000 pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-05-22 14:35:55.000000 pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:35:55.000000 pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-22 14:35:55.000000 pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-22 14:35:55.000000 pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 14:35:55.570649 pyhyypapihawkmod-0.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-05-22 14:33:08.000000 pyhyypapihawkmod-0.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/
+-rw-rw-rw-   0        0        0    11357 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0       19 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1178 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 15:01:42.717686 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      412 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      146 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     4682 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2780 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2825 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    25351 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     3869 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      235 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7492 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    15720 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-22 15:01:42.000000 pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 15:01:42.746430 pyhyypapihawkmod-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-05-22 14:58:31.000000 pyhyypapihawkmod-0.0.0.6/setup.py
```

### Comparing `pyhyypapihawkmod-0.0.0.5/LICENSE.md` & `pyhyypapihawkmod-0.0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/PKG-INFO` & `pyhyypapihawkmod-0.0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.5/README.md` & `pyhyypapihawkmod-0.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/alarm_info.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/client.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/constants.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyHyypApihawkmod/push_receiver.py` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-0.0.0.5/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-0.0.0.6/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE.md
 MANIFEST.in
 README.md
 setup.py
-pyHyypApihawkmod/__init__.py
-pyHyypApihawkmod/__main__.py
-pyHyypApihawkmod/alarm_info.py
-pyHyypApihawkmod/android_checkin_pb2.py
-pyHyypApihawkmod/checkin_pb2.py
-pyHyypApihawkmod/client.py
-pyHyypApihawkmod/constants.py
-pyHyypApihawkmod/exceptions.py
-pyHyypApihawkmod/mcs_pb2.py
-pyHyypApihawkmod/push_receiver.py
+pyhyypapihawkmod/__init__.py
+pyhyypapihawkmod/__main__.py
+pyhyypapihawkmod/alarm_info.py
+pyhyypapihawkmod/android_checkin_pb2.py
+pyhyypapihawkmod/checkin_pb2.py
+pyhyypapihawkmod/client.py
+pyhyypapihawkmod/constants.py
+pyhyypapihawkmod/exceptions.py
+pyhyypapihawkmod/mcs_pb2.py
+pyhyypapihawkmod/push_receiver.py
 pyhyypapihawkmod.egg-info/PKG-INFO
 pyhyypapihawkmod.egg-info/SOURCES.txt
 pyhyypapihawkmod.egg-info/dependency_links.txt
 pyhyypapihawkmod.egg-info/requires.txt
 pyhyypapihawkmod.egg-info/top_level.txt
```

### Comparing `pyhyypapihawkmod-0.0.0.5/setup.py` & `pyhyypapihawkmod-0.0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="0.0.0.5",
+    version="0.0.0.6",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

