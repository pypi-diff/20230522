# Comparing `tmp/HolisticTraceAnalysis-0.1.3.tar.gz` & `tmp/HolisticTraceAnalysis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HolisticTraceAnalysis-0.1.3.tar", last modified: Fri Feb 10 01:07:30 2023, max compression
+gzip compressed data, was "HolisticTraceAnalysis-0.2.0.tar", last modified: Mon May 22 18:55:24 2023, max compression
```

## Comparing `HolisticTraceAnalysis-0.1.3.tar` & `HolisticTraceAnalysis-0.2.0.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.332898 HolisticTraceAnalysis-0.1.3/
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.257590 HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/
--rw-r--r--   0 anupamb    (501) staff       (20)      683 2023-02-10 01:07:30.000000 HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 anupamb    (501) staff       (20)     1148 2023-02-10 01:07:30.000000 HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 anupamb    (501) staff       (20)        1 2023-02-10 01:07:30.000000 HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 anupamb    (501) staff       (20)       61 2023-02-10 01:07:30.000000 HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/requires.txt
--rw-r--r--   0 anupamb    (501) staff       (20)        4 2023-02-10 01:07:30.000000 HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/top_level.txt
--rw-r--r--   0 anupamb    (501) staff       (20)     1088 2022-12-06 23:02:22.000000 HolisticTraceAnalysis-0.1.3/LICENSE
--rw-r--r--   0 anupamb    (501) staff       (20)      121 2023-01-07 01:16:49.000000 HolisticTraceAnalysis-0.1.3/MANIFEST.in
--rw-r--r--   0 anupamb    (501) staff       (20)      683 2023-02-10 01:07:30.332980 HolisticTraceAnalysis-0.1.3/PKG-INFO
--rw-r--r--   0 anupamb    (501) staff       (20)     6952 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/README.md
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.260248 HolisticTraceAnalysis-0.1.3/docs/
--rw-r--r--   0 anupamb    (501) staff       (20)     3030 2022-12-14 22:16:54.000000 HolisticTraceAnalysis-0.1.3/docs/conf.py
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.269562 HolisticTraceAnalysis-0.1.3/hta/
--rw-r--r--   0 anupamb    (501) staff       (20)      100 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/__init__.py
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.290241 HolisticTraceAnalysis-0.1.3/hta/analyzers/
--rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/__init__.py
--rw-r--r--   0 anupamb    (501) staff       (20)    22410 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/breakdown_analysis.py
--rw-r--r--   0 anupamb    (501) staff       (20)     3889 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/communication_analysis.py
--rw-r--r--   0 anupamb    (501) staff       (20)    17560 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/cuda_kernel_analysis.py
--rw-r--r--   0 anupamb    (501) staff       (20)    11565 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/straggler.py
--rw-r--r--   0 anupamb    (501) staff       (20)     2719 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/straggler_analysis.py
--rw-r--r--   0 anupamb    (501) staff       (20)     8330 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/timeline.py
--rw-r--r--   0 anupamb    (501) staff       (20)    11664 2023-02-09 20:02:24.000000 HolisticTraceAnalysis-0.1.3/hta/analyzers/trace_counters.py
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.298373 HolisticTraceAnalysis-0.1.3/hta/common/
--rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/common/__init__.py
--rw-r--r--   0 anupamb    (501) staff       (20)    16783 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/common/call_stack.py
--rw-r--r--   0 anupamb    (501) staff       (20)    27448 2023-02-09 20:02:24.000000 HolisticTraceAnalysis-0.1.3/hta/common/trace.py
--rw-r--r--   0 anupamb    (501) staff       (20)     6067 2023-01-13 02:52:28.000000 HolisticTraceAnalysis-0.1.3/hta/common/trace_file.py
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.307654 HolisticTraceAnalysis-0.1.3/hta/configs/
--rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/configs/__init__.py
--rw-r--r--   0 anupamb    (501) staff       (20)     5111 2023-01-07 01:16:49.000000 HolisticTraceAnalysis-0.1.3/hta/configs/config.py
--rw-r--r--   0 anupamb    (501) staff       (20)      453 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/configs/default_values.py
--rw-r--r--   0 anupamb    (501) staff       (20)      434 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/configs/logging.config
--rw-r--r--   0 anupamb    (501) staff       (20)      203 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/configs/trace_analyzer.json
--rw-r--r--   0 anupamb    (501) staff       (20)    23273 2023-02-09 20:02:24.000000 HolisticTraceAnalysis-0.1.3/hta/trace_analysis.py
--rw-r--r--   0 anupamb    (501) staff       (20)    20923 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/hta/trace_diff.py
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.311616 HolisticTraceAnalysis-0.1.3/hta/utils/
--rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/utils/__init__.py
--rw-r--r--   0 anupamb    (501) staff       (20)     4975 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.1.3/hta/utils/utils.py
--rw-r--r--   0 anupamb    (501) staff       (20)      208 2023-02-10 00:38:00.000000 HolisticTraceAnalysis-0.1.3/hta/version.py
--rw-r--r--   0 anupamb    (501) staff       (20)      293 2022-12-14 01:56:02.000000 HolisticTraceAnalysis-0.1.3/pyproject.toml
--rw-r--r--   0 anupamb    (501) staff       (20)      102 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/requirements.txt
--rw-r--r--   0 anupamb    (501) staff       (20)      258 2023-02-10 01:07:30.333539 HolisticTraceAnalysis-0.1.3/setup.cfg
--rw-r--r--   0 anupamb    (501) staff       (20)     1271 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/setup.py
-drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-02-10 01:07:30.332353 HolisticTraceAnalysis-0.1.3/tests/
--rw-r--r--   0 anupamb    (501) staff       (20)     4235 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/tests/test_call_stack.py
--rw-r--r--   0 anupamb    (501) staff       (20)     2951 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/tests/test_config.py
--rw-r--r--   0 anupamb    (501) staff       (20)      968 2022-12-14 22:16:15.000000 HolisticTraceAnalysis-0.1.3/tests/test_correlation.py
--rw-r--r--   0 anupamb    (501) staff       (20)     2559 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/tests/test_symbol_table.py
--rw-r--r--   0 anupamb    (501) staff       (20)    11678 2023-02-09 20:02:24.000000 HolisticTraceAnalysis-0.1.3/tests/test_trace_analysis.py
--rw-r--r--   0 anupamb    (501) staff       (20)     7053 2022-12-14 22:16:03.000000 HolisticTraceAnalysis-0.1.3/tests/test_trace_diff.py
--rw-r--r--   0 anupamb    (501) staff       (20)     2977 2023-01-13 02:52:28.000000 HolisticTraceAnalysis-0.1.3/tests/test_trace_file.py
--rw-r--r--   0 anupamb    (501) staff       (20)     4597 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.1.3/tests/test_trace_parse.py
--rw-r--r--   0 anupamb    (501) staff       (20)     1009 2022-12-14 22:16:42.000000 HolisticTraceAnalysis-0.1.3/tests/test_trace_utils.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.702610 HolisticTraceAnalysis-0.2.0/
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.668856 HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/
+-rw-r--r--   0 anupamb    (501) staff       (20)      683 2023-05-22 18:55:24.000000 HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 anupamb    (501) staff       (20)     1188 2023-05-22 18:55:24.000000 HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 anupamb    (501) staff       (20)        1 2023-05-22 18:55:24.000000 HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 anupamb    (501) staff       (20)       61 2023-05-22 18:55:24.000000 HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/requires.txt
+-rw-r--r--   0 anupamb    (501) staff       (20)        4 2023-05-22 18:55:24.000000 HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 anupamb    (501) staff       (20)     1088 2022-12-06 23:02:22.000000 HolisticTraceAnalysis-0.2.0/LICENSE
+-rw-r--r--   0 anupamb    (501) staff       (20)      121 2023-01-07 01:16:49.000000 HolisticTraceAnalysis-0.2.0/MANIFEST.in
+-rw-r--r--   0 anupamb    (501) staff       (20)      683 2023-05-22 18:55:24.702685 HolisticTraceAnalysis-0.2.0/PKG-INFO
+-rw-r--r--   0 anupamb    (501) staff       (20)     7182 2023-05-22 18:40:56.000000 HolisticTraceAnalysis-0.2.0/README.md
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.669529 HolisticTraceAnalysis-0.2.0/docs/
+-rw-r--r--   0 anupamb    (501) staff       (20)     3052 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/docs/conf.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.672466 HolisticTraceAnalysis-0.2.0/hta/
+-rw-r--r--   0 anupamb    (501) staff       (20)      100 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/__init__.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.679560 HolisticTraceAnalysis-0.2.0/hta/analyzers/
+-rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/__init__.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    23401 2023-05-22 18:40:56.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/breakdown_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     4155 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/communication_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    18494 2023-05-22 18:40:56.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/cuda_kernel_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     5907 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/cupti_counter_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    11641 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/straggler.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     2872 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/straggler_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     8514 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/timeline.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    12012 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/analyzers/trace_counters.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.681713 HolisticTraceAnalysis-0.2.0/hta/common/
+-rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/common/__init__.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    16916 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/common/call_stack.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    28640 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/common/trace.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     5733 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/common/trace_file.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.684540 HolisticTraceAnalysis-0.2.0/hta/configs/
+-rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/configs/__init__.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     5281 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/configs/config.py
+-rw-r--r--   0 anupamb    (501) staff       (20)      453 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/configs/default_values.py
+-rw-r--r--   0 anupamb    (501) staff       (20)      434 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/configs/logging.config
+-rw-r--r--   0 anupamb    (501) staff       (20)      203 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/configs/trace_analyzer.json
+-rw-r--r--   0 anupamb    (501) staff       (20)    25077 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/trace_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    21311 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/trace_diff.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.686090 HolisticTraceAnalysis-0.2.0/hta/utils/
+-rw-r--r--   0 anupamb    (501) staff       (20)        0 2023-01-06 01:52:32.000000 HolisticTraceAnalysis-0.2.0/hta/utils/__init__.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     4626 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/hta/utils/utils.py
+-rw-r--r--   0 anupamb    (501) staff       (20)      208 2023-05-22 18:42:00.000000 HolisticTraceAnalysis-0.2.0/hta/version.py
+-rw-r--r--   0 anupamb    (501) staff       (20)      321 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/pyproject.toml
+-rw-r--r--   0 anupamb    (501) staff       (20)      102 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.2.0/requirements.txt
+-rw-r--r--   0 anupamb    (501) staff       (20)      258 2023-05-22 18:55:24.722874 HolisticTraceAnalysis-0.2.0/setup.cfg
+-rw-r--r--   0 anupamb    (501) staff       (20)     1285 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/setup.py
+drwxr-xr-x   0 anupamb    (501) staff       (20)        0 2023-05-22 18:55:24.701218 HolisticTraceAnalysis-0.2.0/tests/
+-rw-r--r--   0 anupamb    (501) staff       (20)     4235 2023-02-08 01:12:52.000000 HolisticTraceAnalysis-0.2.0/tests/test_call_stack.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     3017 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/tests/test_config.py
+-rw-r--r--   0 anupamb    (501) staff       (20)      959 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/tests/test_correlation.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     2581 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/tests/test_symbol_table.py
+-rw-r--r--   0 anupamb    (501) staff       (20)    13428 2023-05-22 18:40:56.000000 HolisticTraceAnalysis-0.2.0/tests/test_trace_analysis.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     7277 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/tests/test_trace_diff.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     3855 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/tests/test_trace_file.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     4877 2023-05-12 16:48:58.000000 HolisticTraceAnalysis-0.2.0/tests/test_trace_parse.py
+-rw-r--r--   0 anupamb    (501) staff       (20)     1009 2022-12-14 22:16:42.000000 HolisticTraceAnalysis-0.2.0/tests/test_trace_utils.py
```

### Comparing `HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/PKG-INFO` & `HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HolisticTraceAnalysis
-Version: 0.1.3
+Version: 0.2.0
 Summary: A python library for analyzing PyTorch Profiler traces
 Home-page: https://github.com/facebookresearch/HolisticTraceAnalysis
 Author: Meta Platforms Inc.
 Author-email: todo@meta.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `HolisticTraceAnalysis-0.1.3/HolisticTraceAnalysis.egg-info/SOURCES.txt` & `HolisticTraceAnalysis-0.2.0/HolisticTraceAnalysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 hta/trace_analysis.py
 hta/trace_diff.py
 hta/version.py
 hta/analyzers/__init__.py
 hta/analyzers/breakdown_analysis.py
 hta/analyzers/communication_analysis.py
 hta/analyzers/cuda_kernel_analysis.py
+hta/analyzers/cupti_counter_analysis.py
 hta/analyzers/straggler.py
 hta/analyzers/straggler_analysis.py
 hta/analyzers/timeline.py
 hta/analyzers/trace_counters.py
 hta/common/__init__.py
 hta/common/call_stack.py
 hta/common/trace.py
```

### Comparing `HolisticTraceAnalysis-0.1.3/LICENSE` & `HolisticTraceAnalysis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HolisticTraceAnalysis-0.1.3/PKG-INFO` & `HolisticTraceAnalysis-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HolisticTraceAnalysis
-Version: 0.1.3
+Version: 0.2.0
 Summary: A python library for analyzing PyTorch Profiler traces
 Home-page: https://github.com/facebookresearch/HolisticTraceAnalysis
 Author: Meta Platforms Inc.
 Author-email: todo@meta.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `HolisticTraceAnalysis-0.1.3/README.md` & `HolisticTraceAnalysis-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,17 @@
    PyTorch or user defined operator.
 1. __CUDA Kernel Launch Statistics__ - Distributions of GPU kernels with very small duration, large
    duration, and excessive launch time.
 1. __Augmented Counters (Queue length, Memory bandwidth)__ - Augmented trace files which provide
    insights into memory bandwidth utilized and number of outstanding operations on each CUDA stream.
 1. __Trace Comparison__ - A trace comparison tool to identify and visualize the differences between
    traces.
+1. __CUPTI Counter Analysis__ - An experimental API to get GPU performance counters. By attributing
+   performance measurements from kernels to PyTorch operators roofline analysis can be performed and
+   kernels can be optimized.
 
 ## Installation
 
 HTA runs on Linux and Mac with Python >= 3.8.
 
 ### Setup a Conda environment (optional)
```

### Comparing `HolisticTraceAnalysis-0.1.3/docs/conf.py` & `HolisticTraceAnalysis-0.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 
 
 sys.path.insert(0, os.path.abspath(".."))
 
 
 def find_version(version_file_path) -> str:
     with open(version_file_path) as version_file:
-        version_match = re.search(r"^__version_tuple__ = (.*)", version_file.read(), re.M)
+        version_match = re.search(
+            r"^__version_tuple__ = (.*)", version_file.read(), re.M
+        )
         if version_match:
             ver_tup = eval(version_match.group(1))
             ver_str = ".".join([str(x) for x in ver_tup])
             return ver_str
         raise RuntimeError("Unable to find version tuple.")
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/breakdown_analysis.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/breakdown_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from collections import defaultdict
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple, TYPE_CHECKING
 
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
-from plotly.subplots import make_subplots
 
 from hta.configs.config import logger
-from hta.utils.utils import IdleTimeType, KernelType, get_kernel_type, merge_kernel_intervals
+from hta.utils.utils import (
+    get_kernel_type,
+    IdleTimeType,
+    KernelType,
+    merge_kernel_intervals,
+)
+from plotly.subplots import make_subplots
 
 # import statement used without the "if TYPE_CHECKING" guard will cause a circular
 # dependency with trace_analysis.py causing mypy to fail and should not be removed.
 if TYPE_CHECKING:
     from hta.common.trace import Trace
 
 # This configures the threshold under which we consider gaps between
@@ -97,29 +102,37 @@
                     num_kernels=num_kernels,
                 )
 
                 kernel_per_rank[kernel_type][rank] = gpu_kernel_time
 
                 gpu_kernel_time["kernel_type"] = kernel_type
                 gpu_kernel_time["rank"] = int(rank)
-                all_kernel_df = pd.concat([all_kernel_df, gpu_kernel_time], ignore_index=True)
+                all_kernel_df = pd.concat(
+                    [all_kernel_df, gpu_kernel_time], ignore_index=True
+                )
 
         kernel_type_df = kernel_type_df.groupby(by=["kernel_type"])["sum"].agg(["sum"])
         kernel_type_df.reset_index(inplace=True)
-        kernel_type_df.sort_values(by=["sum"], ignore_index=True, inplace=True, ascending=False)
-        kernel_type_df["percentage"] = (kernel_type_df["sum"] / kernel_type_df["sum"].sum()) * 100
+        kernel_type_df.sort_values(
+            by=["sum"], ignore_index=True, inplace=True, ascending=False
+        )
+        kernel_type_df["percentage"] = (
+            kernel_type_df["sum"] / kernel_type_df["sum"].sum()
+        ) * 100
         kernel_type_df = kernel_type_df.round({"percentage": 1})
 
-        all_kernel_df.sort_values(by=["kernel_type", "name", "rank"], ignore_index=True, inplace=True)
+        all_kernel_df.sort_values(
+            by=["kernel_type", "name", "rank"], ignore_index=True, inplace=True
+        )
         all_kernel_df.rename(
             columns={
-                "sum": "sum (ns)",
-                "mean": "mean (ns)",
-                "max": "max (ns)",
-                "min": "min (ns)",
+                "sum": "sum (us)",
+                "mean": "mean (us)",
+                "max": "max (us)",
+                "min": "min (us)",
                 "std": "stddev",
             },
             inplace=True,
         )
 
         if visualize:  # pragma: no cover
             non_zero_kernel_df = kernel_type_df[(kernel_type_df["percentage"] > 0)]
@@ -174,51 +187,59 @@
                 kernel_name = kernel_df["name"].unique()
                 for name in kernel_name:
                     if name != "others":
                         kernel_name_df = kernel_df[kernel_df["name"].eq(name)]
                         fig = px.bar(
                             kernel_name_df,
                             x="rank",
-                            y="mean (ns)",
+                            y="mean (us)",
                             title=name,
                             labels={
                                 "rank": "Rank",
-                                "mean (ns)": "Mean Duration (ns)",
+                                "mean (us)": "Mean Duration (us)",
                             },
-                            error_y=kernel_name_df["max (ns)"] - kernel_name_df["mean (ns)"],
-                            error_y_minus=kernel_name_df["mean (ns)"] - kernel_name_df["min (ns)"],
+                            error_y=kernel_name_df["max (us)"]
+                            - kernel_name_df["mean (us)"],
+                            error_y_minus=kernel_name_df["mean (us)"]
+                            - kernel_name_df["min (us)"],
                         )
                         fig.update_layout(
                             title_text=f'Kernel type "{kernel}" - {name}',
                             xaxis=dict(tickmode="linear", tick0=0, dtick=1),
                         )
                         fig.show(renderer=image_renderer)
 
         return kernel_type_df, all_kernel_df
 
     @classmethod
-    def _get_gpu_kernel_type_time(cls, gpu_kernels: pd.DataFrame, kernel_type_to_analysis: List[str]) -> pd.DataFrame:
+    def _get_gpu_kernel_type_time(
+        cls, gpu_kernels: pd.DataFrame, kernel_type_to_analysis: List[str]
+    ) -> pd.DataFrame:
         overlap_kernel_type_df = pd.DataFrame(
             {
                 "status": pd.Series(dtype="str"),
                 "time": pd.Series(dtype="int"),
             }
         )
 
         kernel_t_mapping: Dict[str, int] = defaultdict(int)
         for idx, kernel_type in enumerate(kernel_type_to_analysis):
             value = 1 << idx
             kernel_t_mapping[kernel_type] = value
-            kernel_t_df = merge_kernel_intervals(gpu_kernels[gpu_kernels["kernel_type"].eq(kernel_type)].copy())
+            kernel_t_df = merge_kernel_intervals(
+                gpu_kernels[gpu_kernels["kernel_type"].eq(kernel_type)].copy()
+            )
 
             overlap_kernel_type_df = (
                 pd.concat(
                     [
                         overlap_kernel_type_df,
-                        kernel_t_df.melt(var_name="status", value_name="time").replace({"ts": value, "end": -value}),
+                        kernel_t_df.melt(var_name="status", value_name="time").replace(
+                            {"ts": value, "end": -value}
+                        ),
                     ]
                 )
                 .sort_values(by="time")
                 .reset_index(drop=True)
             )
 
         overlap_kernel_type_df["running"] = overlap_kernel_type_df["status"].cumsum()
