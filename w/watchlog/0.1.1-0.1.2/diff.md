# Comparing `tmp/watchlog-0.1.1.tar.gz` & `tmp/watchlog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchlog-0.1.1.tar", max compression
+gzip compressed data, was "watchlog-0.1.2.tar", max compression
```

## Comparing `watchlog-0.1.1.tar` & `watchlog-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1086 2023-04-11 06:24:22.861180 watchlog-0.1.1/LICENSE
--rwxr-xr-x   0        0        0     2328 2023-04-11 05:51:59.149720 watchlog-0.1.1/README.md
--rwxr-xr-x   0        0        0      638 2023-04-11 06:27:29.054519 watchlog-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-04-11 05:12:32.140833 watchlog-0.1.1/watchlog/__init__.py
--rwxr-xr-x   0        0        0     5140 2023-04-11 06:26:49.304008 watchlog-0.1.1/watchlog/watchlog.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 watchlog-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1086 2023-04-11 06:24:22.861180 watchlog-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     2587 2023-05-19 10:05:40.246187 watchlog-0.1.2/README.md
+-rwxr-xr-x   0        0        0      659 2023-05-22 02:00:27.435329 watchlog-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-04-11 05:12:32.140833 watchlog-0.1.2/watchlog/__init__.py
+-rwxr-xr-x   0        0        0     8430 2023-05-22 01:59:38.588286 watchlog-0.1.2/watchlog/watchlog.py
+-rw-r--r--   0        0        0     3508 1970-01-01 00:00:00.000000 watchlog-0.1.2/PKG-INFO
```

### Comparing `watchlog-0.1.1/LICENSE` & `watchlog-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watchlog-0.1.1/README.md` & `watchlog-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-
 # watchlog
 
-`watchlog` is a Python package for monitoring log files and sending parsed logs to a specified URL using HTTP POST requests.
+`watchlog` is a Python package for monitoring log files and sending parsed logs to a specified URL using HTTP POST
+requests.
 
 - name = "watchlog"
 - description = "monitoring log files and sending parsed logs to a specified URL"
 - authors = ["Euraxluo <euraxluo@outlook.com>"]
 - license = "The MIT LICENSE"
 - repository = "https://github.com/Euraxluo/watchlog"
 - version = "0.1.*"
 
-
-
 ## Installation
 
 You can install `watchlog` using pip:
 
 ```bash
 pip install watchlog
 ```
 
 ## Usage
 
 To use `watchlog`, you need to create a configuration file in JSON format. Here is an example configuration file:
 
 ```json
 {
+  "check_interval": 5,
+  "check": true,
   "files": [
     {
       "path": "/path/to/log/file.log",
       "reg": "^(?P<time>[^ ]*) (?P<level>[^ ]*) (?P<module>[^ ]*) (?P<line>[^ ]*) (?P<message>.*)$",
       "url": "http://example.com/api/logs",
       "latest": true,
+      "enable": true,
       "headers": {
         "Content-Type": "application/json"
       },
       "auth": {
         "username": "user",
         "password": "pass"
       }
@@ -44,42 +45,49 @@
 }
 ```
 
 - `path`: The path of the log file to monitor.
 - `reg`: A regular expression used to parse the log file.
 - `url`: The URL to send the parsed logs to.
 - `latest`: Start monitoring from the latest logs.
+- `enable`: Indicates that this configuration will be enabled, which defaults to true.
 - `headers`: A dictionary of headers to include in the HTTP POST request.
 - `auth`: A dictionary with `username` and `password` keys for basic authentication.
+- `check`: if open check ,it will loop check the config file
+- `check_interval`: circle check interval time(s)
 
-Once you have created the configuration file, you can start monitoring the log file by calling the `start()` function from the `watchlog` module:
+Once you have created the configuration file, you can start monitoring the log file by calling the `start()` function
+from the `watchlog` module:
 
 ```python
 import asyncio
 from watchlog import start
+
 loop = asyncio.get_event_loop()
 loop.run_until_complete(start('path/to/config.json'))
 ```
 
 You can also use we provide small scripts
+
 ```bash
 watchlog path/to/config/file
 ```
 
-This will start monitoring the log file specified in the configuration file and sending parsed logs to the specified URL using HTTP POST requests.
+This will start monitoring the log file specified in the configuration file and sending parsed logs to the specified URL
+using HTTP POST requests.
 
 ## example
+
 example use zinc_observe as log search_engine,Illustrates the use of the process
 
 ```
 .                     
 ├── __init__.py       
 ├── config.json             config file
 ├── docker-compose.yml      log search engine service
 ├── log.log                 log file
 └── main.py                 main python file to monitor log file
 ```
 
