# Comparing `tmp/e6data-python-connector-1.0.4.tar.gz` & `tmp/e6data-python-connector-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e6data-python-connector-1.0.4.tar", last modified: Sun May 14 05:55:19 2023, max compression
+gzip compressed data, was "e6data-python-connector-1.0.5.tar", last modified: Mon May 22 19:33:11 2023, max compression
```

## Comparing `e6data-python-connector-1.0.4.tar` & `e6data-python-connector-1.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vishal     (501) staff       (20)        0 2023-05-14 05:55:19.508740 e6data-python-connector-1.0.4/
--rw-r--r--   0 vishal     (501) staff       (20)    11357 2023-04-03 09:33:07.000000 e6data-python-connector-1.0.4/LICENSE
--rw-r--r--   0 vishal     (501) staff       (20)       55 2023-04-03 09:29:00.000000 e6data-python-connector-1.0.4/MANIFEST.in
--rw-r--r--   0 vishal     (501) staff       (20)     5869 2023-05-14 05:55:19.509103 e6data-python-connector-1.0.4/PKG-INFO
--rw-r--r--   0 vishal     (501) staff       (20)     5189 2023-05-14 05:49:39.000000 e6data-python-connector-1.0.4/README.md
-drwxr-xr-x   0 vishal     (501) staff       (20)        0 2023-05-14 05:55:19.450983 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/
--rw-r--r--   0 vishal     (501) staff       (20)     5869 2023-05-14 05:55:19.000000 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 vishal     (501) staff       (20)      632 2023-05-14 05:55:19.000000 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 vishal     (501) staff       (20)        1 2023-05-14 05:55:19.000000 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 vishal     (501) staff       (20)       62 2023-05-14 05:55:19.000000 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/entry_points.txt
--rw-r--r--   0 vishal     (501) staff       (20)       66 2023-05-14 05:55:19.000000 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/requires.txt
--rw-r--r--   0 vishal     (501) staff       (20)        6 2023-05-14 05:55:19.000000 e6data-python-connector-1.0.4/e6data_python_connector.egg-info/top_level.txt
-drwxr-xr-x   0 vishal     (501) staff       (20)        0 2023-05-14 05:55:19.496557 e6data-python-connector-1.0.4/e6xdb/
--rw-r--r--   0 vishal     (501) staff       (20)      334 2022-04-08 08:47:22.000000 e6data-python-connector-1.0.4/e6xdb/__init__.py
--rw-r--r--   0 vishal     (501) staff       (20)     9958 2022-08-30 11:00:15.000000 e6data-python-connector-1.0.4/e6xdb/common.py
--rw-r--r--   0 vishal     (501) staff       (20)      682 2023-01-02 09:34:23.000000 e6data-python-connector-1.0.4/e6xdb/constants.py
--rw-r--r--   0 vishal     (501) staff       (20)     6052 2023-03-15 05:26:00.000000 e6data-python-connector-1.0.4/e6xdb/datainputstream.py
--rw-r--r--   0 vishal     (501) staff       (20)    13623 2023-03-15 05:26:00.000000 e6data-python-connector-1.0.4/e6xdb/date_time_utils.py
--rw-r--r--   0 vishal     (501) staff       (20)    15415 2023-04-06 10:02:43.000000 e6data-python-connector-1.0.4/e6xdb/e6x.py
--rw-r--r--   0 vishal     (501) staff       (20)      382 2022-04-08 08:47:22.000000 e6data-python-connector-1.0.4/e6xdb/exceptions.py
-drwxr-xr-x   0 vishal     (501) staff       (20)        0 2023-05-14 05:55:19.507031 e6data-python-connector-1.0.4/e6xdb/server/
--rw-r--r--   0 vishal     (501) staff       (20)   133637 2023-05-14 05:49:39.000000 e6data-python-connector-1.0.4/e6xdb/server/QueryEngineService.py
--rw-r--r--   0 vishal     (501) staff       (20)       56 2023-03-29 06:00:44.000000 e6data-python-connector-1.0.4/e6xdb/server/__init__.py
--rw-r--r--   0 vishal     (501) staff       (20)      366 2023-05-14 05:49:39.000000 e6data-python-connector-1.0.4/e6xdb/server/constants.py
--rw-r--r--   0 vishal     (501) staff       (20)    12609 2023-05-14 05:49:39.000000 e6data-python-connector-1.0.4/e6xdb/server/ttypes.py
--rw-r--r--   0 vishal     (501) staff       (20)    11833 2022-08-30 11:00:15.000000 e6data-python-connector-1.0.4/e6xdb/sqlalchemy_e6x.py
--rw-r--r--   0 vishal     (501) staff       (20)     1777 2022-04-08 08:47:22.000000 e6data-python-connector-1.0.4/e6xdb/typeId.py
--rw-r--r--   0 vishal     (501) staff       (20)       64 2023-04-03 09:31:35.000000 e6data-python-connector-1.0.4/pyproject.toml
--rw-r--r--   0 vishal     (501) staff       (20)       73 2023-05-14 05:55:19.513071 e6data-python-connector-1.0.4/setup.cfg
--rw-r--r--   0 vishal     (501) staff       (20)     1925 2023-05-14 05:49:39.000000 e6data-python-connector-1.0.4/setup.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 19:33:11.260081 e6data-python-connector-1.0.5/
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11357 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/LICENSE
+-rw-r--r--   0 vishalanand   (501) staff       (20)       55 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/MANIFEST.in
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-22 19:33:11.260297 e6data-python-connector-1.0.5/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)     5189 2023-05-22 18:39:03.000000 e6data-python-connector-1.0.5/README.md
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 19:33:11.219512 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/
+-rw-r--r--   0 vishalanand   (501) staff       (20)     7301 2023-05-22 19:33:10.000000 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 vishalanand   (501) staff       (20)      632 2023-05-22 19:33:11.000000 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        1 2023-05-22 19:33:10.000000 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       63 2023-05-22 19:33:10.000000 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/entry_points.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)       66 2023-05-22 19:33:10.000000 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/requires.txt
+-rw-r--r--   0 vishalanand   (501) staff       (20)        6 2023-05-22 19:33:10.000000 e6data-python-connector-1.0.5/e6data_python_connector.egg-info/top_level.txt
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 19:33:11.245708 e6data-python-connector-1.0.5/e6xdb/
+-rw-r--r--   0 vishalanand   (501) staff       (20)      334 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     9958 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/common.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      682 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     6052 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/datainputstream.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    13623 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/date_time_utils.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    16791 2023-05-22 19:31:44.000000 e6data-python-connector-1.0.5/e6xdb/e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      382 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/exceptions.py
+drwxr-xr-x   0 vishalanand   (501) staff       (20)        0 2023-05-22 19:33:11.258697 e6data-python-connector-1.0.5/e6xdb/server/
+-rw-r--r--   0 vishalanand   (501) staff       (20)   191597 2023-05-22 18:51:52.000000 e6data-python-connector-1.0.5/e6xdb/server/QueryEngineService.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       56 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/server/__init__.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)      366 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/server/constants.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    12609 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/server/ttypes.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)    11833 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/sqlalchemy_e6x.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1777 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/e6xdb/typeId.py
+-rw-r--r--   0 vishalanand   (501) staff       (20)       64 2023-05-22 17:52:46.000000 e6data-python-connector-1.0.5/pyproject.toml
+-rw-r--r--   0 vishalanand   (501) staff       (20)       73 2023-05-22 19:33:11.265715 e6data-python-connector-1.0.5/setup.cfg
+-rw-r--r--   0 vishalanand   (501) staff       (20)     1925 2023-05-22 18:39:03.000000 e6data-python-connector-1.0.5/setup.py
```

### Comparing `e6data-python-connector-1.0.4/LICENSE` & `e6data-python-connector-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/PKG-INFO` & `e6data-python-connector-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,10 @@
-Metadata-Version: 2.1
-Name: e6data-python-connector
-Version: 1.0.4
-Summary: Client for the e6data distributed SQL Engine.
-Home-page: https://github.com/e6x-labs/e6data-python-connector
-Author: Uniphi, Inc.
-Author-email: info@e6data.com
-License: Apache 2.0
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # e6data Python Connector
 
