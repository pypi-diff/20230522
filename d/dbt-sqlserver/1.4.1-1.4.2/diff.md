# Comparing `tmp/dbt-sqlserver-1.4.1.tar.gz` & `tmp/dbt-sqlserver-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-sqlserver-1.4.1.tar", last modified: Mon May 22 07:58:14 2023, max compression
+gzip compressed data, was "dbt-sqlserver-1.4.2.tar", last modified: Mon May 22 20:32:32 2023, max compression
```

## Comparing `dbt-sqlserver-1.4.1.tar` & `dbt-sqlserver-1.4.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.312620 dbt-sqlserver-1.4.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.312620 dbt-sqlserver-1.4.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.316620 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 20:32:32.000000 dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:32:32.320621 dbt-sqlserver-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-22 20:31:55.000000 dbt-sqlserver-1.4.2/setup.py
```

### Comparing `dbt-sqlserver-1.4.1/LICENSE` & `dbt-sqlserver-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/PKG-INFO` & `dbt-sqlserver-1.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
+Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile
+Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/mssql-configs
+Project-URL: Changelog, https://github.com/dbt-msft/dbt-sqlserver/blob/master/CHANGELOG.md
+Project-URL: Issue Tracker, https://github.com/dbt-msft/dbt-sqlserver/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbt-sqlserver-1.4.1/README.md` & `dbt-sqlserver-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/__init__.py` & `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_adapter.py` & `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_column.py` & `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_column.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_connection_manager.py` & `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_credentials.py` & `dbt-sqlserver-1.4.2/dbt/adapters/sqlserver/sql_server_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/apply_grants.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/apply_grants.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% macro sqlserver__get_show_grant_sql(relation) %}
     select
         GRANTEE as grantee,
         PRIVILEGE_TYPE as privilege_type
-    from INFORMATION_SCHEMA.TABLE_PRIVILEGES with (nolock)
+    from INFORMATION_SCHEMA.TABLE_PRIVILEGES {{ information_schema_hints() }}
     where TABLE_CATALOG = '{{ relation.database }}'
       and TABLE_SCHEMA = '{{ relation.schema }}'
       and TABLE_NAME = '{{ relation.identifier }}'
 {% endmacro %}
 
 
 {%- macro sqlserver__get_grant_sql(relation, privilege, grantees) -%}
```

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/columns.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/columns.sql`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
         select
             row_number() over (partition by object_name(c.object_id) order by c.column_id) as ordinal_position,
             c.name collate database_default as column_name,
             t.name as data_type,
             c.max_length as character_maximum_length,
             c.precision as numeric_precision,
             c.scale as numeric_scale
-        from [{{ 'tempdb' if '#' in relation.identifier else relation.database }}].sys.columns c with (nolock)
-        inner join sys.types t with (nolock)
+        from [{{ 'tempdb' if '#' in relation.identifier else relation.database }}].sys.columns c {{ information_schema_hints() }}
+        inner join sys.types t {{ information_schema_hints() }}
         on c.user_type_id = t.user_type_id
         where c.object_id = object_id('{{ 'tempdb..' ~ relation.include(database=false, schema=false) if '#' in relation.identifier else relation }}')
     )
 
     select
         column_name,
         data_type,
