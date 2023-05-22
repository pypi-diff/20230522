# Comparing `tmp/alibabacloud_bpstudio20210931_py2-1.0.2.tar.gz` & `tmp/alibabacloud_bpstudio20210931_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-1.0.2.tar", last modified: Fri Mar 31 06:11:48 2023, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-1.0.3.tar", last modified: Mon May 22 09:08:04 2023, max compression
```

## Comparing `alibabacloud_bpstudio20210931_py2-1.0.2.tar` & `alibabacloud_bpstudio20210931_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)       82 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21867 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)   110937 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-31 06:11:48.000000 alibabacloud_bpstudio20210931_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-03-31 06:11:47.000000 alibabacloud_bpstudio20210931_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21867 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   104364 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-05-22 09:08:04.000000 alibabacloud_bpstudio20210931_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/LICENSE` & `alibabacloud_bpstudio20210931_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/README-CN.md` & `alibabacloud_bpstudio20210931_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/README.md` & `alibabacloud_bpstudio20210931_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -600,66 +600,18 @@
             temp_model = DeployApplicationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ExecuteOperationASyncRequest(TeaModel):
     def __init__(self, attributes=None, operation=None, resource_group_id=None, service_type=None):
-        # The parameters that you need to specify when you perform an operation. The parameters vary based on the operation and are specified in the map format. The following examples show how to specify the parameters if you perform an operation on an ECS instance:
-        # 
-        # *   The following common parameters need to be specified for operations on an ECS instance:
-        # 
-        # change_type, regionId, instanceId, and appId.
-        # 
-        # *   To change the instance type of an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_instance_type","instance_type":"ecs.hfr7.2xlarge","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # *   To stop an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_status","status":"Stopped","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # *   To start an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_status","status":"Running","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # *   To restart an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_status","status":"Restart","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # Enumeration values
-        # 
-        # <!-- -->
-        # 
-        # :
-        # 
-        # *   { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
         self.attributes = attributes  # type: dict[str, str]
-        # The type of the operation to be performed to modify the parameters of an instance of the specified service. Some operations are common to different services, and other operations are specific to each service. For example, set this parameter to one of the following values to perform the corresponding operation on an ECS instance:
-        # 
-        # *   rename: modifies the name of an ECS instance.
-        # *   modifyInstanceType: changes the instance type of an ECS instance.
-        # *   modifyInstanceType: starts an ECS instance.
-        # *   modifyInstanceType: stops an ECS instance.
-        # *   modifyInstanceType: restarts an ECS instance.
-        # *   addTags: adds tags to an ECS instance.
-        # *   ecsDelete: deletes an ECS instance.
-        # *   modifyPayType: changes the billing method of an ECS instance.
         self.operation = operation  # type: str
-        # The ID of the resource group. This parameter is specified to verify the permissions on the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The type of the service. If you want to modify the parameters of an Elastic Compute Service (ECS) instance, set this parameter to ecs.
+        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
         self.service_type = service_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ExecuteOperationASyncRequest, self).to_map()
@@ -688,66 +640,18 @@
         if m.get('ServiceType') is not None:
             self.service_type = m.get('ServiceType')
         return self
 
 
 class ExecuteOperationASyncShrinkRequest(TeaModel):
     def __init__(self, attributes_shrink=None, operation=None, resource_group_id=None, service_type=None):
-        # The parameters that you need to specify when you perform an operation. The parameters vary based on the operation and are specified in the map format. The following examples show how to specify the parameters if you perform an operation on an ECS instance:
-        # 
-        # *   The following common parameters need to be specified for operations on an ECS instance:
-        # 
-        # change_type, regionId, instanceId, and appId.
-        # 
-        # *   To change the instance type of an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_instance_type","instance_type":"ecs.hfr7.2xlarge","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # *   To stop an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_status","status":"Stopped","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # *   To start an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_status","status":"Running","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # *   To restart an ECS instance, specify the following parameters:
-        # 
-        # { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{"change_type":"modify_status","status":"Restart","instanceId":"i-xxxxxxxxx","regionId":"cn-beijing","appId":"xxxxxxxxxxxxx"}" }
-        # 
-        # Enumeration values
-        # 
-        # <!-- -->
-        # 
-        # :
-        # 
-        # *   { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
-        # 
-        #     <!-- -->
-        # 
-        #     :
-        # 
-        #     <!-- -->
-        # 
-        #     { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
         self.attributes_shrink = attributes_shrink  # type: str