-
 ## License
 
 `watchlog` is licensed under the MIT license.
```

### Comparing `watchlog-0.1.1/pyproject.toml` & `watchlog-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "watchlog"
-version = "0.1.1"
+version = "0.1.2"
 description = "monitoring log files and sending parsed logs to a specified URL"
 authors = ["euraxluo <euraxluo@outlook.com>"]
 license = "The MIT LICENSE"
 readme = "README.md"
 homepage = "https://github.com/Euraxluo/watchlog"
 repository = "https://github.com/Euraxluo/watchlog"
 keywords = ["log monitor","loguru","watchdog"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 loguru = "^0.7.0"
 watchdog = "^3.0.0"
 asyncio = "^3.4.3"
 httpx = "^0.23.3"
+requests = "^2.30.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `watchlog-0.1.1/PKG-INFO` & `watchlog-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchlog
-Version: 0.1.1
+Version: 0.1.2
 Summary: monitoring log files and sending parsed logs to a specified URL
 Home-page: https://github.com/Euraxluo/watchlog
 License: The MIT LICENSE
 Keywords: log monitor,loguru,watchdog
 Author: euraxluo
 Author-email: euraxluo@outlook.com
 Requires-Python: >=3.8,<4.0
@@ -13,52 +13,54 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/Euraxluo/watchlog
 Description-Content-Type: text/markdown
 
-
 # watchlog
 
-`watchlog` is a Python package for monitoring log files and sending parsed logs to a specified URL using HTTP POST requests.
+`watchlog` is a Python package for monitoring log files and sending parsed logs to a specified URL using HTTP POST
+requests.
 
 - name = "watchlog"
 - description = "monitoring log files and sending parsed logs to a specified URL"
 - authors = ["Euraxluo <euraxluo@outlook.com>"]
 - license = "The MIT LICENSE"
 - repository = "https://github.com/Euraxluo/watchlog"
 - version = "0.1.*"
 
-
-
 ## Installation
 
 You can install `watchlog` using pip:
 
 ```bash
 pip install watchlog
 ```
 
 ## Usage
 
 To use `watchlog`, you need to create a configuration file in JSON format. Here is an example configuration file:
 
 ```json
 {
+  "check_interval": 5,
+  "check": true,
   "files": [
     {
       "path": "/path/to/log/file.log",
       "reg": "^(?P<time>[^ ]*) (?P<level>[^ ]*) (?P<module>[^ ]*) (?P<line>[^ ]*) (?P<message>.*)$",
       "url": "http://example.com/api/logs",
       "latest": true,
+      "enable": true,
       "headers": {
         "Content-Type": "application/json"
       },
       "auth": {
         "username": "user",
         "password": "pass"
       }
@@ -67,42 +69,49 @@
 }
 ```
 
 - `path`: The path of the log file to monitor.
 - `reg`: A regular expression used to parse the log file.
 - `url`: The URL to send the parsed logs to.
 - `latest`: Start monitoring from the latest logs.
+- `enable`: Indicates that this configuration will be enabled, which defaults to true.
 - `headers`: A dictionary of headers to include in the HTTP POST request.
 - `auth`: A dictionary with `username` and `password` keys for basic authentication.
+- `check`: if open check ,it will loop check the config file
+- `check_interval`: circle check interval time(s)
 
-Once you have created the configuration file, you can start monitoring the log file by calling the `start()` function from the `watchlog` module:
+Once you have created the configuration file, you can start monitoring the log file by calling the `start()` function
+from the `watchlog` module:
 
 ```python
 import asyncio
 from watchlog import start
+
 loop = asyncio.get_event_loop()
 loop.run_until_complete(start('path/to/config.json'))
 ```
 
 You can also use we provide small scripts
+
 ```bash
 watchlog path/to/config/file
 ```
 
-This will start monitoring the log file specified in the configuration file and sending parsed logs to the specified URL using HTTP POST requests.
+This will start monitoring the log file specified in the configuration file and sending parsed logs to the specified URL
+using HTTP POST requests.
 
 ## example
+
 example use zinc_observe as log search_engine,Illustrates the use of the process
 
 ```
 .                     
 ├── __init__.py       
 ├── config.json             config file
 ├── docker-compose.yml      log search engine service
 ├── log.log                 log file
 └── main.py                 main python file to monitor log file
 ```
 
-
 ## License
 
 `watchlog` is licensed under the MIT license.
```

