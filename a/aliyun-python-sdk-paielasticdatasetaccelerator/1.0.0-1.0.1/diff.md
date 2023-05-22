# Comparing `tmp/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0.tar.gz` & `tmp/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0.tar", last modified: Tue Jan  3 13:29:03 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1.tar", last modified: Mon May 22 06:43:59 2023, max compression
```

## Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0.tar` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      575 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1662 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      577 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1662 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2488 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/
--rw-r--r--   0 root         (0) root         (0)       21 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/
--rw-r--r--   0 root         (0) root         (0)     1459 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2651 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2469 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2577 2023-01-03 13:29:03.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      577 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3039 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2469 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1436 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-22 06:43:59.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-05-22 06:43:58.000000 aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/setup.py
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/LICENSE` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/PKG-INFO` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-paielasticdatasetaccelerator
-Version: 1.0.0
+Version: 1.0.1
 Summary: The paielasticdatasetaccelerator module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-paielasticdatasetaccelerator
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/README.rst` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-paielasticdatasetaccelerator
-Version: 1.0.0
+Version: 1.0.1
 Summary: The paielasticdatasetaccelerator module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-paielasticdatasetaccelerator
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyun_python_sdk_paielasticdatasetaccelerator.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 aliyunsdkpaielasticdatasetaccelerator/__init__.py
 aliyunsdkpaielasticdatasetaccelerator/request/__init__.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py
+aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteEndpointRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py
 aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/BindEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/CreateTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DeleteTagRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeComponentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/DescribeSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListComponentsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListEndpointsRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 		self.set_method('GET')
 
 	def get_SlotIds(self): # String
 		return self.get_query_params().get('SlotIds')
 
 	def set_SlotIds(self, SlotIds):  # String
 		self.add_query_param('SlotIds', SlotIds)
+	def get_InstanceIds(self): # String
+		return self.get_query_params().get('InstanceIds')
+
+	def set_InstanceIds(self, InstanceIds):  # String
+		self.add_query_param('InstanceIds', InstanceIds)
 	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
 	def set_Name(self, Name):  # String
 		self.add_query_param('Name', Name)
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListSlotsRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,24 +22,39 @@
 class ListSlotsRequest(RoaRequest):
 
 	def __init__(self):
 		RoaRequest.__init__(self, 'PAIElasticDatasetAccelerator', '2022-08-01', 'ListSlots','datasetacc')
 		self.set_uri_pattern('/api/v1/slots')
 		self.set_method('GET')
 
-	def get_SlotIds(self): # String
-		return self.get_query_params().get('SlotIds')
-
-	def set_SlotIds(self, SlotIds):  # String
-		self.add_query_param('SlotIds', SlotIds)
 	def get_Phase(self): # String
 		return self.get_query_params().get('Phase')
 
 	def set_Phase(self, Phase):  # String
 		self.add_query_param('Phase', Phase)
+	def get_StorageType(self): # String
+		return self.get_query_params().get('StorageType')
+
+	def set_StorageType(self, StorageType):  # String
+		self.add_query_param('StorageType', StorageType)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_EndpointIds(self): # String
+		return self.get_query_params().get('EndpointIds')
+
+	def set_EndpointIds(self, EndpointIds):  # String
+		self.add_query_param('EndpointIds', EndpointIds)
+	def get_SlotIds(self): # String
+		return self.get_query_params().get('SlotIds')
+
+	def set_SlotIds(self, SlotIds):  # String
+		self.add_query_param('SlotIds', SlotIds)
 	def get_InstanceIds(self): # String
 		return self.get_query_params().get('InstanceIds')
 
 	def set_InstanceIds(self, InstanceIds):  # String
 		self.add_query_param('InstanceIds', InstanceIds)
 	def get_Name(self): # String
 		return self.get_query_params().get('Name')
@@ -52,22 +67,17 @@
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
 	def get_SortBy(self): # String
 		return self.get_query_params().get('SortBy')
 
 	def set_SortBy(self, SortBy):  # String
 		self.add_query_param('SortBy', SortBy)
-	def get_StorageType(self): # String
-		return self.get_query_params().get('StorageType')
+	def get_StorageUri(self): # String
+		return self.get_query_params().get('StorageUri')
 
-	def set_StorageType(self, StorageType):  # String
-		self.add_query_param('StorageType', StorageType)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
+	def set_StorageUri(self, StorageUri):  # String
+		self.add_query_param('StorageUri', StorageUri)
 	def get_Order(self): # String
 		return self.get_query_params().get('Order')
 
 	def set_Order(self, Order):  # String
 		self.add_query_param('Order', Order)
```

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/ListTagsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryInstanceMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QuerySlotMetricsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/QueryStatisticRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/StopSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UnbindEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/aliyunsdkpaielasticdatasetaccelerator/request/v20220801/UpdateSlotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.0/setup.py` & `aliyun-python-sdk-paielasticdatasetaccelerator-1.0.1/setup.py`

 * *Files identical despite different names*