@@ -228,62 +249,76 @@
         for u_running in unique_running:
             if u_running > 0:
                 for k_t, v_t in kernel_t_mapping.items():
                     if u_running & v_t:
                         if u_running not in running_mapping:
                             running_mapping[u_running] = k_t
                         else:
-                            running_mapping[u_running] = f"{running_mapping[u_running]} overlapping {k_t}"
+                            running_mapping[
+                                u_running
+                            ] = f"{running_mapping[u_running]} overlapping {k_t}"
 
         overlap_kernel_type_df["kernel_type"] = ""
-        overlap_kernel_type_df = overlap_kernel_type_df[overlap_kernel_type_df["running"] > 0]
+        overlap_kernel_type_df = overlap_kernel_type_df[
+            overlap_kernel_type_df["running"] > 0
+        ]
         for running in running_mapping:
-            overlap_kernel_type_df.loc[overlap_kernel_type_df["running"].eq(running), "kernel_type"] = running_mapping[
-                running
-            ]
-        overlap_kernel_type_df["dur"] = (overlap_kernel_type_df["next_time"] - overlap_kernel_type_df["time"]).astype(
-            int
-        )
-
-        overlap_kernel_type_df = overlap_kernel_type_df.groupby(by=["kernel_type"])["dur"].agg(["sum"])
+            overlap_kernel_type_df.loc[
+                overlap_kernel_type_df["running"].eq(running), "kernel_type"
+            ] = running_mapping[running]
+        overlap_kernel_type_df["dur"] = (
+            overlap_kernel_type_df["next_time"] - overlap_kernel_type_df["time"]
+        ).astype(int)
+
+        overlap_kernel_type_df = overlap_kernel_type_df.groupby(by=["kernel_type"])[
+            "dur"
+        ].agg(["sum"])
         overlap_kernel_type_df.reset_index(inplace=True)
 
         return overlap_kernel_type_df
 
     @classmethod
     def _aggr_gpu_kernel_time(
         cls,
         gpu_kernel_time: pd.DataFrame,
         duration_ratio: float = 0.8,
         num_kernels: int = 10,
     ) -> pd.DataFrame:
-        gpu_kernel_time = gpu_kernel_time.groupby(by=["name"])["dur"].agg(["sum", "max", "min", "mean", "std"])
+        gpu_kernel_time = gpu_kernel_time.groupby(by=["name"])["dur"].agg(
+            ["sum", "max", "min", "mean", "std"]
+        )
         gpu_kernel_time.reset_index(inplace=True)
-        gpu_kernel_time = gpu_kernel_time.sort_values(by=["sum"], ascending=False, ignore_index=True)
+        gpu_kernel_time = gpu_kernel_time.sort_values(
+            by=["sum"], ascending=False, ignore_index=True
+        )
         gpu_kernel_time["std"].fillna(0, inplace=True)
 
         # if there are more than num_kernels kernels, starting to aggregate kernels
         if gpu_kernel_time.shape[0] > num_kernels:
             gpu_kernel_time["cumsum"] = gpu_kernel_time["sum"].cumsum()
             quantiles = gpu_kernel_time["cumsum"].quantile(duration_ratio)
-            gpu_kernel_time.loc[gpu_kernel_time["cumsum"] > quantiles, "name"] = "others"
+            gpu_kernel_time.loc[
+                gpu_kernel_time["cumsum"] > quantiles, "name"
+            ] = "others"
             gpu_kernel_time.loc[gpu_kernel_time.index >= num_kernels, "name"] = "others"
-            gpu_kernel_time = gpu_kernel_time.groupby(by=["name"])["sum"].agg(["sum", "max", "min", "mean", "std"])
+            gpu_kernel_time = gpu_kernel_time.groupby(by=["name"])["sum"].agg(
+                ["sum", "max", "min", "mean", "std"]
+            )
             gpu_kernel_time.reset_index(inplace=True)
             gpu_kernel_time["std"].fillna(0, inplace=True)
 
         return gpu_kernel_time
 
     @classmethod
     def _get_idle_time_for_kernels(cls, kernels_df: pd.DataFrame) -> Tuple[int, int]:
         """
         Compute idle time for given set of GPU kernels :
           returns :
-            idle time (ns) = kernel time - merged execution time of all kernels
-            kernel time (ns) = defined as the time difference between end of the
+            idle time (us) = kernel time - merged execution time of all kernels
+            kernel time (us) = defined as the time difference between end of the
                          last kernel and start of the first kernel.
             PS: we exclude the last profiler iteration while reading trace
             so total time is exclusive of that.
         """
         merged_kernels = merge_kernel_intervals(kernels_df)
         kernel_time = merged_kernels.iloc[-1]["end"] - merged_kernels.iloc[0]["ts"]
         # differences of end - ts are commutative
@@ -294,51 +329,63 @@
     def get_temporal_breakdown(cls, t: "Trace", visualize: bool = True) -> pd.DataFrame:
         """
         Temporal breakdown implementation. See `get_temporal_breakdown` in `trace_analysis.py` for details.
         """
         sym_table = t.symbol_table.get_sym_table()
 
         def idle_time_per_rank(trace_df: pd.DataFrame) -> Tuple[int, int, int, int]:
-            """returns idle_time (ns) , compute_time (ns), non_compute_time (ns), total_time (ns)"""
+            """returns idle_time (us) , compute_time (us), non_compute_time (us), total_time (us)"""
             gpu_kernels = trace_df[trace_df["stream"].ne(-1)].copy()
             idle_time, kernel_time = cls._get_idle_time_for_kernels(gpu_kernels)
 
             gpu_kernels["kernel_type"] = gpu_kernels[["name"]].apply(
                 lambda x: get_kernel_type(sym_table[x["name"]]), axis=1
             )
 
             # Isolate computation kernels and merge each one of them.
             comp_kernels = merge_kernel_intervals(
-                gpu_kernels[gpu_kernels["kernel_type"].eq(KernelType.COMPUTATION.name)].copy()
+                gpu_kernels[
+                    gpu_kernels["kernel_type"].eq(KernelType.COMPUTATION.name)
+                ].copy()
             )
             compute_time = comp_kernels.end.sum() - comp_kernels.ts.sum()
             non_compute_time = kernel_time - compute_time - idle_time
 
             assert idle_time <= kernel_time
             assert compute_time <= kernel_time
             assert non_compute_time >= 0
 
             return idle_time, compute_time, non_compute_time, kernel_time
 
         result: Dict[str, List[float]] = defaultdict(list)
         for rank, trace_df in t.traces.items():
             result["rank"].append(rank)
-            idle_time, compute_time, non_compute_time, kernel_time = idle_time_per_rank(trace_df)
-            result["idle_time(ns)"].append(idle_time)
-            result["compute_time(ns)"].append(compute_time)
-            result["non_compute_time(ns)"].append(non_compute_time)
-            result["kernel_time(ns)"].append(kernel_time)
+            idle_time, compute_time, non_compute_time, kernel_time = idle_time_per_rank(
+                trace_df
+            )
+            result["idle_time(us)"].append(idle_time)
+            result["compute_time(us)"].append(compute_time)
+            result["non_compute_time(us)"].append(non_compute_time)
+            result["kernel_time(us)"].append(kernel_time)
 
         result_df = pd.DataFrame(result)
-        result_df["idle_time"] = result_df["idle_time(ns)"] / result_df["kernel_time(ns)"]
+        result_df["idle_time"] = (
+            result_df["idle_time(us)"] / result_df["kernel_time(us)"]
+        )
         result_df["idle_time_pctg"] = round(100 * result_df["idle_time"], 2)
-        result_df["compute_time"] = result_df["compute_time(ns)"] / result_df["kernel_time(ns)"]
+        result_df["compute_time"] = (
+            result_df["compute_time(us)"] / result_df["kernel_time(us)"]
+        )
         result_df["compute_time_pctg"] = round(100 * result_df["compute_time"], 2)
-        result_df["non_compute_time"] = result_df["non_compute_time(ns)"] / result_df["kernel_time(ns)"]
-        result_df["non_compute_time_pctg"] = round(100 * result_df["non_compute_time"], 2)
+        result_df["non_compute_time"] = (
+            result_df["non_compute_time(us)"] / result_df["kernel_time(us)"]
+        )
+        result_df["non_compute_time_pctg"] = round(
+            100 * result_df["non_compute_time"], 2
+        )
 
         if visualize:  # pragma: no cover
             fig = px.bar(
                 result_df,
                 x="rank",
                 y=["idle_time", "compute_time", "non_compute_time"],
                 title="Temporal breakdown across ranks",
@@ -352,18 +399,18 @@
                 legend_title="Time Breakdown",
             )
             fig.show()
 
         return result_df[
             [
                 "rank",
-                "idle_time(ns)",
-                "compute_time(ns)",
-                "non_compute_time(ns)",
-                "kernel_time(ns)",
+                "idle_time(us)",
+                "compute_time(us)",
+                "non_compute_time(us)",
+                "kernel_time(us)",
                 "idle_time_pctg",
                 "compute_time_pctg",
                 "non_compute_time_pctg",
             ]
         ]
 
     @classmethod
@@ -382,19 +429,23 @@
         returns
         1) dataframe with idle time breakdown.
         1) optional dataframe showing idle interval statistics.
         """
         logger.info(f"Processing stream {stream}")
         idle_interval_stats: Optional[pd.DataFrame] = None
 
-        gpu_kernels_s = gpu_kernels[gpu_kernels.stream == stream].copy().sort_values(by="ts")
+        gpu_kernels_s = (
+            gpu_kernels[gpu_kernels.stream == stream].copy().sort_values(by="ts")
+        )
 
         gpu_kernels_s["end_ts"] = gpu_kernels_s.ts + gpu_kernels_s.dur
         gpu_kernels_s["prev_end_ts"] = gpu_kernels_s.end_ts.shift(1)
-        gpu_kernels_s["idle_interval"] = gpu_kernels_s["ts"] - gpu_kernels_s["prev_end_ts"]
+        gpu_kernels_s["idle_interval"] = (
+            gpu_kernels_s["ts"] - gpu_kernels_s["prev_end_ts"]
+        )
 
         # Default idle time category
         gpu_kernels_s["idle_category"] = IdleTimeType.OTHER.value
 
         """
         Host wait:
             If the current kernel's runtime started after previous kernel's end time
@@ -406,20 +457,26 @@
         gpu_kernels_s.loc[is_host_wait, "idle_category"] = IdleTimeType.HOST_WAIT.value
 
         """
         Kernel wait:
             If the gap between kernels is below a threshold the idle time is
             likely due to the overhead for launching kernels.
         """
-        is_kernel_kernel_delay = ~is_host_wait & (gpu_kernels_s["idle_interval"] < consecutive_kernel_delay)
-        gpu_kernels_s.loc[is_kernel_kernel_delay, "idle_category"] = IdleTimeType.KERNEL_WAIT.value
+        is_kernel_kernel_delay = ~is_host_wait & (
+            gpu_kernels_s["idle_interval"] < consecutive_kernel_delay
+        )
+        gpu_kernels_s.loc[
+            is_kernel_kernel_delay, "idle_category"
+        ] = IdleTimeType.KERNEL_WAIT.value
 
         gpu_kernels_groupby = gpu_kernels_s.groupby("idle_category")
         if show_idle_interval_stats:
-            logger.info(f"Computing descriptive statistics for idle time intervals on stream {stream}:")
+            logger.info(
+                f"Computing descriptive statistics for idle time intervals on stream {stream}:"
+            )
             idle_interval_stats = gpu_kernels_groupby.idle_interval.describe()
             idle_interval_stats.insert(0, "stream", stream)
 
         result = pd.DataFrame(gpu_kernels_groupby.idle_interval.sum())
         total_idle_time = result.idle_interval.sum()
         result["stream"] = stream
         result["idle_time_ratio"] = result["idle_interval"] / total_idle_time
@@ -448,18 +505,22 @@
         visualize (bool): show the visualization chart or not (default = True).
         visualize_pctg (bool): show relative percentage across streams (default = True).
         show_idle_interval_stats (bool): prints statistics of the idle intervals like the min, max
            and median of idle intervals between kernels on a CUDA stream, also broken down by
            the idleness category (default = False).
         """
         trace_df: pd.DataFrame = t.get_trace(rank)
-        gpu_kernels_pre = trace_df[trace_df["stream"].ne(-1)].copy().set_index("index_correlation")
+        gpu_kernels_pre = (
+            trace_df[trace_df["stream"].ne(-1)].copy().set_index("index_correlation")
+        )
 
         # correlate with the runtime event whenever possible
-        gpu_kernels = gpu_kernels_pre.join(trace_df[["ts", "index"]], on="index_correlation", rsuffix="_runtime")
+        gpu_kernels = gpu_kernels_pre.join(
+            trace_df[["ts", "index"]], on="index_correlation", rsuffix="_runtime"
+        )
 
         if streams is None or len(streams) == 0:
             streams = list(gpu_kernels.stream.unique())
 
         result_list: List[pd.DataFrame] = []
         interval_stats_list: List[pd.DataFrame] = []
 
@@ -472,15 +533,18 @@
             )
             result_list.append(breakdown_df)
             if idle_interval_df is not None:
                 interval_stats_list.append(idle_interval_df)
 
         result_df = pd.concat(result_list)
 
-        idle_category_name_map = {member.value: name.lower() for name, member in IdleTimeType.__members__.items()}
+        idle_category_name_map = {
+            member.value: name.lower()
+            for name, member in IdleTimeType.__members__.items()
+        }
         result_df.rename(mapper=idle_category_name_map, axis=0, inplace=True)
         result_df.reset_index(inplace=True)
 
         if visualize:  # pragma: no cover
             result_df["stream"] = result_df.stream.astype(str)
             ycol = "idle_time_ratio" if visualize_pctg else "idle_time"
             fig = px.bar(
@@ -494,20 +558,30 @@
             if visualize_pctg:
                 fig.update_layout(
                     yaxis_tickformat=".2%",
                     yaxis_title="Percentage",
                     legend_title="Idle Time Breakdown",
                 )
             else:
-                fig.update_layout(yaxis_title="Idle time (ns)", legend_title="Idle Time Breakdown")
+                fig.update_layout(
+                    yaxis_title="Idle time (us)", legend_title="Idle Time Breakdown"
+                )
             fig.show()
 
         result_df["rank"] = rank
-        interval_stats_df = pd.concat(interval_stats_list).round(2) if show_idle_interval_stats else None
+        interval_stats_df = (
+            pd.concat(interval_stats_list).round(2)
+            if show_idle_interval_stats
+            else None
+        )
         if interval_stats_df is not None:
             # add rank column to the starting
             interval_stats_df.insert(0, "rank", rank)
-            interval_stats_df.rename(mapper=idle_category_name_map, axis=0, inplace=True)
+            interval_stats_df.rename(
+                mapper=idle_category_name_map, axis=0, inplace=True
+            )
 
-        result_df = result_df[["rank", "stream", "idle_category", "idle_time", "idle_time_ratio"]].round(2)
+        result_df = result_df[
+            ["rank", "stream", "idle_category", "idle_time", "idle_time_ratio"]
+        ].round(2)
 
         return result_df, interval_stats_df
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/communication_analysis.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/communication_analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from collections import defaultdict
-from typing import TYPE_CHECKING, Dict, List
+from typing import Dict, List, TYPE_CHECKING
 
 import pandas as pd
 import plotly.express as px
 
-from hta.utils.utils import KernelType, get_kernel_type, merge_kernel_intervals
+from hta.utils.utils import get_kernel_type, KernelType, merge_kernel_intervals
 
 # import statement used without the "if TYPE_CHECKING" guard will cause a circular
 # dependency with trace_analysis.py causing mypy to fail and should not be removed.
 if TYPE_CHECKING:
     from hta.trace import Trace
 
 
@@ -34,46 +34,60 @@
             gpu_kernels = trace_df[trace_df["stream"].ne(-1)].copy()
             gpu_kernels["kernel_type"] = gpu_kernels[["name"]].apply(
                 lambda x: get_kernel_type(sym_table[x["name"]]), axis=1
             )
 
             # Isolate communication and computation kernels and merge each one of them.
             comp_kernels = merge_kernel_intervals(
-                gpu_kernels[gpu_kernels["kernel_type"].eq(KernelType.COMPUTATION.name)].copy()
+                gpu_kernels[
+                    gpu_kernels["kernel_type"].eq(KernelType.COMPUTATION.name)
+                ].copy()
             )
             comm_kernels = merge_kernel_intervals(
-                gpu_kernels[gpu_kernels["kernel_type"].eq(KernelType.COMMUNICATION.name)].copy()
+                gpu_kernels[
+                    gpu_kernels["kernel_type"].eq(KernelType.COMMUNICATION.name)
+                ].copy()
             )
 
             # When a communication kernel starts and ends, the cumulative status is changed by 1 and -1;
             # when a computation kernel starts and ends, the cumulative status is changed by 2 and -2.
             status_df = (
                 pd.concat(
                     [
-                        comm_kernels.melt(var_name="status", value_name="time").replace({"ts": 1, "end": -1}),
-                        comp_kernels.melt(var_name="status", value_name="time").replace({"ts": 2, "end": -2}),
+                        comm_kernels.melt(var_name="status", value_name="time").replace(
+                            {"ts": 1, "end": -1}
+                        ),
+                        comp_kernels.melt(var_name="status", value_name="time").replace(
+                            {"ts": 2, "end": -2}
+                        ),
                     ]
                 )
                 .sort_values(by="time")
                 .reset_index(drop=True)
             )
             status_df["running"] = status_df["status"].cumsum()
             # Time intervals when status is 3 indicate overlapping communication and computation kernels.
             overlap = status_df[status_df["running"].eq(3)]
-            shifted_overlap = overlap.merge(status_df.shift(-1).dropna(), left_index=True, right_index=True)
+            shifted_overlap = overlap.merge(
+                status_df.shift(-1).dropna(), left_index=True, right_index=True
+            )
             return (shifted_overlap["time_y"] - shifted_overlap["time_x"]).sum() / (
                 comm_kernels["end"] - comm_kernels["ts"]
             ).sum()
 
         result: Dict[str, List[float]] = defaultdict(list)
         for rank, trace_df in t.traces.items():
             result["rank"].append(rank)
-            result["comp_comm_overlap_ratio"].append(get_comm_comp_overlap_value(trace_df))
+            result["comp_comm_overlap_ratio"].append(
+                get_comm_comp_overlap_value(trace_df)
+            )
         result_df = pd.DataFrame(result)
-        result_df["comp_comm_overlap_pctg"] = round(100 * result_df["comp_comm_overlap_ratio"], 2)
+        result_df["comp_comm_overlap_pctg"] = round(
+            100 * result_df["comp_comm_overlap_ratio"], 2
+        )
 
         if visualize:  # pragma: no cover
             fig = px.bar(
                 result_df,
                 x="rank",
                 y="comp_comm_overlap_ratio",
                 title="Computation-Communication Overlap",
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/cuda_kernel_analysis.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/cuda_kernel_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,23 @@
         compress_other_kernels: bool = True,
     ) -> pd.DataFrame:
         """
         Frequent CUDA kernel sequences implementation. See `get_frequent_cuda_kernel_sequences` in `trace_analysis.py`
         for details.
         """
         if not operator_name:
-            logger.error("operator_name must be a non-empty string and a valid operator name in the trace file.")
+            logger.error(
+                "operator_name must be a non-empty string and a valid operator name in the trace file."
+            )
             return pd.DataFrame()
 
         if not output_dir:
-            logger.error("output_dir must be a non-empty string and a valid folder name.")
+            logger.error(
+                "output_dir must be a non-empty string and a valid folder name."
+            )
             return pd.DataFrame()
 
         # check output_dir is a valid path and a directory
         path = Path(output_dir)
         if not path.exists():
             logger.error(f"The path {str(path)} does not exist.")
             return pd.DataFrame()
@@ -56,52 +60,64 @@
         cg = CallGraph(t, ranks=[rank])
         trace_df = t.get_trace(rank)
 
         cpu_kernels = trace_df[trace_df["stream"].eq(-1)].copy()
         gpu_kernels = trace_df[trace_df["stream"].ne(-1)].copy()
 
         # get all the CPU operators which contain operator_name in their names
-        candidate_root_idx = [idx for name, idx in sym_index.items() if operator_name in name]
+        candidate_root_idx = [
+            idx for name, idx in sym_index.items() if operator_name in name
+        ]
         candidate_nodes = cpu_kernels[cpu_kernels["name"].isin(candidate_root_idx)]
         # to avoid double-counting when the same CPU operators appear multiple times in the call graph
         # hierarchy, only start the search from the shallowest CPU operators
         min_depth = candidate_nodes["depth"].min()
-        root_nodes = candidate_nodes[candidate_nodes["depth"].eq(min_depth)][["index", "dur"]]
+        root_nodes = candidate_nodes[candidate_nodes["depth"].eq(min_depth)][
+            ["index", "dur"]
+        ]
 
         pattern_counts: Dict[Tuple[int, ...], int] = defaultdict(int)
         # duration of the pattern: [GPU kernel duration, CPU op duration]
-        pattern_durations: Dict[Tuple[int, ...], List[int]] = defaultdict(lambda: [0, 0])
+        pattern_durations: Dict[Tuple[int, ...], List[int]] = defaultdict(
+            lambda: [0, 0]
+        )
         # record the indices of frequent patterns.
         pattern_occurrences: Dict[Tuple[int, ...], Set[int]] = defaultdict(set)
 
         for cs in cg.call_stacks:
             for _, root_node, root_dur in root_nodes.itertuples():
                 if root_node in cs.get_nodes():
                     # find all cuda kernels launched by the root_node by joining GPU kernels with leaf nodes.
                     cuda_kernels = gpu_kernels.merge(
-                        cpu_kernels[cpu_kernels["index"].isin(cs.get_leaf_nodes(root_node))][["correlation"]],
+                        cpu_kernels[
+                            cpu_kernels["index"].isin(cs.get_leaf_nodes(root_node))
+                        ][["correlation"]],
                         on="correlation",
                         how="inner",
                     ).sort_values(by="ts")
                     # discard the pattern if it is too short
                     if len(cuda_kernels) < min_pattern_len:
                         continue
                     cpu_operator = cpu_kernels[cpu_kernels["index"].eq(root_node)]
-                    pattern: Tuple[int, ...] = tuple(pd.concat([cpu_operator["name"], cuda_kernels["name"]]))
+                    pattern: Tuple[int, ...] = tuple(
+                        pd.concat([cpu_operator["name"], cuda_kernels["name"]])
+                    )
                     pattern_counts[pattern] += 1
                     # update the duration for GPU kernels in the pattern
                     pattern_durations[pattern][0] += cuda_kernels["dur"].sum()
                     # update the duration for CPU operators in the pattern
                     pattern_durations[pattern][1] += root_dur
                     for p in cs.get_paths_to_leaves(root_node):
                         pattern_occurrences[pattern].update(p)
                     pattern_occurrences[pattern].update(cuda_kernels["index"])
 
         if not pattern_counts:
-            logger.error("operator_name not found in the trace file, or no frequent cuda kernel sequences found.")
+            logger.error(
+                "operator_name not found in the trace file, or no frequent cuda kernel sequences found."
+            )
             return pd.DataFrame()
 
         return cls._generate_frequent_pattern_results(
             t,
             pattern_counts,
             pattern_durations,
             pattern_occurrences,
@@ -143,35 +159,47 @@
                               frequent patterns
             compress_other_kernels (bool): should the names and args for other kernels not belonging to
                                            any frequent patterns be compressed to save memory in the overlaid
                                            trace file
         Returns:
             patterns_df (pd.DataFrame): a dataframe with all patterns and their frequencies
         """
