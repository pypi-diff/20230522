# Comparing `tmp/dbt-singlestore-1.1.2.tar.gz` & `tmp/dbt-singlestore-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbt-singlestore-1.1.2.tar", last modified: Wed Jun 22 19:59:56 2022, max compression
+gzip compressed data, was "dist/dbt-singlestore-1.2.2.tar", last modified: Mon May 22 19:02:54 2023, max compression
```

## Comparing `dbt-singlestore-1.1.2.tar` & `dbt-singlestore-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)    11356 2022-01-12 14:48:12.000000 dbt-singlestore-1.1.2/LICENSE
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       46 2021-12-14 12:24:22.000000 dbt-singlestore-1.1.2/MANIFEST.in
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      332 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/PKG-INFO
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     3159 2022-06-22 19:54:04.000000 dbt-singlestore-1.1.2/README.md
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/adapters/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      433 2022-01-12 13:59:39.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/__init__.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       18 2022-06-22 19:54:13.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/__version__.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      751 2022-01-24 13:04:48.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/column.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     3480 2022-06-22 14:31:34.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/connections.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     5770 2022-06-22 14:31:34.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/impl.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      952 2022-01-25 11:30:29.000000 dbt-singlestore-1.1.2/dbt/adapters/singlestore/relation.py
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/include/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       51 2021-12-14 12:24:22.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/__init__.py
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       79 2021-12-14 12:24:22.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/dbt_project.yml
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     1555 2022-01-25 11:30:29.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/catalog.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      806 2022-06-22 14:31:34.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/columns.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     9297 2022-06-22 19:08:32.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/common.sql
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     4394 2022-01-26 15:42:32.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     4084 2022-06-22 14:31:34.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      917 2021-12-16 10:56:23.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      225 2021-12-21 15:47:49.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      482 2022-01-25 16:24:27.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/profile_template.yml
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      420 2022-01-25 16:25:45.000000 dbt-singlestore-1.1.2/dbt/include/singlestore/sample_profiles.yml
-drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt_singlestore.egg-info/
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      332 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt_singlestore.egg-info/PKG-INFO
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     1034 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt_singlestore.egg-info/SOURCES.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        1 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt_singlestore.egg-info/dependency_links.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       55 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt_singlestore.egg-info/requires.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        4 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/dbt_singlestore.egg-info/top_level.txt
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       38 2022-06-22 19:59:56.000000 dbt-singlestore-1.1.2/setup.cfg
--rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      765 2022-06-22 19:54:09.000000 dbt-singlestore-1.1.2/setup.py
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)    11356 2022-01-12 14:48:12.000000 dbt-singlestore-1.2.2/LICENSE
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       46 2021-12-14 12:24:22.000000 dbt-singlestore-1.2.2/MANIFEST.in
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      332 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/PKG-INFO
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     3273 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/README.md
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/adapters/
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      433 2022-01-12 13:59:39.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/__init__.py
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       18 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/__version__.py
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      751 2022-01-24 13:04:48.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/column.py
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     2993 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/connections.py
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     6075 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/impl.py
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      952 2022-01-25 11:30:29.000000 dbt-singlestore-1.2.2/dbt/adapters/singlestore/relation.py
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       51 2021-12-14 12:24:22.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/__init__.py
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       79 2021-12-14 12:24:22.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/dbt_project.yml
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     1554 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/catalog.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      806 2022-06-22 14:31:34.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/columns.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     9113 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/common.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      606 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/grants.sql
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     4394 2022-01-26 15:42:32.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     4373 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      916 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      224 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       90 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/bool_or.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      135 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      203 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/dateadd.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      193 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/datediff.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      122 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/hash.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      624 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/listagg.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       94 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/safe_cast.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      389 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/macros/utils/split_part.sql
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      482 2022-01-25 16:24:27.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/profile_template.yml
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      420 2022-01-25 16:25:45.000000 dbt-singlestore-1.2.2/dbt/include/singlestore/sample_profiles.yml
+drwxr-xr-x   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        0 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      332 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/PKG-INFO
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)     1481 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/SOURCES.txt
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        1 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/dependency_links.txt
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       55 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/requires.txt
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)        4 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/dbt_singlestore.egg-info/top_level.txt
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)       38 2023-05-22 19:02:54.000000 dbt-singlestore-1.2.2/setup.cfg
+-rw-r--r--   0 pmishchenko-ua (185476184) pmishchenko-ua (185476184)      765 2023-05-22 18:49:56.000000 dbt-singlestore-1.2.2/setup.py
```

### Comparing `dbt-singlestore-1.1.2/LICENSE` & `dbt-singlestore-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.1.2/README.md` & `dbt-singlestore-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,19 @@
 Administration    | Hooks             | Yes        | Yes
 Models            | Custom schema     | Limited*   | Yes
 
 * Custom schemas can be defined in a project models, but they can only serve as a modification to the prefix of the corresponding table names.  
 
 ## Testing and supported versions
 
