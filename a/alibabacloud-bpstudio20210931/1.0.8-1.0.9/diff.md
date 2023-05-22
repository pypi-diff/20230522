# Comparing `tmp/alibabacloud_bpstudio20210931-1.0.8.tar.gz` & `tmp/alibabacloud_bpstudio20210931-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931-1.0.8.tar", last modified: Fri Oct 21 01:54:54 2022, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931-1.0.9.tar", last modified: Tue Mar 14 05:24:45 2023, max compression
```

## Comparing `alibabacloud_bpstudio20210931-1.0.8.tar` & `alibabacloud_bpstudio20210931-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      266 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47984 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)    84901 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2022-10-21 01:54:54.000000 alibabacloud_bpstudio20210931-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      307 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47984 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)    85024 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-03-14 05:24:45.000000 alibabacloud_bpstudio20210931-1.0.9/setup.py
```

### Comparing `alibabacloud_bpstudio20210931-1.0.8/LICENSE` & `alibabacloud_bpstudio20210931-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.8/PKG-INFO` & `alibabacloud_bpstudio20210931-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-1.0.8/README-CN.md` & `alibabacloud_bpstudio20210931-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.8/README.md` & `alibabacloud_bpstudio20210931-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 class ChangeResourceGroupRequest(TeaModel):
     def __init__(
         self,
         new_resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
+        # rg-aek2ajbjoloa23q
         self.new_resource_group_id = new_resource_group_id
+        # P7RMVSVM9LOVYQOM
         self.resource_id = resource_id
+        # APPLICATION
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -50,14 +53,15 @@
         data: str = None,
         message: str = None,
         request_id: str = None,
     ):
         self.code = code
         self.data = data
         self.message = message
+        # Id of the request
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1386,14 +1390,15 @@
         self,
         code: int = None,
         data: GetExecuteOperationResultResponseBodyData = None,
         message: str = None,
         request_id: str = None,
     ):
         self.code = code
+        # Status
         self.data = data
         self.message = message
         self.request_id = request_id
 
     def validate(self):
         if self.data:
             self.data.validate()
@@ -1901,15 +1906,15 @@
     def __init__(
         self,
         application_id: str = None,
         create_time: str = None,
         image_url: str = None,
         name: str = None,
         resource_group_id: str = None,
-        status: int = None,
+        status: str = None,
         topo_url: str = None,
     ):
         self.application_id = application_id
         self.create_time = create_time
         self.image_url = image_url
         self.name = name
         self.resource_group_id = resource_group_id
```

### Comparing `alibabacloud_bpstudio20210931-1.0.8/alibabacloud_bpstudio20210931.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931-1.0.9/alibabacloud_bpstudio20210931.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-1.0.8/setup.py` & `alibabacloud_bpstudio20210931-1.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931.
 
-Created on 21/10/2022
+Created on 14/03/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