-        output_file = os.path.join(str(Path(output_dir)), "overlaid_" + t.trace_files[rank].split("/")[-1])
+        output_file = os.path.join(
+            str(Path(output_dir)), "overlaid_" + t.trace_files[rank].split("/")[-1]
+        )
 
         sym_table = t.symbol_table.get_sym_table()
         patterns_result: Dict[str, List[Union[int, str, Set[int]]]] = defaultdict(list)
         for pattern, count in pattern_counts.items():
             patterns_result["pattern"].append("|".join(sym_table[x] for x in pattern))
             patterns_result["count"].append(count)
-            patterns_result["GPU kernel duration (ns)"].append(pattern_durations[pattern][0])
-            patterns_result["CPU op duration (ns)"].append(pattern_durations[pattern][1])
+            patterns_result["GPU kernel duration (us)"].append(
+                pattern_durations[pattern][0]
+            )
+            patterns_result["CPU op duration (us)"].append(
+                pattern_durations[pattern][1]
+            )
             patterns_result["pattern_indices"].append(pattern_occurrences[pattern])
 
         patterns_df = pd.DataFrame(patterns_result).sort_values(
             by=["count", "pattern"], ascending=[False, True], ignore_index=True
         )
         if top_k > len(patterns_df):
             top_k = len(patterns_df)
-            logger.info("The top_k argument value exceeds the number of patterns. Displaying all patterns.")
+            logger.info(
+                "The top_k argument value exceeds the number of patterns. Displaying all patterns."
+            )
 
-        overlaid_trace = cls._overlay_frequent_patterns_with_trace(t, patterns_df[:top_k], rank, compress_other_kernels)
+        overlaid_trace = cls._overlay_frequent_patterns_with_trace(
+            t, patterns_df[:top_k], rank, compress_other_kernels
+        )
         t.write_raw_trace(output_file, overlaid_trace)
-        logger.info(f"Overlaid trace file for rank {rank} has been generated at {output_file}.")
+        logger.info(
+            f"Overlaid trace file for rank {rank} has been generated at {output_file}."
+        )
         logger.info(
             'View the generated trace file using Chrome Tracing and search for "Patterns" to highlight the frequent patterns.'
         )
 
         if visualize:  # pragma: no cover
             vis_df = patterns_df[:top_k].copy()
             # show the pattern in multiple lines in visualization
@@ -213,18 +241,28 @@
         raw_trace_df["index"] = pd.to_numeric(raw_trace_df["index"], downcast="integer")
         sym_id_map = t.symbol_table.get_sym_id_map()
 
         # get a counter of patterns that each CPU operator/GPU kernel is in.
         top_patterns_df = (
             patterns_df.explode("pattern_indices")
             .groupby("pattern_indices", as_index=False)
-            .apply(lambda g: pd.Series({"active_patterns": {r["pattern"]: r["count"] for _, r in g.iterrows()}}))
+            .apply(
+                lambda g: pd.Series(
+                    {
+                        "active_patterns": {
+                            r["pattern"]: r["count"] for _, r in g.iterrows()
+                        }
+                    }
+                )
+            )
         )
         # join the pattern counter with the original events on their indices
-        merged_df = raw_trace_df.merge(top_patterns_df, left_on="index", right_on="pattern_indices", how="left")
+        merged_df = raw_trace_df.merge(
+            top_patterns_df, left_on="index", right_on="pattern_indices", how="left"
+        )
 
         def _add_patterns_to_args(row, compress_other_kernels):
             args = row["args"]
             if pd.isna(row["pattern_indices"]):
                 # only drop complete events to ensure important information is retained
                 return {} if compress_other_kernels and row["ph"] == "X" else args
             # add the frequent patterns to the args field
@@ -237,62 +275,77 @@
             # do not compress events that are part of a frequent pattern, or we don't know how to compress
             if row["args"] or row["name"] not in sym_id_map:
                 return row["name"]
             # otherwise return the symbol id created during trace parsing of that event
             return str(sym_id_map[row["name"]])
 
         # add the frequent patterns information to the args field so that it is searchable
-        merged_df["args"] = merged_df.apply(lambda r: _add_patterns_to_args(r, compress_other_kernels), axis=1)
+        merged_df["args"] = merged_df.apply(
+            lambda r: _add_patterns_to_args(r, compress_other_kernels), axis=1
+        )
 
         if compress_other_kernels:
             # compress kernel/operator names
             merged_df["name"] = merged_df.apply(_compress_kernel_names, axis=1)
             # add the symbol id -> event name mapping information to the PyTorch Profiler event for reference
             profiler_event = raw_trace_df[
-                (raw_trace_df["name"].str.contains("PyTorch Profiler")) & (raw_trace_df["pid"].eq("Spans"))
+                (raw_trace_df["name"].str.contains("PyTorch Profiler"))
+                & (raw_trace_df["pid"].eq("Spans"))
+            ]
+            merged_df.loc[profiler_event.index, "args"] = [
+                {str(i): name for name, i in sym_id_map.items()}
             ]
-            merged_df.loc[profiler_event.index, "args"] = [{str(i): name for name, i in sym_id_map.items()}]
         # drop unused columns before writing back to the overlaid trace file
-        merged_df.drop(["index", "active_patterns", "pattern_indices"], axis=1, inplace=True)
-        raw_trace_content["traceEvents"] = list(merged_df.apply(lambda row: row.dropna().to_dict(), axis=1))
+        merged_df.drop(
+            ["index", "active_patterns", "pattern_indices"], axis=1, inplace=True
+        )
+        raw_trace_content["traceEvents"] = list(
+            merged_df.apply(lambda row: row.dropna().to_dict(), axis=1)
+        )
         return raw_trace_content
 
     @classmethod
     def visualize_cuda_kernel_launch_stats(
         cls, rank: int, df: pd.DataFrame, runtime_cutoff: int, launch_delay_cutoff: int
     ) -> None:  # pragma: no cover
-        short_kernels = df[(df["cpu_duration"] <= runtime_cutoff) & (df["gpu_duration"] < df["cpu_duration"])]
+        short_kernels = df[
+            (df["cpu_duration"] <= runtime_cutoff)
+            & (df["gpu_duration"] < df["cpu_duration"])
+        ]
         runtime_outliers = df[df["cpu_duration"] > runtime_cutoff]
         launch_delay_outliers = df[df["launch_delay"] > launch_delay_cutoff]
         fig1 = px.histogram(
             short_kernels,
             x=short_kernels["cpu_duration"],
-            title="Short GPU kernels (gpu op duration < cpu op duration) on rank %d" % rank,
+            title="Short GPU kernels (gpu op duration < cpu op duration) on rank %d"
+            % rank,
             labels={
                 "cpu_duration": "Cuda Runtime Event Duration (us)",
             },
         )
         fig1.show()
 
         fig2 = px.histogram(
             runtime_outliers,
             x=runtime_outliers["cpu_duration"],
             nbins=300,
-            title="Runtime Event Duration Outliers (duration > %s us)  on rank %d" % (runtime_cutoff, rank),
+            title="Runtime Event Duration Outliers (duration > %s us)  on rank %d"
+            % (runtime_cutoff, rank),
             labels={
                 "cpu_duration": "Cuda Runtime Event Duration (us)",
             },
         )
         fig2.show()
 
         fig3 = px.histogram(
             launch_delay_outliers,
             x=launch_delay_outliers["launch_delay"],
             nbins=300,
-            title="Launch Delay Outliers (duration > %s us) on rank %d" % (launch_delay_cutoff, rank),
+            title="Launch Delay Outliers (duration > %s us) on rank %d"
+            % (launch_delay_cutoff, rank),
             labels={
                 "launch_delay": "Launch Delay Duration (us)",
             },
         )
         fig3.show()
 
     @classmethod
@@ -328,15 +381,16 @@
             cudaLaunchKernel_correlation_series: pd.Series = trace_df[
                 trace_df["name"] == cudaLaunchKernel_id
             ].correlation
 
             # whether to use memory events - cudaMemsetAsync and cudaMemcpyAsync.
             if include_memory_events:
                 memory_event_correlation_series: pd.Series = trace_df[
-                    (trace_df["name"] == cudaMemsetAsync_id) | (trace_df["name"] == cudaMemcpyAsync_id)
+                    (trace_df["name"] == cudaMemsetAsync_id)
+                    | (trace_df["name"] == cudaMemcpyAsync_id)
                 ].correlation
                 merged_series: pd.Series = pd.concat(
                     [
                         cudaLaunchKernel_correlation_series,
                         memory_event_correlation_series,
                     ]
                 )
@@ -344,33 +398,41 @@
                 merged_series = cudaLaunchKernel_correlation_series
 
             # filter cpu and gpu ops
             cpu_kernels = trace_df[trace_df["stream"].eq(-1)].copy()
             gpu_kernels = trace_df[trace_df["stream"].ne(-1)].copy()
 
             # get correlation id, duration, timestamp and name of cpu and gpu events
-            cpu_kernels_filtered = cpu_kernels[(cpu_kernels["correlation"]).isin(merged_series)][
-                ["correlation", "dur", "name", "ts"]
-            ]
-            gpu_kernels_filtered = gpu_kernels[(gpu_kernels["correlation"]).isin(merged_series)][
-                ["correlation", "dur", "name", "ts"]
-            ]
+            cpu_kernels_filtered = cpu_kernels[
+                (cpu_kernels["correlation"]).isin(merged_series)
+            ][["correlation", "dur", "name", "ts"]]
+            gpu_kernels_filtered = gpu_kernels[
+                (gpu_kernels["correlation"]).isin(merged_series)
+            ][["correlation", "dur", "name", "ts"]]
 
             # join the dataframes created above on correlation. This is required to calculate the launch delay
             # for each correlation id.
             joined_df = pd.merge(
                 cpu_kernels_filtered,
                 gpu_kernels_filtered,
                 how="inner",
                 on="correlation",
             )
-            joined_df["launch_delay"] = joined_df["ts_y"] - joined_df["ts_x"] + joined_df["dur_x"]
+            joined_df["launch_delay"] = (
+                joined_df["ts_y"] - joined_df["ts_x"] + joined_df["dur_x"]
+            )
 
             # rename columns and select the required columns from the final dataframe
-            renamed_df = joined_df.rename(columns={"dur_x": "cpu_duration", "dur_y": "gpu_duration"})
-            events_df = renamed_df[["correlation", "cpu_duration", "gpu_duration", "launch_delay"]]
+            renamed_df = joined_df.rename(
+                columns={"dur_x": "cpu_duration", "dur_y": "gpu_duration"}
+            )
+            events_df = renamed_df[
+                ["correlation", "cpu_duration", "gpu_duration", "launch_delay"]
+            ]
 
             if visualize:  # pragma: no cover