-![version](https://img.shields.io/badge/version-1.0.4-blue.svg)
+![version](https://img.shields.io/badge/version-1.0.5-blue.svg)
 
 ## Introduction
 
 The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
 
 To install the Python package, use the command below:
 ```shell
@@ -190,8 +172,8 @@
    row = dict(zip(columns, row))
    results.append(row)
    print(row)
 print('Total row count {}, Execution Time (seconds): {}'.format(row_count, execution_time))
 cursor.clear()
 cursor.close()
 conn.close()
-```
+```
```

### Comparing `e6data-python-connector-1.0.4/README.md` & `e6data-python-connector-1.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,179 +1,196 @@
-# e6data Python Connector
-
-![version](https://img.shields.io/badge/version-1.0.4-blue.svg)
-
-## Introduction
-
-The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
-
-To install the Python package, use the command below:
-```shell
-pip install e6data-python-connector
-```
-### Prerequisites
-
-* Open Inbound Port 9000 in the Engine Cluster.
-* Limit access to Port 9000 according to your organizational security policy. Public access is not encouraged.
-* Access Token generated in the e6data console.
-
-### Create a Connection
-
-Use your e6data Email ID as the username and your access token as the password.
-
-```python
-import e6xdb.e6x as edb
-
-username = '<username>'  # Your e6data Email ID.
-password = '<password>'  # Access Token generated in the e6data console.
-
-host = '<host>'  # IP address or hostname of the cluster to be used.
-database = '<database>'  # # Database to perform the query on.
-port = 9000  # Port of the e6data engine.
-
-conn = edb.connect(
-    host=host,
-    port=port,
-    username=username,
-    database=database,
-    password=password
-)
-```
-
-### Perform a Queries & Get Results
-
-```python
-
-query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
-
-cursor = conn.cursor()
-query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
-all_records = cursor.fetchall()
-for row in all_records:
-   print(row)
-```
-
-To fetch all the records:
-```python
-records = cursor.fetchall()
-```
-
-To fetch one record:
-```python
-record = cursor.fetchone()
-```
-
-To fetch limited records:
-```python
-limit = 500
-records = cursor.fetchmany(limit)
-```
-
-To get the execution plan after query execution:
-```python
-import json
-
-query_planner = json.loads(cursor.explain_analyse())
-```
-
-To abort a running query:
-```python
-query_id = '<query_id>'  # query id from execute function response.
-cursor.cancel(query_id)
-```
-
-Switch database in an existing connection:
-```python
-database = '<new_database_name>'  # Replace with the new database.
-cursor = conn.cursor(database)
-```
-
-### Get Query Time Metrics
-```python
-import json
-query = 'SELECT * FROM <TABLE_NAME>'
-
-cursor = conn.cursor()
-query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
-all_records = cursor.fetchall()
-
-query_planner = json.loads(cursor.explain_analyse())
-
-execution_time = query_planner.get("total_query_time")  # In milliseconds
-queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
-parsing_time = query_planner.get("parsingTime")  # In milliseconds
-row_count = query_planner.get('row_count_out')
-```
-
-### Get Schema - a list of Databases, Tables or Columns
-The following code returns a dictionary of all databases, all tables and all columns connected to the cluster currently in use.
-This function can be used without passing database name to get list of all databases.
-
-```python
-databases = conn.get_schema_names()  # To get list of databases.
-print(databases)
-
-database = '<database_name>'  # Replace with actual database name.
-tables = conn.get_tables(database=database)  # To get list of tables from a database.
-print(tables)
-
-table_name = '<table_name>'  # Replace with actual table name.
-columns = conn.get_tables(database=database, table=table_name)  # To get the list of columns from a table.
-columns_with_type = list()
-"""
-Getting the column name and type.
-"""
-for column in columns:
-   columns_with_type.append(dict(column_name=column.fieldName, column_type=column.fieldType))
-print(columns_with_type)
-```
-
-### Code Hygiene
-It is recommended to clear the cursor, close the cursor and close the connection after running a function as a best practice. 
-This enhances performance by clearing old data from memory.
-
-```python
-cursor.clear() # Not needed when aborting a query
-cursor.close()
-conn.close()
-```
-
-### Code Example
-The following code is an example which combines a few functions described above.
-```python
-import e6xdb.e6x as edb
-import json
-
-username = '<username>'  # Your e6data Email ID.
-password = '<password>'  # Access Token generated in the e6data console.
-
-host = '<host>'  # IP address or hostname of the cluster to be used.
-database = '<database>'  # # Database to perform the query on.
-port = 9000  # Port of the e6data engine.
-
-sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
-
-conn = edb.connect(
-    host=host,
-    port=port,
-    username=username,
-    database=database,
-    password=password
-)
-
-cursor = conn.cursor(db_name=database)
-query_id = cursor.execute(sql_query)
-all_records = cursor.fetchall()
-planner_result = json.loads(cursor.explain_analyse())
-execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
-row_count = planner_result.get('row_count_out')
-columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
-results = []
-for row in all_records:
-   row = dict(zip(columns, row))
-   results.append(row)
-   print(row)
-print('Total row count {}, Execution Time (seconds): {}'.format(row_count, execution_time))
-cursor.clear()
-cursor.close()
-conn.close()
-```
+Metadata-Version: 2.1
+Name: e6data-python-connector
+Version: 1.0.5
+Summary: Client for the e6data distributed SQL Engine.
+Home-page: https://github.com/e6x-labs/e6data-python-connector
+Author: Uniphi, Inc.
+Author-email: info@e6data.com
+License: Apache 2.0
+Description: # e6data Python Connector
+        
+        ![version](https://img.shields.io/badge/version-1.0.5-blue.svg)
+        
+        ## Introduction
+        
+        The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
+        
+        To install the Python package, use the command below:
+        ```shell
+        pip install e6data-python-connector
+        ```
+        ### Prerequisites
+        
+        * Open Inbound Port 9000 in the Engine Cluster.
+        * Limit access to Port 9000 according to your organizational security policy. Public access is not encouraged.
+        * Access Token generated in the e6data console.
+        
+        ### Create a Connection
+        
+        Use your e6data Email ID as the username and your access token as the password.
+        
+        ```python
+        import e6xdb.e6x as edb
+        
+        username = '<username>'  # Your e6data Email ID.
+        password = '<password>'  # Access Token generated in the e6data console.
+        
+        host = '<host>'  # IP address or hostname of the cluster to be used.
+        database = '<database>'  # # Database to perform the query on.
+        port = 9000  # Port of the e6data engine.
+        
+        conn = edb.connect(
+            host=host,
+            port=port,
+            username=username,
+            database=database,
+            password=password
+        )
+        ```
+        
+        ### Perform a Queries & Get Results
+        
+        ```python
+        
+        query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
+        
+        cursor = conn.cursor()
+        query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
+        all_records = cursor.fetchall()
+        for row in all_records:
+           print(row)
+        ```
+        
+        To fetch all the records:
+        ```python
+        records = cursor.fetchall()
+        ```
+        
+        To fetch one record:
+        ```python
+        record = cursor.fetchone()
+        ```
+        
+        To fetch limited records:
+        ```python
+        limit = 500
+        records = cursor.fetchmany(limit)
+        ```
+        
+        To get the execution plan after query execution:
+        ```python
+        import json
+        
+        query_planner = json.loads(cursor.explain_analyse())
+        ```
+        
+        To abort a running query:
+        ```python
+        query_id = '<query_id>'  # query id from execute function response.
+        cursor.cancel(query_id)
+        ```
+        
+        Switch database in an existing connection:
+        ```python
+        database = '<new_database_name>'  # Replace with the new database.
+        cursor = conn.cursor(database)
+        ```
+        
+        ### Get Query Time Metrics
+        ```python
+        import json
+        query = 'SELECT * FROM <TABLE_NAME>'
+        
+        cursor = conn.cursor()
+        query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
+        all_records = cursor.fetchall()
+        
+        query_planner = json.loads(cursor.explain_analyse())
+        
+        execution_time = query_planner.get("total_query_time")  # In milliseconds
+        queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
+        parsing_time = query_planner.get("parsingTime")  # In milliseconds
+        row_count = query_planner.get('row_count_out')
+        ```
+        
+        ### Get Schema - a list of Databases, Tables or Columns
+        The following code returns a dictionary of all databases, all tables and all columns connected to the cluster currently in use.
+        This function can be used without passing database name to get list of all databases.
+        
+        ```python
+        databases = conn.get_schema_names()  # To get list of databases.
+        print(databases)
+        
+        database = '<database_name>'  # Replace with actual database name.
+        tables = conn.get_tables(database=database)  # To get list of tables from a database.
+        print(tables)
+        
+        table_name = '<table_name>'  # Replace with actual table name.
+        columns = conn.get_tables(database=database, table=table_name)  # To get the list of columns from a table.
+        columns_with_type = list()
+        """
+        Getting the column name and type.
+        """
+        for column in columns:
+           columns_with_type.append(dict(column_name=column.fieldName, column_type=column.fieldType))
+        print(columns_with_type)
+        ```
+        
+        ### Code Hygiene
+        It is recommended to clear the cursor, close the cursor and close the connection after running a function as a best practice. 
+        This enhances performance by clearing old data from memory.
+        
+        ```python
+        cursor.clear() # Not needed when aborting a query
+        cursor.close()
+        conn.close()
+        ```
+        
+        ### Code Example
+        The following code is an example which combines a few functions described above.
+        ```python
+        import e6xdb.e6x as edb
+        import json
+        
+        username = '<username>'  # Your e6data Email ID.
+        password = '<password>'  # Access Token generated in the e6data console.
+        
+        host = '<host>'  # IP address or hostname of the cluster to be used.
+        database = '<database>'  # # Database to perform the query on.
+        port = 9000  # Port of the e6data engine.
+        
+        sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
+        
+        conn = edb.connect(
+            host=host,
+            port=port,
+            username=username,
+            database=database,
+            password=password
+        )
+        
+        cursor = conn.cursor(db_name=database)
+        query_id = cursor.execute(sql_query)
+        all_records = cursor.fetchall()
+        planner_result = json.loads(cursor.explain_analyse())
+        execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
+        row_count = planner_result.get('row_count_out')
+        columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
+        results = []
+        for row in all_records:
+           row = dict(zip(columns, row))
+           results.append(row)
+           print(row)
+        print('Total row count {}, Execution Time (seconds): {}'.format(row_count, execution_time))
+        cursor.clear()
+        cursor.close()
+        conn.close()
+        ```
+Platform: UNKNOWN
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
```

### Comparing `e6data-python-connector-1.0.4/e6data_python_connector.egg-info/PKG-INFO` & `e6data-python-connector-1.0.5/e6data_python_connector.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,197 +1,196 @@
 Metadata-Version: 2.1
 Name: e6data-python-connector
-Version: 1.0.4
+Version: 1.0.5
 Summary: Client for the e6data distributed SQL Engine.
 Home-page: https://github.com/e6x-labs/e6data-python-connector
 Author: Uniphi, Inc.
 Author-email: info@e6data.com
 License: Apache 2.0
+Description: # e6data Python Connector
+        
+        ![version](https://img.shields.io/badge/version-1.0.5-blue.svg)
+        
+        ## Introduction
+        
+        The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
+        
+        To install the Python package, use the command below:
+        ```shell
+        pip install e6data-python-connector
+        ```
+        ### Prerequisites
+        
+        * Open Inbound Port 9000 in the Engine Cluster.
+        * Limit access to Port 9000 according to your organizational security policy. Public access is not encouraged.
+        * Access Token generated in the e6data console.
+        
+        ### Create a Connection
+        
+        Use your e6data Email ID as the username and your access token as the password.
+        
+        ```python
+        import e6xdb.e6x as edb
+        
+        username = '<username>'  # Your e6data Email ID.
+        password = '<password>'  # Access Token generated in the e6data console.
+        
+        host = '<host>'  # IP address or hostname of the cluster to be used.
+        database = '<database>'  # # Database to perform the query on.
+        port = 9000  # Port of the e6data engine.
+        
+        conn = edb.connect(
+            host=host,
+            port=port,
+            username=username,
+            database=database,
+            password=password
+        )
+        ```
+        
+        ### Perform a Queries & Get Results
+        
+        ```python
+        
+        query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
+        
+        cursor = conn.cursor()
+        query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
+        all_records = cursor.fetchall()
+        for row in all_records:
+           print(row)
+        ```
+        
+        To fetch all the records:
+        ```python
+        records = cursor.fetchall()
+        ```
+        
+        To fetch one record:
+        ```python
+        record = cursor.fetchone()
+        ```
+        
+        To fetch limited records:
+        ```python
+        limit = 500
+        records = cursor.fetchmany(limit)
+        ```
+        
+        To get the execution plan after query execution:
+        ```python
+        import json
+        
+        query_planner = json.loads(cursor.explain_analyse())
+        ```
+        
+        To abort a running query:
+        ```python
+        query_id = '<query_id>'  # query id from execute function response.
+        cursor.cancel(query_id)
+        ```
+        
+        Switch database in an existing connection:
+        ```python
+        database = '<new_database_name>'  # Replace with the new database.
+        cursor = conn.cursor(database)
+        ```
+        
+        ### Get Query Time Metrics
+        ```python
+        import json
+        query = 'SELECT * FROM <TABLE_NAME>'
+        
+        cursor = conn.cursor()
+        query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
+        all_records = cursor.fetchall()
+        
+        query_planner = json.loads(cursor.explain_analyse())
+        
+        execution_time = query_planner.get("total_query_time")  # In milliseconds
+        queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
+        parsing_time = query_planner.get("parsingTime")  # In milliseconds
+        row_count = query_planner.get('row_count_out')
+        ```
+        
+        ### Get Schema - a list of Databases, Tables or Columns
+        The following code returns a dictionary of all databases, all tables and all columns connected to the cluster currently in use.
+        This function can be used without passing database name to get list of all databases.
+        
+        ```python
+        databases = conn.get_schema_names()  # To get list of databases.
+        print(databases)
+        
+        database = '<database_name>'  # Replace with actual database name.
+        tables = conn.get_tables(database=database)  # To get list of tables from a database.
+        print(tables)
+        
+        table_name = '<table_name>'  # Replace with actual table name.
+        columns = conn.get_tables(database=database, table=table_name)  # To get the list of columns from a table.
+        columns_with_type = list()
+        """
+        Getting the column name and type.
+        """
+        for column in columns:
+           columns_with_type.append(dict(column_name=column.fieldName, column_type=column.fieldType))
+        print(columns_with_type)
+        ```
+        
+        ### Code Hygiene
+        It is recommended to clear the cursor, close the cursor and close the connection after running a function as a best practice. 
+        This enhances performance by clearing old data from memory.
+        
+        ```python
+        cursor.clear() # Not needed when aborting a query
+        cursor.close()
+        conn.close()
+        ```
+        
+        ### Code Example
+        The following code is an example which combines a few functions described above.
+        ```python
+        import e6xdb.e6x as edb
+        import json
+        
+        username = '<username>'  # Your e6data Email ID.
+        password = '<password>'  # Access Token generated in the e6data console.
+        
+        host = '<host>'  # IP address or hostname of the cluster to be used.
+        database = '<database>'  # # Database to perform the query on.
+        port = 9000  # Port of the e6data engine.
+        
+        sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
+        
+        conn = edb.connect(
+            host=host,
+            port=port,
+            username=username,
+            database=database,
+            password=password
+        )
+        
+        cursor = conn.cursor(db_name=database)
+        query_id = cursor.execute(sql_query)
+        all_records = cursor.fetchall()
+        planner_result = json.loads(cursor.explain_analyse())
+        execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
+        row_count = planner_result.get('row_count_out')
+        columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
+        results = []
+        for row in all_records:
+           row = dict(zip(columns, row))
+           results.append(row)
+           print(row)
+        print('Total row count {}, Execution Time (seconds): {}'.format(row_count, execution_time))
+        cursor.clear()
+        cursor.close()
+        conn.close()
+        ```
+Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# e6data Python Connector
-
-![version](https://img.shields.io/badge/version-1.0.4-blue.svg)
-
-## Introduction
-
-The e6data Connector for Python provides an interface for writing Python applications that can connect to e6data and perform operations.
-
-To install the Python package, use the command below:
-```shell
-pip install e6data-python-connector
-```
-### Prerequisites
-
-* Open Inbound Port 9000 in the Engine Cluster.
-* Limit access to Port 9000 according to your organizational security policy. Public access is not encouraged.
-* Access Token generated in the e6data console.
-
-### Create a Connection
-
-Use your e6data Email ID as the username and your access token as the password.
-
-```python
-import e6xdb.e6x as edb
-
-username = '<username>'  # Your e6data Email ID.
-password = '<password>'  # Access Token generated in the e6data console.
-
-host = '<host>'  # IP address or hostname of the cluster to be used.
-database = '<database>'  # # Database to perform the query on.
-port = 9000  # Port of the e6data engine.
-
-conn = edb.connect(
-    host=host,
-    port=port,
-    username=username,
-    database=database,
-    password=password
-)
-```
-
-### Perform a Queries & Get Results
-
-```python
-
-query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the query.
-
-cursor = conn.cursor()
-query_id = cursor.execute(query)  # The execute function returns a unique query ID, which can be use to abort the query.
-all_records = cursor.fetchall()
-for row in all_records:
-   print(row)
-```
-
-To fetch all the records:
-```python
-records = cursor.fetchall()
-```
-
-To fetch one record:
-```python
-record = cursor.fetchone()
-```
-
-To fetch limited records:
-```python
-limit = 500
-records = cursor.fetchmany(limit)
-```
-
-To get the execution plan after query execution:
-```python
-import json
-
-query_planner = json.loads(cursor.explain_analyse())
-```
-
-To abort a running query:
-```python
-query_id = '<query_id>'  # query id from execute function response.
-cursor.cancel(query_id)
-```
-
-Switch database in an existing connection:
-```python
-database = '<new_database_name>'  # Replace with the new database.
-cursor = conn.cursor(database)
-```
-
-### Get Query Time Metrics
-```python
-import json
-query = 'SELECT * FROM <TABLE_NAME>'
-
-cursor = conn.cursor()
-query_id = cursor.execute(query)  # execute function returns query id, can be use for aborting th query.
-all_records = cursor.fetchall()
-
-query_planner = json.loads(cursor.explain_analyse())
-
-execution_time = query_planner.get("total_query_time")  # In milliseconds
-queue_time = query_planner.get("executionQueueingTime")  # In milliseconds
-parsing_time = query_planner.get("parsingTime")  # In milliseconds
-row_count = query_planner.get('row_count_out')
-```
-
-### Get Schema - a list of Databases, Tables or Columns
-The following code returns a dictionary of all databases, all tables and all columns connected to the cluster currently in use.
-This function can be used without passing database name to get list of all databases.
-
-```python
-databases = conn.get_schema_names()  # To get list of databases.
-print(databases)
-
-database = '<database_name>'  # Replace with actual database name.
-tables = conn.get_tables(database=database)  # To get list of tables from a database.
-print(tables)
-
-table_name = '<table_name>'  # Replace with actual table name.
-columns = conn.get_tables(database=database, table=table_name)  # To get the list of columns from a table.
-columns_with_type = list()
-"""
-Getting the column name and type.
-"""
-for column in columns:
-   columns_with_type.append(dict(column_name=column.fieldName, column_type=column.fieldType))
-print(columns_with_type)
-```
-
-### Code Hygiene
-It is recommended to clear the cursor, close the cursor and close the connection after running a function as a best practice. 
-This enhances performance by clearing old data from memory.
-
-```python
-cursor.clear() # Not needed when aborting a query
-cursor.close()
-conn.close()
-```
-
-### Code Example
-The following code is an example which combines a few functions described above.
-```python
-import e6xdb.e6x as edb
-import json
-
-username = '<username>'  # Your e6data Email ID.
-password = '<password>'  # Access Token generated in the e6data console.
-
-host = '<host>'  # IP address or hostname of the cluster to be used.
-database = '<database>'  # # Database to perform the query on.
-port = 9000  # Port of the e6data engine.
-
-sql_query = 'SELECT * FROM <TABLE_NAME>'  # Replace with the actual query.
-
-conn = edb.connect(
-    host=host,
-    port=port,
-    username=username,
-    database=database,
-    password=password
-)
-
-cursor = conn.cursor(db_name=database)
-query_id = cursor.execute(sql_query)
-all_records = cursor.fetchall()
-planner_result = json.loads(cursor.explain_analyse())
-execution_time = planner_result.get("total_query_time") / 1000  # Converting into seconds.
-row_count = planner_result.get('row_count_out')
-columns = [col[0] for col in cursor.description]  # Get the column names and merge them with the results.
-results = []
-for row in all_records:
-   row = dict(zip(columns, row))
-   results.append(row)
-   print(row)
-print('Total row count {}, Execution Time (seconds): {}'.format(row_count, execution_time))
-cursor.clear()
-cursor.close()
-conn.close()
-```
```

### Comparing `e6data-python-connector-1.0.4/e6data_python_connector.egg-info/SOURCES.txt` & `e6data-python-connector-1.0.5/e6data_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/common.py` & `e6data-python-connector-1.0.5/e6xdb/common.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/constants.py` & `e6data-python-connector-1.0.5/e6xdb/constants.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/datainputstream.py` & `e6data-python-connector-1.0.5/e6xdb/datainputstream.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/date_time_utils.py` & `e6data-python-connector-1.0.5/e6xdb/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/e6x.py` & `e6data-python-connector-1.0.5/e6xdb/e6x.py`

 * *Files 8% similar despite different names*

```diff
@@ -185,23 +185,50 @@
 
     def query_cancel(self, query_id):
         self._client.cancelQuery(sessionId=self.get_session_id, queryId=query_id)
 
     def dry_run(self, query):
         return self._client.dryRun(sessionId=self.get_session_id, sSchema=self._database, sQueryString=query)
 
+    def dry_run_v2(self, catalog_name, query):
+        return self._client.dryRunV2(
+            sessionId=self.get_session_id,
+            catalogName=catalog_name,
+            sSchema=self._database,
+            sQueryString=query
+        )
+
     def get_tables(self, database):
         return self._client.getTables(sessionId=self.get_session_id, schema=database)
 
+    def get_tables_v2(self, catalog_name, database):
+        return self._client.getTablesV2(sessionId=self.get_session_id, catalogName=catalog_name, schema=database)
+
     def get_columns(self, database, table):
-        return self._client.getColumns(sessionId=self.get_session_id, schema=database, table=table)
+        catalog_name = ''
+        return self._client.getColumns(sessionId=self.get_session_id, catalogName=catalog_name, schema=database,
+                                       table=table)
+
+    def get_columns_v2(self, catalog_name, database, table):
+        return self._client.getColumnsV2(
+            sessionId=self.get_session_id,
+            catalogName=catalog_name,
+            schema=database,
+            table=table
+        )
 
     def get_schema_names(self):
         return self._client.getSchemaNames(sessionId=self.get_session_id)
 
+    def get_schema_names_v2(self, catalog_name):
+        return self._client.getSchemaNamesV2(sessionId=self.get_session_id, catalogName=catalog_name)
+
+    def add_catalogs(self, catalogs_info):
+        return self._client.addCatalogs(sessionId=self.get_session_id, jsonString=catalogs_info)
+
     def commit(self):
         """We do not support transactions, so this does nothing."""
         pass
 
     def cursor(self, db_name=None):
         """Return a new :py:class:`Cursor` object using the connection."""
         return Cursor(self, database=db_name)
@@ -218,16 +245,17 @@
     """These objects represent a database cursor, which is used to manage the context of a fetch
     operation.
     Cursors are not isolated, i.e., any changes done to the database by a cursor are immediately
     visible by other cursors or connections.
     """
     rows_count = 0
 
-    def __init__(self, connection, arraysize=1000, database=None):
+    def __init__(self, connection, catalog_name=None, arraysize=1000, database=None):
         super(Cursor, self).__init__()
+        self._catalog_name = catalog_name
         self._arraysize = arraysize
         self.connection = connection
         self._data = None
         self._query_columns_description = None
         self._is_metadata_updated = False
         self._description = None
         self._query_id = None
@@ -328,19 +356,27 @@
         # Prepare statement
         if parameters is None:
             sql = operation
         else:
             sql = operation % _escaper.escape_args(parameters)
 
         client = self.connection.client
-        self._query_id = client.prepareStatement(
-            self.connection.get_session_id,
-            self._database,
-            sql
-        )
+        if self._catalog_name:
+            self._query_id = client.prepareStatementV2(
+                self.connection.get_session_id,
+                self._catalog_name,
+                self._database,
+                sql
+            )
+        else:
+            self._query_id = client.prepareStatement(
+                self.connection.get_session_id,
+                self._database,
+                sql
+            )
         client.executeStatement(self.connection.get_session_id, self._query_id)
         self.update_mete_data()
         return self._query_id
 
     def rowcount(self):
         return self._rowcount
```

### Comparing `e6data-python-connector-1.0.4/e6xdb/server/QueryEngineService.py` & `e6data-python-connector-1.0.5/e6xdb/server/QueryEngineService.py`

 * *Files 13% similar despite different names*

```diff
@@ -52,14 +52,25 @@
          - sessionId
          - sSchema
          - sQueryString
 
         """
         pass
 
+    def dryRunV2(self, sessionId, catalogName, sSchema, sQueryString):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - sSchema
+         - sQueryString
+
+        """
+        pass
+
     def explainAnalyze(self, sessionId, queryId):
         """
         Parameters:
          - sessionId
          - queryId
 
         """
@@ -71,14 +82,25 @@
          - sessionId
          - sSchemaName
          - query
 
         """
         pass
 
+    def prepareStatementV2(self, sessionId, catalogName, sSchemaName, query):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - sSchemaName
+         - query
+
+        """
+        pass
+
     def executeStatement(self, sessionId, queryId):
         """
         Parameters:
          - sessionId
          - queryId
 
         """
@@ -125,26 +147,57 @@
         Parameters:
          - sessionId
          - schema
 
         """
         pass
 
+    def getTablesV2(self, sessionId, catalogName, schema):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - schema
+
+        """
+        pass
+
     def getSchemaNames(self, sessionId):
         """
         Parameters:
          - sessionId
 
         """
         pass
 
-    def getColumns(self, sessionId, schema, table):
+    def getSchemaNamesV2(self, sessionId, catalogName):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+
+        """
+        pass
+
+    def getColumns(self, sessionId, catalogName, schema, table):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - schema
+         - table
+
+        """
+        pass
+
+    def getColumnsV2(self, sessionId, catalogName, schema, table):
         """
         Parameters:
          - sessionId
+         - catalogName
          - schema
          - table
 
         """
         pass
 
     def updateUsers(self, userInfo):
@@ -160,14 +213,23 @@
         Parameters:
          - sessionId
          - propMap
 
         """
         pass
 
+    def addCatalogs(self, sessionId, jsonString):
+        """
+        Parameters:
+         - sessionId
+         - jsonString
+
+        """
+        pass
+
 
 class Client(Iface):
     def __init__(self, iprot, oprot=None):
         self._iprot = self._oprot = iprot
         if oprot is not None:
             self._oprot = oprot
         self._seqid = 0
@@ -318,14 +380,56 @@
             return result.success
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         raise TApplicationException(TApplicationException.MISSING_RESULT, "dryRun failed: unknown result")
 
+    def dryRunV2(self, sessionId, catalogName, sSchema, sQueryString):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - sSchema
+         - sQueryString
+
+        """
+        self.send_dryRunV2(sessionId, catalogName, sSchema, sQueryString)
+        return self.recv_dryRunV2()
+
+    def send_dryRunV2(self, sessionId, catalogName, sSchema, sQueryString):
+        self._oprot.writeMessageBegin('dryRunV2', TMessageType.CALL, self._seqid)
+        args = dryRunV2_args()
+        args.sessionId = sessionId
+        args.catalogName = catalogName
+        args.sSchema = sSchema
+        args.sQueryString = sQueryString
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_dryRunV2(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = dryRunV2_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "dryRunV2 failed: unknown result")
+
     def explainAnalyze(self, sessionId, queryId):
         """
         Parameters:
          - sessionId
          - queryId
 
         """
@@ -396,14 +500,56 @@
             return result.success
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         raise TApplicationException(TApplicationException.MISSING_RESULT, "prepareStatement failed: unknown result")
 
+    def prepareStatementV2(self, sessionId, catalogName, sSchemaName, query):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - sSchemaName
+         - query
+
+        """
+        self.send_prepareStatementV2(sessionId, catalogName, sSchemaName, query)
+        return self.recv_prepareStatementV2()
+
+    def send_prepareStatementV2(self, sessionId, catalogName, sSchemaName, query):
+        self._oprot.writeMessageBegin('prepareStatementV2', TMessageType.CALL, self._seqid)
+        args = prepareStatementV2_args()
+        args.sessionId = sessionId
+        args.catalogName = catalogName
+        args.sSchemaName = sSchemaName
+        args.query = query
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_prepareStatementV2(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = prepareStatementV2_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "prepareStatementV2 failed: unknown result")
+
     def executeStatement(self, sessionId, queryId):
         """
         Parameters:
          - sessionId
          - queryId
 
         """
@@ -620,14 +766,54 @@
             return result.success
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         raise TApplicationException(TApplicationException.MISSING_RESULT, "getTables failed: unknown result")
 
+    def getTablesV2(self, sessionId, catalogName, schema):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - schema
+
+        """
+        self.send_getTablesV2(sessionId, catalogName, schema)
+        return self.recv_getTablesV2()
+
+    def send_getTablesV2(self, sessionId, catalogName, schema):
+        self._oprot.writeMessageBegin('getTablesV2', TMessageType.CALL, self._seqid)
+        args = getTablesV2_args()
+        args.sessionId = sessionId
+        args.catalogName = catalogName
+        args.schema = schema
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_getTablesV2(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = getTablesV2_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "getTablesV2 failed: unknown result")
+
     def getSchemaNames(self, sessionId):
         """
         Parameters:
          - sessionId
 
         """
         self.send_getSchemaNames(sessionId)
@@ -656,29 +842,69 @@
             return result.success
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         raise TApplicationException(TApplicationException.MISSING_RESULT, "getSchemaNames failed: unknown result")
 
-    def getColumns(self, sessionId, schema, table):
+    def getSchemaNamesV2(self, sessionId, catalogName):
         """
         Parameters:
          - sessionId
+         - catalogName
+
+        """
+        self.send_getSchemaNamesV2(sessionId, catalogName)
+        return self.recv_getSchemaNamesV2()
+
+    def send_getSchemaNamesV2(self, sessionId, catalogName):
+        self._oprot.writeMessageBegin('getSchemaNamesV2', TMessageType.CALL, self._seqid)
+        args = getSchemaNamesV2_args()
+        args.sessionId = sessionId
+        args.catalogName = catalogName
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_getSchemaNamesV2(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = getSchemaNamesV2_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "getSchemaNamesV2 failed: unknown result")
+
+    def getColumns(self, sessionId, catalogName, schema, table):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
          - schema
          - table
 
         """
-        self.send_getColumns(sessionId, schema, table)
+        self.send_getColumns(sessionId, catalogName, schema, table)
         return self.recv_getColumns()
 
-    def send_getColumns(self, sessionId, schema, table):
+    def send_getColumns(self, sessionId, catalogName, schema, table):
         self._oprot.writeMessageBegin('getColumns', TMessageType.CALL, self._seqid)
         args = getColumns_args()
         args.sessionId = sessionId
+        args.catalogName = catalogName
         args.schema = schema
         args.table = table
         args.write(self._oprot)
         self._oprot.writeMessageEnd()
         self._oprot.trans.flush()
 
     def recv_getColumns(self):
@@ -696,14 +922,56 @@
             return result.success
         if result.error1 is not None:
             raise result.error1
         if result.error2 is not None:
             raise result.error2
         raise TApplicationException(TApplicationException.MISSING_RESULT, "getColumns failed: unknown result")
 
+    def getColumnsV2(self, sessionId, catalogName, schema, table):
+        """
+        Parameters:
+         - sessionId
+         - catalogName
+         - schema
+         - table
+
+        """
+        self.send_getColumnsV2(sessionId, catalogName, schema, table)
+        return self.recv_getColumnsV2()
+
+    def send_getColumnsV2(self, sessionId, catalogName, schema, table):
+        self._oprot.writeMessageBegin('getColumnsV2', TMessageType.CALL, self._seqid)
+        args = getColumnsV2_args()
+        args.sessionId = sessionId
+        args.catalogName = catalogName
+        args.schema = schema
+        args.table = table
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_getColumnsV2(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = getColumnsV2_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.success is not None:
+            return result.success
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        raise TApplicationException(TApplicationException.MISSING_RESULT, "getColumnsV2 failed: unknown result")
+
     def updateUsers(self, userInfo):
         """
         Parameters:
          - userInfo
 
         """
         self.send_updateUsers(userInfo)
@@ -764,35 +1032,77 @@
         result = setProps_result()
         result.read(iprot)
         iprot.readMessageEnd()
         if result.error2 is not None:
             raise result.error2
         return
 
+    def addCatalogs(self, sessionId, jsonString):
+        """
+        Parameters:
+         - sessionId
+         - jsonString
+
+        """
+        self.send_addCatalogs(sessionId, jsonString)
+        self.recv_addCatalogs()
+
+    def send_addCatalogs(self, sessionId, jsonString):
+        self._oprot.writeMessageBegin('addCatalogs', TMessageType.CALL, self._seqid)
+        args = addCatalogs_args()
+        args.sessionId = sessionId
+        args.jsonString = jsonString
+        args.write(self._oprot)
+        self._oprot.writeMessageEnd()
+        self._oprot.trans.flush()
+
+    def recv_addCatalogs(self):
+        iprot = self._iprot
+        (fname, mtype, rseqid) = iprot.readMessageBegin()
+        if mtype == TMessageType.EXCEPTION:
+            x = TApplicationException()
+            x.read(iprot)
+            iprot.readMessageEnd()
+            raise x
+        result = addCatalogs_result()
+        result.read(iprot)
+        iprot.readMessageEnd()
+        if result.error1 is not None:
+            raise result.error1
+        if result.error2 is not None:
+            raise result.error2
+        return
+
 
 class Processor(Iface, TProcessor):
     def __init__(self, handler):
         self._handler = handler
         self._processMap = {}
         self._processMap["clear"] = Processor.process_clear
         self._processMap["cancelQuery"] = Processor.process_cancelQuery
         self._processMap["explain"] = Processor.process_explain
         self._processMap["dryRun"] = Processor.process_dryRun
+        self._processMap["dryRunV2"] = Processor.process_dryRunV2
         self._processMap["explainAnalyze"] = Processor.process_explainAnalyze
         self._processMap["prepareStatement"] = Processor.process_prepareStatement
+        self._processMap["prepareStatementV2"] = Processor.process_prepareStatementV2
         self._processMap["executeStatement"] = Processor.process_executeStatement
         self._processMap["getNextResultRow"] = Processor.process_getNextResultRow
         self._processMap["getNextResultBatch"] = Processor.process_getNextResultBatch
         self._processMap["getResultMetadata"] = Processor.process_getResultMetadata
         self._processMap["authenticate"] = Processor.process_authenticate
         self._processMap["getTables"] = Processor.process_getTables
+        self._processMap["getTablesV2"] = Processor.process_getTablesV2
         self._processMap["getSchemaNames"] = Processor.process_getSchemaNames
+        self._processMap["getSchemaNamesV2"] = Processor.process_getSchemaNamesV2
         self._processMap["getColumns"] = Processor.process_getColumns
+        self._processMap["getColumnsV2"] = Processor.process_getColumnsV2
         self._processMap["updateUsers"] = Processor.process_updateUsers
         self._processMap["setProps"] = Processor.process_setProps
+        self._processMap["addCatalogs"] = Processor.process_addCatalogs
         self._on_message_begin = None
 
     def on_message_begin(self, func):
         self._on_message_begin = func
 
     def process(self, iprot, oprot):
         (name, type, seqid) = iprot.readMessageBegin()
@@ -923,14 +1233,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("dryRun", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_dryRunV2(self, seqid, iprot, oprot):
+        args = dryRunV2_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = dryRunV2_result()
+        try:
+            result.success = self._handler.dryRunV2(args.sessionId, args.catalogName, args.sSchema, args.sQueryString)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("dryRunV2", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_explainAnalyze(self, seqid, iprot, oprot):
         args = explainAnalyze_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = explainAnalyze_result()
         try:
             result.success = self._handler.explainAnalyze(args.sessionId, args.queryId)
@@ -981,14 +1320,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("prepareStatement", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_prepareStatementV2(self, seqid, iprot, oprot):
+        args = prepareStatementV2_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = prepareStatementV2_result()
+        try:
+            result.success = self._handler.prepareStatementV2(args.sessionId, args.catalogName, args.sSchemaName, args.query)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("prepareStatementV2", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_executeStatement(self, seqid, iprot, oprot):
         args = executeStatement_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = executeStatement_result()
         try:
             self._handler.executeStatement(args.sessionId, args.queryId)
@@ -1152,14 +1520,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("getTables", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_getTablesV2(self, seqid, iprot, oprot):
+        args = getTablesV2_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = getTablesV2_result()
+        try:
+            result.success = self._handler.getTablesV2(args.sessionId, args.catalogName, args.schema)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("getTablesV2", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_getSchemaNames(self, seqid, iprot, oprot):
         args = getSchemaNames_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = getSchemaNames_result()
         try:
             result.success = self._handler.getSchemaNames(args.sessionId)
@@ -1181,21 +1578,50 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("getSchemaNames", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_getSchemaNamesV2(self, seqid, iprot, oprot):
+        args = getSchemaNamesV2_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = getSchemaNamesV2_result()
+        try:
+            result.success = self._handler.getSchemaNamesV2(args.sessionId, args.catalogName)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("getSchemaNamesV2", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_getColumns(self, seqid, iprot, oprot):
         args = getColumns_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = getColumns_result()
         try:
-            result.success = self._handler.getColumns(args.sessionId, args.schema, args.table)
+            result.success = self._handler.getColumns(args.sessionId, args.catalogName, args.schema, args.table)
             msg_type = TMessageType.REPLY
         except TTransport.TTransportException:
             raise
         except QueryProcessingException as error1:
             msg_type = TMessageType.REPLY
             result.error1 = error1
         except AccessDeniedException as error2:
@@ -1210,14 +1636,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("getColumns", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_getColumnsV2(self, seqid, iprot, oprot):
+        args = getColumnsV2_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = getColumnsV2_result()
+        try:
+            result.success = self._handler.getColumnsV2(args.sessionId, args.catalogName, args.schema, args.table)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("getColumnsV2", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
     def process_updateUsers(self, seqid, iprot, oprot):
         args = updateUsers_args()
         args.read(iprot)
         iprot.readMessageEnd()
         result = updateUsers_result()
         try:
             self._handler.updateUsers(args.userInfo)
@@ -1265,14 +1720,43 @@
             msg_type = TMessageType.EXCEPTION
             result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
         oprot.writeMessageBegin("setProps", msg_type, seqid)
         result.write(oprot)
         oprot.writeMessageEnd()
         oprot.trans.flush()
 
+    def process_addCatalogs(self, seqid, iprot, oprot):
+        args = addCatalogs_args()
+        args.read(iprot)
+        iprot.readMessageEnd()
+        result = addCatalogs_result()
+        try:
+            self._handler.addCatalogs(args.sessionId, args.jsonString)
+            msg_type = TMessageType.REPLY
+        except TTransport.TTransportException:
+            raise
+        except QueryProcessingException as error1:
+            msg_type = TMessageType.REPLY
+            result.error1 = error1
+        except AccessDeniedException as error2:
+            msg_type = TMessageType.REPLY
+            result.error2 = error2
+        except TApplicationException as ex:
+            logging.exception('TApplication exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = ex
+        except Exception:
+            logging.exception('Unexpected exception in handler')
+            msg_type = TMessageType.EXCEPTION
+            result = TApplicationException(TApplicationException.INTERNAL_ERROR, 'Internal error')
+        oprot.writeMessageBegin("addCatalogs", msg_type, seqid)
+        result.write(oprot)
+        oprot.writeMessageEnd()
+        oprot.trans.flush()
+
 # HELPER FUNCTIONS AND STRUCTURES
 
 
 class clear_args(object):
     """
     Attributes:
      - sessionId
@@ -1894,14 +2378,197 @@
 dryRun_result.thrift_spec = (
     (0, TType.STRING, 'success', 'UTF8', None, ),  # 0
     (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
     (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
 )
 
 
+class dryRunV2_args(object):
+    """
+    Attributes:
+     - sessionId
+     - catalogName
+     - sSchema
+     - sQueryString
+
+    """
+
+
+    def __init__(self, sessionId=None, catalogName=None, sSchema=None, sQueryString=None,):
+        self.sessionId = sessionId
+        self.catalogName = catalogName
+        self.sSchema = sSchema
+        self.sQueryString = sQueryString
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.sSchema = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRING:
+                    self.sQueryString = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('dryRunV2_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.catalogName is not None:
+            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
+            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
+            oprot.writeFieldEnd()
+        if self.sSchema is not None:
+            oprot.writeFieldBegin('sSchema', TType.STRING, 3)
+            oprot.writeString(self.sSchema.encode('utf-8') if sys.version_info[0] == 2 else self.sSchema)
+            oprot.writeFieldEnd()
+        if self.sQueryString is not None:
+            oprot.writeFieldBegin('sQueryString', TType.STRING, 4)
+            oprot.writeString(self.sQueryString.encode('utf-8') if sys.version_info[0] == 2 else self.sQueryString)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(dryRunV2_args)
+dryRunV2_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'sSchema', 'UTF8', None, ),  # 3
+    (4, TType.STRING, 'sQueryString', 'UTF8', None, ),  # 4
+)
+
+
+class dryRunV2_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.STRING:
+                    self.success = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('dryRunV2_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.STRING, 0)
+            oprot.writeString(self.success.encode('utf-8') if sys.version_info[0] == 2 else self.success)
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(dryRunV2_result)
+dryRunV2_result.thrift_spec = (
+    (0, TType.STRING, 'success', 'UTF8', None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
+
+
 class explainAnalyze_args(object):
     """
     Attributes:
      - sessionId
      - queryId
 
     """
@@ -2224,14 +2891,197 @@
 prepareStatement_result.thrift_spec = (
     (0, TType.STRING, 'success', 'UTF8', None, ),  # 0
     (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
     (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
 )
 
 
+class prepareStatementV2_args(object):
+    """
+    Attributes:
+     - sessionId
+     - catalogName
+     - sSchemaName
+     - query
+
+    """
+
+
+    def __init__(self, sessionId=None, catalogName=None, sSchemaName=None, query=None,):
+        self.sessionId = sessionId
+        self.catalogName = catalogName
+        self.sSchemaName = sSchemaName
+        self.query = query
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.sSchemaName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRING:
+                    self.query = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('prepareStatementV2_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.catalogName is not None:
+            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
+            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
+            oprot.writeFieldEnd()
+        if self.sSchemaName is not None:
+            oprot.writeFieldBegin('sSchemaName', TType.STRING, 3)
+            oprot.writeString(self.sSchemaName.encode('utf-8') if sys.version_info[0] == 2 else self.sSchemaName)
+            oprot.writeFieldEnd()
+        if self.query is not None:
+            oprot.writeFieldBegin('query', TType.STRING, 4)
+            oprot.writeString(self.query.encode('utf-8') if sys.version_info[0] == 2 else self.query)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(prepareStatementV2_args)
+prepareStatementV2_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'sSchemaName', 'UTF8', None, ),  # 3
+    (4, TType.STRING, 'query', 'UTF8', None, ),  # 4
+)
+
+
+class prepareStatementV2_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.STRING:
+                    self.success = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('prepareStatementV2_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.STRING, 0)
+            oprot.writeString(self.success.encode('utf-8') if sys.version_info[0] == 2 else self.success)
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(prepareStatementV2_result)
+prepareStatementV2_result.thrift_spec = (
+    (0, TType.STRING, 'success', 'UTF8', None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
+
+
 class executeStatement_args(object):
     """
     Attributes:
      - sessionId
      - queryId
 
     """
@@ -3163,14 +4013,193 @@
 getTables_result.thrift_spec = (
     (0, TType.LIST, 'success', (TType.STRING, 'UTF8', False), None, ),  # 0
     (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
     (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
 )
 
 
+class getTablesV2_args(object):
+    """
+    Attributes:
+     - sessionId
+     - catalogName
+     - schema
+
+    """
+
+
+    def __init__(self, sessionId=None, catalogName=None, schema=None,):
+        self.sessionId = sessionId
+        self.catalogName = catalogName
+        self.schema = schema
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.schema = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getTablesV2_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.catalogName is not None:
+            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
+            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
+            oprot.writeFieldEnd()
+        if self.schema is not None:
+            oprot.writeFieldBegin('schema', TType.STRING, 3)
+            oprot.writeString(self.schema.encode('utf-8') if sys.version_info[0] == 2 else self.schema)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getTablesV2_args)
+getTablesV2_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'schema', 'UTF8', None, ),  # 3
+)
+
+
+class getTablesV2_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.LIST:
+                    self.success = []
+                    (_etype17, _size14) = iprot.readListBegin()
+                    for _i18 in range(_size14):
+                        _elem19 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem19)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getTablesV2_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.LIST, 0)
+            oprot.writeListBegin(TType.STRING, len(self.success))
+            for iter20 in self.success:
+                oprot.writeString(iter20.encode('utf-8') if sys.version_info[0] == 2 else iter20)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getTablesV2_result)
+getTablesV2_result.thrift_spec = (
+    (0, TType.LIST, 'success', (TType.STRING, 'UTF8', False), None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
+
+
 class getSchemaNames_args(object):
     """
     Attributes:
      - sessionId
 
     """
 
@@ -3252,18 +4281,18 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype17, _size14) = iprot.readListBegin()
-                    for _i18 in range(_size14):
-                        _elem19 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
-                        self.success.append(_elem19)
+                    (_etype24, _size21) = iprot.readListBegin()
+                    for _i25 in range(_size21):
+                        _elem26 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem26)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -3282,16 +4311,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getSchemaNames_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRING, len(self.success))
-            for iter20 in self.success:
-                oprot.writeString(iter20.encode('utf-8') if sys.version_info[0] == 2 else iter20)
+            for iter27 in self.success:
+                oprot.writeString(iter27.encode('utf-8') if sys.version_info[0] == 2 else iter27)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -3318,26 +4347,195 @@
 getSchemaNames_result.thrift_spec = (
     (0, TType.LIST, 'success', (TType.STRING, 'UTF8', False), None, ),  # 0
     (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
     (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
 )
 
 
+class getSchemaNamesV2_args(object):
+    """
+    Attributes:
+     - sessionId
+     - catalogName
+
+    """
+
+
+    def __init__(self, sessionId=None, catalogName=None,):
+        self.sessionId = sessionId
+        self.catalogName = catalogName
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getSchemaNamesV2_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.catalogName is not None:
+            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
+            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getSchemaNamesV2_args)
+getSchemaNamesV2_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
+)
+
+
+class getSchemaNamesV2_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.LIST:
+                    self.success = []
+                    (_etype31, _size28) = iprot.readListBegin()
+                    for _i32 in range(_size28):
+                        _elem33 = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                        self.success.append(_elem33)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getSchemaNamesV2_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.LIST, 0)
+            oprot.writeListBegin(TType.STRING, len(self.success))
+            for iter34 in self.success:
+                oprot.writeString(iter34.encode('utf-8') if sys.version_info[0] == 2 else iter34)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getSchemaNamesV2_result)
+getSchemaNamesV2_result.thrift_spec = (
+    (0, TType.LIST, 'success', (TType.STRING, 'UTF8', False), None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
+
+
 class getColumns_args(object):
     """
     Attributes:
      - sessionId
+     - catalogName
      - schema
      - table
 
     """
 
 
-    def __init__(self, sessionId=None, schema=None, table=None,):
+    def __init__(self, sessionId=None, catalogName=None, schema=None, table=None,):
         self.sessionId = sessionId
+        self.catalogName = catalogName
         self.schema = schema
         self.table = table
 
     def read(self, iprot):
         if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
             iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
             return
@@ -3349,19 +4547,24 @@
             if fid == 1:
                 if ftype == TType.STRING:
                     self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 2:
                 if ftype == TType.STRING:
-                    self.schema = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             elif fid == 3:
                 if ftype == TType.STRING:
+                    self.schema = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRING:
                     self.table = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
                 else:
                     iprot.skip(ftype)
             else:
                 iprot.skip(ftype)
             iprot.readFieldEnd()
         iprot.readStructEnd()
@@ -3371,20 +4574,24 @@
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getColumns_args')
         if self.sessionId is not None:
             oprot.writeFieldBegin('sessionId', TType.STRING, 1)
             oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
             oprot.writeFieldEnd()
+        if self.catalogName is not None:
+            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
+            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
+            oprot.writeFieldEnd()
         if self.schema is not None:
-            oprot.writeFieldBegin('schema', TType.STRING, 2)
+            oprot.writeFieldBegin('schema', TType.STRING, 3)
             oprot.writeString(self.schema.encode('utf-8') if sys.version_info[0] == 2 else self.schema)
             oprot.writeFieldEnd()
         if self.table is not None:
-            oprot.writeFieldBegin('table', TType.STRING, 3)
+            oprot.writeFieldBegin('table', TType.STRING, 4)
             oprot.writeString(self.table.encode('utf-8') if sys.version_info[0] == 2 else self.table)
             oprot.writeFieldEnd()
         oprot.writeFieldStop()
         oprot.writeStructEnd()
 
     def validate(self):
         return
@@ -3399,16 +4606,17 @@
 
     def __ne__(self, other):
         return not (self == other)
 all_structs.append(getColumns_args)
 getColumns_args.thrift_spec = (
     None,  # 0
     (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
-    (2, TType.STRING, 'schema', 'UTF8', None, ),  # 2
-    (3, TType.STRING, 'table', 'UTF8', None, ),  # 3
+    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'schema', 'UTF8', None, ),  # 3
+    (4, TType.STRING, 'table', 'UTF8', None, ),  # 4
 )
 
 
 class getColumns_result(object):
     """
     Attributes:
      - success
@@ -3431,19 +4639,19 @@
         while True:
             (fname, ftype, fid) = iprot.readFieldBegin()
             if ftype == TType.STOP:
                 break
             if fid == 0:
                 if ftype == TType.LIST:
                     self.success = []
-                    (_etype24, _size21) = iprot.readListBegin()
-                    for _i25 in range(_size21):
-                        _elem26 = TFieldInfo()
-                        _elem26.read(iprot)
-                        self.success.append(_elem26)
+                    (_etype38, _size35) = iprot.readListBegin()
+                    for _i39 in range(_size35):
+                        _elem40 = TFieldInfo()
+                        _elem40.read(iprot)
+                        self.success.append(_elem40)
                     iprot.readListEnd()
                 else:
                     iprot.skip(ftype)
             elif fid == 1:
                 if ftype == TType.STRUCT:
                     self.error1 = QueryProcessingException.read(iprot)
                 else:
@@ -3462,16 +4670,16 @@
         if oprot._fast_encode is not None and self.thrift_spec is not None:
             oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
             return
         oprot.writeStructBegin('getColumns_result')
         if self.success is not None:
             oprot.writeFieldBegin('success', TType.LIST, 0)
             oprot.writeListBegin(TType.STRUCT, len(self.success))
-            for iter27 in self.success:
-                iter27.write(oprot)
+            for iter41 in self.success:
+                iter41.write(oprot)
             oprot.writeListEnd()
             oprot.writeFieldEnd()
         if self.error1 is not None:
             oprot.writeFieldBegin('error1', TType.STRUCT, 1)
             self.error1.write(oprot)
             oprot.writeFieldEnd()
         if self.error2 is not None:
@@ -3498,14 +4706,206 @@
 getColumns_result.thrift_spec = (
     (0, TType.LIST, 'success', (TType.STRUCT, [TFieldInfo, None], False), None, ),  # 0
     (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
     (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
 )
 
 
+class getColumnsV2_args(object):
+    """
+    Attributes:
+     - sessionId
+     - catalogName
+     - schema
+     - table
+
+    """
+
+
+    def __init__(self, sessionId=None, catalogName=None, schema=None, table=None,):
+        self.sessionId = sessionId
+        self.catalogName = catalogName
+        self.schema = schema
+        self.table = table
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.catalogName = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 3:
+                if ftype == TType.STRING:
+                    self.schema = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 4:
+                if ftype == TType.STRING:
+                    self.table = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getColumnsV2_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.catalogName is not None:
+            oprot.writeFieldBegin('catalogName', TType.STRING, 2)
+            oprot.writeString(self.catalogName.encode('utf-8') if sys.version_info[0] == 2 else self.catalogName)
+            oprot.writeFieldEnd()
+        if self.schema is not None:
+            oprot.writeFieldBegin('schema', TType.STRING, 3)
+            oprot.writeString(self.schema.encode('utf-8') if sys.version_info[0] == 2 else self.schema)
+            oprot.writeFieldEnd()
+        if self.table is not None:
+            oprot.writeFieldBegin('table', TType.STRING, 4)
+            oprot.writeString(self.table.encode('utf-8') if sys.version_info[0] == 2 else self.table)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getColumnsV2_args)
+getColumnsV2_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'catalogName', 'UTF8', None, ),  # 2
+    (3, TType.STRING, 'schema', 'UTF8', None, ),  # 3
+    (4, TType.STRING, 'table', 'UTF8', None, ),  # 4
+)
+
+
+class getColumnsV2_result(object):
+    """
+    Attributes:
+     - success
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, success=None, error1=None, error2=None,):
+        self.success = success
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 0:
+                if ftype == TType.LIST:
+                    self.success = []
+                    (_etype45, _size42) = iprot.readListBegin()
+                    for _i46 in range(_size42):
+                        _elem47 = TFieldInfo()
+                        _elem47.read(iprot)
+                        self.success.append(_elem47)
+                    iprot.readListEnd()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('getColumnsV2_result')
+        if self.success is not None:
+            oprot.writeFieldBegin('success', TType.LIST, 0)
+            oprot.writeListBegin(TType.STRUCT, len(self.success))
+            for iter48 in self.success:
+                iter48.write(oprot)
+            oprot.writeListEnd()
+            oprot.writeFieldEnd()
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(getColumnsV2_result)
+getColumnsV2_result.thrift_spec = (
+    (0, TType.LIST, 'success', (TType.STRUCT, [TFieldInfo, None], False), None, ),  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
+
+
 class updateUsers_args(object):
     """
     Attributes:
      - userInfo
 
     """
 
@@ -3768,9 +5168,157 @@
     def __ne__(self, other):
         return not (self == other)
 all_structs.append(setProps_result)
 setProps_result.thrift_spec = (
     None,  # 0
     (1, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 1
 )
+
+
+class addCatalogs_args(object):
+    """
+    Attributes:
+     - sessionId
+     - jsonString
+
+    """
+
+
+    def __init__(self, sessionId=None, jsonString=None,):
+        self.sessionId = sessionId
+        self.jsonString = jsonString
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRING:
+                    self.sessionId = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRING:
+                    self.jsonString = iprot.readString().decode('utf-8', errors='replace') if sys.version_info[0] == 2 else iprot.readString()
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('addCatalogs_args')
+        if self.sessionId is not None:
+            oprot.writeFieldBegin('sessionId', TType.STRING, 1)
+            oprot.writeString(self.sessionId.encode('utf-8') if sys.version_info[0] == 2 else self.sessionId)
+            oprot.writeFieldEnd()
+        if self.jsonString is not None:
+            oprot.writeFieldBegin('jsonString', TType.STRING, 2)
+            oprot.writeString(self.jsonString.encode('utf-8') if sys.version_info[0] == 2 else self.jsonString)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(addCatalogs_args)
+addCatalogs_args.thrift_spec = (
+    None,  # 0
+    (1, TType.STRING, 'sessionId', 'UTF8', None, ),  # 1
+    (2, TType.STRING, 'jsonString', 'UTF8', None, ),  # 2
+)
+
+
+class addCatalogs_result(object):
+    """
+    Attributes:
+     - error1
+     - error2
+
+    """
+
+
+    def __init__(self, error1=None, error2=None,):
+        self.error1 = error1
+        self.error2 = error2
+
+    def read(self, iprot):
+        if iprot._fast_decode is not None and isinstance(iprot.trans, TTransport.CReadableTransport) and self.thrift_spec is not None:
+            iprot._fast_decode(self, iprot, [self.__class__, self.thrift_spec])
+            return
+        iprot.readStructBegin()
+        while True:
+            (fname, ftype, fid) = iprot.readFieldBegin()
+            if ftype == TType.STOP:
+                break
+            if fid == 1:
+                if ftype == TType.STRUCT:
+                    self.error1 = QueryProcessingException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            elif fid == 2:
+                if ftype == TType.STRUCT:
+                    self.error2 = AccessDeniedException.read(iprot)
+                else:
+                    iprot.skip(ftype)
+            else:
+                iprot.skip(ftype)
+            iprot.readFieldEnd()
+        iprot.readStructEnd()
+
+    def write(self, oprot):
+        if oprot._fast_encode is not None and self.thrift_spec is not None:
+            oprot.trans.write(oprot._fast_encode(self, [self.__class__, self.thrift_spec]))
+            return
+        oprot.writeStructBegin('addCatalogs_result')
+        if self.error1 is not None:
+            oprot.writeFieldBegin('error1', TType.STRUCT, 1)
+            self.error1.write(oprot)
+            oprot.writeFieldEnd()
+        if self.error2 is not None:
+            oprot.writeFieldBegin('error2', TType.STRUCT, 2)
+            self.error2.write(oprot)
+            oprot.writeFieldEnd()
+        oprot.writeFieldStop()
+        oprot.writeStructEnd()
+
+    def validate(self):
+        return
+
+    def __repr__(self):
+        L = ['%s=%r' % (key, value)
+             for key, value in self.__dict__.items()]
+        return '%s(%s)' % (self.__class__.__name__, ', '.join(L))
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
+
+    def __ne__(self, other):
+        return not (self == other)
+all_structs.append(addCatalogs_result)
+addCatalogs_result.thrift_spec = (
+    None,  # 0
+    (1, TType.STRUCT, 'error1', [QueryProcessingException, None], None, ),  # 1
+    (2, TType.STRUCT, 'error2', [AccessDeniedException, None], None, ),  # 2
+)
 fix_spec(all_structs)
 del all_structs
```

### Comparing `e6data-python-connector-1.0.4/e6xdb/server/ttypes.py` & `e6data-python-connector-1.0.5/e6xdb/server/ttypes.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/sqlalchemy_e6x.py` & `e6data-python-connector-1.0.5/e6xdb/sqlalchemy_e6x.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/e6xdb/typeId.py` & `e6data-python-connector-1.0.5/e6xdb/typeId.py`

 * *Files identical despite different names*

### Comparing `e6data-python-connector-1.0.4/setup.py` & `e6data-python-connector-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import os
 
 import setuptools
 
 envstring = lambda var: os.environ.get(var) or ""
 
-VERSION = [1, 0, 4]
+VERSION = [1, 0, 5]
 
 
 def get_long_desc():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     return long_description
```