-        # The type of the operation to be performed to modify the parameters of an instance of the specified service. Some operations are common to different services, and other operations are specific to each service. For example, set this parameter to one of the following values to perform the corresponding operation on an ECS instance:
-        # 
-        # *   rename: modifies the name of an ECS instance.
-        # *   modifyInstanceType: changes the instance type of an ECS instance.
-        # *   modifyInstanceType: starts an ECS instance.
-        # *   modifyInstanceType: stops an ECS instance.
-        # *   modifyInstanceType: restarts an ECS instance.
-        # *   addTags: adds tags to an ECS instance.
-        # *   ecsDelete: deletes an ECS instance.
-        # *   modifyPayType: changes the billing method of an ECS instance.
         self.operation = operation  # type: str
-        # The ID of the resource group. This parameter is specified to verify the permissions on the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The type of the service. If you want to modify the parameters of an Elastic Compute Service (ECS) instance, set this parameter to ecs.
+        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
         self.service_type = service_type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ExecuteOperationASyncShrinkRequest, self).to_map()
@@ -776,21 +680,17 @@
         if m.get('ServiceType') is not None:
             self.service_type = m.get('ServiceType')
         return self
 
 
 class ExecuteOperationASyncResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # The HTTP status code. A value of 200 indicates that the request is successful, and other values indicate that the request fails.
         self.code = code  # type: int
-        # The ID of the operation.
-        self.data = data  # type: dict[str, str]
-        # The error message.
+        self.data = data  # type: str
         self.message = message  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ExecuteOperationASyncResponseBody, self).to_map()
@@ -858,17 +758,17 @@
             temp_model = ExecuteOperationASyncResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetApplicationRequest(TeaModel):
     def __init__(self, application_id=None, resource_group_id=None):
-        # The ID of the application.
+        # The ID of the request.
         self.application_id = application_id  # type: str
-        # The ID of the resource group.
+        # Queries the basic information, verification results, billing results, and deployment results of an application.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetApplicationRequest, self).to_map()
@@ -890,27 +790,27 @@
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class GetApplicationResponseBodyDataChecklist(TeaModel):
     def __init__(self, lifecycle=None, region=None, remark=None, resource_code=None, resource_name=None, result=None,
                  specification=None):
-        # The resource tag.
+        # The message returned for verification.
         self.lifecycle = lifecycle  # type: str
-        # The ID of the region.
+        # The verification results returned.
         self.region = region  # type: str
-        # The message returned for verification.
+        # The name of the instance.
         self.remark = remark  # type: str
-        # The service code.
+        # The error message that is returned when a price query fails.
         self.resource_code = resource_code  # type: str
-        # The name of the instance.
+        # ECS instance sold out
         self.resource_name = resource_name  # type: str
-        # The verification result.
+        # The service code.
         self.result = result  # type: str
-        # The resource specification.
+        # The verification result.
         self.specification = specification  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetApplicationResponseBodyDataChecklist, self).to_map()
@@ -953,39 +853,39 @@
         return self
 
 
 class GetApplicationResponseBodyDataPriceList(TeaModel):
     def __init__(self, charge_type=None, count=None, instance_name=None, lifecycle=None, one_price=None,
                  original_price=None, period=None, price=None, price_unit=None, region=None, remark=None, resource_code=None,
                  specification=None):
-        # The billing method.
+        # The price unit.
         self.charge_type = charge_type  # type: str
-        # The quantity.
+        # The original price.
         self.count = count  # type: long
-        # The name of the instance.
+        # The ID of the resource group to which the application belongs.
         self.instance_name = instance_name  # type: str
-        # The resource tag.
+        # The ID of the region.
         self.lifecycle = lifecycle  # type: str
-        # The unit price.
+        # The service code.
         self.one_price = one_price  # type: float
-        # The original price.
+        # The billing results.
         self.original_price = original_price  # type: float
-        # The service duration.
+        # The name of the instance.
         self.period = period  # type: float
-        # The total price.
+        # The quantity.
         self.price = price  # type: float
-        # The price unit.
+        # The unit price.
         self.price_unit = price_unit  # type: str
-        # The ID of the region.
+        # USD/Hour
         self.region = region  # type: str
-        # The error message that is returned when a price query fails.
+        # The instance type.
         self.remark = remark  # type: str
-        # The service code.
+        # The time when the application was created.
         self.resource_code = resource_code  # type: str
-        # The instance type.
+        # The total price.
         self.specification = specification  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetApplicationResponseBodyDataPriceList, self).to_map()
@@ -1051,29 +951,29 @@
             self.specification = m.get('Specification')
         return self
 
 
 class GetApplicationResponseBodyDataResourceList(TeaModel):
     def __init__(self, charge_type=None, lifecycle=None, remark=None, resource_code=None, resource_id=None,
                  resource_name=None, resource_type=None, status=None):
-        # The billing method.
+        # The service code.
         self.charge_type = charge_type  # type: str
-        # The resource tag.
+        # The billing method.
         self.lifecycle = lifecycle  # type: str
