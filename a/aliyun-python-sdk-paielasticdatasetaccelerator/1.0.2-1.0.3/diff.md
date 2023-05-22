# Comparing `tmp/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2.tar.gz` & `tmp/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2.tar", last modified: Mon May 22 11:42:55 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3.tar", last modified: Mon May 22 12:07:57 2023, max compression
```

## Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2.tar` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1662 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2569 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/
--rw-r--r--   0 root         (0) root         (0)     1459 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2657 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3039 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2469 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2577 2023-05-22 11:42:55.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-05-22 12:07:57.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/setup.py
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/LICENSE` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/PKG-INFO` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-paielasticdatasetaccelerator
-Version: 1.0.2
+Version: 1.0.3
 Summary: The paielasticdatasetaccelerator module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-paielasticdatasetaccelerator
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/README.rst` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-paielasticdatasetaccelerator
-Version: 1.0.2
+Version: 1.0.3
 Summary: The paielasticdatasetaccelerator module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-paielasticdatasetaccelerator
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.2/setup.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.3/setup.py`

 * *Files identical despite different names*