-Default dbt [test suite](test/singlestore.dbtspec) is used to check the adapter functionality. [Development](Development.md) overview has a section "Run tests" which contains instructions on running the tests. Currently, the tests have been successfully run for the following product versions:
+Default dbt [test suite](tests/test_basic.py) is used to check the adapter functionality. [Development](Development.md) overview has a section "Run tests" which contains instructions on running the tests. Currently, the tests have been successfully run for the following product versions:
+
+Singlestore | dbt-core | dbt-tests-adapter
+------------|----------|-------------------
+7.8.29      | 1.2.2    | 1.2.2
 
 Singlestore | dbt-core | pytest-dbt-adapter
 ------------|----------|-------------------
 7.8.3       | 1.1.1    | 0.6.0
 7.6.6       | 1.0.1    | 0.6.0
 7.5.12      | 1.0.1    | 0.6.0
```

### Comparing `dbt-singlestore-1.1.2/dbt/adapters/singlestore/column.py` & `dbt-singlestore-1.2.2/dbt/adapters/singlestore/column.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.1.2/dbt/adapters/singlestore/connections.py` & `dbt-singlestore-1.2.2/dbt/adapters/singlestore/connections.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     # Add credentials members here, like:
     host: str = 'localhost'
     port: int = 3306
     user: str = 'root'
     password: str = ''
     database: str
     schema: str
+    retries: int = 1
 
     ALIASES = {
         'db': 'database',
         'username': 'user'
     }
 
     @property
@@ -53,43 +54,36 @@
     def open(cls, connection):
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         credentials = cls.get_credentials(connection.credentials)
 
-        try:
-            handle = pymysql.connect(
+        def connect():
+            return pymysql.connect(
                 user=credentials.user,
                 password=credentials.password,
                 host=credentials.host,
                 port=credentials.port,
                 database=credentials.database,
                 client_flag=pymysql.constants.CLIENT.MULTI_STATEMENTS
             )
 
-            connection.handle = handle
-            connection.state = "open"
-        except pymysql.Error as e:
-            logger.debug(
-                "Got an error when attempting to open a "
-                "connection: '{}'".format(e)
-            )
-
-            connection.handle = None
-            connection.state = "fail"
-            err_msg = str(e)
-            err_msg += "\nFailed to connect to Singlestore server with the credentials specified in profile:" + \
-                f"\n  host={credentials.host}, port={credentials.port}, " + \
-                f"database={credentials.database}, user={credentials.user}, password=****." + \
-                "\nPlease check that your dbt profile contains valid credentials and SingleStore server is running"
-
-            raise dbt.exceptions.FailedToConnectException(err_msg)
-
-        return connection
+        retryable_exceptions = [
+            pymysql.OperationalError,
+            pymysql.DatabaseError
+        ]
+
+        return cls.retry_connection(
+            connection,
+            connect=connect,
+            logger=logger,
+            retry_limit=credentials.retries,
+            retryable_exceptions=retryable_exceptions,
+        )
 
     @classmethod
     def get_response(cls, cursor: Cursor) -> AdapterResponse:
         return AdapterResponse(
             _message="{}".format(f"OK. Rows affected: {cursor.rowcount}"),
             rows_affected=cursor.rowcount,
             code=DUMMY_RESPONSE_CODE
```

### Comparing `dbt-singlestore-1.1.2/dbt/adapters/singlestore/impl.py` & `dbt-singlestore-1.2.2/dbt/adapters/singlestore/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         # We append the current timestamp to the index name because otherwise
         # the index will only be created on every other run. See
         # https://github.com/dbt-labs/dbt-core/issues/1945#issuecomment-576714925
         # for an explanation.
         now = datetime.utcnow().isoformat()
         inputs = self.columns + [relation.render(), str(self.unique), str(self.type), now]
         string = "_".join(inputs)
-        return dbt.utils.md5(string)
+        return "index_" + dbt.utils.md5(string)
 
     @classmethod
     def parse(cls, raw_index) -> Optional["SingleStoreIndexConfig"]:
         if raw_index is None:
             return None
         try:
             cls.validate(raw_index)
@@ -90,14 +90,19 @@
             table_owner=None,
             table_stats=None,
             column=column.column,
             column_index=idx,
             dtype=column.dtype,
         ) for idx, column in enumerate(raw_rows)]
 
