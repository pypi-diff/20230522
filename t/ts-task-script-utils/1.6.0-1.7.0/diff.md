# Comparing `tmp/ts_task_script_utils-1.6.0.tar.gz` & `tmp/ts_task_script_utils-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts_task_script_utils-1.6.0.tar", max compression
+gzip compressed data, was "ts_task_script_utils-1.7.0.tar", max compression
```

## Comparing `ts_task_script_utils-1.6.0.tar` & `ts_task_script_utils-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-04-13 20:01:25.929169 ts_task_script_utils-1.6.0/LICENSE
--rw-r--r--   0        0        0     5183 2023-04-13 20:01:25.929169 ts_task_script_utils-1.6.0/README.md
--rw-r--r--   0        0        0     1238 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/check_file_type.py
--rw-r--r--   0        0        0     2454 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/convert_datetime_to_ts_format.py
--rw-r--r--   0        0        0     3596 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datacubes/README.md
--rw-r--r--   0        0        0     5309 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datacubes/parquet.py
--rw-r--r--   0        0        0    24970 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/README.md
--rw-r--r--   0        0        0       96 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/__init__.py
--rw-r--r--   0        0        0     2680 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_config.py
--rw-r--r--   0        0        0    30200 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_info.py
--rw-r--r--   0        0        0    88298 2023-04-13 20:01:25.933169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/parse.png
--rw-r--r--   0        0        0    70421 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png
--rw-r--r--   0        0        0     1827 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py
--rw-r--r--   0        0        0   104888 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parse-white.png
--rw-r--r--   0        0        0     2248 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser.py
--rw-r--r--   0        0        0      841 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser_exceptions.py
--rw-r--r--   0        0        0     3999 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/ts_datetime.py
--rw-r--r--   0        0        0      178 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/tz_dicts.py
--rw-r--r--   0        0        0     2357 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/tz_list.py
--rw-r--r--   0        0        0     3710 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/manipulation.py
--rw-r--r--   0        0        0     4558 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/parsing.py
--rw-r--r--   0        0        0     7486 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/extract_to_decorate.py
--rw-r--r--   0        0        0      424 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/is_number.py
--rw-r--r--   0        0        0     4227 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/parse.py
--rw-r--r--   0        0        0     2795 2023-04-13 20:01:25.937169 ts_task_script_utils-1.6.0/task_script_utils/random.py
--rw-r--r--   0        0        0     6159 1970-01-01 00:00:00.000000 ts_task_script_utils-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-22 17:11:52.874755 ts_task_script_utils-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6752 2023-05-22 17:11:52.874755 ts_task_script_utils-1.7.0/README.md
+-rw-r--r--   0        0        0     1238 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/__init__.py
+-rw-r--r--   0        0        0     1123 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/check_file_type.py
+-rw-r--r--   0        0        0     2454 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/convert_datetime_to_ts_format.py
+-rw-r--r--   0        0        0     3596 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datacubes/README.md
+-rw-r--r--   0        0        0     5309 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datacubes/parquet.py
+-rw-r--r--   0        0        0    24970 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/README.md
+-rw-r--r--   0        0        0       96 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_config.py
+-rw-r--r--   0        0        0    30200 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_info.py
+-rw-r--r--   0        0        0    88298 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/parse.png
+-rw-r--r--   0        0        0    70421 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png
+-rw-r--r--   0        0        0     1827 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py
+-rw-r--r--   0        0        0   104888 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parse-white.png
+-rw-r--r--   0        0        0     2248 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser.py
+-rw-r--r--   0        0        0      841 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser_exceptions.py
+-rw-r--r--   0        0        0     3999 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/ts_datetime.py
+-rw-r--r--   0        0        0      178 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/tz_dicts.py
+-rw-r--r--   0        0        0     2357 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/tz_list.py
+-rw-r--r--   0        0        0     3710 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/manipulation.py
+-rw-r--r--   0        0        0     4558 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/parsing.py
+-rw-r--r--   0        0        0     7486 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/extract_to_decorate.py
+-rw-r--r--   0        0        0      424 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/is_number.py
+-rw-r--r--   0        0        0     4227 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/parse.py
+-rw-r--r--   0        0        0     2795 2023-05-22 17:11:52.878755 ts_task_script_utils-1.7.0/task_script_utils/random.py
+-rw-r--r--   0        0        0     3153 2023-05-22 17:11:52.882755 ts_task_script_utils-1.7.0/task_script_utils/workflow_logging.py
+-rw-r--r--   0        0        0     7680 1970-01-01 00:00:00.000000 ts_task_script_utils-1.7.0/PKG-INFO
```

### Comparing `ts_task_script_utils-1.6.0/LICENSE` & `ts_task_script_utils-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/README.md` & `ts_task_script_utils-1.7.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # ts-task-script-utils <!-- omit in toc -->
 
 [![Build Status](https://travis-ci.com/tetrascience/ts-task-script-utils.svg?branch=master)](https://travis-ci.com/tetrascience/ts-task-script-utils)
 
 ## Version <!-- omit in toc -->
 
-v1.6.0
+v1.7.0
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Summary](#summary)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Parsing Numbers](#parsing-numbers)
   - [Parsing Datetimes](#parsing-datetimes)
     - [`parse` Usage](#parse-usage)
   - [Generating Random UUIDs for Task Scripts](#generating-random-uuids-for-task-scripts)
   - [Creating datacube Parquet files](#creating-datacube-parquet-files)
+  - [Logging warning messages in Task Scripts](#logging-warning-messages-in-task-scripts)
 - [Changelog](#changelog)
+  - [v1.7.0](#v170)
   - [v1.6.0](#v160)
   - [v1.5.0](#v150)
   - [v1.4.0](#v140)
   - [v1.3.1](#v131)
   - [v1.3.0](#v130)
   - [v1.2.0](#v120)
   - [v1.1.1](#v111)
@@ -109,27 +111,29 @@
 input_file = Path(...)
 file_content = input_file.read_bytes()
 rand = TaskScriptUUIDGenerator.from_task_script_identifier_parts("common", "my-task-script", "v1.0.0", file_content)
 ```
 
 This is a singleton class, meaning creating multiple instances of the class with the same arguments results in getting
 the identical object back, e.g.:
+
 ```python
 from pathlib import Path
 from task_script_utils.random import TaskScriptUUIDGenerator
 
 input_file = Path(...)
 file_content = input_file.read_bytes()
 rand1 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
 rand2 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
 
 assert rand1 is rand2
 ```
 
 It's also possible to get the most-recently-created instance through the `get_last_created` method:
+
 ```python
 from pathlib import Path
 from task_script_utils.random import TaskScriptUUIDGenerator
 
 input_file = Path(...)
 file_content = input_file.read_bytes()
 rand1 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
@@ -139,16 +143,55 @@
 assert rand1 is rand2
 ```
 
 ### Creating datacube Parquet files
 
 [See the docs](task_script_utils/datacubes/README.md).
 
+### Using Python's `logging` module in Task Scripts
+
+Task Scripts can write workflow logs which are visible to users on TDP, but only if the logs are written via the logger provided by the `context` object. The `context` logger is documented here: [context.get_logger](https://developers.tetrascience.com/docs/context-api#contextget_logger).
+
+This utility is a wrapper for the `context` logger which allows Task Scripts to use Python's `logging` module for creating TDP workflow logs, instead of directly using the `context` logger object. This means the `context` logger object doesn't need to be passed around to each function which needs to do logging, and Task Script code can benefit from other features of the Python `logging` module such as [integration with `pytest`](https://docs.pytest.org/en/7.1.x/how-to/logging.html).
+
+To log warning messages on the platform from a task script do the following:
+
+- Setup the log handler in `main.py`:
+
+```python
+from task_script_utils.logging import (
+    setup_ts_log_handler,
+)
+```
+
+- Then within the function called by the protocol:
+
+```python
+setup_ts_log_handler(context.get_logger(), "main")
+```
+
+- In a module where you wish to log a warning:
+
+```python
+import logging
+logger = logging.getLogger("main." + __name__)
+```
+
+- Log a warning message with:
+
+```python
+logger.warning("This is a warning message")
+```
+
 ## Changelog
 
+### v1.7.0
+
+- Add `task_script_utils.logging` for logging warning messages in task scripts
+
 ### v1.6.0
 
 - Add `task_script_utils.datacubes.parquet` for creating Parquet file representations of datacubes
 
 ### v1.5.0
 
 - Add `TaskScriptUUIDGenerator` class for generating random UUIDs and random bytes.
```

### Comparing `ts_task_script_utils-1.6.0/pyproject.toml` & `ts_task_script_utils-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 line-length = 88
 target-version = ['py37', 'py38', 'py39']
 include = '\.pyi?$'
 extend-exclude = 'snapshots'
 
 [tool.poetry]
 name = "ts-task-script-utils"
-version = "1.6.0"
+version = "1.7.0"
 description = "Python utility for Tetra Task Scripts"
 authors = ["Tetrascience <developers@tetrascience.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 include = ["LICENSE"]
 classifiers =[
   "Programming Language :: Python :: 3",
```

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/check_file_type.py` & `ts_task_script_utils-1.7.0/task_script_utils/check_file_type.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/convert_datetime_to_ts_format.py` & `ts_task_script_utils-1.7.0/task_script_utils/convert_datetime_to_ts_format.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datacubes/README.md` & `ts_task_script_utils-1.7.0/task_script_utils/datacubes/README.md`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datacubes/parquet.py` & `ts_task_script_utils-1.7.0/task_script_utils/datacubes/parquet.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/README.md` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/README.md`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_config.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_config.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/datetime_info.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/datetime_info.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/parse.png` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/parse.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/flowcharts/short-date-format-resolution.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/fractional_seconds_formatter.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parse-white.png` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parse-white.png`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/parser_exceptions.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/parser_exceptions.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/ts_datetime.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/ts_datetime.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/tz_list.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/tz_list.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/manipulation.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/manipulation.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/datetime_parser/utils/parsing.py` & `ts_task_script_utils-1.7.0/task_script_utils/datetime_parser/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/extract_to_decorate.py` & `ts_task_script_utils-1.7.0/task_script_utils/extract_to_decorate.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/parse.py` & `ts_task_script_utils-1.7.0/task_script_utils/parse.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/task_script_utils/random.py` & `ts_task_script_utils-1.7.0/task_script_utils/random.py`

 * *Files identical despite different names*

### Comparing `ts_task_script_utils-1.6.0/PKG-INFO` & `ts_task_script_utils-1.7.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: ts-task-script-utils
-Version: 1.6.0
+Version: 1.7.0
 Summary: Python utility for Tetra Task Scripts
 License: Apache-2.0
 Author: Tetrascience
 Author-email: developers@tetrascience.com
 Requires-Python: >=3.7.2,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: arrow (>=1.2.2,<2.0.0)
 Requires-Dist: dateparser (>=1.1.1,<2.0.0)
 Requires-Dist: fastparquet (>=0.8.1)
 Requires-Dist: fsspec (<=2023.1.0)
 Requires-Dist: numpy (>=1.17.0,<2.0.0)
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
@@ -26,27 +25,29 @@
 
 # ts-task-script-utils <!-- omit in toc -->
 
 [![Build Status](https://travis-ci.com/tetrascience/ts-task-script-utils.svg?branch=master)](https://travis-ci.com/tetrascience/ts-task-script-utils)
 
 ## Version <!-- omit in toc -->
 
-v1.6.0
+v1.7.0
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Summary](#summary)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Parsing Numbers](#parsing-numbers)
   - [Parsing Datetimes](#parsing-datetimes)
     - [`parse` Usage](#parse-usage)
   - [Generating Random UUIDs for Task Scripts](#generating-random-uuids-for-task-scripts)
   - [Creating datacube Parquet files](#creating-datacube-parquet-files)
+  - [Logging warning messages in Task Scripts](#logging-warning-messages-in-task-scripts)
 - [Changelog](#changelog)
+  - [v1.7.0](#v170)
   - [v1.6.0](#v160)
   - [v1.5.0](#v150)
   - [v1.4.0](#v140)
   - [v1.3.1](#v131)
   - [v1.3.0](#v130)
   - [v1.2.0](#v120)
   - [v1.1.1](#v111)
@@ -135,27 +136,29 @@
 input_file = Path(...)
 file_content = input_file.read_bytes()
 rand = TaskScriptUUIDGenerator.from_task_script_identifier_parts("common", "my-task-script", "v1.0.0", file_content)
 ```
 
 This is a singleton class, meaning creating multiple instances of the class with the same arguments results in getting
 the identical object back, e.g.:
+
 ```python
 from pathlib import Path
 from task_script_utils.random import TaskScriptUUIDGenerator
 
 input_file = Path(...)
 file_content = input_file.read_bytes()
 rand1 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
 rand2 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
 
 assert rand1 is rand2
 ```
 
 It's also possible to get the most-recently-created instance through the `get_last_created` method:
+
 ```python
 from pathlib import Path
 from task_script_utils.random import TaskScriptUUIDGenerator
 
 input_file = Path(...)
 file_content = input_file.read_bytes()
 rand1 = TaskScriptUUIDGenerator("common/my-task-script:v1.0.0", file_content)
@@ -165,16 +168,55 @@
 assert rand1 is rand2
 ```
 
 ### Creating datacube Parquet files
 
 [See the docs](task_script_utils/datacubes/README.md).
 
+### Using Python's `logging` module in Task Scripts
+
+Task Scripts can write workflow logs which are visible to users on TDP, but only if the logs are written via the logger provided by the `context` object. The `context` logger is documented here: [context.get_logger](https://developers.tetrascience.com/docs/context-api#contextget_logger).
+
+This utility is a wrapper for the `context` logger which allows Task Scripts to use Python's `logging` module for creating TDP workflow logs, instead of directly using the `context` logger object. This means the `context` logger object doesn't need to be passed around to each function which needs to do logging, and Task Script code can benefit from other features of the Python `logging` module such as [integration with `pytest`](https://docs.pytest.org/en/7.1.x/how-to/logging.html).
+
+To log warning messages on the platform from a task script do the following:
+
+- Setup the log handler in `main.py`:
+
+```python
+from task_script_utils.logging import (
+    setup_ts_log_handler,
+)
+```
+
+- Then within the function called by the protocol:
+
+```python
+setup_ts_log_handler(context.get_logger(), "main")
+```
+
+- In a module where you wish to log a warning:
+
+```python
+import logging
+logger = logging.getLogger("main." + __name__)
+```
+
+- Log a warning message with:
+
+```python
+logger.warning("This is a warning message")
+```
+
 ## Changelog
 
+### v1.7.0
+
+- Add `task_script_utils.logging` for logging warning messages in task scripts
+
 ### v1.6.0
 
 - Add `task_script_utils.datacubes.parquet` for creating Parquet file representations of datacubes
 
 ### v1.5.0
 
 - Add `TaskScriptUUIDGenerator` class for generating random UUIDs and random bytes.
```