```

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/indexes.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/indexes.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% macro sqlserver__create_clustered_columnstore_index(relation) -%}
   {%- set cci_name = (relation.schema ~ '_' ~ relation.identifier ~ '_cci') | replace(".", "") | replace(" ", "") -%}
   {%- set relation_name = relation.schema ~ '_' ~ relation.identifier -%}
   {%- set full_relation = '"' ~ relation.schema ~ '"."' ~ relation.identifier ~ '"' -%}
   use [{{ relation.database }}];
   if EXISTS (
         SELECT *
-        FROM sys.indexes with (nolock)
+        FROM sys.indexes {{ information_schema_hints() }}
         WHERE name = '{{cci_name}}'
         AND object_id=object_id('{{relation_name}}')
     )
   DROP index {{full_relation}}.{{cci_name}}
   CREATE CLUSTERED COLUMNSTORE INDEX {{cci_name}}
     ON {{full_relation}}
 {% endmacro %}
@@ -29,16 +29,16 @@
 
 
 {{ log("Running drop_xml_indexes() macro...") }}
 
 declare @drop_xml_indexes nvarchar(max);
 select @drop_xml_indexes = (
     select 'IF INDEXPROPERTY(' + CONVERT(VARCHAR(MAX), sys.tables.[object_id]) + ', ''' + sys.indexes.[name] + ''', ''IndexId'') IS NOT NULL DROP INDEX [' + sys.indexes.[name] + '] ON ' + '[' + SCHEMA_NAME(sys.tables.[schema_id]) + '].[' + OBJECT_NAME(sys.tables.[object_id]) + ']; '
-	from sys.indexes with (nolock)
-    inner join sys.tables with (nolock)
+	from sys.indexes {{ information_schema_hints() }}
+    inner join sys.tables {{ information_schema_hints() }}
     on sys.indexes.object_id = sys.tables.object_id
     where sys.indexes.[name] is not null
       and sys.indexes.type_desc = 'XML'
       and sys.tables.[name] = '{{ this.table }}'
     for xml path('')
 ); exec sp_executesql @drop_xml_indexes;
 
@@ -50,16 +50,16 @@
 {# and https://stackoverflow.com/a/33785833/10415173         #}
 
 {{ log("Running drop_spatial_indexes() macro...") }}
 
 declare @drop_spatial_indexes nvarchar(max);
 select @drop_spatial_indexes = (
     select 'IF INDEXPROPERTY(' + CONVERT(VARCHAR(MAX), sys.tables.[object_id]) + ', ''' + sys.indexes.[name] + ''', ''IndexId'') IS NOT NULL DROP INDEX [' + sys.indexes.[name] + '] ON ' + '[' + SCHEMA_NAME(sys.tables.[schema_id]) + '].[' + OBJECT_NAME(sys.tables.[object_id]) + ']; '
-    from sys.indexes with (nolock)
-    inner join sys.tables with (nolock)
+    from sys.indexes {{ information_schema_hints() }}
+    inner join sys.tables {{ information_schema_hints() }}
     on sys.indexes.object_id = sys.tables.object_id
     where sys.indexes.[name] is not null
       and sys.indexes.type_desc = 'Spatial'
       and sys.tables.[name] = '{{ this.table }}'
     for xml path('')
 ); exec sp_executesql @drop_spatial_indexes;
 
@@ -115,16 +115,16 @@
 {{ drop_pk_constraints() }}
 
 {{ log("Dropping remaining indexes...") }}
 
 declare @drop_remaining_indexes_last nvarchar(max);
 select @drop_remaining_indexes_last = (
     select 'IF INDEXPROPERTY(' + CONVERT(VARCHAR(MAX), sys.tables.[object_id]) + ', ''' + sys.indexes.[name] + ''', ''IndexId'') IS NOT NULL DROP INDEX [' + sys.indexes.[name] + '] ON ' + '[' + SCHEMA_NAME(sys.tables.[schema_id]) + '].[' + OBJECT_NAME(sys.tables.[object_id]) + ']; '
-    from sys.indexes with (nolock)
-    inner join sys.tables with (nolock)
+    from sys.indexes {{ information_schema_hints() }}
+    inner join sys.tables {{ information_schema_hints() }}
     on sys.indexes.object_id = sys.tables.object_id
     where sys.indexes.[name] is not null
       and sys.tables.[name] = '{{ this.table }}'
     for xml path('')
 ); exec sp_executesql @drop_remaining_indexes_last;
 
 {%- endmacro %}
@@ -133,15 +133,15 @@
 {% macro create_clustered_index(columns, unique=False) -%}
 
 {{ log("Creating clustered index...") }}
 
 {% set idx_name = "clustered_" + local_md5(columns | join("_")) %}
 
 if not exists(select *
-                from sys.indexes with (nolock)
+                from sys.indexes {{ information_schema_hints() }}
                 where name = '{{ idx_name }}'
                 and object_id = OBJECT_ID('{{ this }}')
 )
 begin
 
 create
 {% if unique -%}
@@ -166,15 +166,15 @@
         + local_md5(includes | join("_"))
     ) %}
 {% else -%}
     {% set idx_name = "nonclustered_" + local_md5(columns | join("_")) %}
 {% endif %}
 
 if not exists(select *
-                from sys.indexes with (nolock)
+                from sys.indexes {{ information_schema_hints() }}
                 where name = '{{ idx_name }}'
                 and object_id = OBJECT_ID('{{ this }}')
 )
 begin
 create nonclustered index
     {{ idx_name }}
       on {{ this }} ({{ '[' + columns|join("], [") + ']' }})
```

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/metadata.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/metadata.sql`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,44 @@
+{% macro information_schema_hints() %}
+    {{ return(adapter.dispatch('information_schema_hints')()) }}
+{% endmacro %}
+
+{% macro default__information_schema_hints() %}{% endmacro %}
+{% macro sqlserver__information_schema_hints() %}with (nolock){% endmacro %}
 
 {% macro sqlserver__get_catalog(information_schemas, schemas) -%}
 
   {%- call statement('catalog', fetch_result=True) -%}
 
     with
     principals as (
         select
             name as principal_name,
             principal_id as principal_id
         from
-            sys.database_principals with (nolock)
+            sys.database_principals {{ information_schema_hints() }}
     ),
 
     schemas as (
         select
             name as schema_name,
             schema_id as schema_id,
             principal_id as principal_id
         from
-            sys.schemas with (nolock)
+            sys.schemas {{ information_schema_hints() }}
     ),
 
     tables as (
         select
             name as table_name,
             schema_id as schema_id,
             principal_id as principal_id,
             'BASE TABLE' as table_type
         from
-            sys.tables with (nolock)
+            sys.tables {{ information_schema_hints() }}
     ),
 
     tables_with_metadata as (
         select
             table_name,
             schema_name,
             coalesce(tables.principal_id, schemas.principal_id) as owner_principal_id,
@@ -45,15 +51,15 @@
     views as (
         select
             name as table_name,
             schema_id as schema_id,
             principal_id as principal_id,
             'VIEW' as table_type
         from
-            sys.views with (nolock)
+            sys.views {{ information_schema_hints() }}
     ),
 
     views_with_metadata as (
         select
             table_name,
             schema_name,
             coalesce(views.principal_id, schemas.principal_id) as owner_principal_id,
@@ -88,15 +94,15 @@
         select
             table_catalog as table_database,
             table_schema,
             table_name,
             column_name,
             ordinal_position as column_index,
             data_type as column_type
-        from INFORMATION_SCHEMA.COLUMNS with (nolock)
+        from INFORMATION_SCHEMA.COLUMNS {{ information_schema_hints() }}
 
     )
 
     select
         cols.table_database,
         tv.schema_name as table_schema,
         tv.table_name,
@@ -125,15 +131,15 @@
   {%- endif -%}
 {%- endmacro %}
 
 {% macro sqlserver__list_schemas(database) %}
   {% call statement('list_schemas', fetch_result=True, auto_begin=False) -%}
     USE {{ database }};
     select  name as [schema]
-    from sys.schemas with (nolock)
+    from sys.schemas {{ information_schema_hints() }}
   {% endcall %}
   {{ return(load_result('list_schemas').table) }}
 {% endmacro %}
 
 {% macro sqlserver__check_schema_exists(information_schema, schema) -%}
   {% call statement('check_schema_exists', fetch_result=True, auto_begin=False) -%}
     --USE {{ database_name }}
@@ -149,12 +155,12 @@
       table_name as [name],
       table_schema as [schema],
       case when table_type = 'BASE TABLE' then 'table'
            when table_type = 'VIEW' then 'view'
            else table_type
       end as table_type
 
-    from [{{ schema_relation.database }}].INFORMATION_SCHEMA.TABLES with (nolock)
+    from [{{ schema_relation.database }}].INFORMATION_SCHEMA.TABLES {{ information_schema_hints() }}
     where table_schema = '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
```

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/relation.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/relation.sql`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,12 @@
 
 {% macro sqlserver__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
     USE [{{ to_relation.database }}];
     EXEC sp_rename '{{ from_relation.schema }}.{{ from_relation.identifier }}', '{{ to_relation.identifier }}'
     IF EXISTS(
     SELECT *
-    FROM sys.indexes with (nolock)
+    FROM sys.indexes {{ information_schema_hints() }}
     WHERE name='{{ from_relation.schema }}_{{ from_relation.identifier }}_cci' and object_id = OBJECT_ID('{{ from_relation.schema }}.{{ to_relation.identifier }}'))
     EXEC sp_rename N'{{ from_relation.schema }}.{{ to_relation.identifier }}.{{ from_relation.schema }}_{{ from_relation.identifier }}_cci', N'{{ from_relation.schema }}_{{ to_relation.identifier }}_cci', N'INDEX'
   {%- endcall %}
 {% endmacro %}
```

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/schema.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/test.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/split_part.sql` & `dbt-sqlserver-1.4.2/dbt/include/sqlserver/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/PKG-INFO` & `dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
+Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile
+Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/mssql-configs
+Project-URL: Changelog, https://github.com/dbt-msft/dbt-sqlserver/blob/master/CHANGELOG.md
+Project-URL: Issue Tracker, https://github.com/dbt-msft/dbt-sqlserver/issues
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/SOURCES.txt` & `dbt-sqlserver-1.4.2/dbt_sqlserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.1/setup.py` & `dbt-sqlserver-1.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,8 +81,14 @@
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
+    project_urls={
+        "Setup & configuration": "https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile",  # noqa: E501
+        "Documentation & usage": "https://docs.getdbt.com/reference/resource-configs/mssql-configs",  # noqa: E501
+        "Changelog": "https://github.com/dbt-msft/dbt-sqlserver/blob/master/CHANGELOG.md",  # noqa: E501
+        "Issue Tracker": "https://github.com/dbt-msft/dbt-sqlserver/issues",  # noqa: E501
+    },
 )
```

