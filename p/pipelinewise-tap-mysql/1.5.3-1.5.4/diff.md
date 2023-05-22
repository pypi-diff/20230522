# Comparing `tmp/pipelinewise-tap-mysql-1.5.3.tar.gz` & `tmp/pipelinewise-tap-mysql-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-mysql-1.5.3.tar", last modified: Tue Apr 25 09:51:10 2023, max compression
+gzip compressed data, was "pipelinewise-tap-mysql-1.5.4.tar", last modified: Mon May 22 15:06:18 2023, max compression
```

## Comparing `pipelinewise-tap-mysql-1.5.3.tar` & `pipelinewise-tap-mysql-1.5.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 09:51:10.000000 pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/tap_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/binlogstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/discover_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 09:51:10.762766 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35207 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/binlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-25 09:50:55.000000 pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 15:06:18.000000 pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/tap_mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/discover_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:18.202822 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/binlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-22 15:06:02.000000 pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/incremental.py
```

### Comparing `pipelinewise-tap-mysql-1.5.3/LICENSE` & `pipelinewise-tap-mysql-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/PKG-INFO` & `pipelinewise-tap-mysql-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.3
+Version: 1.5.4
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -480,14 +480,15 @@
 
 2. Define the environment variables that are required to run the tests:
 ```
   export TAP_MYSQL_HOST=<mysql-host>
   export TAP_MYSQL_PORT=<mysql-port>
   export TAP_MYSQL_USER=<mysql-user>
   export TAP_MYSQL_PASSWORD=<mysql-password>
+  export TAP_MYSQL_ENGINE=<engine>
 ```
 
 3. Install python test dependencies in a virtual env
 
 ```bash
 python3 -m venv venv
 . venv/bin/activate
```

### Comparing `pipelinewise-tap-mysql-1.5.3/README.md` & `pipelinewise-tap-mysql-1.5.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -468,14 +468,15 @@
 
 2. Define the environment variables that are required to run the tests:
 ```
   export TAP_MYSQL_HOST=<mysql-host>
   export TAP_MYSQL_PORT=<mysql-port>
   export TAP_MYSQL_USER=<mysql-user>
   export TAP_MYSQL_PASSWORD=<mysql-password>
+  export TAP_MYSQL_ENGINE=<engine>
 ```
 
 3. Install python test dependencies in a virtual env
 
 ```bash
 python3 -m venv venv
 . venv/bin/activate
```

### Comparing `pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/PKG-INFO` & `pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.3
+Version: 1.5.4
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -480,14 +480,15 @@
 
 2. Define the environment variables that are required to run the tests:
 ```
   export TAP_MYSQL_HOST=<mysql-host>
   export TAP_MYSQL_PORT=<mysql-port>
   export TAP_MYSQL_USER=<mysql-user>
   export TAP_MYSQL_PASSWORD=<mysql-password>
+  export TAP_MYSQL_ENGINE=<engine>
 ```
 
 3. Install python test dependencies in a virtual env
 
 ```bash
 python3 -m venv venv
 . venv/bin/activate
```

### Comparing `pipelinewise-tap-mysql-1.5.3/pipelinewise_tap_mysql.egg-info/SOURCES.txt` & `pipelinewise-tap-mysql-1.5.4/pipelinewise_tap_mysql.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pipelinewise_tap_mysql.egg-info/PKG-INFO
 pipelinewise_tap_mysql.egg-info/SOURCES.txt
 pipelinewise_tap_mysql.egg-info/dependency_links.txt
 pipelinewise_tap_mysql.egg-info/entry_points.txt
 pipelinewise_tap_mysql.egg-info/requires.txt
 pipelinewise_tap_mysql.egg-info/top_level.txt
 tap_mysql/__init__.py
-tap_mysql/binlogstream.py
 tap_mysql/connection.py
 tap_mysql/discover_utils.py
 tap_mysql/stream_utils.py
 tap_mysql/sync_strategies/__init__.py
 tap_mysql/sync_strategies/binlog.py
 tap_mysql/sync_strategies/common.py
 tap_mysql/sync_strategies/full_table.py