-                cls.visualize_cuda_kernel_launch_stats(rank, events_df, runtime_cutoff, launch_delay_cutoff)
+                cls.visualize_cuda_kernel_launch_stats(
+                    rank, events_df, runtime_cutoff, launch_delay_cutoff
+                )
 
             result_dict[rank] = events_df
         return result_dict
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/straggler.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/straggler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,246 +1,279 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# This source code is licensed under the MIT license found in the
-# LICENSE file in the root directory of this source tree.
-
-import re
-from typing import Tuple
-
-import pandas as pd
-import plotly.express as px
-
-from hta.analyzers.timeline import _get_unique_values, plot_timeline_gpu_kernels
-from hta.common.trace import Trace, TraceSymbolTable
-
-
-def extract_iteration_info(trace: Trace) -> pd.DataFrame:
-    """Extract the iteration information from a trace.
-
-    Args:
-          trace (Trace) : a trace object
-
-    Returns:
-        a DataFrame that contains all the iteration information with rank as a column.
-    """
-    ranks = [k for k in trace.get_all_traces().keys()]
-    sym_map = trace.symbol_table.get_sym_id_map()
-    sym_tab = trace.symbol_table.get_sym_table()
-
-    def get_iter_nbr(profiler_step_name_id: int) -> int:
-        iter_re = re.compile(r"ProfilerStep\s*#\s*(\d+)")
-        m = iter_re.match(sym_tab[profiler_step_name_id])
-        if m:
-            return int(m.group(1))
-        return -1
-
-    def _extract_one_rank(df) -> pd.DataFrame:
-        profiler_step_name_ids = [
-            sym_map[k] for k in sorted([k for k in sym_map.keys() if k.startswith("ProfilerStep")])
-        ]
-        profiler_step_index = df["name"].isin(profiler_step_name_ids)
-        p_steps = df.loc[profiler_step_index, ["name", "ts", "dur"]].copy().rename(columns={"name": "profiler_step"})
-        p_steps["iter"] = p_steps["profiler_step"].apply(get_iter_nbr)
-        p_steps["end"] = p_steps["ts"] + p_steps["dur"]
-        p_steps.set_index("iter", inplace=True)
-        p_steps.drop(["profiler_step"], axis=1, inplace=True)
-        return p_steps
-
-    df_iterations = pd.concat(
-        [_extract_one_rank(trace.get_trace(r)) for r in ranks],
-        keys=ranks,
-        names=["rank", "iter"],
-    ).reset_index()
-    return df_iterations
-
-
-def _compute_normalized_start_time_of_significant_comm_kernels(
-    df: pd.DataFrame,
-    symbol_table: TraceSymbolTable,
-    visualize: bool = False,
-    min_normalized_duration: float = 0.01,
-) -> Tuple[pd.DataFrame, str]:
-    """
-    Computes the normalized start time of significant comm_kernels.
-
-    Args:
-        df (pd.DataFrame) : an input DataFrame with traces for selected ranks and iterations.
-        symbol_table (TraceSymbolTable) : the Trace Symbol Table for encoding/decoding the symbols in the trace DataFrame
-        visualize (bool): a flag to enable/disable visualizing the intermediate results.
-        min_normalized_duration (float) : a ratio for filtering out operators/kernels which are unlikely
-            to cause a rank to be a straggler.
-
-    Return:
-        Tuple[df: PdDataFrame, metric_name: str]
-            df is a DataFrame which contains
-            metric_name is a column name which can be used for straggler detection
-
-    Note:
-        + We break down straggler identification into two steps:
-            1. compute metric for straggler detection
-            2. detect straggler from the metric
-        + This function provides a reference implementation for computing a metric for straggler detection. A user
-            can choose a different metric and implement the corresponding metric computing function.
-        + The metric used in this function is the starting time of the last most dominating communication kernel. It
-            is computed in the following steps:
-            1. find all communication kernels which pass the duration test, i.e.,
-                kernel duration > mean_iter_time * min_normalized_duration (the default value is 1%)
-            2. pick the last kernel on each stream
-            3. select the stream-kernel combination which has the largest average standard deviation across ranks
-        + This metric is defined for each rank and for each iteration (excluding the last iteration
-            if it should be ignored).
-
-        + One implicit assumption underlying this function is that candidate GPU communication kernels for straggler
-            detection will involve a blocking all-to-all synchronization and thus end at about the same time.
-            Therefore, the later a kernel start, the bigger overall delay it likely causes.
-
-        + With more model-specific information, a user can create a metric easier to compute and understand.
-    """
-    # find all communication kernels
-    sym_table = symbol_table.get_sym_table()
-    sym_map = symbol_table.get_sym_id_map()
-    comm_op_ids = [sym_map[s] for s in sym_table if s.startswith("ncclKernel")]
-    iterations = _get_unique_values(df, "iteration")
-    ranks = _get_unique_values(df, "rank")
-    df = df.loc[df["iteration"].isin(iterations)]
-
-    # filter out short communication kernels with a duration threshold
-    n_iters = len(iterations)
-    t_min = df["ts"].min()
-    mean_iter_time = ((df["ts"] + df["dur"]).max() - t_min) / float(n_iters)
-    min_duration = mean_iter_time * min_normalized_duration
-    long_comm_kernels = df.loc[
-        (df["stream"] > 0) & (df["iteration"] > 0) & (df["dur"] >= min_duration) & (df["name"].isin(comm_op_ids))
-    ]
-    if visualize:  # pragma: no cover
-        plot_timeline_gpu_kernels(
-            f"Timeline of Communication Kernels Longer Than {min_normalized_duration * 100:.2f}% of Iteration Time\n",
-            long_comm_kernels,
-            symbol_table,
-            ranks=ranks,
-            duration_threshold=2000,
-        )
-
-    # select the last long communication kernel for all combinations of (rank, stream, iteration, kernel_name)
-    last_long_comm_kernels = long_comm_kernels.groupby(["rank", "stream", "iteration", "name"], as_index=False).last()
-
-    # select the (stream, name) combination whose duration has the largest mean standard deviation across all ranks
-    metric_name: str = "normalized_start_time"
-    last_long_comm_kernels[metric_name] = (last_long_comm_kernels["ts"] - t_min) / mean_iter_time
-    last_long_comm_kernels["duration"] = last_long_comm_kernels["dur"] / mean_iter_time
-    duration_diff_across_ranks = last_long_comm_kernels.groupby(["stream", "iteration", "name"])["duration"].std()
-    average_duration_diff = duration_diff_across_ranks.groupby(["stream", "name"]).mean()
-    (stream, name) = average_duration_diff.idxmax()
-
-    # Filter last_longer_comm_kernels
-    candidate_metric_kernels = last_long_comm_kernels.loc[
-        (last_long_comm_kernels["stream"].eq(stream)) & (last_long_comm_kernels["name"].eq(name))
-    ]
-
-    if visualize:  # pragma: no cover
-        plot_timeline_gpu_kernels(
-            f"Timeline of Candidate Kernels (Iterations={iterations})",
-            candidate_metric_kernels,
-            symbol_table,
-            ranks=ranks,
-        )
-
-    return candidate_metric_kernels, metric_name
-
-
-def _get_top_k_stragglers_with_metric(
-    metric_df: pd.DataFrame,
-    metric_name: str,
-    n_stragglers: int = 2,
-    visualize: bool = False,
-) -> pd.Series:
-    """
-    Get the top k potential straggler ranks.
-
-    Args:
-          metric_df (pd.DataFrame) : an input DataFrame which contains the performance metrics
-            for determining whether a particular rank could be a straggler.
-          metric_name (str) : a column name to select the metric from the DataFrame.
-          n_stragglers (int) : how many candidate stragglers to use in this algorithm?
-          visualize (bool) : a flag to enable/disable visualizing the results.
-
-    Returns:
-        A Series of integers with ranks as the index and the values indicating whether a rank is a potential straggler.
-        If the value for a rank <r> is positive, then rank <r> is a potential straggler;
-        otherwise it is treated as a non-straggler.
-
-    Notes:
-        + This function is built upon the metric derived for straggler detection and applies a candidate selection
-            algorithm to select potential straggler candidates.
-        + The algorithm implemented here is a k late start candidate which choose the top k candidates ranked by the
-            metric values.
-        + This function consider two scenarios:
-            (1) metric_df only contains metric for one iteration;
-            (2) metric_df contains metric for multiple iterations.
-    """
-    if n_stragglers <= 0:
-        n_stragglers = 1
-    n_iterations = metric_df["iteration"].nunique() if "iteration" in metric_df.columns else 1
-    with_iteration = True if n_iterations > 1 else False
-    if not with_iteration:
-        metric = metric_df[["rank", metric_name]].copy()
-        threshold = metric.sort_values(by=metric_name, ascending=False)[metric_name].tolist()[n_stragglers - 1]
-        metric["is_straggler"] = metric[metric_name].apply(lambda x: 1 if x >= threshold else 0)
-        data_columns = ["rank", metric_name]
-        results = metric[["rank", "is_straggler"]].copy().set_index("rank")["is_straggler"]
-    else:
-        metric = metric_df[["rank", "iteration", metric_name]].copy()
-        metric["is_straggler"] = 0
-        for iteration, group in metric.groupby("iteration"):
-            if iteration < 0:
-                continue
-            threshold = group.sort_values(by=metric_name, ascending=False)[metric_name].tolist()[n_stragglers - 1]
-            metric.loc[group.index, "is_straggler"] = group[metric_name].apply(lambda x: 1 if x >= threshold else 0)
-        data_columns = ["rank", "iteration", metric_name]
-        results = metric.groupby("rank")["is_straggler"].sum()
-
-    metric["is_straggler"] = metric["is_straggler"].apply(lambda x: "Yes" if x > 0 else "No")
-    for col in data_columns:
-        metric[col] = pd.to_numeric(metric[col])
-
-    color_map = {"Yes": "red", "No": "blue"}
-    if visualize:  # pragma: no cover
-        fig = px.bar(
-            metric,
-            x="rank",
-            y=metric_name,
-            facet_col="iteration" if with_iteration else None,
-            color="is_straggler",
-            color_discrete_map=color_map,
-            hover_data=data_columns,
-            width=300 * n_iterations,
-            title="Potential Stragglers",
-        )
-        fig.show()
-
-    return results
-
-
-def find_stragglers_with_late_start_comm_kernels(
-    df: pd.DataFrame,
-    symbol_table: TraceSymbolTable,
-    n_stragglers: int = 2,
-    visualize: bool = False,
-) -> pd.Series:
-    """Identify potential stragglers from the traces.
-
-    Args:
-          df (pd.DataFrame) : an input DataFrame with traces for selected ranks and iterations.
-          symbol_table (TraceSymbolTable) : the Trace Symbol Table for encoding/decoding the symbols in the trace DataFrame
-          n_stragglers (int) : how many candidate stragglers to use in this algorithm?
-          visualize (bool) : a flag to enable/disable visualizing the results.
-
-    Returns:
-        stragglers (pd.Series): a Series of which ranks are the index and values are the number of times
-            that a rank is detected as a potential straggler. For example, given a rank r,
-            if stragglers[r] > 0, then rank <r> is detected as a straggler for stragglers[r] times.
-    """
-
-    metric_df, metric_name = _compute_normalized_start_time_of_significant_comm_kernels(df, symbol_table, visualize)
-    stragglers = _get_top_k_stragglers_with_metric(
-        metric_df, metric_name, visualize=visualize, n_stragglers=n_stragglers
-    )
-    return stragglers
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
+
+import re
+from typing import Tuple
+
+import pandas as pd
+import plotly.express as px
+
+from hta.analyzers.timeline import _get_unique_values, plot_timeline_gpu_kernels
+from hta.common.trace import Trace, TraceSymbolTable
+
+
+def extract_iteration_info(trace: Trace) -> pd.DataFrame:
+    """Extract the iteration information from a trace.
+
+    Args:
+          trace (Trace) : a trace object
+
+    Returns:
+        a DataFrame that contains all the iteration information with rank as a column.
+    """
+    ranks = [k for k in trace.get_all_traces().keys()]
+    sym_map = trace.symbol_table.get_sym_id_map()
+    sym_tab = trace.symbol_table.get_sym_table()
+
+    def get_iter_nbr(profiler_step_name_id: int) -> int:
+        iter_re = re.compile(r"ProfilerStep\s*#\s*(\d+)")
+        m = iter_re.match(sym_tab[profiler_step_name_id])
+        if m:
+            return int(m.group(1))
+        return -1
+
+    def _extract_one_rank(df) -> pd.DataFrame:
+        profiler_step_name_ids = [
+            sym_map[k]
+            for k in sorted([k for k in sym_map.keys() if k.startswith("ProfilerStep")])
+        ]
+        profiler_step_index = df["name"].isin(profiler_step_name_ids)
+        p_steps = (
+            df.loc[profiler_step_index, ["name", "ts", "dur"]]
+            .copy()
+            .rename(columns={"name": "profiler_step"})
+        )
+        p_steps["iter"] = p_steps["profiler_step"].apply(get_iter_nbr)
+        p_steps["end"] = p_steps["ts"] + p_steps["dur"]
+        p_steps.set_index("iter", inplace=True)
+        p_steps.drop(["profiler_step"], axis=1, inplace=True)
+        return p_steps
+
+    df_iterations = pd.concat(
+        [_extract_one_rank(trace.get_trace(r)) for r in ranks],
+        keys=ranks,
+        names=["rank", "iter"],
+    ).reset_index()
+    return df_iterations
+
+
+def _compute_normalized_start_time_of_significant_comm_kernels(
+    df: pd.DataFrame,
+    symbol_table: TraceSymbolTable,
+    visualize: bool = False,
+    min_normalized_duration: float = 0.01,
+) -> Tuple[pd.DataFrame, str]:
+    """
+    Computes the normalized start time of significant comm_kernels.
+
+    Args:
+        df (pd.DataFrame) : an input DataFrame with traces for selected ranks and iterations.
+        symbol_table (TraceSymbolTable) : the Trace Symbol Table for encoding/decoding the symbols in the trace DataFrame
+        visualize (bool): a flag to enable/disable visualizing the intermediate results.
+        min_normalized_duration (float) : a ratio for filtering out operators/kernels which are unlikely
+            to cause a rank to be a straggler.
+
+    Return:
+        Tuple[df: PdDataFrame, metric_name: str]
+            df is a DataFrame which contains
+            metric_name is a column name which can be used for straggler detection
+
+    Note:
+        + We break down straggler identification into two steps:
+            1. compute metric for straggler detection
+            2. detect straggler from the metric
+        + This function provides a reference implementation for computing a metric for straggler detection. A user
+            can choose a different metric and implement the corresponding metric computing function.
+        + The metric used in this function is the starting time of the last most dominating communication kernel. It
+            is computed in the following steps:
+            1. find all communication kernels which pass the duration test, i.e.,
+                kernel duration > mean_iter_time * min_normalized_duration (the default value is 1%)
+            2. pick the last kernel on each stream
+            3. select the stream-kernel combination which has the largest average standard deviation across ranks
+        + This metric is defined for each rank and for each iteration (excluding the last iteration
+            if it should be ignored).
+
+        + One implicit assumption underlying this function is that candidate GPU communication kernels for straggler
+            detection will involve a blocking all-to-all synchronization and thus end at about the same time.
+            Therefore, the later a kernel start, the bigger overall delay it likely causes.
+
+        + With more model-specific information, a user can create a metric easier to compute and understand.
+    """
+    # find all communication kernels
+    sym_table = symbol_table.get_sym_table()
+    sym_map = symbol_table.get_sym_id_map()
+    comm_op_ids = [sym_map[s] for s in sym_table if s.startswith("ncclKernel")]
+    iterations = _get_unique_values(df, "iteration")
+    ranks = _get_unique_values(df, "rank")
+    df = df.loc[df["iteration"].isin(iterations)]
+
+    # filter out short communication kernels with a duration threshold
+    n_iters = len(iterations)
+    t_min = df["ts"].min()
+    mean_iter_time = ((df["ts"] + df["dur"]).max() - t_min) / float(n_iters)
+    min_duration = mean_iter_time * min_normalized_duration
+    long_comm_kernels = df.loc[
+        (df["stream"] > 0)
+        & (df["iteration"] > 0)
+        & (df["dur"] >= min_duration)
+        & (df["name"].isin(comm_op_ids))
+    ]
+    if visualize:  # pragma: no cover
+        plot_timeline_gpu_kernels(
+            f"Timeline of Communication Kernels Longer Than {min_normalized_duration * 100:.2f}% of Iteration Time\n",
+            long_comm_kernels,
+            symbol_table,
+            ranks=ranks,
+            duration_threshold=2000,
+        )
+
+    # select the last long communication kernel for all combinations of (rank, stream, iteration, kernel_name)
+    last_long_comm_kernels = long_comm_kernels.groupby(
+        ["rank", "stream", "iteration", "name"], as_index=False
+    ).last()
+
+    # select the (stream, name) combination whose duration has the largest mean standard deviation across all ranks
+    metric_name: str = "normalized_start_time"
+    last_long_comm_kernels[metric_name] = (
+        last_long_comm_kernels["ts"] - t_min
+    ) / mean_iter_time
+    last_long_comm_kernels["duration"] = last_long_comm_kernels["dur"] / mean_iter_time
+    duration_diff_across_ranks = last_long_comm_kernels.groupby(
+        ["stream", "iteration", "name"]
+    )["duration"].std()
+    average_duration_diff = duration_diff_across_ranks.groupby(
+        ["stream", "name"]
+    ).mean()
+    (stream, name) = average_duration_diff.idxmax()
+
+    # Filter last_longer_comm_kernels
+    candidate_metric_kernels = last_long_comm_kernels.loc[
+        (last_long_comm_kernels["stream"].eq(stream))
+        & (last_long_comm_kernels["name"].eq(name))
+    ]
+
+    if visualize:  # pragma: no cover
+        plot_timeline_gpu_kernels(
+            f"Timeline of Candidate Kernels (Iterations={iterations})",
+            candidate_metric_kernels,
+            symbol_table,
+            ranks=ranks,
+        )
+
+    return candidate_metric_kernels, metric_name
+
+
+def _get_top_k_stragglers_with_metric(
+    metric_df: pd.DataFrame,
+    metric_name: str,
+    n_stragglers: int = 2,
+    visualize: bool = False,
+) -> pd.Series:
+    """
+    Get the top k potential straggler ranks.
+
+    Args:
+          metric_df (pd.DataFrame) : an input DataFrame which contains the performance metrics
+            for determining whether a particular rank could be a straggler.
+          metric_name (str) : a column name to select the metric from the DataFrame.
+          n_stragglers (int) : how many candidate stragglers to use in this algorithm?
+          visualize (bool) : a flag to enable/disable visualizing the results.
+
+    Returns:
+        A Series of integers with ranks as the index and the values indicating whether a rank is a potential straggler.
+        If the value for a rank <r> is positive, then rank <r> is a potential straggler;
+        otherwise it is treated as a non-straggler.
+
+    Notes:
+        + This function is built upon the metric derived for straggler detection and applies a candidate selection
+            algorithm to select potential straggler candidates.
+        + The algorithm implemented here is a k late start candidate which choose the top k candidates ranked by the
+            metric values.
+        + This function consider two scenarios:
+            (1) metric_df only contains metric for one iteration;
+            (2) metric_df contains metric for multiple iterations.
+    """
+    if n_stragglers <= 0:
+        n_stragglers = 1
+    n_iterations = (
+        metric_df["iteration"].nunique() if "iteration" in metric_df.columns else 1
+    )
+    with_iteration = True if n_iterations > 1 else False
+    if not with_iteration:
+        metric = metric_df[["rank", metric_name]].copy()
+        threshold = metric.sort_values(by=metric_name, ascending=False)[
+            metric_name
+        ].tolist()[n_stragglers - 1]
+        metric["is_straggler"] = metric[metric_name].apply(
+            lambda x: 1 if x >= threshold else 0
+        )
+        data_columns = ["rank", metric_name]
+        results = (
+            metric[["rank", "is_straggler"]].copy().set_index("rank")["is_straggler"]
+        )
+    else:
+        metric = metric_df[["rank", "iteration", metric_name]].copy()
+        metric["is_straggler"] = 0
+        for iteration, group in metric.groupby("iteration"):
+            if iteration < 0:
+                continue
+            threshold = group.sort_values(by=metric_name, ascending=False)[
+                metric_name
+            ].tolist()[n_stragglers - 1]
+            metric.loc[group.index, "is_straggler"] = group[metric_name].apply(
+                lambda x: 1 if x >= threshold else 0
+            )
+        data_columns = ["rank", "iteration", metric_name]
+        results = metric.groupby("rank")["is_straggler"].sum()
+
+    metric["is_straggler"] = metric["is_straggler"].apply(
+        lambda x: "Yes" if x > 0 else "No"
+    )
+    for col in data_columns:
+        metric[col] = pd.to_numeric(metric[col])
+
+    color_map = {"Yes": "red", "No": "blue"}
+    if visualize:  # pragma: no cover
+        fig = px.bar(
+            metric,
+            x="rank",
+            y=metric_name,
+            facet_col="iteration" if with_iteration else None,
+            color="is_straggler",
+            color_discrete_map=color_map,
+            hover_data=data_columns,
+            width=300 * n_iterations,
+            title="Potential Stragglers",
+        )
+        fig.show()
+
+    return results
+
+
+def find_stragglers_with_late_start_comm_kernels(
+    df: pd.DataFrame,
+    symbol_table: TraceSymbolTable,
+    n_stragglers: int = 2,
+    visualize: bool = False,
+) -> pd.Series:
+    """Identify potential stragglers from the traces.
+
+    Args:
+          df (pd.DataFrame) : an input DataFrame with traces for selected ranks and iterations.
+          symbol_table (TraceSymbolTable) : the Trace Symbol Table for encoding/decoding the symbols in the trace DataFrame
+          n_stragglers (int) : how many candidate stragglers to use in this algorithm?
+          visualize (bool) : a flag to enable/disable visualizing the results.
+
+    Returns:
+        stragglers (pd.Series): a Series of which ranks are the index and values are the number of times
+            that a rank is detected as a potential straggler. For example, given a rank r,
+            if stragglers[r] > 0, then rank <r> is detected as a straggler for stragglers[r] times.
+    """
+
+    metric_df, metric_name = _compute_normalized_start_time_of_significant_comm_kernels(
+        df, symbol_table, visualize
+    )
+    stragglers = _get_top_k_stragglers_with_metric(
+        metric_df, metric_name, visualize=visualize, n_stragglers=n_stragglers
+    )
+    return stragglers
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/straggler_analysis.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/straggler_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import TYPE_CHECKING, Callable, List, Optional
+from typing import Callable, List, Optional, TYPE_CHECKING
 
 import pandas as pd
 
-from hta.analyzers.straggler import extract_iteration_info, find_stragglers_with_late_start_comm_kernels
+from hta.analyzers.straggler import (
+    extract_iteration_info,
+    find_stragglers_with_late_start_comm_kernels,
+)
 from hta.configs.config import logger
 
 # import statement used without the "if TYPE_CHECKING" guard will cause a circular
 # dependency with trace_analysis.py causing mypy to fail and should not be removed.
 if TYPE_CHECKING:
     from hta.common.trace import Trace
 
@@ -20,50 +23,62 @@
         pass
 
     @classmethod
     def get_profiler_steps(cls, t: "Trace") -> List[int]:
         """
         Profiler steps implementation. Returns the list of profiler steps.
         """
-        return sorted([i for i in extract_iteration_info(t)["iter"].unique() if i != -1])
+        return sorted(
+            [i for i in extract_iteration_info(t)["iter"].unique() if i != -1]
+        )
 
     @classmethod
     def get_potential_stragglers(
         cls,
         t: "Trace",
         profiler_steps: Optional[List[int]] = None,
         num_candidates: int = 2,
         visualize: bool = False,
-        straggler_identification_impl: Callable[..., pd.Series] = find_stragglers_with_late_start_comm_kernels,
+        straggler_identification_impl: Callable[
+            ..., pd.Series
+        ] = find_stragglers_with_late_start_comm_kernels,
     ) -> List[int]:
         """
         Straggler analysis implementation. See `get_potential_stragglers` in `trace_analysis.py` for details.
         """
         if num_candidates < 1:
             num_candidates = 1
 
         available_profiler_steps = cls.get_profiler_steps(t)
         if profiler_steps is None:
             valid_profiler_steps = available_profiler_steps
         else:
-            valid_profiler_steps = [i for i in profiler_steps if i in available_profiler_steps]
+            valid_profiler_steps = [
+                i for i in profiler_steps if i in available_profiler_steps
+            ]
         if len(valid_profiler_steps) == 0:
             raise ValueError(
                 f"invalid value for argument: profiler_steps={profiler_steps}; available profiler steps={available_profiler_steps}"
             )
 
         ranks = list(t.get_all_traces().keys())
-        df_all = pd.concat([t.get_trace(r) for r in ranks], axis=0, keys=ranks, names=["rank", "idx"]).reset_index()
-
-        df_selected_profiler_steps = df_all.loc[df_all["iteration"].isin(valid_profiler_steps)]
+        df_all = pd.concat(
+            [t.get_trace(r) for r in ranks], axis=0, keys=ranks, names=["rank", "idx"]
+        ).reset_index()
+
+        df_selected_profiler_steps = df_all.loc[
+            df_all["iteration"].isin(valid_profiler_steps)
+        ]
 
         straggler_counts = straggler_identification_impl(
             df_selected_profiler_steps, t.symbol_table, num_candidates, visualize
         )
-        stragglers = straggler_counts.sort_values(ascending=False)[:num_candidates].index.tolist()
+        stragglers = straggler_counts.sort_values(ascending=False)[
+            :num_candidates
+        ].index.tolist()
 
         if len(stragglers) > 1:
             logger.debug(f"found ranks {stragglers} are potential stragglers.")
         else:
             logger.debug(f"found rank {stragglers} is a potential straggler.")
 
         return stragglers
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/timeline.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 import pandas as pd
 import plotly.express as px
 
 from hta.common.trace import Trace, TraceSymbolTable
 from hta.configs.config import logger
 
 
-def plot_timeline(title: str, events: pd.DataFrame, ranks: Optional[List[int]] = None) -> None:
+def plot_timeline(
+    title: str, events: pd.DataFrame, ranks: Optional[List[int]] = None
+) -> None:
     """
     Plot the timeline of events
 
     Args:
         title (str): a title for the timeline plot
         events (pd.DataFrame): a data contains the events to be plotted.
         ranks (List[int]) : a list of ranks whose events will be plotted.
@@ -39,15 +41,17 @@
     must_have_columns: List[str] = [
         "calibrated_start_global",
         "calibrated_end_global",
         "task",
         "label",
     ]
     if not set(must_have_columns).issubset(set(events.columns)):
-        raise ValueError(f"the events dataframe doesn't contain all required columns {must_have_columns}")
+        raise ValueError(
+            f"the events dataframe doesn't contain all required columns {must_have_columns}"
+        )
 
     if ranks is None:
         if "rank" not in events.columns:
             ranks = []
         else:
             ranks = sorted(events["rank"].unique())
 
@@ -79,15 +83,17 @@
     )
     fig.show()
 
     t1 = perf_counter()
     logger.debug(f"Plotted timeline in {t1 - t0:.2f} seconds")
 
 
-def _get_unique_values(df: pd.DataFrame, col: str, exclude_values: List[int] = [-1]) -> List[int]:
+def _get_unique_values(
+    df: pd.DataFrame, col: str, exclude_values: List[int] = [-1]
+) -> List[int]:
     """Get the unique values for a given column <col> in the input Dataframe <df>
 
     Args:
         df (pd.DataFrame) : a DataFrame with trace events
         col (str) : a column name
         exclude_values (List[int]) : list of values to be excluded from the returned list
 
