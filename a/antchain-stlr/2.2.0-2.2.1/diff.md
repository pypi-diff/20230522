# Comparing `tmp/antchain_stlr-2.2.0.tar.gz` & `tmp/antchain_stlr-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.2.0.tar", last modified: Thu May 18 01:53:42 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.2.1.tar", last modified: Mon May 22 06:02:56 2023, max compression
```

## Comparing `antchain_stlr-2.2.0.tar` & `antchain_stlr-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96687 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   229400 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-18 01:53:42.000000 antchain_stlr-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96687 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   229440 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/setup.py
```

### Comparing `antchain_stlr-2.2.0/LICENSE` & `antchain_stlr-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.2.0/PKG-INFO` & `antchain_stlr-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.2.0
+Version: 2.2.1
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.2.0/README-CN.md` & `antchain_stlr-2.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.2.0/README.md` & `antchain_stlr-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.2.0/antchain_sdk_stlr/client.py` & `antchain_stlr-2.2.1/antchain_sdk_stlr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.2.0',
+                    'sdk_version': '2.2.1',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.2.0',
+                    'sdk_version': '2.2.1',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_stlr-2.2.0/antchain_sdk_stlr/models.py` & `antchain_stlr-2.2.1/antchain_sdk_stlr/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,15 +860,15 @@
         project_no: str = None,
         account_did: str = None,
         occurrent_time: str = None,
         scenario_code: str = None,
         scenario_name: str = None,
         platform_no: str = None,
         active_datum: List[AnyAmountItem] = None,
-        offset_volume: int = None,
+        offset_volume: str = None,
         carbon_energy: int = None,
     ):
         # 采集数据单号
         self.acquisition_item_no = acquisition_item_no
         # 碳补偿项目编号
         self.project_no = project_no
         # 参与账户DID
@@ -5325,25 +5325,25 @@
 class AddEcarOffsetacquisitionResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         acquisition_item_no: str = None,
-        carbon_emission_amount: int = None,
+        carbon_emission_amount: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 活动数据采集单号
         self.acquisition_item_no = acquisition_item_no
-        # 减碳量
+        # 减碳量，最多4位小数
         self.carbon_emission_amount = carbon_emission_amount
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5383,30 +5383,30 @@
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         translation_item_no: str = None,
         project_no: str = None,
         drawing_account_did: str = None,
         receipt_account_did: str = None,
-        translation_ammount: int = None,
+        translation_ammount: str = None,
         translation_type: str = None,
         occurrent_time: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 转移业务流水单号
         self.translation_item_no = translation_item_no
         # 碳补偿项目编号
         self.project_no = project_no
         # 出账账户DID
         self.drawing_account_did = drawing_account_did
         # 转移入账账户DID
         self.receipt_account_did = receipt_account_did
-        # 转移减碳量额度
+        # 转移减碳量额度，最多六位小数
         self.translation_ammount = translation_ammount
         # 业务类型包括，默认不需要传入，默认值为Translation
         self.translation_type = translation_type
         # 发生时间，格式为yyyy-MM-DD HH:MM:SS
         self.occurrent_time = occurrent_time
 
     def validate(self):
```

### Comparing `antchain_stlr-2.2.0/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.2.1/antchain_stlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.2.0
+Version: 2.2.1
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.2.0/setup.py` & `antchain_stlr-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 18/05/2023
+Created on 22/05/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
```

