# Comparing `tmp/NuOCR-0.2.4.tar.gz` & `tmp/NuOCR-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NuOCR-0.2.4.tar", last modified: Fri May 19 09:41:04 2023, max compression
+gzip compressed data, was "NuOCR-0.2.5.tar", last modified: Mon May 22 06:08:03 2023, max compression
```

## Comparing `NuOCR-0.2.4.tar` & `NuOCR-0.2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.676029 NuOCR-0.2.4/
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.115605 NuOCR-0.2.4/NuOCR/
--rw-rw-rw-   0        0        0      300 2023-05-18 07:54:08.000000 NuOCR-0.2.4/NuOCR/__init__.py
--rw-rw-rw-   0        0        0     3656 2023-05-18 07:04:32.000000 NuOCR-0.2.4/NuOCR/admin.py
--rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.4/NuOCR/channel.py
--rw-rw-rw-   0        0        0     1815 2023-05-17 09:02:23.000000 NuOCR-0.2.4/NuOCR/extractor.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.236421 NuOCR-0.2.4/NuOCR/gRPC_proto/
--rw-rw-rw-   0        0        0      346 2023-05-19 09:40:44.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.301581 NuOCR-0.2.4/NuOCR/gRPC_proto/extractor/
--rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/extractor/__init__.py
--rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/extractor/extractor_pb2.py
--rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.365364 NuOCR-0.2.4/NuOCR/gRPC_proto/io_adaptors/
--rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/io_adaptors/__init__.py
--rw-rw-rw-   0        0        0     6399 2023-05-18 07:55:42.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
--rw-rw-rw-   0        0        0    24998 2023-05-19 09:40:44.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.415204 NuOCR-0.2.4/NuOCR/gRPC_proto/monitor/
--rw-rw-rw-   0        0        0       61 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/monitor/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-04-05 17:01:43.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/monitor/monitor_pb2.py
--rw-rw-rw-   0        0        0     9283 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.457087 NuOCR-0.2.4/NuOCR/gRPC_proto/nufarm_poc/
--rw-rw-rw-   0        0        0       67 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/nufarm_poc/__init__.py
--rw-rw-rw-   0        0        0     1617 2023-01-30 11:12:08.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
--rw-rw-rw-   0        0        0     4171 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.500510 NuOCR-0.2.4/NuOCR/gRPC_proto/preprocessor/
--rw-rw-rw-   0        0        0       71 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     4074 2023-05-17 08:12:10.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
--rw-rw-rw-   0        0        0    13059 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.540008 NuOCR-0.2.4/NuOCR/gRPC_proto/templated_flow/
--rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/templated_flow/__init__.py
--rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
--rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.581172 NuOCR-0.2.4/NuOCR/gRPC_proto/text_processors/
--rw-rw-rw-   0        0        0       75 2023-03-27 09:59:58.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/text_processors/__init__.py
--rw-rw-rw-   0        0        0     2413 2023-04-25 06:16:53.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py
--rw-rw-rw-   0        0        0     8128 2023-05-17 08:56:56.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.652215 NuOCR-0.2.4/NuOCR/gRPC_proto/user/
--rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/user/__init__.py
--rw-rw-rw-   0        0        0     1414 2023-04-25 06:16:53.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/user/auth_pb2.py
--rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
--rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/user/user_pb2.py
--rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.4/NuOCR/gRPC_proto/user/user_pb2_grpc.py
--rw-rw-rw-   0        0        0    15388 2023-05-17 11:23:10.000000 NuOCR-0.2.4/NuOCR/io_adaptor.py
--rw-rw-rw-   0        0        0     2820 2023-05-17 11:55:52.000000 NuOCR-0.2.4/NuOCR/monitor.py
--rw-rw-rw-   0        0        0     5896 2023-05-18 07:54:08.000000 NuOCR-0.2.4/NuOCR/preprocessors.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 11:27:14.000000 NuOCR-0.2.4/NuOCR/templated_flow.py
--rw-rw-rw-   0        0        0     2053 2023-05-19 09:40:44.000000 NuOCR-0.2.4/NuOCR/text.py
--rw-rw-rw-   0        0        0     2314 2023-05-17 12:39:27.000000 NuOCR-0.2.4/NuOCR/user.py
--rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.4/NuOCR/util.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:41:04.218446 NuOCR-0.2.4/NuOCR.egg-info/
--rw-rw-rw-   0        0        0      538 2023-05-19 09:41:02.000000 NuOCR-0.2.4/NuOCR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1563 2023-05-19 09:41:03.000000 NuOCR-0.2.4/NuOCR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 09:41:02.000000 NuOCR-0.2.4/NuOCR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-19 09:41:02.000000 NuOCR-0.2.4/NuOCR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-19 09:41:02.000000 NuOCR-0.2.4/NuOCR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      538 2023-05-19 09:41:04.668175 NuOCR-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 09:41:04.677536 NuOCR-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1130 2023-05-19 09:40:54.000000 NuOCR-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:03.066626 NuOCR-0.2.5/
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.591370 NuOCR-0.2.5/NuOCR/
+-rw-rw-rw-   0        0        0      300 2023-05-18 07:54:08.000000 NuOCR-0.2.5/NuOCR/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-05-18 07:04:32.000000 NuOCR-0.2.5/NuOCR/admin.py
+-rw-rw-rw-   0        0        0      235 2023-03-27 09:59:57.000000 NuOCR-0.2.5/NuOCR/channel.py
+-rw-rw-rw-   0        0        0     1815 2023-05-17 09:02:23.000000 NuOCR-0.2.5/NuOCR/extractor.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.650900 NuOCR-0.2.5/NuOCR/gRPC_proto/
+-rw-rw-rw-   0        0        0      346 2023-05-19 09:40:44.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.692880 NuOCR-0.2.5/NuOCR/gRPC_proto/extractor/
+-rw-rw-rw-   0        0        0       65 2023-03-27 09:59:57.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/extractor/__init__.py
+-rw-rw-rw-   0        0        0     3683 2022-12-13 12:07:32.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/extractor/extractor_pb2.py
+-rw-rw-rw-   0        0        0     9046 2023-05-17 08:54:24.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.743189 NuOCR-0.2.5/NuOCR/gRPC_proto/io_adaptors/
+-rw-rw-rw-   0        0        0       69 2023-03-27 09:59:57.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/io_adaptors/__init__.py
+-rw-rw-rw-   0        0        0     6399 2023-05-18 07:55:42.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py
+-rw-rw-rw-   0        0        0    24998 2023-05-19 09:40:44.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.790032 NuOCR-0.2.5/NuOCR/gRPC_proto/monitor/
+-rw-rw-rw-   0        0        0       61 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/monitor/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-04-05 17:01:43.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/monitor/monitor_pb2.py
+-rw-rw-rw-   0        0        0     9283 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.834378 NuOCR-0.2.5/NuOCR/gRPC_proto/nufarm_poc/
+-rw-rw-rw-   0        0        0       67 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/nufarm_poc/__init__.py
+-rw-rw-rw-   0        0        0     1617 2023-01-30 11:12:08.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py
+-rw-rw-rw-   0        0        0     4171 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.879362 NuOCR-0.2.5/NuOCR/gRPC_proto/preprocessor/
+-rw-rw-rw-   0        0        0       71 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4074 2023-05-17 08:12:10.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py
+-rw-rw-rw-   0        0        0    13059 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.923834 NuOCR-0.2.5/NuOCR/gRPC_proto/templated_flow/
+-rw-rw-rw-   0        0        0       75 2023-03-27 09:59:57.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/templated_flow/__init__.py
+-rw-rw-rw-   0        0        0     3375 2023-03-27 10:00:02.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py
+-rw-rw-rw-   0        0        0     8097 2023-05-17 08:55:07.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.967008 NuOCR-0.2.5/NuOCR/gRPC_proto/text_processors/
+-rw-rw-rw-   0        0        0       75 2023-03-27 09:59:58.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/text_processors/__init__.py
+-rw-rw-rw-   0        0        0     2413 2023-04-25 06:16:53.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py
+-rw-rw-rw-   0        0        0     8128 2023-05-17 08:56:56.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:03.047022 NuOCR-0.2.5/NuOCR/gRPC_proto/user/
+-rw-rw-rw-   0        0        0      110 2023-03-27 09:59:58.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/user/__init__.py
+-rw-rw-rw-   0        0        0     1414 2023-04-25 06:16:53.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/user/auth_pb2.py
+-rw-rw-rw-   0        0        0     2474 2023-05-17 08:55:25.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/user/auth_pb2_grpc.py
+-rw-rw-rw-   0        0        0     4332 2023-03-27 10:00:02.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/user/user_pb2.py
+-rw-rw-rw-   0        0        0    22705 2023-05-17 08:55:31.000000 NuOCR-0.2.5/NuOCR/gRPC_proto/user/user_pb2_grpc.py
+-rw-rw-rw-   0        0        0    15396 2023-05-19 10:10:48.000000 NuOCR-0.2.5/NuOCR/io_adaptor.py
+-rw-rw-rw-   0        0        0     2820 2023-05-17 11:55:52.000000 NuOCR-0.2.5/NuOCR/monitor.py
+-rw-rw-rw-   0        0        0     5896 2023-05-18 07:54:08.000000 NuOCR-0.2.5/NuOCR/preprocessors.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 11:27:14.000000 NuOCR-0.2.5/NuOCR/templated_flow.py
+-rw-rw-rw-   0        0        0     2053 2023-05-19 09:40:44.000000 NuOCR-0.2.5/NuOCR/text.py
+-rw-rw-rw-   0        0        0     2459 2023-05-22 06:06:20.000000 NuOCR-0.2.5/NuOCR/user.py
+-rw-rw-rw-   0        0        0      334 2023-03-27 09:59:59.000000 NuOCR-0.2.5/NuOCR/util.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:08:02.640708 NuOCR-0.2.5/NuOCR.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-05-22 06:08:00.000000 NuOCR-0.2.5/NuOCR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1563 2023-05-22 06:08:01.000000 NuOCR-0.2.5/NuOCR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:08:00.000000 NuOCR-0.2.5/NuOCR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 06:08:00.000000 NuOCR-0.2.5/NuOCR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 06:08:00.000000 NuOCR-0.2.5/NuOCR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      538 2023-05-22 06:08:03.061188 NuOCR-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4053 2023-03-27 09:59:59.000000 NuOCR-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:08:03.067622 NuOCR-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2023-05-22 06:07:52.000000 NuOCR-0.2.5/setup.py
```

### Comparing `NuOCR-0.2.4/NuOCR/admin.py` & `NuOCR-0.2.5/NuOCR/admin.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/extractor.py` & `NuOCR-0.2.5/NuOCR/extractor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/extractor/extractor_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/extractor/extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/extractor/extractor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/io_adaptors/io_adaptors_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/monitor/monitor_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/monitor/monitor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/monitor/monitor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/nufarm_poc/nufarm_poc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/preprocessor/preprocessor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/templated_flow/templated_flow_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/text_processors/text_processor_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/text_processors/text_processor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/user/auth_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/user/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/user/auth_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/user/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/user/user_pb2.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/user/user_pb2.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/gRPC_proto/user/user_pb2_grpc.py` & `NuOCR-0.2.5/NuOCR/gRPC_proto/user/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/io_adaptor.py` & `NuOCR-0.2.5/NuOCR/io_adaptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     def __init__(self, metadata, email_username, email_password, email_server):
         self.stub = io_adaptors_pb2_grpc.IOAdaptorControllerStub(CHANNEL)
         self.metadata = metadata
         self.email_username = email_username
         self.email_password = email_password
         self.email_server = email_server
 
