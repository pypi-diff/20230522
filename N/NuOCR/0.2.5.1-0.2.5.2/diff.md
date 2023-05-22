# Comparing `tmp/NuOCR-0.2.5.1.tar.gz` & `tmp/NuOCR-0.2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuOCR-0.2.5.1.tar", last modified: Mon May 22 08:26:23 2023, max compression
+gzip compressed data, was "NuOCR-0.2.5.2.tar", last modified: Mon May 22 13:43:08 2023, max compression
```

## Comparing `NuOCR-0.2.5.1.tar` & `NuOCR-0.2.5.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.538197 NuOCR-0.2.5.1/
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:22.771231 NuOCR-0.2.5.1/NuOCR/
--rw-rw-rw-   0        0        0      300 2023-05-22 07:40:04.000000 NuOCR-0.2.5.1/NuOCR/__init__.py
--rw-rw-rw-   0        0        0     3656 2023-05-22 07:40:04.000000 NuOCR-0.2.5.1/NuOCR/admin.py
--rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.5.1/NuOCR/channel.py
--rw-rw-rw-   0        0        0     1815 2023-05-22 07:40:04.000000 NuOCR-0.2.5.1/NuOCR/extractor.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:22.843819 NuOCR-0.2.5.1/NuOCR/gRPC_proto/
--rw-rw-rw-   0        0        0      346 2023-05-22 07:40:04.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:22.899402 NuOCR-0.2.5.1/NuOCR/gRPC_proto/extractor/
--rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/extractor/__init__.py
--rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/extractor/extractor_pb2.py
--rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:22.969236 NuOCR-0.2.5.1/NuOCR/gRPC_proto/io_adaptors/
--rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/io_adaptors/__init__.py
--rw-rw-rw-   0        0        0     6450 2023-05-22 07:40:04.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
--rw-rw-rw-   0        0        0    25493 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.073254 NuOCR-0.2.5.1/NuOCR/gRPC_proto/monitor/
--rw-rw-rw-   0        0        0       61 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/monitor/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/monitor/monitor_pb2.py
--rw-rw-rw-   0        0        0     9283 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.195069 NuOCR-0.2.5.1/NuOCR/gRPC_proto/nufarm_poc/
--rw-rw-rw-   0        0        0       67 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/nufarm_poc/__init__.py
--rw-rw-rw-   0        0        0     1648 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
--rw-rw-rw-   0        0        0     4270 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.308523 NuOCR-0.2.5.1/NuOCR/gRPC_proto/preprocessor/
--rw-rw-rw-   0        0        0       71 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     4074 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
--rw-rw-rw-   0        0        0    13059 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.364904 NuOCR-0.2.5.1/NuOCR/gRPC_proto/templated_flow/
--rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/templated_flow/__init__.py
--rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
--rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.424820 NuOCR-0.2.5.1/NuOCR/gRPC_proto/text_processors/
--rw-rw-rw-   0        0        0       75 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/text_processors/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py
--rw-rw-rw-   0        0        0     8128 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:23.515381 NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/
--rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/auth_pb2.py
--rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
--rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/user_pb2.py
--rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/user_pb2_grpc.py
--rw-rw-rw-   0        0        0    15396 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/io_adaptor.py
--rw-rw-rw-   0        0        0     2820 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/monitor.py
--rw-rw-rw-   0        0        0     5896 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/preprocessors.py
--rw-rw-rw-   0        0        0     2732 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/templated_flow.py
--rw-rw-rw-   0        0        0     2053 2023-05-22 07:40:05.000000 NuOCR-0.2.5.1/NuOCR/text.py
--rw-rw-rw-   0        0        0     2788 2023-05-22 08:26:00.000000 NuOCR-0.2.5.1/NuOCR/user.py
--rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.5.1/NuOCR/util.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:26:22.831638 NuOCR-0.2.5.1/NuOCR.egg-info/
--rw-rw-rw-   0        0        0      540 2023-05-22 08:26:21.000000 NuOCR-0.2.5.1/NuOCR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1563 2023-05-22 08:26:22.000000 NuOCR-0.2.5.1/NuOCR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:26:21.000000 NuOCR-0.2.5.1/NuOCR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 08:26:21.000000 NuOCR-0.2.5.1/NuOCR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 08:26:21.000000 NuOCR-0.2.5.1/NuOCR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      540 2023-05-22 08:26:23.531093 NuOCR-0.2.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 08:26:23.539195 NuOCR-0.2.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1132 2023-05-22 08:26:11.000000 NuOCR-0.2.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:08.025848 NuOCR-0.2.5.2/
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.643066 NuOCR-0.2.5.2/NuOCR/
+-rw-rw-rw-   0        0        0      300 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/admin.py
+-rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/channel.py
+-rw-rw-rw-   0        0        0     1815 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/extractor.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.689137 NuOCR-0.2.5.2/NuOCR/gRPC_proto/
+-rw-rw-rw-   0        0        0      346 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.724430 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/
+-rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/__init__.py
+-rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2.py
+-rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.761884 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/
+-rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/__init__.py
+-rw-rw-rw-   0        0        0     6450 2023-05-22 07:40:04.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
+-rw-rw-rw-   0        0        0    25493 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.800615 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/
+-rw-rw-rw-   0        0        0       61 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2.py
+-rw-rw-rw-   0        0        0     9283 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.833600 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/
+-rw-rw-rw-   0        0        0       67 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/__init__.py
+-rw-rw-rw-   0        0        0     1648 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
+-rw-rw-rw-   0        0        0     4270 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.867123 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/
+-rw-rw-rw-   0        0        0       71 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4074 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
+-rw-rw-rw-   0        0        0    13059 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.904038 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/
+-rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
+-rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.944373 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/
+-rw-rw-rw-   0        0        0       75 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py
+-rw-rw-rw-   0        0        0     8128 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:08.010361 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/
+-rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2.py
+-rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2.py
+-rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15396 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/io_adaptor.py
+-rw-rw-rw-   0        0        0     2820 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/monitor.py
+-rw-rw-rw-   0        0        0     5896 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/preprocessors.py
+-rw-rw-rw-   0        0        0     2779 2023-05-22 13:42:36.000000 NuOCR-0.2.5.2/NuOCR/templated_flow.py
+-rw-rw-rw-   0        0        0     2053 2023-05-22 07:40:05.000000 NuOCR-0.2.5.2/NuOCR/text.py
+-rw-rw-rw-   0        0        0     2788 2023-05-22 08:26:00.000000 NuOCR-0.2.5.2/NuOCR/user.py
+-rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.5.2/NuOCR/util.py
+drwxrwxrwx   0        0        0        0 2023-05-22 13:43:07.681228 NuOCR-0.2.5.2/NuOCR.egg-info/
+-rw-rw-rw-   0        0        0      540 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1563 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 13:43:07.000000 NuOCR-0.2.5.2/NuOCR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      540 2023-05-22 13:43:08.020287 NuOCR-0.2.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 13:43:08.025848 NuOCR-0.2.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2023-05-22 13:43:04.000000 NuOCR-0.2.5.2/setup.py
```

### Comparing `NuOCR-0.2.5.1/NuOCR/admin.py` & `NuOCR-0.2.5.2/NuOCR/admin.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/extractor.py` & `NuOCR-0.2.5.2/NuOCR/extractor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/extractor/extractor_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/monitor/monitor_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/auth_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/auth_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/user_pb2.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/gRPC_proto/user/user_pb2_grpc.py` & `NuOCR-0.2.5.2/NuOCR/gRPC_proto/user/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/io_adaptor.py` & `NuOCR-0.2.5.2/NuOCR/io_adaptor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/monitor.py` & `NuOCR-0.2.5.2/NuOCR/monitor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/preprocessors.py` & `NuOCR-0.2.5.2/NuOCR/preprocessors.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/templated_flow.py` & `NuOCR-0.2.5.2/NuOCR/templated_flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,22 +36,23 @@
                           'name': i.documentName,
                           'base64': i.base64,
                           'mimeType': i.mimeType} for i in response]
             return list_data
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
-    def extractTemplate(self, documentName, documentId, base64, fileName, readStatus=True):
+    def extractTemplate(self, documentName, documentId, base64, fileName, readStatus=True, rawJson=True):
         try:
             request = templated_flow_pb2.ExtractRequest(
                 documentId=documentId,
                 documentName=documentName,
                 base64=base64,
                 fileName=fileName,
                 readStatus=readStatus,
+                rawJson=rawJson
             )
             response = self.stub.Extract(request, metadata=self.metadata)
             return json.loads(response.response)
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
     def deleteTemplate(self, documentName, documentId):
```

### Comparing `NuOCR-0.2.5.1/NuOCR/text.py` & `NuOCR-0.2.5.2/NuOCR/text.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR/user.py` & `NuOCR-0.2.5.2/NuOCR/user.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/NuOCR.egg-info/PKG-INFO` & `NuOCR-0.2.5.2/NuOCR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.5.1
+Version: 0.2.5.2
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.5.1/NuOCR.egg-info/SOURCES.txt` & `NuOCR-0.2.5.2/NuOCR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/PKG-INFO` & `NuOCR-0.2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.5.1
+Version: 0.2.5.2
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.5.1/README.md` & `NuOCR-0.2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.5.1/setup.py` & `NuOCR-0.2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.2.5.1'
+VERSION = '0.2.5.2'
 DESCRIPTION = 'Using NuOCR service via APIs'
 LONG_DESCRIPTION = 'A package that allows to utilize NuOCR sevices through API implementation.'
 
 # Setting up
 setup(
     name="NuOCR",
     version=VERSION,
```