-        # The deployment result.
+        # The ID of the instance.
         self.remark = remark  # type: str
-        # The service code.
+        # The status of the application.
         self.resource_code = resource_code  # type: str
-        # The ID of the instance.
+        # The resource deployment result.
         self.resource_id = resource_id  # type: str
-        # The name of the instance.
+        # The resources.
         self.resource_name = resource_name  # type: str
-        # The resource type.
+        # The name of the instance.
         self.resource_type = resource_type  # type: str
-        # The resource deployment result.
+        # The resource tag.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetApplicationResponseBodyDataResourceList, self).to_map()
@@ -1120,39 +1020,39 @@
         return self
 
 
 class GetApplicationResponseBodyData(TeaModel):
     def __init__(self, application_id=None, checklist=None, create_time=None, description=None, error=None,
                  image_url=None, name=None, price_list=None, resource_group_id=None, resource_list=None, status=None,
                  template_id=None, topo_url=None):
-        # The ID of the application.
+        # The description of the application.
         self.application_id = application_id  # type: str
-        # The verification results returned.
+        # The resource tag.
         self.checklist = checklist  # type: list[GetApplicationResponseBodyDataChecklist]
-        # The time when the application was created.
+        # The URL of the application topology image.
         self.create_time = create_time  # type: str
-        # The description of the application.
+        # The message returned for the request.
         self.description = description  # type: str
-        # The message returned for deployment.
+        # The resource type.
         self.error = error  # type: str
-        # The URL of the image in the database.
+        # The ID of the request.
         self.image_url = image_url  # type: str
-        # The name of the application.
+        # The URL of the image in the database.
         self.name = name  # type: str
-        # The billing results.
+        # The ID of the template associated with the application.
         self.price_list = price_list  # type: list[GetApplicationResponseBodyDataPriceList]
-        # The ID of the resource group to which the application belongs.
+        # 1411182597819805/topo-MCEXDI5EL2OM10NY.json
         self.resource_group_id = resource_group_id  # type: str
-        # The resources.
+        # The resource specification.
         self.resource_list = resource_list  # type: list[GetApplicationResponseBodyDataResourceList]
-        # The status of the application.
+        # Verification passed
         self.status = status  # type: str
-        # The ID of the template associated with the application.
+        # CADT application
         self.template_id = template_id  # type: str
-        # The URL of the application topology image.
+        # The ID of the application.
         self.topo_url = topo_url  # type: str
 
     def validate(self):
         if self.checklist:
             for k in self.checklist:
                 if k:
                     k.validate()
@@ -1243,21 +1143,46 @@
         if m.get('TopoURL') is not None:
             self.topo_url = m.get('TopoURL')
         return self
 
 
 class GetApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # The HTTP status code.
+        # The deployment result.
         self.code = code  # type: int
-        # The details of the application.
+        # The ID of the resource group.
         self.data = data  # type: GetApplicationResponseBodyData
-        # The message returned for the request.
+        # Possible application states:
+        # 
+        # *   Creating: The application is being created.
+        # *   Modified: The application has been modified.
+        # *   Verifying: The application is being verified.
+        # *   Verified_Failure: The application failed to pass the verification.
+        # *   Verified_Success: The application has passed the verification.
+        # *   Valuating: Fees are being calculated for the application.
+        # *   Valuating_Failure: Fees failed to be calculated for the application.
+        # *   Valuating_Success: Fees are calculated for the application.
+        # *   Deploying: The application is being deployed.
+        # *   Deployed_Failure: The application failed to be deployed.
+        # *   Partially_Deployed_Success: Some resources of the application are deployed.
+        # *   Deployed_Success: The application is deployed.
+        # *   Destroying: The application is being released.
+        # *   Delayed_Destroy: The application release is delayed.
+        # *   Destroyed_Failure: The application failed to be released.
+        # *   Partially_Destroyed_Success: Some resources of the application are released.
+        # *   Destroyed_Success: The application is released.
+        # *   Revised: The application architecture is adjusted.
+        # *   Verifying_In_Revision: The application resources are being verified during architecture adjustment.
+        # *   Verified_Failure_In_Revision: The application resources failed to pass the verification during architecture adjustment.
+        # *   Verified_Success_In_Revision: The application resources are verified during architecture adjustment.
+        # *   Valuating_In_Revision: Fees are being calculated for the application during architecture adjustment.
+        # *   Valuating_Failure_In_Revision: Fees failed to be calculated for the application during architecture adjustment.
+        # *   Valuating_Success_In_Revision: Fees are calculated for the application during architecture adjustment.
         self.message = message  # type: str