```

### Comparing `pipelinewise-tap-mysql-1.5.3/setup.py` & `pipelinewise-tap-mysql-1.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pipelinewise-tap-mysql',
-      version='1.5.3',
+      version='1.5.4',
       description='Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Wise',
       url='https://github.com/transferwise/pipelinewise-tap-mysql',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Programming Language :: Python :: 3 :: Only'
       ],
       py_modules=['tap_mysql'],
       install_requires=[
           'pendulum==2.1.2',
           'pipelinewise-singer-python==1.*',
           'PyMySQL==1.0.2',
-          'mysql-replication==0.30',
+          'mysql-replication==0.40',
           'plpygis==0.2.0',
           'tzlocal==2.1',
       ],
       extras_require={
           'test': [
               'nose==1.3.*',
               'pylint==2.13.2',
```

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/__init__.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/connection.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/connection.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/discover_utils.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/discover_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/stream_utils.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/stream_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/binlog.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/binlog.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 import pymysql.err
 import pytz
 import singer
 import tzlocal
 
 from typing import Dict, Set, Union, Optional, Any, Tuple
 from plpygis import Geometry
+from pymysqlreplication import BinLogStreamReader
 from pymysqlreplication.constants import FIELD_TYPE
 from pymysqlreplication.event import RotateEvent, MariadbGtidEvent, GtidEvent
 from pymysqlreplication.row_event import (
     DeleteRowsEvent,
     UpdateRowsEvent,
     WriteRowsEvent,
 )
 from singer import utils, Schema, metadata
 
 from tap_mysql import connection
-from tap_mysql.binlogstream import CustomBinlogStreamReader
 from tap_mysql.connection import connect_with_backoff, make_connection_wrapper, MySQLConnection
 from tap_mysql.discover_utils import discover_catalog, desired_columns, should_run_discovery
 from tap_mysql.stream_utils import write_schema_message
 from tap_mysql.sync_strategies import common
 
 LOGGER = singer.get_logger('tap_mysql')
 
@@ -587,15 +587,15 @@
 
     return set(binlog_columns_filtered).difference(schema_properties)
 
 
 # pylint: disable=R1702,R0915
 def _run_binlog_sync(
         mysql_conn: MySQLConnection,
-        reader: CustomBinlogStreamReader,
+        reader: BinLogStreamReader,
         binlog_streams_map: Dict,
         state: Dict,
         config: Dict,
         end_log_file: str,
         end_log_pos: int):
 
     processed_rows_events = 0
@@ -789,15 +789,15 @@
 
 
 def create_binlog_stream_reader(
         config: Dict,
         log_file: Optional[str],
         log_pos: Optional[int],
         gtid_pos: Optional[str]
-) -> CustomBinlogStreamReader:
+) -> BinLogStreamReader:
     """
     Create an instance of BinlogStreamReader with the right config
 
     Args:
         config: dictionary of the content of tap config.json
         log_file: binlog file name to start replication from (Optional if using gtid)
         log_pos: binlog pos to start replication from (Optional if using gtid)
@@ -847,15 +847,15 @@
 
         # When not using GTID, we want to listen in for rotate events, and start from given log position and file
         kwargs['only_events'].append(RotateEvent)
         kwargs['log_file'] = log_file
         kwargs['log_pos'] = log_pos
         kwargs['resume_stream'] = True
 
-    return CustomBinlogStreamReader(**kwargs)
+    return BinLogStreamReader(**kwargs)
 
 
 def sync_binlog_stream(
         mysql_conn: MySQLConnection,
         config: Dict,
         binlog_streams_map: Dict[str, Any],
         state: Dict) -> None:
```

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/common.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/full_table.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.3/tap_mysql/sync_strategies/incremental.py` & `pipelinewise-tap-mysql-1.5.4/tap_mysql/sync_strategies/incremental.py`

 * *Files identical despite different names*