+    def drop_schema(self, relation: SingleStoreRelation) -> None:
+        # in SingleStore, schema does not have a physical representation in the database
+        # so we don't execute DROP SCHEMA macro, only update the cache
+        self.cache.drop_schema(relation.database, relation.schema)
+
     def list_relations_without_caching(
         self, schema_relation: SingleStoreRelation
     ) -> List[SingleStoreRelation]:
         kwargs = {'schema_relation': schema_relation}
         try:
             results = self.execute_macro(
                 'list_relations_without_caching',
```

### Comparing `dbt-singlestore-1.1.2/dbt/adapters/singlestore/relation.py` & `dbt-singlestore-1.2.2/dbt/adapters/singlestore/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.1.2/dbt/include/singlestore/macros/catalog.sql` & `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/catalog.sql`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 {% macro singlestore__get_catalog(information_schema, schemas) -%}
     {% set database = information_schema.database %}
     {%- call statement('catalog', fetch_result=True) -%}
     select
         columns.table_database,
         columns.table_schema,
         columns.table_name,
```

### Comparing `dbt-singlestore-1.1.2/dbt/include/singlestore/macros/columns.sql` & `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.1.2/dbt/include/singlestore/macros/common.sql` & `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/common.sql`

 * *Files 2% similar despite different names*

```diff
@@ -135,21 +135,14 @@
         from information_schema.tables
         where table_schema = '{{ database }}'
     {% endcall %}
     {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 
-{% macro singlestore__drop_schema(relation) -%}
-    {%- call statement('drop_database') -%}
-        drop database if exists {{ relation.database }}
-    {% endcall %}
-{% endmacro %}
-
-
 {% macro singlestore__drop_relation(relation) -%}
     {% call statement('drop_relation', auto_begin=False) -%}
         drop {{ relation.type }} if exists {{ relation.include(database=True) }}
     {%- endcall %}
 {% endmacro %}
 
 
@@ -174,15 +167,15 @@
             {{ 'table' }}
         {% else -%}
             {%- do exceptions.raise_compiler_error('Unknown relation type for {}'.format(relation.identifier)) -%}
         {% endif -%}
     {% else -%}
         {{ '' }}
     {% endif -%}
-{% endmacro -%}}
+{% endmacro -%}
 
 
 {% macro singlestore__rename_relation(from_relation, to_relation) -%}
     {#
       2-step process is needed:
       1. Drop the existing to_relation
       2. Rename from_relation to to_relation
```

### Comparing `dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql` & `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql` & `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-
 {% materialization snapshot, adapter='singlestore' %}
   {%- set config = model['config'] -%}
 
   {%- set target_table = model.get('alias', model.get('name')) -%}
 
   {%- set strategy_name = config.get('strategy') -%}
   {%- set unique_key = config.get('unique_key') %}
+  -- grab current tables grants config for comparision later on
+  {%- set grant_config = config.get('grants') -%}
 
   {% call statement('create_database') %}
      create database if not exists {{ model.database }}
   {% endcall %}
 
   {% set target_relation_exists, target_relation = get_or_create_relation(
           database=model.database,
@@ -88,14 +89,17 @@
 
       {% call statement('main') %}
           {{ final_sql_insert }}
       {% endcall %}
 
   {% endif %}
 
+  {% set should_revoke = should_revoke(target_relation_exists, full_refresh_mode=False) %}
+  {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
+
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
   {{ adapter.commit() }}
 
   {% if staging_table is defined %}
```

### Comparing `dbt-singlestore-1.1.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-singlestore-1.2.2/dbt/include/singlestore/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 {% macro singlestore__snapshot_merge_sql_update(target, source, insert_cols) -%}
     update {{ target }}, (select dbt_scd_id, dbt_change_type, dbt_valid_to from {{ source }}) as dbt_internal_source
        set {{ target }}.dbt_valid_to = dbt_internal_source.dbt_valid_to
      where dbt_internal_source.dbt_scd_id = {{ target }}.dbt_scd_id
        and dbt_internal_source.dbt_change_type = 'update'
        and {{ target }}.dbt_valid_to is null
 {% endmacro %}
```

### Comparing `dbt-singlestore-1.1.2/setup.py` & `dbt-singlestore-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_namespace_packages, setup
 
 package_name = "dbt-singlestore"
 # make sure this always matches dbt/adapters/singlestore/__version__.py
-package_version = "1.1.2"
+package_version = "1.2.2"
 description = """The singlestore adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=description,
```

