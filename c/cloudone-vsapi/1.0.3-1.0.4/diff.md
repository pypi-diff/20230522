# Comparing `tmp/cloudone-vsapi-1.0.3.tar.gz` & `tmp/cloudone-vsapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudone-vsapi-1.0.3.tar", last modified: Thu May 11 05:31:11 2023, max compression
+gzip compressed data, was "cloudone-vsapi-1.0.4.tar", last modified: Mon May 22 17:03:45 2023, max compression
```

## Comparing `cloudone-vsapi-1.0.3.tar` & `cloudone-vsapi-1.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/grpc/aio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/amaas/grpc/exception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.977561 cloudone-vsapi-1.0.3/amaas/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-11 05:31:10.000000 cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-11 05:31:10.000000 cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-11 05:31:10.000000 cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-11 05:31:11.000000 cloudone-vsapi-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 05:31:11.981561 cloudone-vsapi-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 05:29:46.000000 cloudone-vsapi-1.0.3/tests/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.325703 cloudone-vsapi-1.0.4/amaas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/amaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/amaas/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.325703 cloudone-vsapi-1.0.4/amaas/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/amaas/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/amaas/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/amaas/grpc/aio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/amaas/grpc/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/amaas/grpc/exception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/amaas/grpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-22 17:03:43.000000 cloudone-vsapi-1.0.4/amaas/grpc/protos/scan_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-22 17:03:43.000000 cloudone-vsapi-1.0.4/amaas/grpc/protos/scan_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-22 17:03:43.000000 cloudone-vsapi-1.0.4/amaas/grpc/protos/scan_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-22 17:03:45.000000 cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-22 17:03:45.000000 cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:03:45.000000 cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 17:03:45.000000 cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 17:03:45.000000 cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-22 17:03:44.000000 cloudone-vsapi-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:03:45.329703 cloudone-vsapi-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 17:02:17.000000 cloudone-vsapi-1.0.4/tests/test_simple.py
```

### Comparing `cloudone-vsapi-1.0.3/LICENSE` & `cloudone-vsapi-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.3/PKG-INFO` & `cloudone-vsapi-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudone-vsapi-1.0.3/README.md` & `cloudone-vsapi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.3/amaas/grpc/__init__.py` & `cloudone-vsapi-1.0.4/amaas/grpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 LOG_LEVEL = os.environ.get('LOG_LEVEL', 'INFO')
 logger.setLevel(LOG_LEVEL)
 logger.propagate = False
 
+timeout_in_seconds = 180
+
 
 class Pipeline:
     """
     Class to allow a single element pipeline between producer and consumer.
     """
 
     def __init__(self):
@@ -139,15 +141,15 @@
 def scan_data(data_reader: BinaryIO, size: int, identifier: str, channel: grpc.Channel) -> str:
     stub = scan_pb2_grpc.ScanStub(channel)
     pipeline = Pipeline()
     stats = {}
     result = None
 
     try:
-        responses = stub.Run(generate_messages(pipeline, data_reader, stats))
+        responses = stub.Run(generate_messages(pipeline, data_reader, stats), timeout=timeout_in_seconds)
         message = scan_pb2.C2S(stage=scan_pb2.STAGE_INIT,
                                file_name=identifier,
                                rs_size=size,
                                offset=0,
                                chunk=None)
 
         pipeline.set_message(message)
```

### Comparing `cloudone-vsapi-1.0.3/amaas/grpc/aio/__init__.py` & `cloudone-vsapi-1.0.4/amaas/grpc/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.StreamHandler())
 LOG_LEVEL = os.environ.get('LOG_LEVEL', 'INFO')
 logger.setLevel(LOG_LEVEL)
 logger.propagate = False
 
+timeout_in_seconds = 180
+
 
 def init(host, api_key=None, enable_tls=False, ca_cert=None):
     call_creds = None
     if api_key:
         match = re.search(r'ey[^.]+.ey[^.]+.ey[^.]+', api_key)
         if match:
             str = 'Bearer ' + api_key
@@ -81,15 +83,15 @@
 
 
 async def scan_data(data_reader: BinaryIO, size: int, identifier: str, channel: grpc.Channel) -> str:
     stub = scan_pb2_grpc.ScanStub(channel)
     stats = {}
     result = None
     try:
-        call = stub.Run()
+        call = stub.Run(timeout=timeout_in_seconds)
 
         request = scan_pb2.C2S(stage=scan_pb2.STAGE_INIT,
                                file_name=identifier,
                                rs_size=size,
                                offset=0,
                                chunk=None)
```

### Comparing `cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.py` & `cloudone-vsapi-1.0.4/amaas/grpc/protos/scan_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2.pyi` & `cloudone-vsapi-1.0.4/amaas/grpc/protos/scan_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.3/amaas/grpc/protos/scan_pb2_grpc.py` & `cloudone-vsapi-1.0.4/amaas/grpc/protos/scan_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudone-vsapi-1.0.3/cloudone_vsapi.egg-info/PKG-INFO` & `cloudone-vsapi-1.0.4/cloudone_vsapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudone-vsapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: Trend Micro Cloud One VSAPI SDK for python
 Home-page: https://github.com/trendmicro/cloudone-antimalware-python-sdk
 Author: Trend Micro Cloud One Team
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudone-vsapi-1.0.3/setup.py` & `cloudone-vsapi-1.0.4/setup.py`

 * *Files identical despite different names*