@@ -134,42 +140,58 @@
         duration_threshold (int) : the minimum duration given for short kernels for them to be visible on the figure.
     Return:
         a DataFrame for selected GPU events for plot_timeline_px
     """
     t0 = perf_counter()
     required_columns: List[str] = ["iteration", "name", "cat", "rank", "stream", "ts"]
     if not set(required_columns).issubset(set(df.columns)):
-        raise ValueError(f"columns {set(required_columns) - set(df.columns)} are not in input DataFrame")
+        raise ValueError(
+            f"columns {set(required_columns) - set(df.columns)} are not in input DataFrame"
+        )
 
     if ranks is None:
         ranks = _get_unique_values(df, "rank")
 
     if iterations is None:
         iterations = _get_unique_values(df, "iteration")
 
     if streams is None:
         streams = _get_unique_values(df, "stream")
 
-    events = df.loc[(df["rank"].isin(ranks)) & (df["iteration"].isin(iterations)) & (df["stream"].isin(streams))].copy()
+    events = df.loc[
+        (df["rank"].isin(ranks))
+        & (df["iteration"].isin(iterations))
+        & (df["stream"].isin(streams))
+    ].copy()
 
     sym_tab = symbol_table.get_sym_table()
     events["s_name"] = events["name"].apply(lambda i: sym_tab[i]).apply(_simplify_name)
     events["s_cat"] = events["cat"].apply(lambda i: sym_tab[i])
     events["calibrated_start_global"] = pd.to_datetime(events["ts"], unit="us")
     events["calibrated_end_global"] = pd.to_datetime(
-        events["ts"] + events["dur"].apply(lambda x: x if x >= duration_threshold else duration_threshold),
+        events["ts"]
+        + events["dur"].apply(
+            lambda x: x if x >= duration_threshold else duration_threshold
+        ),
         unit="us",
     )
 
     events["label"] = events["s_name"]
-    events["task"] = "rank " + events["rank"].astype("str") + " stream " + events["stream"].astype("str")
+    events["task"] = (
+        "rank "
+        + events["rank"].astype("str")
+        + " stream "
+        + events["stream"].astype("str")
+    )
     events = events.sort_values(by=["rank", "stream", "ts"])
 
     t1 = perf_counter()
-    logger.debug(f"Preprocessed events data for timeline visualization in {t1 - t0:.2f} seconds")
+    logger.debug(
+        f"Preprocessed events data for timeline visualization in {t1 - t0:.2f} seconds"
+    )
 
     return events
 
 
 def plot_timeline_gpu_kernels(
     title: str,
     df: pd.DataFrame,
@@ -187,15 +209,17 @@
         df: an input DataFrame.
         symbol_table: input trace symbol table for mapping symbol id back to text.
         ranks List[int]: filter the input DataFrame with the given set of ranks; use all ranks if None.
         iterations List[int]: filter the input DataFrame with the given set of iterations; use all iterations if None.
         streams List[int]: filter the input DataFrame with the given set of streams; use all streams if None.
         duration_threshold (int) : the minimum duration given for short kernels for them to be visible on the figure.
     """