-    def inbound(self, email_folder, email_filter="UNSEEN"):
+    def inbound(self, email_folder="INBOX", email_filter="UNSEEN"):
         try:
             request = io_adaptors_pb2.EmailOutBoundRequest(email_username=self.email_username,
                                                            email_password=self.email_password,
                                                            email_server=self.email_server, email_folder=email_folder,
                                                            email_filter=email_filter)
             response = self.stub.EmailInBound(request, metadata=self.metadata)
             lst_response = []
```

### Comparing `NuOCR-0.2.4/NuOCR/monitor.py` & `NuOCR-0.2.5/NuOCR/monitor.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/preprocessors.py` & `NuOCR-0.2.5/NuOCR/preprocessors.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/templated_flow.py` & `NuOCR-0.2.5/NuOCR/templated_flow.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/text.py` & `NuOCR-0.2.5/NuOCR/text.py`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/NuOCR/user.py` & `NuOCR-0.2.5/NuOCR/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import json
 import grpc
 from .channel import CHANNEL
 from .gRPC_proto.user import user_pb2, user_pb2_grpc, auth_pb2_grpc, auth_pb2
 
 
 class User:
-    def __init__(self, username, password):
+    def __init__(self, username=None, password=None, metadata=None):
         self.stub = user_pb2_grpc.UserControllerStub(CHANNEL)
         self.auth_stub = auth_pb2_grpc.AuthenticationStub(CHANNEL)
         self.username = username
         self.password = password
+        self.metadata = metadata
 
     def change_password(self, new_password):
         try:
             response = self.stub.ChangePassword(
                 user_pb2.PasswordRequest(username=self.username, password=self.password,
                                          new_password=new_password))
             return response
@@ -46,11 +47,13 @@
                     ('username', response['username'])]
             return meta
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
 
     def dropdown(self):
         try:
-            response = self.stub.DropDown(user_pb2.UserListRequest(), metadata=self.login())
+            if self.metadata is None:
+                self.metadata = self.login()
+            response = self.stub.DropDown(user_pb2.UserListRequest(), metadata=self.metadata)
             return response.option
         except grpc.RpcError as e:
             raise Exception('Error ' + str(e.code()) + ': ' + str(e.details()))
```

### Comparing `NuOCR-0.2.4/NuOCR.egg-info/PKG-INFO` & `NuOCR-0.2.5/NuOCR.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.4
+Version: 0.2.5
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.4/NuOCR.egg-info/SOURCES.txt` & `NuOCR-0.2.5/NuOCR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/PKG-INFO` & `NuOCR-0.2.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NuOCR
-Version: 0.2.4
+Version: 0.2.5
 Summary: Using NuOCR service via APIs
 Author: Nuvento Systems Pvt. Ltd. (Jigar Makwana)
 Author-email: <makwana.jigar@nuvento.com>
 Keywords: python,NuOCR,OCR
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NuOCR-0.2.4/README.md` & `NuOCR-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `NuOCR-0.2.4/setup.py` & `NuOCR-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.2.4'
+VERSION = '0.2.5'
 DESCRIPTION = 'Using NuOCR service via APIs'
 LONG_DESCRIPTION = 'A package that allows to utilize NuOCR sevices through API implementation.'
 
 # Setting up
 setup(
     name="NuOCR",
     version=VERSION,
```

