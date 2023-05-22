# Comparing `tmp/dbt-sqlserver-1.4.0.tar.gz` & `tmp/dbt-sqlserver-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-sqlserver-1.4.0.tar", last modified: Mon May 15 20:55:07 2023, max compression
+gzip compressed data, was "dbt-sqlserver-1.4.1.tar", last modified: Mon May 22 07:58:14 2023, max compression
```

## Comparing `dbt-sqlserver-1.4.0.tar` & `dbt-sqlserver-1.4.1.tar`

### file list

```diff
@@ -1,72 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.116782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.120782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/test.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 20:55:06.000000 dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:55:07.124782 dbt-sqlserver-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-15 20:54:09.000000 dbt-sqlserver-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.678176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/test.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 07:58:14.000000 dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:58:14.682176 dbt-sqlserver-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-22 07:57:34.000000 dbt-sqlserver-1.4.1/setup.py
```

### Comparing `dbt-sqlserver-1.4.0/LICENSE` & `dbt-sqlserver-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/PKG-INFO` & `dbt-sqlserver-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
 
 ## Documentation
 
 We've bundled all documentation on the dbt docs site:
 
 * [Profile setup & authentication](https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile)
-* [Adapter-specific configuration](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
+* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
 
 Join us on the [dbt Slack](https://getdbt.slack.com/archives/CMRMDDQ9W) to ask questions, get help, or to discuss the project.
 
 ## Installation
 
 This adapter requires the Microsoft ODBC driver to be installed:
 [Windows](https://docs.microsoft.com/nl-be/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16#download-for-windows) |
```

### Comparing `dbt-sqlserver-1.4.0/README.md` & `dbt-sqlserver-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
 
 ## Documentation
 
 We've bundled all documentation on the dbt docs site:
 
 * [Profile setup & authentication](https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile)
-* [Adapter-specific configuration](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
+* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
 
 Join us on the [dbt Slack](https://getdbt.slack.com/archives/CMRMDDQ9W) to ask questions, get help, or to discuss the project.
 
 ## Installation
 
 This adapter requires the Microsoft ODBC driver to be installed:
 [Windows](https://docs.microsoft.com/nl-be/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16#download-for-windows) |
```

### Comparing `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/__init__.py` & `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_adapter.py` & `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 from typing import List, Optional
 
 import agate
 from dbt.adapters.base.relation import BaseRelation
+from dbt.adapters.cache import _make_ref_key_msg
 from dbt.adapters.sql import SQLAdapter
+from dbt.adapters.sql.impl import CREATE_SCHEMA_MACRO_NAME
+from dbt.events.functions import fire_event
+from dbt.events.types import SchemaCreation
 
 from dbt.adapters.sqlserver.sql_server_column import SQLServerColumn
 from dbt.adapters.sqlserver.sql_server_configs import SQLServerConfigs
 from dbt.adapters.sqlserver.sql_server_connection_manager import SQLServerConnectionManager
 
 
 class SQLServerAdapter(SQLAdapter):
     ConnectionManager = SQLServerConnectionManager
     Column = SQLServerColumn
     AdapterSpecificConfigs = SQLServerConfigs
 
+    def create_schema(self, relation: BaseRelation) -> None:
+        relation = relation.without_identifier()
+        fire_event(SchemaCreation(relation=_make_ref_key_msg(relation)))
+        macro_name = CREATE_SCHEMA_MACRO_NAME
+        kwargs = {
+            "relation": relation,
+        }
+
+        if self.config.credentials.schema_authorization:
+            kwargs["schema_authorization"] = self.config.credentials.schema_authorization
+            macro_name = "sqlserver__create_schema_with_authorization"
+
+        self.execute_macro(macro_name, kwargs=kwargs)
+        self.commit_if_has_connection()
+
     @classmethod
     def date_function(cls):
         return "getdate()"
 
     @classmethod
     def convert_text_type(cls, agate_table, col_idx):
         column = agate_table.columns[col_idx]
```

### Comparing `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_column.py` & `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_column.py`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_connection_manager.py` & `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_connection_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime as dt
 import struct
 import time
 from contextlib import contextmanager
 from itertools import chain, repeat
 from typing import Any, Callable, Dict, Mapping, Optional, Tuple
 
 import agate
@@ -229,14 +230,48 @@
     -------
     out : str
         The connection string argument.
     """
     return f'{key}={"Yes" if value else "No"}'
 
 
+def byte_array_to_datetime(value: bytes) -> dt.datetime:
+    """
+    Converts a DATETIMEOFFSET byte array to a timezone-aware datetime object
+
+    Parameters
+    ----------
+    value : buffer
+        A binary value conforming to SQL_SS_TIMESTAMPOFFSET_STRUCT
+
+    Returns
+    -------
+    out : datetime
+
+    Source
+    ------
+    SQL_SS_TIMESTAMPOFFSET datatype and SQL_SS_TIMESTAMPOFFSET_STRUCT layout:
+    https://learn.microsoft.com/sql/relational-databases/native-client-odbc-date-time/data-type-support-for-odbc-date-and-time-improvements
+    """
+    # unpack 20 bytes of data into a tuple of 9 values
+    tup = struct.unpack("<6hI2h", value)
+
+    # construct a datetime object
+    return dt.datetime(
+        year=tup[0],
+        month=tup[1],
+        day=tup[2],
+        hour=tup[3],
+        minute=tup[4],
+        second=tup[5],
+        microsecond=tup[6] // 1000,  # https://bugs.python.org/issue15443
+        tzinfo=dt.timezone(dt.timedelta(hours=tup[7], minutes=tup[8])),
+    )
+
+
 class SQLServerConnectionManager(SQLConnectionManager):
     TYPE = "sqlserver"
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
@@ -338,15 +373,17 @@
             logger.debug(f"Using connection string: {con_str_display}")
 
             attrs_before = get_pyodbc_attrs_before(credentials)
             handle = pyodbc.connect(
                 con_str_concat,
                 attrs_before=attrs_before,
                 autocommit=True,
+                timeout=credentials.login_timeout,
             )
+            handle.timeout = credentials.query_timeout
             logger.debug(f"Connected to db: {credentials.database}")
             return handle
 
         return cls.retry_connection(
             connection,
             connect=connect,
             logger=logger,
@@ -390,14 +427,18 @@
 
             # pyodbc does not handle a None type binding!
             if bindings is None:
                 cursor.execute(sql)
             else:
                 cursor.execute(sql, bindings)
 
+            # convert DATETIMEOFFSET binary structures to datetime ojbects
+            # https://github.com/mkleehammer/pyodbc/issues/134#issuecomment-281739794
+            connection.handle.add_output_converter(-155, byte_array_to_datetime)
+
             logger.debug(
                 "SQL status: {} in {:0.2f} seconds".format(
                     self.get_response(cursor), (time.time() - pre)
                 )
             )
 
             return connection, cursor
```

### Comparing `dbt-sqlserver-1.4.0/dbt/adapters/sqlserver/sql_server_credentials.py` & `dbt-sqlserver-1.4.1/dbt/adapters/sqlserver/sql_server_credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,30 @@
     tenant_id: Optional[str] = None
     client_id: Optional[str] = None
     client_secret: Optional[str] = None
     authentication: Optional[str] = "sql"
     encrypt: Optional[bool] = True  # default value in MS ODBC Driver 18 as well
     trust_cert: Optional[bool] = False  # default value in MS ODBC Driver 18 as well
     retries: int = 1
+    schema_authorization: Optional[str] = None
+    login_timeout: Optional[int] = 0
+    query_timeout: Optional[int] = 0
 
     _ALIASES = {
         "user": "UID",
         "username": "UID",
         "pass": "PWD",
         "password": "PWD",
         "server": "host",
         "trusted_connection": "windows_login",
         "auth": "authentication",
         "app_id": "client_id",
         "app_secret": "client_secret",
         "TrustServerCertificate": "trust_cert",
+        "schema_auth": "schema_authorization",
     }
 
     @property
     def type(self):
         return "sqlserver"
 
     def _connection_keys(self):
@@ -52,12 +56,14 @@
             "port",
             "UID",
             "client_id",
             "authentication",
             "encrypt",
             "trust_cert",
             "retries",
+            "login_timeout",
+            "query_timeout",
         )
 
     @property
     def unique_field(self):
         return self.host
```

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/apply_grants.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/columns.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/indexes.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/indexes.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 {% macro sqlserver__create_clustered_columnstore_index(relation) -%}
   {%- set cci_name = (relation.schema ~ '_' ~ relation.identifier ~ '_cci') | replace(".", "") | replace(" ", "") -%}
   {%- set relation_name = relation.schema ~ '_' ~ relation.identifier -%}
   {%- set full_relation = '"' ~ relation.schema ~ '"."' ~ relation.identifier ~ '"' -%}
   use [{{ relation.database }}];
   if EXISTS (
-        SELECT * FROM
-        sys.indexes WHERE name = '{{cci_name}}'
+        SELECT *
+        FROM sys.indexes with (nolock)
+        WHERE name = '{{cci_name}}'
         AND object_id=object_id('{{relation_name}}')
     )
   DROP index {{full_relation}}.{{cci_name}}
   CREATE CLUSTERED COLUMNSTORE INDEX {{cci_name}}
     ON {{full_relation}}
 {% endmacro %}
 
@@ -28,16 +29,17 @@
 
 
 {{ log("Running drop_xml_indexes() macro...") }}
 
 declare @drop_xml_indexes nvarchar(max);
 select @drop_xml_indexes = (
     select 'IF INDEXPROPERTY(' + CONVERT(VARCHAR(MAX), sys.tables.[object_id]) + ', ''' + sys.indexes.[name] + ''', ''IndexId'') IS NOT NULL DROP INDEX [' + sys.indexes.[name] + '] ON ' + '[' + SCHEMA_NAME(sys.tables.[schema_id]) + '].[' + OBJECT_NAME(sys.tables.[object_id]) + ']; '
-	from sys.indexes
-    inner join sys.tables on sys.indexes.object_id = sys.tables.object_id
+	from sys.indexes with (nolock)
+    inner join sys.tables with (nolock)
+    on sys.indexes.object_id = sys.tables.object_id
     where sys.indexes.[name] is not null
       and sys.indexes.type_desc = 'XML'
       and sys.tables.[name] = '{{ this.table }}'
     for xml path('')
 ); exec sp_executesql @drop_xml_indexes;
 
 {%- endmacro %}
@@ -48,16 +50,17 @@
 {# and https://stackoverflow.com/a/33785833/10415173         #}
 
 {{ log("Running drop_spatial_indexes() macro...") }}
 
 declare @drop_spatial_indexes nvarchar(max);
 select @drop_spatial_indexes = (
     select 'IF INDEXPROPERTY(' + CONVERT(VARCHAR(MAX), sys.tables.[object_id]) + ', ''' + sys.indexes.[name] + ''', ''IndexId'') IS NOT NULL DROP INDEX [' + sys.indexes.[name] + '] ON ' + '[' + SCHEMA_NAME(sys.tables.[schema_id]) + '].[' + OBJECT_NAME(sys.tables.[object_id]) + ']; '
-    from sys.indexes
-    inner join sys.tables on sys.indexes.object_id = sys.tables.object_id
+    from sys.indexes with (nolock)
+    inner join sys.tables with (nolock)
+    on sys.indexes.object_id = sys.tables.object_id
     where sys.indexes.[name] is not null
       and sys.indexes.type_desc = 'Spatial'
       and sys.tables.[name] = '{{ this.table }}'
     for xml path('')
 ); exec sp_executesql @drop_spatial_indexes;
 
 {%- endmacro %}
@@ -112,34 +115,35 @@
 {{ drop_pk_constraints() }}
 
 {{ log("Dropping remaining indexes...") }}
 
 declare @drop_remaining_indexes_last nvarchar(max);
 select @drop_remaining_indexes_last = (
     select 'IF INDEXPROPERTY(' + CONVERT(VARCHAR(MAX), sys.tables.[object_id]) + ', ''' + sys.indexes.[name] + ''', ''IndexId'') IS NOT NULL DROP INDEX [' + sys.indexes.[name] + '] ON ' + '[' + SCHEMA_NAME(sys.tables.[schema_id]) + '].[' + OBJECT_NAME(sys.tables.[object_id]) + ']; '
-    from sys.indexes
-    inner join sys.tables on sys.indexes.object_id = sys.tables.object_id
+    from sys.indexes with (nolock)
+    inner join sys.tables with (nolock)
+    on sys.indexes.object_id = sys.tables.object_id
     where sys.indexes.[name] is not null
       and sys.tables.[name] = '{{ this.table }}'
     for xml path('')
 ); exec sp_executesql @drop_remaining_indexes_last;
 
 {%- endmacro %}
 
 
 {% macro create_clustered_index(columns, unique=False) -%}
 
 {{ log("Creating clustered index...") }}
 
-{% set idx_name = this.table + '__clustered_index_on_' + columns|join('_') %}
+{% set idx_name = "clustered_" + local_md5(columns | join("_")) %}
 
-if not exists(select * from sys.indexes
-                where
-                name = '{{ idx_name }}' and
-                object_id = OBJECT_ID('{{ this }}')
+if not exists(select *
+                from sys.indexes with (nolock)
+                where name = '{{ idx_name }}'
+                and object_id = OBJECT_ID('{{ this }}')
 )
 begin
 
 create
 {% if unique -%}
 unique
 {% endif %}
@@ -151,23 +155,28 @@
 
 
 {% macro create_nonclustered_index(columns, includes=False) %}
 
 {{ log("Creating nonclustered index...") }}
 
 {% if includes -%}
-  {% set idx_name = this.table + '__index_on_' + columns|join('_')|replace(" ", "_") + '_includes_' + includes|join('_')|replace(" ", "_") %}
+    {% set idx_name = (
+        "nonclustered_"
+        + local_md5(columns | join("_"))
+        + "_incl_"
+        + local_md5(includes | join("_"))
+    ) %}
 {% else -%}
-  {% set idx_name = this.table + '__index_on_' + columns|join('_')|replace(" ", "_") %}
+    {% set idx_name = "nonclustered_" + local_md5(columns | join("_")) %}
 {% endif %}
 
-if not exists(select * from sys.indexes
-                where
-                name = '{{ idx_name }}' and
-                object_id = OBJECT_ID('{{ this }}')
+if not exists(select *
+                from sys.indexes with (nolock)
+                where name = '{{ idx_name }}'
+                and object_id = OBJECT_ID('{{ this }}')
 )
 begin
 create nonclustered index
     {{ idx_name }}
       on {{ this }} ({{ '[' + columns|join("], [") + ']' }})
       {% if includes -%}
         include ({{ '[' + includes|join("], [") + ']' }})
```

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/metadata.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/metadata.sql`

 * *Files 9% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 
     with
     principals as (
         select
             name as principal_name,
             principal_id as principal_id
         from
-            sys.database_principals
+            sys.database_principals with (nolock)
     ),
 
     schemas as (
         select
             name as schema_name,
             schema_id as schema_id,
             principal_id as principal_id
         from
-            sys.schemas
+            sys.schemas with (nolock)
     ),
 
     tables as (
         select
             name as table_name,
             schema_id as schema_id,
             principal_id as principal_id,
             'BASE TABLE' as table_type
         from
-            sys.tables
+            sys.tables with (nolock)
     ),
 
     tables_with_metadata as (
         select
             table_name,
             schema_name,
             coalesce(tables.principal_id, schemas.principal_id) as owner_principal_id,
@@ -45,15 +45,15 @@
     views as (
         select
             name as table_name,
             schema_id as schema_id,
             principal_id as principal_id,
             'VIEW' as table_type
         from
-            sys.views
+            sys.views with (nolock)
     ),
 
     views_with_metadata as (
         select
             table_name,
             schema_name,
             coalesce(views.principal_id, schemas.principal_id) as owner_principal_id,
@@ -150,11 +150,11 @@
       table_schema as [schema],
       case when table_type = 'BASE TABLE' then 'table'
            when table_type = 'VIEW' then 'view'
            else table_type
       end as table_type
 
     from [{{ schema_relation.database }}].INFORMATION_SCHEMA.TABLES with (nolock)
-    where table_schema like '{{ schema_relation.schema }}'
+    where table_schema = '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
```

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/relation.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/relation.sql`

 * *Files 1% similar despite different names*

```diff
@@ -41,12 +41,12 @@
 
 {% macro sqlserver__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
     USE [{{ to_relation.database }}];
     EXEC sp_rename '{{ from_relation.schema }}.{{ from_relation.identifier }}', '{{ to_relation.identifier }}'
     IF EXISTS(
     SELECT *
-    FROM sys.indexes
+    FROM sys.indexes with (nolock)
     WHERE name='{{ from_relation.schema }}_{{ from_relation.identifier }}_cci' and object_id = OBJECT_ID('{{ from_relation.schema }}.{{ to_relation.identifier }}'))
     EXEC sp_rename N'{{ from_relation.schema }}.{{ to_relation.identifier }}.{{ from_relation.schema }}_{{ from_relation.identifier }}_cci', N'{{ from_relation.schema }}_{{ to_relation.identifier }}_cci', N'INDEX'
   {%- endcall %}
 {% endmacro %}
```

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/adapters/schema.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/adapters/schema.sql`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 {% macro sqlserver__create_schema(relation) -%}
   {% call statement('create_schema') -%}
     USE [{{ relation.database }}];
-    IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = '{{ relation.without_identifier().schema }}')
+    IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = '{{ relation.schema }}')
     BEGIN
-    EXEC('CREATE SCHEMA [{{ relation.without_identifier().schema }}]')
+    EXEC('CREATE SCHEMA [{{ relation.schema }}]')
+    END
+  {% endcall %}
+{% endmacro %}
+
+{% macro sqlserver__create_schema_with_authorization(relation, schema_authorization) -%}
+  {% call statement('create_schema') -%}
+    USE [{{ relation.database }}];
+    IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = '{{ relation.schema }}')
+    BEGIN
+    EXEC('CREATE SCHEMA [{{ relation.schema }}] AUTHORIZATION [{{ schema_authorization }}]')
     END
   {% endcall %}
 {% endmacro %}
 
 {% macro sqlserver__drop_schema(relation) -%}
   {%- set relations_in_schema = list_relations_without_caching(relation) %}
```

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/seeds/helpers.sql`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-{% macro calc_batch_size(num_columns,max_batch_size) %}
-    {#
-        SQL Server allows for a max of 2100 parameters in a single statement.
-        Check if the max_batch_size fits with the number of columns, otherwise
-        reduce the batch size so it fits.
-    #}
-    {% if num_columns * max_batch_size < 2100 %}
-    {% set batch_size = max_batch_size %}
-    {% else %}
-    {% set batch_size = (2100 / num_columns)|int %}
-    {% endif %}
-
-    {{ return(batch_size) }}
-{%  endmacro %}
-
 {% macro sqlserver__get_binding_char() %}
   {{ return('?') }}
 {% endmacro %}
 
 {% macro sqlserver__get_batch_size() %}
   {{ return(400) }}
 {% endmacro %}
 
-{% macro basic_load_csv_rows(model, batch_size, agate_table) %}
+{% macro calc_batch_size(num_columns) %}
+    {#
+        SQL Server allows for a max of 2100 parameters in a single statement.
+        Check if the max_batch_size fits with the number of columns, otherwise
+        reduce the batch size so it fits.
+    #}
+    {% set max_batch_size = get_batch_size() %}
+    {% set calculated_batch = (2100 / num_columns)|int %}
+    {% set batch_size = [max_batch_size, calculated_batch] | min %}
+
+    {{ return(batch_size) }}
+{%  endmacro %}
 
+{% macro sqlserver__load_csv_rows(model, agate_table) %}
   {% set cols_sql = get_seed_column_quoted_csv(model, agate_table.column_names) %}
+  {% set batch_size = calc_batch_size(agate_table.column_names|length) %}
   {% set bindings = [] %}
-
   {% set statements = [] %}
 
+  {{ log("Inserting batches of " ~ batch_size ~ " records") }}
+
   {% for chunk in agate_table.rows | batch(batch_size) %}
       {% set bindings = [] %}
 
       {% for row in chunk %}
           {% do bindings.extend(row) %}
       {% endfor %}
 
@@ -52,15 +51,7 @@
           {% do statements.append(sql) %}
       {% endif %}
   {% endfor %}
 
   {# Return SQL so we can render it out into the compiled files #}
   {{ return(statements[0]) }}
 {% endmacro %}
-
-{% macro sqlserver__load_csv_rows(model, agate_table) %}
-  {% set max_batch_size = get_batch_size() %}
-  {% set cols_sql = get_seed_column_quoted_csv(model, agate_table.column_names) %}
-  {% set batch_size = calc_batch_size(cols_sql|length, max_batch_size) %}
-
-  {{ return(basic_load_csv_rows(model, batch_size, agate_table) )}}
-{% endmacro %}
```

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/materializations/tests/test.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt/include/sqlserver/macros/utils/split_part.sql` & `dbt-sqlserver-1.4.1/dbt/include/sqlserver/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/PKG-INFO` & `dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-sqlserver
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Microsoft SQL Server adapter plugin for dbt
 Home-page: https://github.com/dbt-msft/dbt-sqlserver
 Author: Mikael Ene, Anders Swanson, Sam Debruyn, Cor Zuurmond
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
 E.g. version 1.1.x of the adapter will be compatible with dbt-core 1.1.x.
 
 ## Documentation
 
 We've bundled all documentation on the dbt docs site:
 
 * [Profile setup & authentication](https://docs.getdbt.com/reference/warehouse-profiles/mssql-profile)
-* [Adapter-specific configuration](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
+* [Adapter documentation, usage and important notes](https://docs.getdbt.com/reference/resource-configs/mssql-configs)
 
 Join us on the [dbt Slack](https://getdbt.slack.com/archives/CMRMDDQ9W) to ask questions, get help, or to discuss the project.
 
 ## Installation
 
 This adapter requires the Microsoft ODBC driver to be installed:
 [Windows](https://docs.microsoft.com/nl-be/sql/connect/odbc/download-odbc-driver-for-sql-server?view=sql-server-ver16#download-for-windows) |
```

### Comparing `dbt-sqlserver-1.4.0/dbt_sqlserver.egg-info/SOURCES.txt` & `dbt-sqlserver-1.4.1/dbt_sqlserver.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-dbt/__init__.py
-dbt/adapters/__init__.py
 dbt/adapters/sqlserver/__init__.py
 dbt/adapters/sqlserver/__version__.py
 dbt/adapters/sqlserver/sql_server_adapter.py
 dbt/adapters/sqlserver/sql_server_column.py
 dbt/adapters/sqlserver/sql_server_configs.py
 dbt/adapters/sqlserver/sql_server_connection_manager.py
 dbt/adapters/sqlserver/sql_server_credentials.py
-dbt/include/__init__.py
 dbt/include/sqlserver/__init__.py
 dbt/include/sqlserver/dbt_project.yml
 dbt/include/sqlserver/macros/adapters/apply_grants.sql
 dbt/include/sqlserver/macros/adapters/columns.sql
 dbt/include/sqlserver/macros/adapters/indexes.sql
 dbt/include/sqlserver/macros/adapters/metadata.sql
 dbt/include/sqlserver/macros/adapters/persist_docs.sql
```

### Comparing `dbt-sqlserver-1.4.0/setup.py` & `dbt-sqlserver-1.4.1/setup.py`

 * *Files identical despite different names*

