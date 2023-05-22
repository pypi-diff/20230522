# Comparing `tmp/pydal-20230511.1.tar.gz` & `tmp/pydal-20230521.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydal-20230511.1.tar", last modified: Fri May 12 02:29:54 2023, max compression
+gzip compressed data, was "pydal-20230521.1.tar", last modified: Mon May 22 05:48:49 2023, max compression
```

## Comparing `pydal-20230511.1.tar` & `pydal-20230521.1.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.736696 pydal-20230511.1/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      344 2022-10-17 00:44:46.000000 pydal-20230511.1/AUTHORS
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6546 2022-10-17 00:44:46.000000 pydal-20230511.1/CHANGES
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1555 2022-10-17 00:44:46.000000 pydal-20230511.1/LICENSE.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      170 2022-11-11 06:37:56.000000 pydal-20230511.1/MANIFEST.in
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2903 2023-05-12 02:29:54.736696 pydal-20230511.1/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2034 2022-10-17 00:44:46.000000 pydal-20230511.1/README.md
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.712696 pydal-20230511.1/docs/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6758 2022-10-17 00:44:46.000000 pydal-20230511.1/docs/Makefile
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8083 2023-05-07 23:00:04.000000 pydal-20230511.1/docs/conf.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      833 2022-10-17 00:44:46.000000 pydal-20230511.1/docs/index.rst
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2834 2022-10-17 00:44:46.000000 pydal-20230511.1/docs/pydal.adapters.rst
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      664 2022-10-17 00:44:46.000000 pydal-20230511.1/docs/pydal.helpers.rst
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       29 2022-10-17 00:44:46.000000 pydal-20230511.1/docs/requirements.txt
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.716696 pydal-20230511.1/pydal/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      179 2023-05-12 02:29:04.000000 pydal-20230511.1/pydal/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5439 2023-05-07 22:57:55.000000 pydal-20230511.1/pydal/_compat.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      466 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/_gae.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      208 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/_globals.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/_load.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.720696 pydal-20230511.1/pydal/adapters/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2372 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    38893 2023-05-07 23:00:01.000000 pydal-20230511.1/pydal/adapters/base.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5691 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/couchdb.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2000 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/db2.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3145 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/firebird.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18365 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2076 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/informix.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1882 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/ingres.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    37772 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/mongo.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6161 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/mssql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3412 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/mysql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9170 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/oracle.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9327 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/postgres.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1460 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/sap.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4894 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/snowflake.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4392 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/sqlite.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      799 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/adapters/teradata.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    38526 2023-05-07 22:59:58.000000 pydal-20230511.1/pydal/base.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6427 2023-05-07 22:57:59.000000 pydal-20230511.1/pydal/connection.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.720696 pydal-20230511.1/pydal/contrib/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/contrib/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    44547 2023-05-07 22:58:08.000000 pydal-20230511.1/pydal/contrib/imap_adapter.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    79364 2023-05-07 22:58:11.000000 pydal-20230511.1/pydal/contrib/ipaddress.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    10686 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/contrib/mockimaplib.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4071 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/contrib/ordereddict.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5584 2023-05-07 22:58:06.000000 pydal-20230511.1/pydal/contrib/portalocker.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    33372 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/contrib/reserved_sql_keywords.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3532 2023-05-07 22:58:07.000000 pydal-20230511.1/pydal/default_validators.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.724696 pydal-20230511.1/pydal/dialects/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3803 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    23464 2023-05-07 22:58:13.000000 pydal-20230511.1/pydal/dialects/base.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1390 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/couchdb.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3374 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/db2.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4307 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/firebird.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5953 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3275 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/informix.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3929 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/ingres.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    22110 2023-05-07 22:58:11.000000 pydal-20230511.1/pydal/dialects/mongo.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    15758 2023-05-07 23:00:00.000000 pydal-20230511.1/pydal/dialects/mssql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3413 2023-05-07 22:51:50.000000 pydal-20230511.1/pydal/dialects/mysql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8928 2023-05-07 22:58:13.000000 pydal-20230511.1/pydal/dialects/oracle.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    14396 2023-05-07 22:58:15.000000 pydal-20230511.1/pydal/dialects/postgre.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3001 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/sap.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    12077 2023-05-07 22:58:18.000000 pydal-20230511.1/pydal/dialects/snowflake.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4295 2023-05-07 22:52:12.000000 pydal-20230511.1/pydal/dialects/sqlite.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3400 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/dialects/teradata.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3179 2023-05-07 22:59:59.000000 pydal-20230511.1/pydal/drivers.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      347 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/exceptions.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.724696 pydal-20230511.1/pydal/helpers/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/helpers/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      652 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/helpers/_internals.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    16529 2023-05-07 22:59:59.000000 pydal-20230511.1/pydal/helpers/classes.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      971 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/helpers/gae.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    14800 2023-05-07 22:59:59.000000 pydal-20230511.1/pydal/helpers/methods.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1144 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/helpers/regex.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    16447 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/helpers/rest.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1839 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/helpers/serializers.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    27287 2023-05-07 22:58:25.000000 pydal-20230511.1/pydal/migrator.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   128633 2023-05-07 22:59:58.000000 pydal-20230511.1/pydal/objects.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.728696 pydal-20230511.1/pydal/parsers/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3394 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/parsers/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4718 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/parsers/base.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      360 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/parsers/google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1605 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/parsers/mongo.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1654 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/parsers/oracle.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      815 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/parsers/postgre.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1064 2023-05-07 23:00:00.000000 pydal-20230511.1/pydal/parsers/sqlite.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.728696 pydal-20230511.1/pydal/representers/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8831 2023-05-07 22:59:59.000000 pydal-20230511.1/pydal/representers/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8810 2023-05-07 22:59:59.000000 pydal-20230511.1/pydal/representers/base.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1210 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/couchdb.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      680 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/db2.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1446 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/google.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      884 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/informix.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1757 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/mongo.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      948 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/mssql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      214 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/mysql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1286 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/oracle.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1643 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/postgre.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      752 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/representers/sqlite.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    22856 2023-05-12 02:28:52.000000 pydal-20230511.1/pydal/restapi.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.728696 pydal-20230511.1/pydal/tools/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/tools/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1946 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/tools/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1904 2022-10-17 00:44:46.000000 pydal-20230511.1/pydal/utils.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   158796 2023-05-07 22:59:58.000000 pydal-20230511.1/pydal/validators.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.716696 pydal-20230511.1/pydal.egg-info/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2903 2023-05-12 02:29:54.000000 pydal-20230511.1/pydal.egg-info/PKG-INFO
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3965 2023-05-12 02:29:54.000000 pydal-20230511.1/pydal.egg-info/SOURCES.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-12 02:29:54.000000 pydal-20230511.1/pydal.egg-info/dependency_links.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)        6 2023-05-12 02:29:54.000000 pydal-20230511.1/pydal.egg-info/top_level.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      822 2023-05-12 02:29:16.000000 pydal-20230511.1/pyproject.toml
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       99 2023-05-12 02:29:54.736696 pydal-20230511.1/setup.cfg
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.732696 pydal-20230511.1/tests/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      355 2023-05-07 23:00:04.000000 pydal-20230511.1/tests/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-12 02:29:54.736696 pydal-20230511.1/tests/__pycache__/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      463 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      463 2023-05-07 23:37:01.000000 pydal-20230511.1/tests/__pycache__/__init__.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1002 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/_adapt.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1002 2023-05-07 22:45:50.000000 pydal-20230511.1/tests/__pycache__/_adapt.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      235 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/_compat.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      235 2023-05-07 22:45:51.000000 pydal-20230511.1/tests/__pycache__/_compat.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1189 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/_helpers.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1197 2023-05-07 23:37:02.000000 pydal-20230511.1/tests/__pycache__/_helpers.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7191 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/base.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7225 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/base.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3136 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/caching.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3136 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/caching.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5395 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/contribs.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5409 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/contribs.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2539 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/indexes.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2567 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/indexes.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    22630 2023-05-07 22:38:52.000000 pydal-20230511.1/tests/__pycache__/is_url_validators.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    22135 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/is_url_validators.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    69633 2023-05-07 22:38:52.000000 pydal-20230511.1/tests/__pycache__/nosql.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5459 2023-05-07 22:38:52.000000 pydal-20230511.1/tests/__pycache__/restapi.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5457 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/restapi.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3467 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/smart_query.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3467 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/smart_query.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    91125 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/sql.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    90885 2023-05-07 23:37:01.000000 pydal-20230511.1/tests/__pycache__/sql.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1086 2023-05-07 22:38:52.000000 pydal-20230511.1/tests/__pycache__/tags.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1086 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/tags.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3312 2023-05-07 22:38:51.000000 pydal-20230511.1/tests/__pycache__/validation.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3304 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/validation.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    37800 2023-05-07 22:38:52.000000 pydal-20230511.1/tests/__pycache__/validators.cpython-38.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    37768 2023-05-07 23:37:03.000000 pydal-20230511.1/tests/__pycache__/validators.cpython-39.pyc
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      954 2022-10-17 00:44:46.000000 pydal-20230511.1/tests/_adapt.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       95 2022-10-17 00:44:46.000000 pydal-20230511.1/tests/_compat.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      765 2023-05-07 23:00:04.000000 pydal-20230511.1/tests/_helpers.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     8127 2023-05-07 23:00:04.000000 pydal-20230511.1/tests/base.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2554 2023-05-07 23:00:03.000000 pydal-20230511.1/tests/caching.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     4967 2023-05-07 23:00:01.000000 pydal-20230511.1/tests/contribs.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2279 2023-05-07 23:00:03.000000 pydal-20230511.1/tests/indexes.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    29377 2023-05-07 23:00:03.000000 pydal-20230511.1/tests/is_url_validators.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    99834 2023-05-07 23:00:04.000000 pydal-20230511.1/tests/nosql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    14103 2023-05-07 23:00:01.000000 pydal-20230511.1/tests/restapi.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    12552 2023-05-07 23:00:04.000000 pydal-20230511.1/tests/smart_query.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   137742 2023-05-07 23:00:03.000000 pydal-20230511.1/tests/sql.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      990 2023-05-07 23:00:04.000000 pydal-20230511.1/tests/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3579 2023-05-07 23:00:03.000000 pydal-20230511.1/tests/validation.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    67656 2023-05-07 23:00:02.000000 pydal-20230511.1/tests/validators.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.313074 pydal-20230521.1/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      344 2022-10-17 00:44:46.000000 pydal-20230521.1/AUTHORS
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6546 2022-10-17 00:44:46.000000 pydal-20230521.1/CHANGES
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1555 2022-10-17 00:44:46.000000 pydal-20230521.1/LICENSE.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      170 2022-11-11 06:37:56.000000 pydal-20230521.1/MANIFEST.in
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2903 2023-05-22 05:48:49.313074 pydal-20230521.1/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2034 2022-10-17 00:44:46.000000 pydal-20230521.1/README.md
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.285076 pydal-20230521.1/docs/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6758 2022-10-17 00:44:46.000000 pydal-20230521.1/docs/Makefile
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8083 2023-05-07 23:00:04.000000 pydal-20230521.1/docs/conf.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      833 2022-10-17 00:44:46.000000 pydal-20230521.1/docs/index.rst
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2834 2022-10-17 00:44:46.000000 pydal-20230521.1/docs/pydal.adapters.rst
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      664 2022-10-17 00:44:46.000000 pydal-20230521.1/docs/pydal.helpers.rst
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       29 2022-10-17 00:44:46.000000 pydal-20230521.1/docs/requirements.txt
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.289076 pydal-20230521.1/pydal/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      179 2023-05-22 05:48:14.000000 pydal-20230521.1/pydal/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5439 2023-05-07 22:57:55.000000 pydal-20230521.1/pydal/_compat.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      466 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/_gae.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      208 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/_globals.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      396 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/_load.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.293076 pydal-20230521.1/pydal/adapters/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2372 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    38893 2023-05-07 23:00:01.000000 pydal-20230521.1/pydal/adapters/base.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5691 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/couchdb.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2000 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/db2.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3145 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/firebird.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18365 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2076 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/informix.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1882 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/ingres.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    37772 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/mongo.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6161 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/mssql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3412 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/mysql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9170 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/oracle.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9327 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/postgres.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1460 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/sap.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4894 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/snowflake.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4392 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/sqlite.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      799 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/adapters/teradata.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    38526 2023-05-07 22:59:58.000000 pydal-20230521.1/pydal/base.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6427 2023-05-07 22:57:59.000000 pydal-20230521.1/pydal/connection.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.293076 pydal-20230521.1/pydal/contrib/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/contrib/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    44547 2023-05-07 22:58:08.000000 pydal-20230521.1/pydal/contrib/imap_adapter.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    79364 2023-05-07 22:58:11.000000 pydal-20230521.1/pydal/contrib/ipaddress.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    10686 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/contrib/mockimaplib.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4071 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/contrib/ordereddict.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5584 2023-05-07 22:58:06.000000 pydal-20230521.1/pydal/contrib/portalocker.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    33372 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/contrib/reserved_sql_keywords.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3532 2023-05-07 22:58:07.000000 pydal-20230521.1/pydal/default_validators.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.297075 pydal-20230521.1/pydal/dialects/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3803 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    23464 2023-05-07 22:58:13.000000 pydal-20230521.1/pydal/dialects/base.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1390 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/couchdb.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3374 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/db2.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4307 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/firebird.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5953 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3275 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/informix.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3929 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/ingres.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    22110 2023-05-07 22:58:11.000000 pydal-20230521.1/pydal/dialects/mongo.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    15758 2023-05-07 23:00:00.000000 pydal-20230521.1/pydal/dialects/mssql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3413 2023-05-07 22:51:50.000000 pydal-20230521.1/pydal/dialects/mysql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8928 2023-05-07 22:58:13.000000 pydal-20230521.1/pydal/dialects/oracle.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    14396 2023-05-07 22:58:15.000000 pydal-20230521.1/pydal/dialects/postgre.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3001 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/sap.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    12077 2023-05-07 22:58:18.000000 pydal-20230521.1/pydal/dialects/snowflake.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4295 2023-05-07 22:52:12.000000 pydal-20230521.1/pydal/dialects/sqlite.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3400 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/dialects/teradata.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3179 2023-05-07 22:59:59.000000 pydal-20230521.1/pydal/drivers.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      347 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/exceptions.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.297075 pydal-20230521.1/pydal/helpers/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/helpers/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      652 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/helpers/_internals.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    16529 2023-05-07 22:59:59.000000 pydal-20230521.1/pydal/helpers/classes.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      971 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/helpers/gae.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    14800 2023-05-07 22:59:59.000000 pydal-20230521.1/pydal/helpers/methods.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1144 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/helpers/regex.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    16447 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/helpers/rest.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1839 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/helpers/serializers.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    27287 2023-05-07 22:58:25.000000 pydal-20230521.1/pydal/migrator.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   128642 2023-05-22 05:47:34.000000 pydal-20230521.1/pydal/objects.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.301075 pydal-20230521.1/pydal/parsers/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3394 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/parsers/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4718 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/parsers/base.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      360 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/parsers/google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1605 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/parsers/mongo.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1654 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/parsers/oracle.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      815 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/parsers/postgre.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1064 2023-05-07 23:00:00.000000 pydal-20230521.1/pydal/parsers/sqlite.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.301075 pydal-20230521.1/pydal/representers/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8831 2023-05-07 22:59:59.000000 pydal-20230521.1/pydal/representers/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8810 2023-05-07 22:59:59.000000 pydal-20230521.1/pydal/representers/base.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1210 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/couchdb.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      680 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/db2.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1446 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/google.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      884 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/informix.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1757 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/mongo.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      948 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/mssql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      214 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/mysql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1286 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/oracle.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1643 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/postgre.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      752 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/representers/sqlite.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    22856 2023-05-12 02:28:52.000000 pydal-20230521.1/pydal/restapi.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.301075 pydal-20230521.1/pydal/tools/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/tools/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1946 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/tools/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1904 2022-10-17 00:44:46.000000 pydal-20230521.1/pydal/utils.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   158796 2023-05-07 22:59:58.000000 pydal-20230521.1/pydal/validators.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.289076 pydal-20230521.1/pydal.egg-info/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2903 2023-05-22 05:48:49.000000 pydal-20230521.1/pydal.egg-info/PKG-INFO
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3965 2023-05-22 05:48:49.000000 pydal-20230521.1/pydal.egg-info/SOURCES.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        1 2023-05-22 05:48:49.000000 pydal-20230521.1/pydal.egg-info/dependency_links.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)        6 2023-05-22 05:48:49.000000 pydal-20230521.1/pydal.egg-info/top_level.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      822 2023-05-22 05:48:06.000000 pydal-20230521.1/pyproject.toml
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       99 2023-05-22 05:48:49.313074 pydal-20230521.1/setup.cfg
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.305075 pydal-20230521.1/tests/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      355 2023-05-07 23:00:04.000000 pydal-20230521.1/tests/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-05-22 05:48:49.313074 pydal-20230521.1/tests/__pycache__/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      463 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      463 2023-05-07 23:37:01.000000 pydal-20230521.1/tests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1002 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/_adapt.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1002 2023-05-07 22:45:50.000000 pydal-20230521.1/tests/__pycache__/_adapt.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      235 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/_compat.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      235 2023-05-07 22:45:51.000000 pydal-20230521.1/tests/__pycache__/_compat.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1189 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/_helpers.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1197 2023-05-07 23:37:02.000000 pydal-20230521.1/tests/__pycache__/_helpers.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7191 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/base.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7225 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/base.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3136 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/caching.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3136 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/caching.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5395 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/contribs.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5409 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/contribs.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2539 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/indexes.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2567 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/indexes.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    22630 2023-05-07 22:38:52.000000 pydal-20230521.1/tests/__pycache__/is_url_validators.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    22135 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/is_url_validators.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    69633 2023-05-07 22:38:52.000000 pydal-20230521.1/tests/__pycache__/nosql.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5459 2023-05-07 22:38:52.000000 pydal-20230521.1/tests/__pycache__/restapi.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5457 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/restapi.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3467 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/smart_query.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3467 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/smart_query.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    91125 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/sql.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    90885 2023-05-07 23:37:01.000000 pydal-20230521.1/tests/__pycache__/sql.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1086 2023-05-07 22:38:52.000000 pydal-20230521.1/tests/__pycache__/tags.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1086 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/tags.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3312 2023-05-07 22:38:51.000000 pydal-20230521.1/tests/__pycache__/validation.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3304 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/validation.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    37800 2023-05-07 22:38:52.000000 pydal-20230521.1/tests/__pycache__/validators.cpython-38.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    37768 2023-05-07 23:37:03.000000 pydal-20230521.1/tests/__pycache__/validators.cpython-39.pyc
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      954 2022-10-17 00:44:46.000000 pydal-20230521.1/tests/_adapt.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       95 2022-10-17 00:44:46.000000 pydal-20230521.1/tests/_compat.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      765 2023-05-07 23:00:04.000000 pydal-20230521.1/tests/_helpers.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     8127 2023-05-07 23:00:04.000000 pydal-20230521.1/tests/base.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2554 2023-05-07 23:00:03.000000 pydal-20230521.1/tests/caching.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     4967 2023-05-07 23:00:01.000000 pydal-20230521.1/tests/contribs.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2279 2023-05-07 23:00:03.000000 pydal-20230521.1/tests/indexes.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    29377 2023-05-07 23:00:03.000000 pydal-20230521.1/tests/is_url_validators.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    99834 2023-05-07 23:00:04.000000 pydal-20230521.1/tests/nosql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    14103 2023-05-07 23:00:01.000000 pydal-20230521.1/tests/restapi.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    12552 2023-05-07 23:00:04.000000 pydal-20230521.1/tests/smart_query.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)   137742 2023-05-07 23:00:03.000000 pydal-20230521.1/tests/sql.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      990 2023-05-07 23:00:04.000000 pydal-20230521.1/tests/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3579 2023-05-07 23:00:03.000000 pydal-20230521.1/tests/validation.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    67656 2023-05-07 23:00:02.000000 pydal-20230521.1/tests/validators.py
```

### Comparing `pydal-20230511.1/CHANGES` & `pydal-20230521.1/CHANGES`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/LICENSE.txt` & `pydal-20230521.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/PKG-INFO` & `pydal-20230521.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20230511.1
+Version: 20230521.1
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20230511.1/README.md` & `pydal-20230521.1/README.md`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/docs/Makefile` & `pydal-20230521.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/docs/conf.py` & `pydal-20230521.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/docs/index.rst` & `pydal-20230521.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/docs/pydal.adapters.rst` & `pydal-20230521.1/docs/pydal.adapters.rst`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/docs/pydal.helpers.rst` & `pydal-20230521.1/docs/pydal.helpers.rst`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/_compat.py` & `pydal-20230521.1/pydal/_compat.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/__init__.py` & `pydal-20230521.1/pydal/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/base.py` & `pydal-20230521.1/pydal/adapters/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/couchdb.py` & `pydal-20230521.1/pydal/adapters/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/db2.py` & `pydal-20230521.1/pydal/adapters/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/firebird.py` & `pydal-20230521.1/pydal/adapters/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/google.py` & `pydal-20230521.1/pydal/adapters/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/informix.py` & `pydal-20230521.1/pydal/adapters/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/ingres.py` & `pydal-20230521.1/pydal/adapters/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/mongo.py` & `pydal-20230521.1/pydal/adapters/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/mssql.py` & `pydal-20230521.1/pydal/adapters/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/mysql.py` & `pydal-20230521.1/pydal/adapters/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/oracle.py` & `pydal-20230521.1/pydal/adapters/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/postgres.py` & `pydal-20230521.1/pydal/adapters/postgres.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/sap.py` & `pydal-20230521.1/pydal/adapters/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/snowflake.py` & `pydal-20230521.1/pydal/adapters/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/sqlite.py` & `pydal-20230521.1/pydal/adapters/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/adapters/teradata.py` & `pydal-20230521.1/pydal/adapters/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/base.py` & `pydal-20230521.1/pydal/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/connection.py` & `pydal-20230521.1/pydal/connection.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/contrib/imap_adapter.py` & `pydal-20230521.1/pydal/contrib/imap_adapter.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/contrib/ipaddress.py` & `pydal-20230521.1/pydal/contrib/ipaddress.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/contrib/mockimaplib.py` & `pydal-20230521.1/pydal/contrib/mockimaplib.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/contrib/ordereddict.py` & `pydal-20230521.1/pydal/contrib/ordereddict.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/contrib/portalocker.py` & `pydal-20230521.1/pydal/contrib/portalocker.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/contrib/reserved_sql_keywords.py` & `pydal-20230521.1/pydal/contrib/reserved_sql_keywords.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/default_validators.py` & `pydal-20230521.1/pydal/default_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/__init__.py` & `pydal-20230521.1/pydal/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/base.py` & `pydal-20230521.1/pydal/dialects/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/couchdb.py` & `pydal-20230521.1/pydal/dialects/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/db2.py` & `pydal-20230521.1/pydal/dialects/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/firebird.py` & `pydal-20230521.1/pydal/dialects/firebird.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/google.py` & `pydal-20230521.1/pydal/dialects/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/informix.py` & `pydal-20230521.1/pydal/dialects/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/ingres.py` & `pydal-20230521.1/pydal/dialects/ingres.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/mongo.py` & `pydal-20230521.1/pydal/dialects/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/mssql.py` & `pydal-20230521.1/pydal/dialects/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/mysql.py` & `pydal-20230521.1/pydal/dialects/mysql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/oracle.py` & `pydal-20230521.1/pydal/dialects/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/postgre.py` & `pydal-20230521.1/pydal/dialects/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/sap.py` & `pydal-20230521.1/pydal/dialects/sap.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/snowflake.py` & `pydal-20230521.1/pydal/dialects/snowflake.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/sqlite.py` & `pydal-20230521.1/pydal/dialects/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/dialects/teradata.py` & `pydal-20230521.1/pydal/dialects/teradata.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/drivers.py` & `pydal-20230521.1/pydal/drivers.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/_internals.py` & `pydal-20230521.1/pydal/helpers/_internals.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/classes.py` & `pydal-20230521.1/pydal/helpers/classes.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/gae.py` & `pydal-20230521.1/pydal/helpers/gae.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/methods.py` & `pydal-20230521.1/pydal/helpers/methods.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/regex.py` & `pydal-20230521.1/pydal/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/rest.py` & `pydal-20230521.1/pydal/helpers/rest.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/helpers/serializers.py` & `pydal-20230521.1/pydal/helpers/serializers.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/migrator.py` & `pydal-20230521.1/pydal/migrator.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/objects.py` & `pydal-20230521.1/pydal/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -945,15 +945,15 @@
 
         if record:
             response = self.validate_and_update(_key, **fields)
             if hasattr(self, "_primarykey"):
                 primary_keys = {}
                 for key in self._primarykey:
                     primary_keys[key] = getattr(record, key)
