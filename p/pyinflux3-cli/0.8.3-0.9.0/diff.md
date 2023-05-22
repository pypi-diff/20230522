# Comparing `tmp/pyinflux3-cli-0.8.3.tar.gz` & `tmp/pyinflux3-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinflux3-cli-0.8.3.tar", last modified: Wed May  3 14:06:58 2023, max compression
+gzip compressed data, was "pyinflux3-cli-0.9.0.tar", last modified: Mon May 22 12:56:39 2023, max compression
```

## Comparing `pyinflux3-cli-0.8.3.tar` & `pyinflux3-cli-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/influxdb_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/influxdb_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7626 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/influxdb_cli/influx3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 14:06:58.000000 pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-03 14:06:52.000000 pyinflux3-cli-0.8.3/setup-cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:06:58.796858 pyinflux3-cli-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/influxdb_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/influxdb_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7638 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/influxdb_cli/influx3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-22 12:56:39.000000 pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-22 12:56:32.000000 pyinflux3-cli-0.9.0/setup-cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:56:39.098388 pyinflux3-cli-0.9.0/setup.cfg
```

### Comparing `pyinflux3-cli-0.8.3/PKG-INFO` & `pyinflux3-cli-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.8.3
+Version: 0.9.0
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,87 +21,133 @@
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
 # Install
 To install only the client:
+
 ```bash
 python3 -m pip install pyinflux3
 ```
+
 To install the client and CLI:
+
 ```bash
 sudo python3 -m pip install "pyinflux3[cli]"
 ```
+
 ***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
 
 # Add a Config
-You can drop a config file called config.json in the directory where you are running the influx3 command:
+
+To configure `pyinflux3` and the CLI, do one of the following:
+
+You can drop a config file called `config.json` in the directory where you are running the `influx3` command:
 
 ```json
 {
-{
     "my-config": {
         "database": "your-database",
         "host": "your-host",
         "token": "your-token",
         "org": "your-org-id",
         "active": true
     }
 }
-}
 ```
 
-Or you can use the config command to create or modify a config:
-```
-% influx3 config --name="my-config" --database="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
-```
 
-If you are running against InfluxDB Cloud Serverless, then use the bucket name for the database in you configuration.
+- Use the `config` command to create or modify a config:
+
+    ```
+    influx3 config \
+    --name="my-config" \
+    --database="<database or bucket name>" \
+    --host="us-east-1-1.aws.cloud2.influxdata.com" \
+    --token="<your token>" \
+    --org="<your org ID>"
+    ```
+
+If you are running against InfluxDB Cloud Serverless, then use the _bucket name_ as the database in your configuration.
 
 # Run as a Command
+
 ```
-% influx3 sql "select * from anomalies"
+influx3 sql "select * from anomalies"
 ```
 
 ```
-% influx3 write testmes f=7 
+influx3 write testmes f=7 
 ```
 
 # Query and Write Interactively
 
+In your terminal, enter the following command:
+
+```
+influx3
+```
+
+`influx3` displays the `(>)` interactive prompt and waits for input.
 
 ```
-% influx3
 Welcome to my IOx CLI.
 
+(>)
+```
+
+To query, type `sql` at the prompt.
+
+```
 (>) sql
-(sql >) select * from anomalies
-    check    id  observed                          time     type user_id  value
-0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
-1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
 ```
 
+At the `(sql >)` prompt, enter your query statement:
+
+```
+(sql >) select * from home
+```
+
+The `influx3` CLI displays query results in Markdown table format--for example:
+
+```
+|     |   co |   hum | room        |   temp | time                          |
+|----:|-----:|------:|:------------|-------:|:------------------------------|
+|   0 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:00           |
+|   1 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:50           |
+```
+
+To write, type `write` at the `(>)` prompt.
+
+```
+(>) write
+```
+
+At the `(write >)` prompt, enter line protocol data.
+
 ```
 (>) write 
-testmes f=5 boring-observability
+home,room=kitchen temp=70.5,hum=80
 ```
 
+To exit a prompt, enter `exit`.
+
 # Write from a File
+
 Both the InfluxDB CLI and Client libary support writing from a CSV file. The CSV file must have a header row with the column names. The there must be a column containing a timestamp. Here are the parse options:
 * `--file` - The path to the csv file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurment` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
+* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
 * `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
-
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
 # Contribution
 If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
 ```bash
 python3 -m venv .venv
```

### Comparing `pyinflux3-cli-0.8.3/influxdb_cli/influx3.py` & `pyinflux3-cli-0.9.0/influxdb_cli/influx3.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self._write_prompt_session = PromptSession(lexer=None)
 
     def do_sql(self, arg):
         if self._configurations == {}:
             print("can't query, no active configs")
             return
         try: 
-            reader = self.influxdb_client.query(sql_query=arg)
+            reader = self.influxdb_client.query(query=arg, language="sql")
             table = reader.read_all()
             print(table.to_pandas().to_markdown())
         except Exception as e:
             print(e)
 
     def do_write(self, arg):
         if self._configurations == {}:
```

### Comparing `pyinflux3-cli-0.8.3/pyinflux3_cli.egg-info/PKG-INFO` & `pyinflux3-cli-0.9.0/pyinflux3_cli.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinflux3-cli
-Version: 0.8.3
+Version: 0.9.0
 Summary: Community Python client for InfluxDB IOx (CLI)
 Home-page: https://github.com/InfluxCommunity/pyinflux3
 Author: InfluxData
 Author-email: contact@influxdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,87 +21,133 @@
 
 When installed, you have access to 2 pieces of functionality:
 1. A CLI for reading and writing data to InfluxDB with IOx.
 2. A client library for reading and writing data to InfluxDB with IOx.
 
 # Install
 To install only the client:
+
 ```bash
 python3 -m pip install pyinflux3
 ```
+
 To install the client and CLI:
+
 ```bash
 sudo python3 -m pip install "pyinflux3[cli]"
 ```
+
 ***Note: Use sudo if you would like to directly install the client onto your path. Otherwise use the `--user` flag.**
 
 # Add a Config
-You can drop a config file called config.json in the directory where you are running the influx3 command:
+
+To configure `pyinflux3` and the CLI, do one of the following:
+
+You can drop a config file called `config.json` in the directory where you are running the `influx3` command:
 
 ```json
 {
-{
     "my-config": {
         "database": "your-database",
         "host": "your-host",
         "token": "your-token",
         "org": "your-org-id",
         "active": true
     }
 }
-}
 ```
 
-Or you can use the config command to create or modify a config:
-```
-% influx3 config --name="my-config" --database="<database or bucket name>" --host="us-east-1-1.aws.cloud2.influxdata.com" --token="<your token>" --org="<your org ID>"
-```
 
-If you are running against InfluxDB Cloud Serverless, then use the bucket name for the database in you configuration.
+- Use the `config` command to create or modify a config:
+
+    ```
+    influx3 config \
+    --name="my-config" \
+    --database="<database or bucket name>" \
+    --host="us-east-1-1.aws.cloud2.influxdata.com" \
+    --token="<your token>" \
+    --org="<your org ID>"
+    ```
+
+If you are running against InfluxDB Cloud Serverless, then use the _bucket name_ as the database in your configuration.
 
 # Run as a Command
+
 ```
-% influx3 sql "select * from anomalies"
+influx3 sql "select * from anomalies"
 ```
 
 ```
-% influx3 write testmes f=7 
+influx3 write testmes f=7 
 ```
 
 # Query and Write Interactively
 
+In your terminal, enter the following command:
+
+```
+influx3
+```
+
+`influx3` displays the `(>)` interactive prompt and waits for input.
 
 ```
-% influx3
 Welcome to my IOx CLI.
 
+(>)
+```
+
+To query, type `sql` at the prompt.
+
+```
 (>) sql
-(sql >) select * from anomalies
-    check    id  observed                          time     type user_id  value
-0       1  None       NaN 2023-02-03 20:56:57.513279776    error       1  400.0
-1       1  None       NaN 2023-02-03 17:52:54.328785835  latency       1  900.0
 ```
 
+At the `(sql >)` prompt, enter your query statement:
+
+```
+(sql >) select * from home
+```
+
+The `influx3` CLI displays query results in Markdown table format--for example:
+
+```
+|     |   co |   hum | room        |   temp | time                          |
+|----:|-----:|------:|:------------|-------:|:------------------------------|
+|   0 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:00           |
+|   1 |    0 |  35.9 | Kitchen     |   21   | 2023-03-09 08:00:50           |
+```
+
+To write, type `write` at the `(>)` prompt.
+
+```
+(>) write
+```
+
+At the `(write >)` prompt, enter line protocol data.
+
 ```
 (>) write 
-testmes f=5 boring-observability
+home,room=kitchen temp=70.5,hum=80
 ```
 
+To exit a prompt, enter `exit`.
+
 # Write from a File
+
 Both the InfluxDB CLI and Client libary support writing from a CSV file. The CSV file must have a header row with the column names. The there must be a column containing a timestamp. Here are the parse options:
 * `--file` - The path to the csv file.
 * `--time` - The name of the column containing the timestamp.
-* `--measurment` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
+* `--measurement` - The name of the measurment to store the CSV data under. (Currently only supports user specified string)
 * `--tags` - (optional) Specify an array of column names to use as tags. (Currently only supports user specified strings) for example: `--tags=host,region`
 
 ```bash
 influx3 write_csv --file ./Examples/example.csv --measurement table2 --time Date --tags host,region
 ```
 
-
 # Client library
 This project also includes a new client library that strives for utter simplicity. It includes 3 functions, a constuctor, write(), and read().
 
 # Contribution
 If you are working on a new feature for either the CLI or the Client Libary please make sure you test both for breaking changes. This can currently be achived using the following method:
 ```bash
 python3 -m venv .venv
```

### Comparing `pyinflux3-cli-0.8.3/setup-cli.py` & `pyinflux3-cli-0.9.0/setup-cli.py`

 * *Files identical despite different names*