-        # The ID of the request.
+        # The ID of the application.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -1485,19 +1410,16 @@
             temp_model = GetExecuteOperationResultResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetTemplateRequest(TeaModel):
     def __init__(self, region=None, resource_group_id=None, template_id=None):
-        # The region in which the template resides.
         self.region = region  # type: str
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The ID of the template.
         self.template_id = template_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetTemplateRequest, self).to_map()
@@ -1522,17 +1444,21 @@
         if m.get('TemplateId') is not None:
             self.template_id = m.get('TemplateId')
         return self
 
 
 class GetTemplateResponseBodyDataVariables(TeaModel):
     def __init__(self, attribute=None, data_type=None, default_value=None, variable=None):
+        # 变量名
         self.attribute = attribute  # type: str
+        # 变量类型
         self.data_type = data_type  # type: str
+        # 默认值
         self.default_value = default_value  # type: str
+        # 变量值
         self.variable = variable  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetTemplateResponseBodyDataVariables, self).to_map()
@@ -1562,27 +1488,20 @@
             self.variable = m.get('Variable')
         return self
 
 
 class GetTemplateResponseBodyData(TeaModel):
     def __init__(self, create_time=None, description=None, image_url=None, name=None, resource_group_id=None,
                  template_id=None, topo_url=None, variables=None):
-        # The time when the template was created.
         self.create_time = create_time  # type: str
-        # The description of the template.
         self.description = description  # type: str
-        # The URL of the architecture image.
         self.image_url = image_url  # type: str
-        # The name of the template.
         self.name = name  # type: str
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The ID of the template.
         self.template_id = template_id  # type: str
-        # The URL of the architecture image file.
         self.topo_url = topo_url  # type: str
         self.variables = variables  # type: list[GetTemplateResponseBodyDataVariables]
 
     def validate(self):
         if self.variables:
             for k in self.variables:
                 if k:
@@ -1636,21 +1555,17 @@
                 temp_model = GetTemplateResponseBodyDataVariables()
                 self.variables.append(temp_model.from_map(k))
         return self
 
 
 class GetTemplateResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # The HTTP status code.
         self.code = code  # type: int
-        # The details of the template.
         self.data = data  # type: GetTemplateResponseBodyData
-        # The returned message.
         self.message = message  # type: str
-        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.data:
             self.data.validate()
 
     def to_map(self):
@@ -1886,25 +1801,21 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListApplicationRequest(TeaModel):
     def __init__(self, keyword=None, max_results=None, next_token=None, order_type=None, resource_group_id=None,
                  status=None):
-        # The keyword in the application name.
         self.keyword = keyword  # type: str
-        # The number of entries to return on each page.
+        # The HTTP status code.
         self.max_results = max_results  # type: int
-        # The number of the page to return.
+        # The ID of the resource group to which the application belongs.
         self.next_token = next_token  # type: int
-        # The field by which the list is sorted. Valid values: 1 and 2. The value 1 specifies that the list is sorted in descending order of application update time, and the value 2 specifies that the list is sorted in descending order of application creation time.
         self.order_type = order_type  # type: long
-        # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
-        # The status of the application.
         self.status = status  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListApplicationRequest, self).to_map()
@@ -1942,27 +1853,20 @@
             self.status = m.get('Status')
         return self
 
 
 class ListApplicationResponseBodyData(TeaModel):
     def __init__(self, application_id=None, create_time=None, image_url=None, name=None, resource_group_id=None,
                  status=None, topo_url=None):
-        # The ID of the application.
         self.application_id = application_id  # type: str
-        # The time when the application was created.
         self.create_time = create_time  # type: str
-        # The URL of the application architecture image.
         self.image_url = image_url  # type: str
-        # The name of the application.
         self.name = name  # type: str
-        # The ID of the resource group to which the application belongs.
         self.resource_group_id = resource_group_id  # type: str
-        # The status of the application.
         self.status = status  # type: str
-        # The URL of the application topology image.
         self.topo_url = topo_url  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListApplicationResponseBodyData, self).to_map()
@@ -2003,25 +1907,19 @@
         if m.get('TopoURL') is not None:
             self.topo_url = m.get('TopoURL')
         return self
 
 
 class ListApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, next_token=None, request_id=None, total_count=None):
-        # The HTTP status code.
         self.code = code  # type: int
-        # The information about the applications.
         self.data = data  # type: list[ListApplicationResponseBodyData]
-        # The error message.
         self.message = message  # type: str
-        # The page number of the next page.
         self.next_token = next_token  # type: int
-        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The total number of returned applications.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.data:
             for k in self.data:
                 if k:
                     k.validate()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-1.0.3/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-1.0.2/setup.py` & `alibabacloud_bpstudio20210931_py2-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931_py2.
 
-Created on 31/03/2023
+Created on 22/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python2"
```