-                response.id = primary_keys
+                response["id"] = primary_keys
         else:
             response = self.validate_and_insert(**fields)
         return response
 
     def bulk_insert(self, items):
         """
         here items is a list of dictionaries
@@ -2761,35 +2761,35 @@
         if not row._values:
             raise ValueError("No fields to update")
         ret = self.db._adapter.update(table, self.query, row.op_values())
         return ret
 
     def validate_and_update(self, **update_fields):
         table = self.db._adapter.get_table(self.query)
-        response = Row()
-        response.errors = Row()
+        response = {}
+        response["errors"] = {}
         new_fields = copy.copy(update_fields)
         for key, value in iteritems(update_fields):
             value, error = table[key].validate(value, update_fields.get("id"))
             if error:
-                response.errors[key] = "%s" % error
+                response["errors"][key] = "%s" % error
             else:
                 new_fields[key] = value
-        if response.errors:
-            response.updated = None
+        if response["errors"]:
+            response["updated"] = 0
         else:
             row = table._fields_and_values_for_update(new_fields)
             if not row._values:
                 raise ValueError("No fields to update")
             if any(f(self, row) for f in table._before_update):
                 ret = 0
             else:
                 ret = self.db._adapter.update(table, self.query, row.op_values())
                 ret and [f(self, row) for f in table._after_update]
-            response.updated = ret
+            response["updated"] = ret
         return response
 
 
 class LazyReferenceGetter(object):
     def __init__(self, table, id):
         self.db = table._db
         self.tablename = table._tablename
```

### Comparing `pydal-20230511.1/pydal/parsers/__init__.py` & `pydal-20230521.1/pydal/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/parsers/base.py` & `pydal-20230521.1/pydal/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/parsers/mongo.py` & `pydal-20230521.1/pydal/parsers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/parsers/oracle.py` & `pydal-20230521.1/pydal/parsers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/parsers/postgre.py` & `pydal-20230521.1/pydal/parsers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/parsers/sqlite.py` & `pydal-20230521.1/pydal/parsers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/__init__.py` & `pydal-20230521.1/pydal/representers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/base.py` & `pydal-20230521.1/pydal/representers/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/couchdb.py` & `pydal-20230521.1/pydal/representers/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/db2.py` & `pydal-20230521.1/pydal/representers/db2.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/google.py` & `pydal-20230521.1/pydal/representers/google.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/informix.py` & `pydal-20230521.1/pydal/representers/informix.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/mongo.py` & `pydal-20230521.1/pydal/representers/mongo.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/mssql.py` & `pydal-20230521.1/pydal/representers/mssql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/oracle.py` & `pydal-20230521.1/pydal/representers/oracle.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/postgre.py` & `pydal-20230521.1/pydal/representers/postgre.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/representers/sqlite.py` & `pydal-20230521.1/pydal/representers/sqlite.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/restapi.py` & `pydal-20230521.1/pydal/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/tools/tags.py` & `pydal-20230521.1/pydal/tools/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/utils.py` & `pydal-20230521.1/pydal/utils.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal/validators.py` & `pydal-20230521.1/pydal/validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pydal.egg-info/PKG-INFO` & `pydal-20230521.1/pydal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydal
-Version: 20230511.1
+Version: 20230521.1
 Summary: pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pydal
 Project-URL: Bug Tracker, https://github.com/web2py/pydal/issues
 Project-URL: Documentation, https://py4web.com/_documentation/static/en/chapter-07.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydal-20230511.1/pydal.egg-info/SOURCES.txt` & `pydal-20230521.1/pydal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/pyproject.toml` & `pydal-20230521.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pydal"
-version = "20230511.1"
+version = "20230521.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = 'pyDAL is a Database Abstraction Layer. It generates queries for SQlite, PotsgreSQL, MySQL, and other backends. It was originally part of the web2py frameworks but it is now an independent project. Example: db.define_table("thing",Field("name")) and db.thing.insert(name="Pizza")'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pydal-20230511.1/tests/__pycache__/_adapt.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/_adapt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/_adapt.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/_adapt.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/_helpers.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/_helpers.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/base.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/base.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/caching.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/caching.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/caching.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/caching.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/contribs.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/contribs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/contribs.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/contribs.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/indexes.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/indexes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/indexes.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/indexes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/is_url_validators.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/is_url_validators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/is_url_validators.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/is_url_validators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/nosql.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/nosql.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/restapi.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/restapi.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/restapi.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/restapi.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/smart_query.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/smart_query.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/smart_query.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/smart_query.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/sql.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/sql.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/sql.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/sql.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/tags.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/tags.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/tags.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/tags.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/validation.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/validation.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/validation.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/validation.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/validators.cpython-38.pyc` & `pydal-20230521.1/tests/__pycache__/validators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/__pycache__/validators.cpython-39.pyc` & `pydal-20230521.1/tests/__pycache__/validators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/_adapt.py` & `pydal-20230521.1/tests/_adapt.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/_helpers.py` & `pydal-20230521.1/tests/_helpers.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/base.py` & `pydal-20230521.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/caching.py` & `pydal-20230521.1/tests/caching.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/contribs.py` & `pydal-20230521.1/tests/contribs.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/indexes.py` & `pydal-20230521.1/tests/indexes.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/is_url_validators.py` & `pydal-20230521.1/tests/is_url_validators.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/nosql.py` & `pydal-20230521.1/tests/nosql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/restapi.py` & `pydal-20230521.1/tests/restapi.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/smart_query.py` & `pydal-20230521.1/tests/smart_query.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/sql.py` & `pydal-20230521.1/tests/sql.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/tags.py` & `pydal-20230521.1/tests/tags.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/validation.py` & `pydal-20230521.1/tests/validation.py`

 * *Files identical despite different names*

### Comparing `pydal-20230511.1/tests/validators.py` & `pydal-20230521.1/tests/validators.py`

 * *Files identical despite different names*