-    df_timeline = prepare_timeline_gpu_events(df, symbol_table, ranks, iterations, streams, duration_threshold)
+    df_timeline = prepare_timeline_gpu_events(
+        df, symbol_table, ranks, iterations, streams, duration_threshold
+    )
     plot_timeline(title, df_timeline)
 
 
 def plot_timeline_gpu_kernels_from_trace(
     title: str,
     trace_data: Trace,
     ranks: Optional[List[int]] = None,
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/analyzers/trace_counters.py` & `HolisticTraceAnalysis-0.2.0/hta/analyzers/trace_counters.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 from typing import Dict, List, Optional
 
 import pandas as pd
 
 from hta.common.trace import Trace
 from hta.configs.config import logger
-from hta.utils.utils import KernelType, get_kernel_type, get_memory_kernel_type
+from hta.utils.utils import get_kernel_type, get_memory_kernel_type, KernelType
 
 
 class TraceCounters:
     def __init__(self):
         pass
 
     @classmethod
-    def _get_queue_length_time_series_for_rank(cls, t: "Trace", rank: int) -> Optional[pd.DataFrame]:
+    def _get_queue_length_time_series_for_rank(
+        cls, t: "Trace", rank: int
+    ) -> Optional[pd.DataFrame]:
         """
         Returns an (optional) dataframe with time series for the queue length
         on a CUDA streams within requested rank.
 
         Queue length is defined as the number of outstanding CUDA operations on a stream
         The value of the queue length is:
         1. Incremented when a CUDA runtime operation enqueues a kernel on a stream.
@@ -65,15 +67,17 @@
 
         # Concat the series of runtime launch events and GPU kernel events
         merged_df = (
             pd.concat(
                 [
                     # use the pid, tid and cuda stream from the correlated GPU event.
                     runtime_calls.join(
-                        gpu_kernels[["stream", "pid", "tid", "correlation"]].set_index("correlation"),
+                        gpu_kernels[["stream", "pid", "tid", "correlation"]].set_index(
+                            "correlation"
+                        ),
                         on="correlation",
                     ),
                     gpu_kernels,
                 ]
             )
             .sort_values(by="ts")
             .set_index("index")
@@ -124,15 +128,18 @@
 
         logger.info(
             "Please note that the time series only contains points "
             "when the value changes. Once a values is observed the time series "
             "stays constant until the next update."
         )
 
-        result = {rank: TraceCounters._get_queue_length_time_series_for_rank(t, rank) for rank in ranks}
+        result = {
+            rank: TraceCounters._get_queue_length_time_series_for_rank(t, rank)
+            for rank in ranks
+        }
         return dict(filter(lambda x: x[1] is not None, result.items()))
 
     @classmethod
     def get_queue_length_summary(
         cls,
         t: "Trace",
         ranks: Optional[List[int]] = None,
@@ -150,22 +157,30 @@
                 stream and rank.
         """
         if ranks is None or len(ranks) == 0:
             ranks = [0]
 
         results_list: List[pd.DataFrame] = []
 
-        for rank, rank_df in TraceCounters.get_queue_length_time_series(t, ranks).items():
+        for rank, rank_df in TraceCounters.get_queue_length_time_series(
+            t, ranks
+        ).items():
             rank_df["rank"] = rank
-            result = rank_df[["rank", "stream", "queue_length"]].groupby(["rank", "stream"]).describe()
+            result = (
+                rank_df[["rank", "stream", "queue_length"]]
+                .groupby(["rank", "stream"])
+                .describe()
+            )
             results_list.append(result)
         return pd.concat(results_list) if len(results_list) > 0 else None
 
     @classmethod
-    def _get_memory_bw_time_series_for_rank(cls, t: "Trace", rank: int) -> Optional[pd.DataFrame]:
+    def _get_memory_bw_time_series_for_rank(
+        cls, t: "Trace", rank: int
+    ) -> Optional[pd.DataFrame]:
         """
         Returns time series for the memory bandwidth of memory copy and memory set operations
         for specified rank.
 
         Args:
             t (Trace): Input trace data structure.
             rank (int): rank to generate the time series for.
@@ -182,25 +197,29 @@
         sym_table = t.symbol_table.get_sym_table()
 
         gpu_kernels = trace_df[trace_df["stream"].ne(-1)].copy()
         gpu_kernels["kernel_type"] = gpu_kernels[["name"]].apply(
             lambda x: get_kernel_type(sym_table[x["name"]]), axis=1
         )
 
-        memcpy_kernels = gpu_kernels[gpu_kernels.kernel_type == KernelType.MEMORY.name].copy()
+        memcpy_kernels = gpu_kernels[
+            gpu_kernels.kernel_type == KernelType.MEMORY.name
+        ].copy()
         memcpy_kernels["name"] = memcpy_kernels[["name"]].apply(
             lambda x: get_memory_kernel_type(sym_table[x["name"]]), axis=1
         )
 
         # In case of 0 us duration events round it up to 1 us to avoid -ve values
         # see https://github.com/facebookresearch/HolisticTraceAnalysis/issues/20
         memcpy_kernels.loc[memcpy_kernels.dur == 0, ["dur"]] = 1
 
         membw_time_series_a = memcpy_kernels[["ts", "name", "pid", "memory_bw_gbps"]]
-        membw_time_series_b = memcpy_kernels[["ts", "name", "dur", "pid", "memory_bw_gbps"]].copy()
+        membw_time_series_b = memcpy_kernels[
+            ["ts", "name", "dur", "pid", "memory_bw_gbps"]
+        ].copy()
 
         # The end events have timestamps = start timestamp + duration
         membw_time_series_b.ts = membw_time_series_b.ts + membw_time_series_b.dur
         membw_time_series_b.memory_bw_gbps = -membw_time_series_b.memory_bw_gbps
 
         membw_time_series = pd.concat(
             [
@@ -245,15 +264,18 @@
             ranks = [0]
 
         logger.info(
             "Please note that the time series only contains points "
             "when the value changes. Once a values is observed the time series "
             "stays constant until the next update."
         )
-        result = {rank: TraceCounters._get_memory_bw_time_series_for_rank(t, rank) for rank in ranks}
+        result = {
+            rank: TraceCounters._get_memory_bw_time_series_for_rank(t, rank)
+            for rank in ranks
+        }
         return dict(filter(lambda x: x[1] is not None, result.items()))
 
     @classmethod
     def get_memory_bw_summary(
         cls,
         t: "Trace",
         ranks: Optional[List[int]] = None,
@@ -277,10 +299,14 @@
         results_list: List[pd.DataFrame] = []
 
         for rank, rank_df in TraceCounters.get_memory_bw_time_series(t, ranks).items():
             rank_df["rank"] = rank
             # Exclude the 0 points in time series
             rank_df = rank_df[rank_df.memory_bw_gbps > 0]
 
-            result = rank_df[["rank", "name", "memory_bw_gbps"]].groupby(["rank", "name"]).describe()
+            result = (
+                rank_df[["rank", "name", "memory_bw_gbps"]]
+                .groupby(["rank", "name"])
+                .describe()
+            )
             results_list.append(result)
         return pd.concat(results_list) if len(results_list) > 0 else None
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/common/call_stack.py` & `HolisticTraceAnalysis-0.2.0/hta/common/call_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,14 @@
         self.nodes: Dict[int, CallStackNode] = {}
         self.correlations: pd.Series = None
         self.depth: pd.Series = None
         self._construct_call_stack_graph(df)
         self._compute_depth()
 
     def __repr__(self):
-
         ret = "\n"
         for key, item in self.nodes.items():
             ret = ret + f"    {key}: {item}\n"
 
         return f"CallStackGraph({ret})"
 
     def _construct_call_stack_graph(self, df) -> None:
@@ -199,15 +198,17 @@
         In this function, we assume:
         (1) the traces are from a single thread/stream and therefore
         (2) there is no overlap between the time intervals of the entities on the same level of the graph.
 
         We skip the call graph construction for GPU streams because the kernels on a single stream is just a list.
         """
         if "index_correlation" not in df.columns:
-            raise ValueError("The input DataFrame doesn't have column 'index_correlation'")
+            raise ValueError(
+                "The input DataFrame doesn't have column 'index_correlation'"
+            )
         self.correlations = df["index_correlation"]
 
         if self.device_type == DeviceType.GPU:
             return
 
         self.nodes.clear()
         self.nodes[NULL_NODE_INDEX] = CallStackNode(NULL_NODE_INDEX, -1, [])
@@ -246,15 +247,17 @@
         if parent_index not in self.nodes:
             # This should only occurs for the root node
             self.nodes[parent_index] = CallStackNode(NULL_NODE_INDEX, 0, [child_index])
         else:
             self.nodes[parent_index].children.append(child_index)
 
         # The parent node should always exist at this point.
-        self.nodes[child_index] = CallStackNode(parent_index, self.nodes[parent_index].depth + 1, [])
+        self.nodes[child_index] = CallStackNode(
+            parent_index, self.nodes[parent_index].depth + 1, []
+        )
 
     def get_nodes(self) -> Dict[int, CallStackNode]:
         """Return the nodes of this graph."""
         return self.nodes
 
     def get_parent(self, idx: int) -> int:
         """Return the parent of a given node <idx>""
@@ -422,26 +425,32 @@
                 for tid, tid_group in pid_group.groupby(by="tid"):
                     csi = CallStackIdentity(rank, pid, tid)
                     csg = CallStackGraph(tid_group, csi)
                     self.call_stacks.append(csg)
                     call_stack_ids.append(csi)
 
         t1 = perf_counter()
-        logging.debug(f"Completed constructing call stack graph for in {t1 - t0:.3} seconds")
+        logging.debug(
+            f"Completed constructing call stack graph for in {t1 - t0:.3} seconds"
+        )
 
         # build a map from call stack meta data to call stack objects
         self.mapping = pd.DataFrame(
             {
                 "rank": [csi.rank for csi in call_stack_ids],
                 "pid": [csi.pid for csi in call_stack_ids],
                 "tid": [csi.tid for csi in call_stack_ids],
                 "csg_index": range(len(self.call_stacks)),
             }
         )
 
         # add depth information to the data frame
         for rank in ranks:
-            call_stack_indices = self.mapping[self.mapping["rank"].eq(rank)]["csg_index"]
-            depth = pd.concat([self.call_stacks[idx].get_depth() for idx in call_stack_indices])
+            call_stack_indices = self.mapping[self.mapping["rank"].eq(rank)][
+                "csg_index"
+            ]
+            depth = pd.concat(
+                [self.call_stacks[idx].get_depth() for idx in call_stack_indices]
+            )
             df = self.trace_data.get_trace(rank)
             df["depth"] = depth
         self.mapping.set_index(["rank", "pid", "tid"], inplace=True)
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/common/trace.py` & `HolisticTraceAnalysis-0.2.0/hta/common/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import json
 import multiprocessing as mp
 import os
 import queue
 import re
 import sys
 import time
+import tracemalloc
 from typing import Any, Dict, Iterable, List, Optional, Tuple
 
 import pandas as pd
 
 from hta.common.trace_file import get_trace_files
 from hta.configs.config import logger
 from hta.configs.default_values import DEFAULT_TRACE_DIR
-from hta.utils.utils import get_memory_usage, normalize_path
+from hta.utils.utils import get_mp_pool_size, normalize_path
 
 MetaData = Dict[str, Any]
 PHASE_COUNTER: str = "C"
 
 
 class _SymbolCollector:
     """
@@ -68,15 +69,17 @@
                 self.sym_index[s] = idx
 
     def add_symbols_mp(self, symbols_list: List[Iterable[str]]) -> None:
         m = mp.Manager()
         shared_queue: queue.Queue[Any] = m.Queue()
         collector = _SymbolCollector(shared_queue)
 
-        with mp.get_context("spawn").Pool(min(mp.cpu_count(), len(symbols_list))) as pool:
+        with mp.get_context("spawn").Pool(
+            min(mp.cpu_count(), len(symbols_list))
+        ) as pool:
             pool.map(collector, symbols_list)
             pool.close()
             pool.join()
 
         all_symbols = []
         while not shared_queue.empty():
             all_symbols.append(shared_queue.get())
@@ -104,20 +107,19 @@
     if trace_file_path.endswith(".gz"):
         with gzip.open(trace_file_path, "rb") as fh:
             trace_record = json.loads(fh.read())
     elif trace_file_path.endswith(".json"):
         with open(trace_file_path, "r") as fh2:
             trace_record = json.loads(fh2.read())
     else:
-        raise ValueError(f"expect the value of trace_file ({trace_file_path}) ends with '.gz' or 'json'")
+        raise ValueError(
+            f"expect the value of trace_file ({trace_file_path}) ends with '.gz' or 'json'"
+        )
     t_end = time.perf_counter()
-    logger.info(
-        f"Parsed {trace_file_path} time = {(t_end - t_start):.2f} seconds "
-        f"mem = {get_memory_usage(trace_record) / 1e6:.2f} MB"
-    )
+    logger.info(f"Parsed {trace_file_path} time = {(t_end - t_start):.2f} seconds ")
     return trace_record
 
 
 def compress_df(df: pd.DataFrame) -> Tuple[pd.DataFrame, TraceSymbolTable]:
     """
     Compress a Dataframe to reduce its memory footprint.
 
@@ -138,16 +140,31 @@
     df.drop(df[df["cat"] == "Trace"].index, inplace=True)
 
     # drop columns
     columns_to_drop = {"ph", "id", "bp", "s"}.intersection(set(df.columns))
     df.drop(list(columns_to_drop), axis=1, inplace=True)
 
     # extract arguments; the argument list needs to update when more arguments are used in the analysis.
-    for arg in ["stream", "correlation", "Trace iteration", "memory bandwidth (GB/s)"]:
-        df[arg] = df["args"].apply(lambda row: row.get(arg, -1) if isinstance(row, dict) else -1)
+    args_to_keep = {
+        "stream",
+        "correlation",
+        "Trace iteration",
+        "memory bandwidth (GB/s)",
+    }
+    # performance counters appear as args
+    if "cuda_profiler_range" in df.cat.unique():
+        counter_names = set.union(
+            *[set(d.keys()) for d in df[df.cat == "cuda_profiler_range"]["args"].values]
+        )
+        args_to_keep = args_to_keep.union(counter_names)
+
+    for arg in args_to_keep:
+        df[arg] = df["args"].apply(
+            lambda row: row.get(arg, -1) if isinstance(row, dict) else -1
+        )
     df.drop(["args"], axis=1, inplace=True)
     df.rename(columns={"memory bandwidth (GB/s)": "memory_bw_gbps"}, inplace=True)
 
     # create a local symbol table
     local_symbol_table = TraceSymbolTable()
     symbols = set(df["cat"].unique()).union(set(df["name"].unique()))
     local_symbol_table.add_symbols(symbols)
@@ -212,15 +229,17 @@
     if "correlation" not in df.columns:
         return df
     corr_df = df.loc[df["correlation"].ne(-1), ["index", "correlation", "stream"]]
     on_cpu = corr_df.loc[df["stream"].eq(-1)]
     on_gpu = corr_df.loc[df["stream"].ne(-1)]
     merged_cpu_idx = on_cpu.merge(on_gpu, on="correlation", how="inner")
     merged_gpu_idx = on_gpu.merge(on_cpu, on="correlation", how="inner")
-    matched = pd.concat([merged_cpu_idx, merged_gpu_idx], axis=0)[["index_x", "index_y"]].set_index("index_x")
+    matched = pd.concat([merged_cpu_idx, merged_gpu_idx], axis=0)[
+        ["index_x", "index_y"]
+    ].set_index("index_x")
 
     corr_index_map: Dict[int, int] = matched["index_y"].to_dict()
 
     def _set_corr_index(row):
         idx = row.name
         if idx in corr_index_map:
             return corr_index_map[idx]
@@ -323,15 +342,17 @@
     if "traceEvents" in trace_record:
         df = pd.DataFrame(trace_record["traceEvents"])
         df, local_symbol_table = compress_df(df)
         transform_correlation_to_index(df)
         add_iteration(df, local_symbol_table)
 
     t_end = time.perf_counter()
-    logger.debug(f"Parsed {trace_file_path} in {(t_end - t_start):.2f} seconds")
+    logger.debug(
+        f"Parsed {trace_file_path} in {(t_end - t_start):.2f} seconds; current PID:{os. getpid()}"
+    )
     return meta, df, local_symbol_table
 
 
 class Trace:
     """
     A container for the traces collected for a distributed ML training job.
 
@@ -362,15 +383,17 @@
             trace_dir (str) : a path used to derive `trace_path = normalize_path(trace_dir)`.
 
         Raises:
             AssertionError
         """
         self.trace_path: str = normalize_path(trace_dir)
         logger.info(f"{self.trace_path}")
-        self.trace_files: Dict[int, str] = trace_files if trace_files is not None else get_trace_files(self.trace_path)
+        self.trace_files: Dict[int, str] = (
+            trace_files if trace_files is not None else get_trace_files(self.trace_path)
+        )
         logger.debug(self.trace_files)
         self.traces: Dict[int, pd.DataFrame] = {}
         self.symbol_table = TraceSymbolTable()
         self.meta_data: Dict[int, MetaData] = {}
         self.min_ts: int = 0
 
         self._normalize_trace_filenames()
@@ -411,17 +434,21 @@
             ) = parse_trace_dataframe(trace_filepath)
             # update the global symbol table
             self.symbol_table.add_symbols(local_symbol_table.get_sym_table())
             # fix the encoding of the data frame
             local_table = local_symbol_table.get_sym_table()
             global_map = self.symbol_table.get_sym_id_map()
             for col in ["cat", "name"]:
-                self.traces[rank][col] = self.traces[rank][col].apply(lambda idx: global_map[local_table[idx]])
+                self.traces[rank][col] = self.traces[rank][col].apply(
+                    lambda idx: global_map[local_table[idx]]
+                )
 
-    def parse_multiple_ranks(self, ranks: List[int], use_multiprocessing: bool = True) -> None:
+    def parse_multiple_ranks(
+        self, ranks: List[int], use_multiprocessing: bool = True
+    ) -> None:
         """
         Parse the trace for a given rank.
 
         Args:
             ranks (List[int]) : a list of integers representing the ranks of multiple trainers.
             use_multiprocessing (bool) : whether the parser using multiprocessing or not.
         """
@@ -441,39 +468,52 @@
                     result[1],
                     result[2],
                 )
                 self.symbol_table.add_symbols(local_symbol_tables[rank].get_sym_table())
             logger.debug(f"finished parsing for all {len(ranks)} ranks")
         else:
             num_procs = min(mp.cpu_count(), len(ranks))
+            if len(ranks) <= 8:
+                num_procs = min(len(ranks), mp.cpu_count())
+            else:
+                tracemalloc.start()
+                parse_trace_dataframe(trace_paths[0])
+                current, peak = tracemalloc.get_traced_memory()
+                tracemalloc.stop()
+                num_procs = get_mp_pool_size(peak, len(ranks))
             logger.debug(f"using {num_procs} processes for parsing.")
-            with mp.get_context("spawn").Pool(num_procs) as pool:
+
+            with mp.get_context("fork").Pool(num_procs) as pool:
                 results = pool.map(parse_trace_dataframe, trace_paths)
                 pool.close()
                 pool.join()
             logger.debug(f"finished parallel parsing using {num_procs} processes.")
 
             # collect the results
-            for (rank, result) in zip(ranks, results):
+            for rank, result in zip(ranks, results):
                 self.meta_data[rank], self.traces[rank], local_symbol_tables[rank] = (
                     result[0],
                     result[1],
                     result[2],
                 )
                 self.symbol_table.add_symbols(local_symbol_tables[rank].get_sym_table())
 
         # Now we update the IDs in the Dataframe using the global symbols table.
         global_map = self.symbol_table.get_sym_id_map()
         for rank in ranks:
             local_table = local_symbol_tables[rank].get_sym_table()
             for col in ["cat", "name"]:
-                self.traces[rank][col] = self.traces[rank][col].apply(lambda idx: global_map[local_table[idx]])
+                self.traces[rank][col] = self.traces[rank][col].apply(
+                    lambda idx: global_map[local_table[idx]]
+                )
 
         t1 = time.perf_counter()
-        logger.debug(f"leaving {sys._getframe().f_code.co_name} duration={t1 - t0:.2f} seconds")
+        logger.debug(
+            f"leaving {sys._getframe().f_code.co_name} duration={t1 - t0:.2f} seconds"
+        )
 
     def parse_traces(
         self,
         max_ranks: int = -1,
         use_multiprocessing: bool = True,
     ) -> None:
         """
@@ -497,15 +537,17 @@
         if len(ranks) > 0:
             self.parse_multiple_ranks(ranks, use_multiprocessing and len(ranks) > 1)
             self.is_parsed = True
         else:
             logger.error("The list of ranks to be parsed is empty.")
             self.is_parsed = False
         t1 = time.perf_counter()
-        logger.debug(f"leaving {sys._getframe().f_code.co_name} duration={t1 - t0:.2f} seconds")
+        logger.debug(
+            f"leaving {sys._getframe().f_code.co_name} duration={t1 - t0:.2f} seconds"
+        )
 
     def align_and_filter_trace(self):
         """
         Align the starting time across multiple ranks and filter events that belong to incomplete iterations.
         """
         self._align_all_ranks()
         self._filter_irrelevant_gpu_kernels()
@@ -561,16 +603,20 @@
             json.dump(trace_contents, fp, indent=2)
 
     def _normalize_trace_filenames(self) -> None:
         """
         Normalize the trace filenames so that a rank's trace file can be located by self.trace_files[rank] itself.
         """
         if not isinstance(self.trace_files, dict):
-            logger.error(f"self.trace_files must be of type Dict[int, str]; got {type(self.trace_files)}")
-            raise ValueError(f"Expected trace_files to be Dict[int, str]; got {type(self.trace_files)}")
+            logger.error(
+                f"self.trace_files must be of type Dict[int, str]; got {type(self.trace_files)}"
+            )
+            raise ValueError(
+                f"Expected trace_files to be Dict[int, str]; got {type(self.trace_files)}"
+            )
 
         for rank in self.trace_files:
             filename = self.trace_files[rank]
             if not (filename.startswith(self.trace_path) or filename.startswith("/")):
                 self.trace_files[rank] = os.path.join(self.trace_path, filename)
 
     def _validate_trace_files(self) -> bool:
@@ -578,18 +624,22 @@
         Validate whether all trace files exist and are valid.
 
         Returns:
             success (bool) : True if all trace files in self.trace_files exist and are valid; False otherwise.
         """
         for rank, filepath in self.trace_files.items():
             if not (os.path.exists(filepath) and os.access(filepath, os.R_OK)):
-                logger.error(f"Trace file '{filepath}' doesn't exist or is not readable.")
+                logger.error(
+                    f"Trace file '{filepath}' doesn't exist or is not readable."
+                )
                 return False
             if not (filepath.endswith(".gz") or filepath.endswith(".json")):
-                logger.error(f"The postfix of trace file '{filepath}' is neither '.gz' or '.json'")
+                logger.error(
+                    f"The postfix of trace file '{filepath}' is neither '.gz' or '.json'"
+                )
                 return False
         return True
 
     def _align_all_ranks(self) -> None:
         """
         Align dataframes for all ranks such that the earliest event starts at time 0.
         """
@@ -604,23 +654,31 @@
         """
         sym_index = self.symbol_table.get_sym_id_map()
         profiler_steps = [v for k, v in sym_index.items() if "ProfilerStep" in k]
 
         def filter_gpu_kernels_for_one_rank(trace_df: pd.DataFrame) -> pd.DataFrame:
             cpu_kernels = trace_df[trace_df["stream"].eq(-1)]
             gpu_kernels = trace_df[trace_df["stream"].ne(-1)]
-            last_profiler_start = cpu_kernels[cpu_kernels["name"].isin(profiler_steps)]["ts"].max()
+            last_profiler_start = cpu_kernels[cpu_kernels["name"].isin(profiler_steps)][
+                "ts"
+            ].max()
             cpu_kernels = cpu_kernels[cpu_kernels["ts"] < last_profiler_start]
-            filtered_gpu_kernels = gpu_kernels.merge(cpu_kernels["correlation"], on="correlation", how="inner")
+            filtered_gpu_kernels = gpu_kernels.merge(
+                cpu_kernels["correlation"], on="correlation", how="inner"
+            )
             return pd.concat([filtered_gpu_kernels, cpu_kernels], axis=0)
 
         if not profiler_steps:
-            logger.warning("ProfilerStep not found in the trace. The analysis result may not be accurate.")
+            logger.warning(
+                "ProfilerStep not found in the trace. The analysis result may not be accurate."
+            )
         elif len(profiler_steps) == 1:
-            logger.warning("There is only one iteration in the trace. The analysis result may not be accurate.")
+            logger.warning(
+                "There is only one iteration in the trace. The analysis result may not be accurate."
+            )
         else:
             for rank, trace_df in self.traces.items():
                 self.traces[rank] = filter_gpu_kernels_for_one_rank(trace_df)
 
     def convert_time_series_to_events(
         self, series: pd.DataFrame, counter_name: str, counter_col: str
     ) -> List[Dict[str, Any]]:
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/common/trace_file.py` & `HolisticTraceAnalysis-0.2.0/hta/common/trace_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,73 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import gzip
 import json
 import os
-import sys
+import re
 from typing import Any, Dict, Tuple
 
 from hta.configs.config import logger
 
 
-def create_rank_to_trace_dict(trace_path: str) -> Tuple[bool, Dict]:
+def create_rank_to_trace_dict(trace_dir: str) -> Tuple[bool, Dict]:
     """
     Create a rank -> trace_filename map for traces located within the directory <trace_path>
 
     Args:
-        trace_path (str) : the path to the directory where the traces are located.
+        trace_dir (str) : the path to the directory where the traces are located.
 
     Returns:
         (success: bool, rank_trace_map: dict) : a tuple indicating whether the operation succeeds and the path
          to the map file being created.
             success (bool) : True if the file is created successfully; False otherwise.
             map_file_path (dict) : a dict with rank as key and trace_filename as the value
     """
 
-    if not (os.path.exists(trace_path) and os.access(trace_path, os.R_OK)):
-        logger.error(f"trace_path {trace_path} doesn't exist or is not readable")
+    if not (os.path.exists(trace_dir) and os.access(trace_dir, os.R_OK)):
+        logger.error(f"trace_path {trace_dir} doesn't exist or is not readable")
         return False, {}
 
-    file_list = [fn for fn in os.listdir(trace_path) if fn.endswith(".gz") or fn.endswith(".json")]
+    file_list = [
+        fn for fn in os.listdir(trace_dir) if fn.endswith(".gz") or fn.endswith(".json")
+    ]
     if len(file_list) == 0:
-        logger.warning(f"No trace file is found in {trace_path}")
+        logger.warning(f"No trace file is found in {trace_dir}")
         return False, {}
 
     rank_to_trace_dict: Dict[int, str] = {}
     for file in file_list:
-        filename = os.path.join(trace_path, file)
-        data = None
-        if file.endswith("gz"):
-            gzip_file_handle = gzip.open(filename, "rb")
-            data = json.loads(gzip_file_handle.read())
-        if file.endswith("json"):
-            json_file_handle = open(filename, "r")
-            data = json.loads(json_file_handle.read())
-
-        distributed_info = data.get("distributedInfo", None)
-        if distributed_info is None:
-            logger.error(
-                "If the trace file does not have the rank specified in it, then add the following snippet "
-                'key to the json files to use HTA; "distributedInfo": {"rank": 0}. If there are multiple '
-                "traces files, then each file should have a unique rank value."
-            )
-            sys.exit()
-
-        rank = distributed_info.get("rank", None)
-        if rank is None:
-            logger.error(
-                "If the trace file does not have the rank specified in it, then add the following snippet "
-                'key to the json files to use HTA; "distributedInfo": {"rank": 0}. If there are multiple '
-                "traces files, then each file should have a unique rank value."
-            )
-            sys.exit()
-
-        assert isinstance(rank, int), "Rank is expected to be an integer"
-        assert rank >= 0, "Rank must be a non-negative integer"
-        rank_to_trace_dict[rank] = filename
-    if len(rank_to_trace_dict) == 0:
-        logger.warning("Rank to trace dict has size zero.")
+        file_path = os.path.join(trace_dir, file)
+
+        with gzip.open(file_path, "rb") if file.endswith("gz") else open(
+            file_path, "r"
+        ) as f:
+            for line in f:
+                data = line.decode() if isinstance(line, bytes) else line
+                if "rank" in data:
+                    break
+
+            # match is like "rank": 6,
+            match = re.search(r'"rank": \d+', data)
+            if match:
+                rank = int(match.group().split(": ")[1])
+                if rank in rank_to_trace_dict:
+                    logger.error(
+                        f"File {rank_to_trace_dict[rank]} and file {file_path} has the same rank. Will use {file_path} as the path to rank: {rank}."
+                    )
+                rank_to_trace_dict[int(rank)] = file_path
+            else:
+                logger.error(
+                    "If the trace file does not have the rank specified in it, then add the following snippet "
+                    'key to the json files to use HTA; "distributedInfo": {"rank": 0}. If there are multiple '
+                    "traces files, then each file should have a unique rank value."
+                )
+
     return True, rank_to_trace_dict
 
 
 def get_trace_files(trace_path: str) -> Dict[int, str]:
     """
     Get the rank to trace map from traces in the directory <trace_path>.
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/configs/config.py` & `HolisticTraceAnalysis-0.2.0/hta/configs/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 ConfigValue = Union[None, bool, int, float, str, Dict[str, Any], List[Any], Set[Any]]
 
 
 def setup_logger(config_file: str = "logging.config") -> logging.Logger:
     global logger
     if config_file:
-        log_filepath = os.path.join(os.path.dirname(os.path.realpath(__file__)), "logging.config")
+        log_filepath = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "logging.config"
+        )
         logging.config.fileConfig(log_filepath)
         logger = logging.getLogger("hta")
     elif logger is None:
         logger = logging.getLogger()
     return logger
 
 
@@ -52,15 +54,19 @@
 
         Loading configurations from the subsequent configuration file will update previous configurations.
 
         If a configuration file in the above list doesn't exist, hta will skip such configuration file.
         As a class method, this function does not return the user defined config file path.
         """
         return [
-            str(Path(hta.__file__).parent.joinpath("configs").joinpath(DEFAULT_CONFIG_FILENAME)),
+            str(
+                Path(hta.__file__)
+                .parent.joinpath("configs")
+                .joinpath(DEFAULT_CONFIG_FILENAME)
+            ),
             str(Path.home().joinpath(".hta").joinpath(DEFAULT_CONFIG_FILENAME)),
             str(Path.cwd().joinpath(DEFAULT_CONFIG_FILENAME)),
         ]
 
     def __init__(
         self,
         config_file_path: Optional[str] = None,
@@ -69,15 +75,17 @@
         """
         Constructor of the HtaConfig class.
 
         Args:
              config_file_path (str): a user provided config file path.
              load_default_paths (bool) : control whether the analyzer should use available default configuration files.
         """
-        self.config_file_paths: List[str] = HtaConfig.get_default_paths() if load_default_paths else []
+        self.config_file_paths: List[str] = (
+            HtaConfig.get_default_paths() if load_default_paths else []
+        )
         if config_file_path:
             self.config_file_paths.append(config_file_path)
 
         self.config: Dict[str, Any] = {}
         for path in self.config_file_paths:
             if Path(path).exists() and os.access(path, os.R_OK):
                 with open(path) as fp:
@@ -90,17 +98,23 @@
         else:
             setup_logger()
 
     def get_config_file_paths(self) -> List[str]:
         """
         Return the available config file paths
         """
-        return [path for path in self.config_file_paths if Path(path).exists() and os.access(path, os.R_OK)]
+        return [
+            path
+            for path in self.config_file_paths
+            if Path(path).exists() and os.access(path, os.R_OK)
+        ]
 
-    def get_config(self, dot_path: Optional[str] = None, default_value: ConfigValue = None) -> ConfigValue:
+    def get_config(
+        self, dot_path: Optional[str] = None, default_value: ConfigValue = None
+    ) -> ConfigValue:
         """
          Return the value for a configuration key <doct_keys>.
 
         Args:
              dot_path (str) : a dot representation of a configuration path. For example, `a.b.c` will search the
              configuration for self.configs['a']['b']['c']. If dot_path is None, then the method will return
                  the entire set of configurations.
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/trace_analysis.py` & `HolisticTraceAnalysis-0.2.0/hta/trace_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from collections import defaultdict
-from enum import Flag, auto
+from enum import auto, Flag
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import pandas as pd
 
 from hta.analyzers.breakdown_analysis import BreakdownAnalysis
 from hta.analyzers.communication_analysis import CommunicationAnalysis
 from hta.analyzers.cuda_kernel_analysis import CudaKernelAnalysis
+from hta.analyzers.cupti_counter_analysis import CuptiCounterAnalysis
 from hta.analyzers.straggler import find_stragglers_with_late_start_comm_kernels
 from hta.analyzers.straggler_analysis import StragglerAnalysis
 from hta.analyzers.trace_counters import TraceCounters
 from hta.common.trace import Trace
 from hta.configs.config import logger
 from hta.configs.default_values import DEFAULT_TRACE_DIR
 
@@ -61,15 +62,17 @@
         return StragglerAnalysis.get_profiler_steps(self.t)
 
     def get_potential_stragglers(
         self,
         profiler_steps: Optional[List[int]] = None,
         num_candidates: int = 2,
         visualize: bool = False,
-        straggler_identification_impl: Callable[..., pd.Series] = find_stragglers_with_late_start_comm_kernels,
+        straggler_identification_impl: Callable[
+            ..., pd.Series
+        ] = find_stragglers_with_late_start_comm_kernels,
     ) -> List[int]:
         r"""
         Identify potential stragglers based on a pre-defined metric computed from the trace.
 
         Args:
             profiler_steps (List[int]) : A list of profiler steps used in the straggler analysis. If None, then use all
                                          iterations.
@@ -282,27 +285,33 @@
         Returns:
             None
         """
         if ranks is None or len(ranks) == 0:
             ranks = [0]
 
         if time_series is None:
-            time_series = TimeSeriesTypes.QUEUE_LENGTH | TimeSeriesTypes.MEMCPY_BANDWIDTH
+            time_series = (
+                TimeSeriesTypes.QUEUE_LENGTH | TimeSeriesTypes.MEMCPY_BANDWIDTH
+            )
 
         counter_events: Dict[int, List[Dict[str, Any]]] = defaultdict(list)
         if output_suffix == "":
             output_suffix = "_with_counters"
 
-        def add_time_series(series_dict: Dict[int, pd.DataFrame], counter_name: str, counter_col: str):
+        def add_time_series(
+            series_dict: Dict[int, pd.DataFrame], counter_name: str, counter_col: str
+        ):
             nonlocal counter_events
             """accept a rank -> time series dict and append it"""
             for rank, series in series_dict.items():
                 if "stream" in series.columns:
                     series.rename(columns={"stream": "id"}, inplace=True)
-                ce = self.t.convert_time_series_to_events(series, counter_name, counter_col)
+                ce = self.t.convert_time_series_to_events(
+                    series, counter_name, counter_col
+                )
                 counter_events[rank].extend(ce)
 
         if TimeSeriesTypes.QUEUE_LENGTH in time_series:
             add_time_series(
                 series_dict=TraceCounters.get_queue_length_time_series(self.t, ranks),
                 counter_name="Queue Length",
                 counter_col="queue_length",
@@ -313,15 +322,17 @@
                 counter_name="Memcpy BW",
                 counter_col="memory_bw_gbps",
             )
 
         for rank, ev_list in counter_events.items():
             raw_trace_content = self.t.get_raw_trace_for_one_rank(rank=rank)
             raw_trace_content["traceEvents"].extend(ev_list)
-            output_file = self.t.trace_files[rank].replace(".json", f"{output_suffix}.json")
+            output_file = self.t.trace_files[rank].replace(
+                ".json", f"{output_suffix}.json"
+            )
             logger.info(f"Writing trace with counters for rank {rank} to {output_file}")
             self.t.write_raw_trace(output_file, raw_trace_content)
 
     def get_queue_length_summary(
         self,
         ranks: Optional[List[int]] = None,
     ) -> Optional[pd.DataFrame]:
@@ -458,7 +469,38 @@
             if interval_r_df is not None:
                 interval_df_list.append(interval_r_df)
 
         return (
             pd.concat(idle_time_df_list),
             pd.concat(interval_df_list) if show_idle_interval_stats else None,
         )
+
+    def get_cupti_counter_data_with_operators(
+        self,
+        ranks: Optional[List[int]] = None,
+    ) -> List[pd.DataFrame]:
+        r"""Performance counters provide insights on how to speed up GPU
+        kernels. The PyTorch Profiler has a lightweight API [CUPTI Range
+        Profiler API](https://docs.nvidia.com/cupti/r_main.html#r_profiler)
+        that enables users to monitor performance counters from the device.
+
+        When the CUPTI Profiler mode is enabled then PyTorch will emit the
+        performance counters and annotates them in the trace.
+            * The events are logged under the `cuda_profiler_range` category.
+            * Counter values are logged in the `args` section of the trace.
+
+        This API can investigate performance measurements per kernel and
+        associate them to operators that the kernel belongs to. A single kernel
+        can map to multiple levels of operators (as operators can be nested).
+        To represent this we basically provide a list column called `op_stack`.
+        For further convenience we add the top and bottom level operator column
+        as well.
+
+        Args:
+            ranks (List[int]): List of ranks on which to run the analysis. Default = [0].
+        Returns:
+            List[pd.DataFrame]
+                A list of dataframes, one per rank, containing kernel name,
+                op_stack (operator stack), top and bottom level op, and columns
+                for individual performance counters.
+        """
+        return CuptiCounterAnalysis.get_counter_data_with_operators(self.t, ranks)
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/trace_diff.py` & `HolisticTraceAnalysis-0.2.0/hta/trace_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,17 @@
         """Construct a LabeledTrace from either a Trace object or trace files in trace_dir."""
         self.label = label if label else f"t{random.randint(0,10)}"
         if t is not None:
             self.t = t
         elif trace_dir is not None and os.path.isdir(trace_dir):
             self.t = Trace(trace_dir=trace_dir)
         else:
-            raise ValueError("either a trace object or a valid trace dir must be provided in LabeledTrace.__init__()")
+            raise ValueError(
+                "either a trace object or a valid trace dir must be provided in LabeledTrace.__init__()"
+            )
         self.t.parse_traces()
 
         self.s_map = pd.Series(self.t.symbol_table.get_sym_id_map())
         self.s_tab = pd.Series(self.t.symbol_table.get_sym_table())
         self.iteration_df = self._extract_iterations()
 
     def ranks(self) -> List[int]:
@@ -62,15 +64,17 @@
         """Get all iterations"""
         return sorted(self.iteration_df["iteration"].values.tolist())
 
     def _extract_iterations(self) -> pd.DataFrame:
         """Extract the iterations from the symbol map"""
         s_map = pd.Series(self.t.symbol_table.get_sym_id_map())
         iteration_df = s_map[s_map.index.str.startswith("ProfilerStep")].reset_index()
-        iteration_df["iteration"] = iteration_df["index"].apply(lambda s: int(s.replace("ProfilerStep#", "")))
+        iteration_df["iteration"] = iteration_df["index"].apply(
+            lambda s: int(s.replace("ProfilerStep#", ""))
+        )
         iteration_df.rename(columns={0: "id", "index": "symbol"}, inplace=True)
         return iteration_df
 
     def extract_ops(
         self,
         rank: Optional[Union[int, List[int]]] = None,
         iteration: Optional[Union[int, List[int]]] = None,
@@ -170,15 +174,19 @@
 
                     cat 	        name 	            short_name 	    counts 	total_duration 	cat_id 	name_id
             0 	user_annotation 	nccl:all_reduce 	nccl:all_reduce 	1 	67 	            10 	    3
             1 	user_annotation 	ProfilerStep#1010 	ProfilerStep#1010 	1 	122149 	        10 	    17
             2 	cpu_op 	            aten::as_strided 	aten::as_strided 	1 	0 	            12 	    0
         """
         s_tab = self.s_tab
-        df = ops[["cat", "name", "dur"]].groupby(["cat", "name"]).aggregate(["count", "sum"])
+        df = (
+            ops[["cat", "name", "dur"]]
+            .groupby(["cat", "name"])
+            .aggregate(["count", "sum"])
+        )
         df.columns = ["_".join(col).rstrip("_") for col in df.columns.values]
         df.reset_index(inplace=True)
         df.rename(
             columns={
                 "name": "name_id",
                 "cat": "cat_id",
                 "dur_count": "counts",
@@ -200,15 +208,17 @@
                 "name_id",
             ]
         ]
 
         return df
 
 
-def _trace_argument_adapter(t: Union[LabeledTrace, Trace, TraceDir], default_label: str) -> LabeledTrace:
+def _trace_argument_adapter(
+    t: Union[LabeledTrace, Trace, TraceDir], default_label: str
+) -> LabeledTrace:
     """A helper function to construct a LabeledTrace from several argument types."""
     lt: LabeledTrace
     if isinstance(t, TraceDir):
         lt = LabeledTrace(label=default_label, trace_dir=t)
     elif isinstance(t, Trace):
         lt = LabeledTrace(label=default_label, t=t)
     elif isinstance(t, LabeledTrace):
@@ -288,44 +298,57 @@
         control_trace = _trace_argument_adapter(control, "Control")
         test_trace = _trace_argument_adapter(test, "Test")
 
         logger.info(f"comparing traces: {control_trace.label} and {test_trace.label}")
         if control_trace.label == test_trace.label:
             test_trace.label = f"{test_trace.label}_control"
             test_trace.label = f"{test_trace.label}_test"
-            logger.warn(f"The two traces have the same label. change test_trace's label to {test_trace.label}")
+            logger.warn(
+                f"The two traces have the same label. change test_trace's label to {test_trace.label}"
+            )
         control_label = control_trace.label
         test_label = test_trace.label
 
         # Determine which column use to group the operators
         col_name = "short_name" if use_short_name else "name"
         control_trace_summary = (
-            control_trace.get_ops_summary(control_trace.extract_ops(control_rank, control_iteration, device_type))
+            control_trace.get_ops_summary(
+                control_trace.extract_ops(control_rank, control_iteration, device_type)
+            )
             .groupby(col_name)[["counts", "total_duration"]]
             .sum()
         )
 
         test_trace_summary = (
-            test_trace.get_ops_summary(test_trace.extract_ops(test_rank, test_iteration, device_type))
+            test_trace.get_ops_summary(
+                test_trace.extract_ops(test_rank, test_iteration, device_type)
+            )
             .groupby(col_name)[["counts", "total_duration"]]
             .sum()
         )
 
         comp = pd.concat(
             [control_trace_summary, test_trace_summary],
             axis=1,
             join="outer",
             keys=[control_label, test_label],
         )
         comp.fillna(0, inplace=True)
         flatten_column_names(comp)
 
-        comp["diff_counts"] = comp[f"{test_label}_counts"] - comp[f"{control_label}_counts"]
-        comp["diff_duration"] = comp[f"{test_label}_total_duration"] - comp[f"{control_label}_total_duration"]
-        comp["counts_change_categories"] = comp["diff_counts"].apply(lambda c: "+" if c > 0 else "-" if c < 0 else "=")
+        comp["diff_counts"] = (
+            comp[f"{test_label}_counts"] - comp[f"{control_label}_counts"]
+        )
+        comp["diff_duration"] = (
+            comp[f"{test_label}_total_duration"]
+            - comp[f"{control_label}_total_duration"]
+        )
+        comp["counts_change_categories"] = comp["diff_counts"].apply(
+            lambda c: "+" if c > 0 else "-" if c < 0 else "="
+        )
 
         return comp
 
     @classmethod
     def ops_diff(
         cls,
         control: Union[LabeledTrace, TraceDir],
@@ -393,16 +416,20 @@
             device_type,
         )
         col_control = f"{control_trace.label}_counts"
         col_test = f"{test_trace.label}_counts"
         col_diff = "diff_counts"
         return {
             "added": df.loc[df[col_control].eq(0) & df[col_test].gt(0)].index.tolist(),
-            "deleted": df.loc[df[col_control].gt(0) & df[col_test].eq(0)].index.tolist(),
-            "increased": df.loc[df[col_control].gt(0) & df[col_diff].gt(0)].index.tolist(),
+            "deleted": df.loc[
+                df[col_control].gt(0) & df[col_test].eq(0)
+            ].index.tolist(),
+            "increased": df.loc[
+                df[col_control].gt(0) & df[col_diff].gt(0)
+            ].index.tolist(),
             "decreased": df.loc[df[col_test].gt(0) & df[col_diff].lt(0)].index.tolist(),
             "unchanged": df.loc[df[col_test].gt(0) & df[col_diff].eq(0)].index.tolist(),
         }
 
     @classmethod
     def visualize_counts_diff(
         cls,
@@ -418,15 +445,17 @@
             show_image (bool): set to True to display the image. Default = True.
             export_image_path (str): location where the image is saved.
 
         Returns:
             None
         """
         labels: List[str] = [
-            col.replace("_total_duration", "") for col in df.columns if col.endswith("_total_duration")
+            col.replace("_total_duration", "")
+            for col in df.columns
+            if col.endswith("_total_duration")
         ]
         assert len(labels) >= 2
 
         fig = go.Figure(
             data=[
                 go.Bar(name=labels[0], x=df.index, y=df[f"{labels[0]}_counts"]),
                 go.Bar(name=labels[1], x=df.index, y=df[f"{labels[1]}_counts"]),
@@ -454,15 +483,17 @@
             show_image (bool): set to True to display the image. Default = True.
             export_image_path (str): location where the image is saved.
 
         Returns:
             None
         """
         labels: List[str] = [
-            col.replace("_total_duration", "") for col in df.columns if col.endswith("_total_duration")
+            col.replace("_total_duration", "")
+            for col in df.columns
+            if col.endswith("_total_duration")
         ]
         assert len(labels) >= 2
 
         fig = go.Figure(
             data=[
                 go.Bar(
                     name=labels[0],
```

### Comparing `HolisticTraceAnalysis-0.1.3/hta/utils/utils.py` & `HolisticTraceAnalysis-0.2.0/hta/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,32 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-import sys
-from collections import deque
+import multiprocessing as mp
 from enum import Enum
 from pathlib import Path
-from typing import Any, List, Set
+from typing import List
 
 import pandas as pd
+import psutil
 
 
 class KernelType(Enum):
     COMMUNICATION = 0
     MEMORY = 1
     COMPUTATION = 2
 
 
 class IdleTimeType(Enum):
     HOST_WAIT = 0
     KERNEL_WAIT = 1
     OTHER = 2
 
 
-def get_memory_usage(o: Any) -> int:
-    """Get the memory usage of an object.
-
-    Args:
-        o (object): an object
-
-    Returns:
-        the memory usage by the object <o>.
-    """
-    seen: Set[int] = set()
-
-    def get_size(obj: Any) -> int:
-        """Get the size of an object recursively."""
-        if id(obj) in seen:
-            return 0
-        size = sys.getsizeof(obj)
-        seen.add(id(obj))
-
-        if isinstance(obj, (str, bytes, bytearray)):
-            pass
-        elif isinstance(obj, dict):
-            size += sum([get_size(v) for v in obj.keys()])
-            size += sum([get_size(v) for v in obj.values()])
-        elif isinstance(obj, (tuple, list, Set, deque)):
-            size += sum(get_size(i) for i in obj)
-        elif hasattr(obj, "__dict__"):
-            size += get_size(vars(obj))
-        return size
-
-    return get_size(o)
-
-
 def normalize_path(path: str) -> str:
     """
     Convert a Linux path to Python path.
 
     Args:
         path (str) : a path acceptable by the OS.
 
@@ -170,7 +138,25 @@
     return "".join(stack).split(" ")[-1]
 
 
 def flatten_column_names(df: pd.DataFrame) -> None:
     """Flatten a DataFrame's a multiple index column names to a single string"""
     if isinstance(df.columns, pd.MultiIndex):
         df.columns = ["_".join(col).rstrip("_") for col in df.columns]
+
+
+def get_mp_pool_size(obj_size: int, num_objs: int) -> int:
+    """
+    Estimate the maximum pool size for multiprocessing
+
+    Args:
+        obj_size (int): the size of objects to be processed
+        num_objs (int): the total number of objects to be processed
+
+    Returns:
+        int
+            the recommend pool size
+    """
+    free_mem = psutil.virtual_memory().available
+    # Leave 20% buffer for system and other processes
+    max_np = int(0.8 * free_mem / obj_size)
+    return min(max_np, num_objs, mp.cpu_count())
```

### Comparing `HolisticTraceAnalysis-0.1.3/setup.py` & `HolisticTraceAnalysis-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     url="https://github.com/facebookresearch/HolisticTraceAnalysis",
     python_requires=">=3.8",
     author="Meta Platforms Inc.",
     author_email="todo@meta.com",
     license="MIT",
     install_requires=fetch_requirements(),
     include_package_data=True,
-    packages=setuptools.find_packages(include=["hta*"]),  # Only include code within hta.
+    packages=setuptools.find_packages(
+        include=["hta*"]
+    ),  # Only include code within hta.
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_call_stack.py` & `HolisticTraceAnalysis-0.2.0/tests/test_call_stack.py`

 * *Files identical despite different names*

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_config.py` & `HolisticTraceAnalysis-0.2.0/tests/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,20 @@
             "c": {"c1": 2, "c2": {"c21": 10.0}},
         }
         with open(self.test_config_path, "w+") as fp:
             json.dump(self.test_config, fp)
 
     def test_get_default_paths(self):
         paths = HtaConfig.get_default_paths()
-        self.assertEqual(len(paths), 3, f"expect the default file paths to be 3 but got {len(paths)}")
-        self.assertTrue(all([str(path).endswith(DEFAULT_CONFIG_FILENAME) for path in paths]))
+        self.assertEqual(
+            len(paths), 3, f"expect the default file paths to be 3 but got {len(paths)}"
+        )
+        self.assertTrue(
+            all([str(path).endswith(DEFAULT_CONFIG_FILENAME) for path in paths])
+        )
 
     def test_constructor_no_config_file(self):
         config = HtaConfig(load_default_paths=False)
         self.assertDictEqual(config.get_config(), {})
 
     def test_constructor_one_config_file(self):
         config = HtaConfig(self.test_config_path, load_default_paths=False)
@@ -49,15 +53,17 @@
         self.assertListEqual(config.get_config("b"), self.test_config["b"])
         self.assertDictEqual(config.get_config("c"), self.test_config["c"])
 
     def test_get_config_multiple_levels(self):
         config = HtaConfig(self.test_config_path, load_default_paths=False)
         self.assertDictEqual(config.get_config("c"), self.test_config["c"])
         self.assertEqual(config.get_config("c.c1"), self.test_config["c"]["c1"])
-        self.assertEqual(config.get_config("c.c2.c21"), self.test_config["c"]["c2"]["c21"])
+        self.assertEqual(
+            config.get_config("c.c2.c21"), self.test_config["c"]["c2"]["c21"]
+        )
         self.assertIsNone(config.get_config("d"))
         self.assertIsNone(config.get_config("c.c2.c22"))
         self.assertIsNone(config.get_config("c.c1.c3"))
 
     def test_get_config_default_values(self):
         config = HtaConfig(self.test_config_path, load_default_paths=False)
         self.assertEqual(config.get_config("c", 10), self.test_config["c"])
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_correlation.py` & `HolisticTraceAnalysis-0.2.0/tests/test_correlation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# Copyright (c) Meta Platforms, Inc. and affiliates.
-# This source code is licensed under the MIT license found in the
-# LICENSE file in the root directory of this source tree.
-
-import unittest
-
-import pandas as pd
-
-from hta.common.trace import transform_correlation_to_index
-
-
-class CorrelationTestCase(unittest.TestCase):
-    def test_something(self):
-        data = [
-            [1, 15, -1],
-            [2, 16, -1],
-            [3, 22, -1],
-            [4, -1, -1],
-            [5, 15, 7],
-            [6, 16, 7],
-            [7, 30, 7],
-            [8, -1, 7],
-        ]
-        df = pd.DataFrame(
-            data,
-            columns=["index", "correlation", "stream"],
-            index=[1, 2, 3, 4, 5, 6, 7, 8],
-        )
-        expected_index_correlation = [5, 6, 0, -1, 1, 2, 0, -1]
-        df2 = transform_correlation_to_index(df)
-        self.assertListEqual(expected_index_correlation, df2["index_correlation"].tolist())
+# Copyright (c) Meta Platforms, Inc. and affiliates.
+# This source code is licensed under the MIT license found in the
+# LICENSE file in the root directory of this source tree.
+
+import unittest
+
+import pandas as pd
+
+from hta.common.trace import transform_correlation_to_index
+
+
+class CorrelationTestCase(unittest.TestCase):
+    def test_something(self):
+        data = [
+            [1, 15, -1],
+            [2, 16, -1],
+            [3, 22, -1],
+            [4, -1, -1],
+            [5, 15, 7],
+            [6, 16, 7],
+            [7, 30, 7],
+            [8, -1, 7],
+        ]
+        df = pd.DataFrame(
+            data,
+            columns=["index", "correlation", "stream"],
+            index=[1, 2, 3, 4, 5, 6, 7, 8],
+        )
+        expected_index_correlation = [5, 6, 0, -1, 1, 2, 0, -1]
+        df2 = transform_correlation_to_index(df)
+        self.assertListEqual(
+            expected_index_correlation, df2["index_correlation"].tolist()
+        )
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_symbol_table.py` & `HolisticTraceAnalysis-0.2.0/tests/test_symbol_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,13 +61,15 @@
         with mp.Pool(np) as pool:
             decoded_symbols = pool.map(decoder, indices)
         pool.join()
         pool.close()
         self.assertEqual(len(decoded_symbols), len(self.symbols))
 
         sym_id_map = st.get_sym_id_map()
-        is_consistent = [sym_id_map[sym] == idx for (sym, idx) in zip(decoded_symbols, indices)]
+        is_consistent = [
+            sym_id_map[sym] == idx for (sym, idx) in zip(decoded_symbols, indices)
+        ]
         self.assertTrue(all(is_consistent))
 
 
 if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_trace_analysis.py` & `HolisticTraceAnalysis-0.2.0/tests/test_trace_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import unittest
 from collections import namedtuple
 from pathlib import Path
 from typing import List
 from unittest.mock import patch
 
 import hta
+from hta.analyzers.cupti_counter_analysis import CUDA_SASS_INSTRUCTION_COUNTER_FLOPS
 from hta.common.trace import PHASE_COUNTER
 from hta.trace_analysis import TimeSeriesTypes, TraceAnalysis
 
 
 class TraceAnalysisTestCase(unittest.TestCase):
     vision_transformer_t: TraceAnalysis
     inference_t: TraceAnalysis
@@ -30,54 +31,64 @@
         cls.vision_transformer_t = TraceAnalysis(trace_dir=vision_transformer_trace_dir)
         cls.inference_t = TraceAnalysis(trace_dir=inference_trace_dir)
         cls.df_index_resolver_t = TraceAnalysis(trace_dir=df_index_resolver_trace_dir)
         cls.rank_non_gpu_t = TraceAnalysis(trace_dir=rank_non_gpu_trace_dir)
 
     def setUp(self):
         self.overlaid_trace_dir = "tests/data"
-        self.overlaid_trace_file = os.path.join(str(Path(self.overlaid_trace_dir)), "overlaid_rank-0.json.gz")
+        self.overlaid_trace_file = os.path.join(
+            str(Path(self.overlaid_trace_dir)), "overlaid_rank-0.json.gz"
+        )
 
     @patch.object(hta.common.trace.Trace, "write_raw_trace")
     def test_frequent_cuda_kernel_sequences(self, mock_write_trace):
-        frequent_patterns_dfs = self.vision_transformer_t.get_frequent_cuda_kernel_sequences(
-            operator_name="aten::linear",
-            output_dir=self.overlaid_trace_dir,
-            visualize=False,
-            compress_other_kernels=True,
+        frequent_patterns_dfs = (
+            self.vision_transformer_t.get_frequent_cuda_kernel_sequences(
+                operator_name="aten::linear",
+                output_dir=self.overlaid_trace_dir,
+                visualize=False,
+                compress_other_kernels=True,
+            )
         )
         self.assertIn(
             "|".join(
                 [
                     "aten::linear",
                     "Memset (Device)",
                     "volta_fp16_s884gemm_fp16_128x128_ldg8_f2f_stages_32x1_tn",
                     "void at::native::elementwise_kernel",
                 ]
             ),
             frequent_patterns_dfs.iloc[2]["pattern"],
         )
         self.assertEqual(frequent_patterns_dfs.iloc[2]["count"], 48)
-        self.assertEqual(frequent_patterns_dfs.iloc[2]["GPU kernel duration (ns)"], 11300)
-        self.assertEqual(frequent_patterns_dfs.iloc[2]["CPU op duration (ns)"], 9652)
+        self.assertEqual(
+            frequent_patterns_dfs.iloc[2]["GPU kernel duration (us)"], 11300
+        )
+        self.assertEqual(frequent_patterns_dfs.iloc[2]["CPU op duration (us)"], 9652)
         mock_write_trace.assert_called_once()
         trace_output_filename, _ = mock_write_trace.call_args.args
         self.assertEqual(trace_output_filename, self.overlaid_trace_file)
 
     def test_no_frequent_cuda_kernel_sequences_found(self):
-        frequent_patterns_dfs = self.df_index_resolver_t.get_frequent_cuda_kernel_sequences(
-            operator_name="aten::clone",
-            output_dir=self.overlaid_trace_dir,
-            rank=1,
-            visualize=False,
-            compress_other_kernels=True,
+        frequent_patterns_dfs = (
+            self.df_index_resolver_t.get_frequent_cuda_kernel_sequences(
+                operator_name="aten::clone",
+                output_dir=self.overlaid_trace_dir,
+                rank=1,
+                visualize=False,
+                compress_other_kernels=True,
+            )
         )
         self.assertTrue(frequent_patterns_dfs.empty)
 
     def test_get_cuda_kernel_launch_stats_training_multiple_ranks(self):
-        dataframe_dict = self.vision_transformer_t.get_cuda_kernel_launch_stats(ranks=[1, 7], visualize=False)
+        dataframe_dict = self.vision_transformer_t.get_cuda_kernel_launch_stats(
+            ranks=[1, 7], visualize=False
+        )
         rank_1_df, rank_7_df = dataframe_dict[1], dataframe_dict[7]
         row1 = rank_1_df[rank_1_df["correlation"] == 373234]
         row2 = rank_7_df[rank_7_df["correlation"] == 327327]
 
         self.assertEqual(row1["cpu_duration"].item(), 16)
         self.assertEqual(row1["gpu_duration"].item(), 2394)
         self.assertEqual(row1["launch_delay"].item(), 16491)
@@ -96,15 +107,17 @@
 
     def test_get_profiler_steps(self):
         results = self.vision_transformer_t.get_profiler_steps()
         expected = [15, 16, 17, 18]
         self.assertListEqual(results, expected)
 
     def test_get_potential_stragglers(self):
-        TCase = namedtuple("TCase", ["profiler_steps", "num_candidates", "expected_results"])
+        TCase = namedtuple(
+            "TCase", ["profiler_steps", "num_candidates", "expected_results"]
+        )
         p_steps = self.vision_transformer_t.get_profiler_steps()
         test_cases: List[TCase] = [
             TCase(p_steps[:1], -1, [7]),
             TCase(p_steps[:1], 2, [6, 7]),
             TCase(p_steps, 2, [0, 1]),
         ]
 
@@ -113,15 +126,17 @@
                 self.vision_transformer_t.get_potential_stragglers(
                     profiler_steps=tc.profiler_steps, num_candidates=tc.num_candidates
                 )
             )
             self.assertListEqual(got_stragglers, tc.expected_results)
 
     def test_comm_comp_overlap(self):
-        comm_comp_overlap = self.vision_transformer_t.get_comm_comp_overlap(visualize=False)
+        comm_comp_overlap = self.vision_transformer_t.get_comm_comp_overlap(
+            visualize=False
+        )
         self.assertAlmostEqual(
             comm_comp_overlap.iloc[0]["comp_comm_overlap_pctg"],
             round((240322 * 100) / 1091957, 3),
             delta=0.01,
         )
         self.assertAlmostEqual(
             comm_comp_overlap.iloc[1]["comp_comm_overlap_pctg"],
@@ -162,22 +177,24 @@
             delta=0.01,
         )
 
     def test_get_gpu_kernel_breakdown(self):
         (
             kernel_type_breakdown,
             kernel_breakdown,
-        ) = self.vision_transformer_t.get_gpu_kernel_breakdown(visualize=False, include_memory_kernels=True)
+        ) = self.vision_transformer_t.get_gpu_kernel_breakdown(
+            visualize=False, include_memory_kernels=True
+        )
 
         self.assertEqual(kernel_type_breakdown.iloc[0]["kernel_type"], "COMMUNICATION")
         self.assertEqual(kernel_type_breakdown.iloc[0]["sum"], 8040285)
         self.assertEqual(kernel_breakdown.iloc[0]["kernel_type"], "COMMUNICATION")
-        self.assertEqual(kernel_breakdown.iloc[0]["sum (ns)"], 627683)
+        self.assertEqual(kernel_breakdown.iloc[0]["sum (us)"], 627683)
         self.assertEqual(kernel_breakdown.iloc[151]["kernel_type"], "MEMORY")
-        self.assertEqual(kernel_breakdown.iloc[151]["sum (ns)"], 1064)
+        self.assertEqual(kernel_breakdown.iloc[151]["sum (us)"], 1064)
 
     def test_get_queue_length_summary(self):
         qd_summary = self.vision_transformer_t.get_queue_length_summary(ranks=[0])
         streams = qd_summary.index.to_list()
         self.assertEqual(streams, list(zip([0] * 6, [7, 20, 24, 26, 28, 30])))
 
         stream7_stats = qd_summary.loc[0, 7]["queue_length"].to_dict()
@@ -188,27 +205,31 @@
             "min": 0.0,
             "25%": 1.0,
             "50%": 9.0,
             "75%": 87.0,
             "max": 403.0,
         }
         for key, expval in expected_stats.items():
-            self.assertAlmostEqual(stream7_stats[key], expval, msg=f"Stream 7 stats mismatch key={key}")
+            self.assertAlmostEqual(
+                stream7_stats[key], expval, msg=f"Stream 7 stats mismatch key={key}"
+            )
 
     @patch.object(hta.common.trace.Trace, "write_raw_trace")
     def test_generate_trace_with_counters(self, mock_write_trace):
         self.vision_transformer_t.generate_trace_with_counters(
             time_series=TimeSeriesTypes.QUEUE_LENGTH | TimeSeriesTypes.MEMCPY_BANDWIDTH
         )
         mock_write_trace.assert_called_once()
         # change to kwargs if you use kwargs while calling write_raw_trace
         trace_filename, trace_json = mock_write_trace.call_args.args
         self.assertTrue("with_counters" in trace_filename)
 
-        counter_events = [ev for ev in trace_json["traceEvents"] if ev["ph"] == PHASE_COUNTER]
+        counter_events = [
+            ev for ev in trace_json["traceEvents"] if ev["ph"] == PHASE_COUNTER
+        ]
         print(f"Trace has {len(counter_events)} counter events")
         self.assertGreaterEqual(len(counter_events), 21000)
 
         counter_names = {ev["name"] for ev in counter_events}
         self.assertEqual(
             counter_names,
             {"Queue Length", "Memcpy DtoH", "Memcpy HtoD", "Memcpy DtoD", "Memset"},
@@ -216,37 +237,46 @@
 
         membw_ts = self.vision_transformer_t.get_memory_bw_time_series()[0]
         self.assertEqual(len(membw_ts[membw_ts.memory_bw_gbps < 0]), 0)
 
         queue_len_ts = self.vision_transformer_t.get_queue_length_time_series()[0]
         self.assertEqual(len(queue_len_ts[queue_len_ts.queue_length < 0]), 0)
 
-        mem_bw_summary_df = self.vision_transformer_t.get_memory_bw_summary(ranks=[0, 2])
+        mem_bw_summary_df = self.vision_transformer_t.get_memory_bw_summary(
+            ranks=[0, 2]
+        )
         # 2 ranks x 4 types of memcpy/memset
         self.assertEqual(len(mem_bw_summary_df), 8)
 
-        queue_len_summary_df = self.vision_transformer_t.get_queue_length_summary(ranks=[0, 2])
+        queue_len_summary_df = self.vision_transformer_t.get_queue_length_summary(
+            ranks=[0, 2]
+        )
         # 2 ranks x 6 streams
         self.assertEqual(len(queue_len_summary_df), 12)
 
         # Test traces without GPU kernels, these should return empty dicts or dataframes
         queue_len_ts_dict = self.rank_non_gpu_t.get_queue_length_time_series()
         self.assertEqual(len(queue_len_ts_dict), 0)
 
         queue_len_summary_df = self.rank_non_gpu_t.get_queue_length_summary(ranks=[0])
         self.assertIsNone(queue_len_summary_df)
 
         mem_bw_summary_df = self.rank_non_gpu_t.get_memory_bw_summary(ranks=[0])
         self.assertIsNone(mem_bw_summary_df)
 
     def test_get_idle_time_breakdown(self):
-        (idle_time_df, idle_interval_df,) = self.vision_transformer_t.get_idle_time_breakdown(
+        (
+            idle_time_df,
+            idle_interval_df,
+        ) = self.vision_transformer_t.get_idle_time_breakdown(
             ranks=[0, 1], visualize=False, show_idle_interval_stats=True
         )
-        ranks = idle_time_df["rank"].unique()  # cannot use dataframe.rank as rank() is a utility too
+        ranks = idle_time_df[
+            "rank"
+        ].unique()  # cannot use dataframe.rank as rank() is a utility too
         streams = idle_time_df.stream.unique()
         idle_categories = idle_time_df.idle_category.unique()
 
         self.assertEqual(set(ranks), {0, 1})
         self.assertEqual(set(streams), {7, 20, 24, 26, 28, 30})
         self.assertEqual(set(idle_categories), {"host_wait", "kernel_wait", "other"})
 
@@ -264,10 +294,38 @@
         for key, expval in expected_stats.items():
             self.assertAlmostEqual(
                 stream7_stats[key],
                 expval,
                 msg=f"Stream 7 idle stats mismatch key={key}",
             )
 
+    def test_get_cupti_counter_data_with_operators(self):
+        # regular trace should return empty list since it will not have cuda_profiler_range events
+        self.assertEqual(self.inference_t.get_cupti_counter_data_with_operators(), [])
+
+        cupti_profiler_trace_dir: str = "tests/data/cupti_profiler/"
+        cupti_profiler_t = TraceAnalysis(trace_dir=cupti_profiler_trace_dir)
+        counters_df = cupti_profiler_t.get_cupti_counter_data_with_operators()[0]
+
+        self.assertEqual(len(counters_df), 77)
+
+        # Example trace has CUPTI SASS FLOPS instruction counters
+        counter_names = set(CUDA_SASS_INSTRUCTION_COUNTER_FLOPS.keys())
+        self.assertEqual(
+            set(counters_df.columns.unique()) & counter_names, counter_names
+        )
+
+        # Pick 5th kernel that executed.
+        test_row = counters_df.sort_values(axis=0, by="ts").iloc[5].to_dict()
+
+        self.assertEqual(test_row["cat"], "cuda_profiler_range")
+        self.assertTrue("fft2d_r2c_32x32" in test_row["name"])
+
+        self.assertEqual(
+            test_row["smsp__sass_thread_inst_executed_op_fadd_pred_on.sum"], 86114304
+        )
+        self.assertEqual(test_row["top_level_op"], "aten::conv2d")
+        self.assertEqual(test_row["bottom_level_op"], "aten::_convolution")
+
 
 if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_trace_diff.py` & `HolisticTraceAnalysis-0.2.0/tests/test_trace_diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,57 +63,69 @@
                     "cudaEventQuery",
                     "cudaLaunchKernel",
                 ],
             },
         }
 
     def test_labeled_trace(self) -> None:
-        base_t = LabeledTrace(label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"])
+        base_t = LabeledTrace(
+            label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"]
+        )
         self.assertListEqual(base_t.ranks(), self.base_trace["ranks"])
         self.assertListEqual(base_t.iterations(), self.base_trace["iterations"])
 
     def test_labeled_trace_random_label(self) -> None:
         base_t = LabeledTrace(trace_dir=self.base_trace["trace_dir"])
         self.assertTrue(base_t.label.startswith("t"))
 
     def test_extract_ops(self) -> None:
-        base_t = LabeledTrace(label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"])
+        base_t = LabeledTrace(
+            label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"]
+        )
         cpu_events: pd.DataFrame = base_t.extract_ops(
             self.base_trace["test_rank"],
             self.base_trace["test_iteration"],
             DeviceType.CPU,
         )
         self.assertEqual(cpu_events.shape[0], self.base_trace["test_num_cpu_events"])
         gpu_events: pd.DataFrame = base_t.extract_ops(
             self.base_trace["test_rank"],
             self.base_trace["test_iteration"],
             DeviceType.GPU,
         )
         self.assertEqual(gpu_events.shape[0], self.base_trace["test_num_gpu_events"])
 
     def test_get_ops_summary(self) -> None:
-        base_t = LabeledTrace(label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"])
+        base_t = LabeledTrace(
+            label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"]
+        )
         df: pd.DataFrame = base_t.get_ops_summary(
             base_t.extract_ops(
                 self.base_trace["test_rank"],
                 self.base_trace["test_iteration"],
                 DeviceType.CPU,
             )
         )
         self.assertDictEqual(
-            df.sort_values(by="name")[["name", "counts", "total_duration"]].set_index("name").to_dict(),
+            df.sort_values(by="name")[["name", "counts", "total_duration"]]
+            .set_index("name")
+            .to_dict(),
             self.base_trace["test_user_annotation_summary"],
         )
 
     def test_compare_trace(self) -> None:
-        base_t = LabeledTrace(label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"])
+        base_t = LabeledTrace(
+            label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"]
+        )
         base_rank = self.base_trace["test_rank"]
         base_iteration = self.base_trace["test_iteration"]
 
-        test_t = LabeledTrace(label=self.test_trace["label"], trace_dir=self.test_trace["trace_dir"])
+        test_t = LabeledTrace(
+            label=self.test_trace["label"], trace_dir=self.test_trace["trace_dir"]
+        )
         test_rank = self.test_trace["test_rank"]
         test_iteration = self.test_trace["test_iteration"]
 
         cpu_df = TraceDiff.compare_traces(
             base_t,
             test_t,
             base_rank,
@@ -140,19 +152,23 @@
         )
         self.assertDictEqual(
             gpu_df["counts_change_categories"].value_counts().to_dict(),
             self.test_trace["counts_change_categories"]["gpu"],
         )
 
     def test_ops_diff(self) -> None:
-        base_t = LabeledTrace(label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"])
+        base_t = LabeledTrace(
+            label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"]
+        )
         base_rank = self.base_trace["test_rank"]
         base_iteration = self.base_trace["test_iteration"]
 
-        test_t = LabeledTrace(label=self.test_trace["label"], trace_dir=self.test_trace["trace_dir"])
+        test_t = LabeledTrace(
+            label=self.test_trace["label"], trace_dir=self.test_trace["trace_dir"]
+        )
         test_rank = self.test_trace["test_rank"]
         test_iteration = self.test_trace["test_iteration"]
 
         diff = TraceDiff.ops_diff(
             base_t,
             test_t,
             base_rank,
@@ -160,19 +176,23 @@
             base_iteration,
             test_iteration,
             device_type=DeviceType.CPU,
         )
         self.assertDictEqual(diff, self.test_trace["ops_diff"])
 
     def test_visualize(self) -> None:
-        base_t = LabeledTrace(label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"])
+        base_t = LabeledTrace(
+            label=self.base_trace["label"], trace_dir=self.base_trace["trace_dir"]
+        )
         base_rank = self.base_trace["test_rank"]
         base_iteration = self.base_trace["test_iteration"]
 
-        test_t = LabeledTrace(label=self.test_trace["label"], trace_dir=self.test_trace["trace_dir"])
+        test_t = LabeledTrace(
+            label=self.test_trace["label"], trace_dir=self.test_trace["trace_dir"]
+        )
         test_rank = self.test_trace["test_rank"]
         test_iteration = self.test_trace["test_iteration"]
 
         cpu_df = TraceDiff.compare_traces(
             base_t,
             test_t,
             base_rank,
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_trace_parse.py` & `HolisticTraceAnalysis-0.2.0/tests/test_trace_parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 import unittest
 
 import pandas as pd
 
-from hta.common.trace import Trace, parse_trace_dict
+from hta.common.trace import parse_trace_dict, Trace
 
 
 class TraceParseTestCase(unittest.TestCase):
     vision_transformer_t: Trace
     vision_transformer_raw_df: pd.DataFrame
     inference_t: Trace
     inference_raw_df: pd.DataFrame
@@ -23,26 +23,32 @@
         inference_trace_dir: str = "tests/data/inference_single_rank"
         vision_transformer_rank_0_file: str = "rank-0.json.gz"
         inference_rank_0_file: str = "inference_rank_0.json.gz"
         max_ranks = 8
 
         # Trace parser for vision transformer
         cls.vision_transformer_t: Trace = Trace(trace_dir=vision_transformer_trace_dir)
-        cls.vision_transformer_t.parse_traces(max_ranks=max_ranks, use_multiprocessing=True)
+        cls.vision_transformer_t.parse_traces(
+            max_ranks=max_ranks, use_multiprocessing=True
+        )
         cls.vision_transformer_raw_df = cls.prepare_ground_truth_df(
             vision_transformer_trace_dir, vision_transformer_rank_0_file
         )
         # Trace parser for inference
         cls.inference_t: Trace = Trace(trace_dir=inference_trace_dir)
         cls.inference_t.parse_traces(max_ranks=max_ranks, use_multiprocessing=True)
-        cls.inference_raw_df = cls.prepare_ground_truth_df(inference_trace_dir, inference_rank_0_file)
+        cls.inference_raw_df = cls.prepare_ground_truth_df(
+            inference_trace_dir, inference_rank_0_file
+        )
 
     @classmethod
     def prepare_ground_truth_df(cls, trace_dir, rank_0_file) -> pd.DataFrame:
-        df = pd.DataFrame(parse_trace_dict(os.path.join(trace_dir, rank_0_file))["traceEvents"])
+        df = pd.DataFrame(
+            parse_trace_dict(os.path.join(trace_dir, rank_0_file))["traceEvents"]
+        )
         df.dropna(axis=0, subset=["dur", "cat"], inplace=True)
         df.drop(df[df["cat"] == "Trace"].index, inplace=True)
         return df
 
     def setUp(self) -> None:
         self.traces = [self.vision_transformer_t, self.inference_t]
         self.raw_dfs = [self.vision_transformer_raw_df, self.inference_raw_df]
@@ -58,15 +64,17 @@
             sym_table = t.symbol_table.get_sym_table()
             rank_0_df_name_id = t.traces[0]["name"]
             rank_0_df_name = t.traces[0]["name"].apply(lambda x: sym_table[x])
 
             ground_truth_name = raw_df["name"]
             ground_truth_name_id = raw_df["name"].apply(lambda x: sym_id_map[x])
 
-            self.assertListEqual(rank_0_df_name_id.to_list(), ground_truth_name_id.to_list())
+            self.assertListEqual(
+                rank_0_df_name_id.to_list(), ground_truth_name_id.to_list()
+            )
             self.assertListEqual(rank_0_df_name.to_list(), ground_truth_name.to_list())
 
             # test aligned and filtered trace
             t.align_and_filter_trace()
 
             raw_profiler_steps = raw_df["name"].str.contains("ProfilerStep").sum()
             sym_id_map = t.symbol_table.get_sym_id_map()
@@ -81,21 +89,33 @@
             self.assertGreaterEqual(t.traces[0]["ts"].min(), 0)
 
     def test_trace_iteration(self) -> None:
         # run tests for each collection of traces
         for t in self.traces:
             df = t.traces[0]
             sym_id_map = t.symbol_table.get_sym_id_map()
-            iterations = {f"ProfilerStep#{i}" for i in set(df["iteration"].unique()) if i != -1}
-
-            valid_gpu_kernels = df.loc[df["stream"].gt(0) & df["index_correlation"].gt(0)]
-            correlated_cpu_ops = df.loc[df.loc[valid_gpu_kernels.index, "index_correlation"]]
-            gpu_kernels_per_iteration = valid_gpu_kernels.groupby("iteration")["index"].agg("count").to_dict()
-            correlated_cpu_ops_per_iteration = correlated_cpu_ops.groupby("iteration")["index"].agg("count").to_dict()
+            iterations = {
+                f"ProfilerStep#{i}" for i in set(df["iteration"].unique()) if i != -1
+            }
+
+            valid_gpu_kernels = df.loc[
+                df["stream"].gt(0) & df["index_correlation"].gt(0)
+            ]
+            correlated_cpu_ops = df.loc[
+                df.loc[valid_gpu_kernels.index, "index_correlation"]
+            ]
+            gpu_kernels_per_iteration = (
+                valid_gpu_kernels.groupby("iteration")["index"].agg("count").to_dict()
+            )
+            correlated_cpu_ops_per_iteration = (
+                correlated_cpu_ops.groupby("iteration")["index"].agg("count").to_dict()
+            )
 
             self.assertTrue("iteration" in df.columns)
             self.assertTrue(all(i in sym_id_map for i in iterations))
-            self.assertDictEqual(gpu_kernels_per_iteration, correlated_cpu_ops_per_iteration)
+            self.assertDictEqual(
+                gpu_kernels_per_iteration, correlated_cpu_ops_per_iteration
+            )
 
 
 if __name__ == "__main__":  # pragma: no cover
     unittest.main()
```

### Comparing `HolisticTraceAnalysis-0.1.3/tests/test_trace_utils.py` & `HolisticTraceAnalysis-0.2.0/tests/test_trace_utils.py`

 * *Files identical despite different names*

