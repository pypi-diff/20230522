# Comparing `tmp/squad_ds_utils-0.1.3.tar.gz` & `tmp/squad_ds_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squad_ds_utils-0.1.3.tar", max compression
+gzip compressed data, was "squad_ds_utils-0.1.6.tar", max compression
```

## Comparing `squad_ds_utils-0.1.3.tar` & `squad_ds_utils-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0        0 2023-04-07 11:48:06.845887 squad_ds_utils-0.1.3/README.md
--rw-r--r--   0        0        0      362 2023-04-07 11:55:37.460758 squad_ds_utils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 11:48:06.846392 squad_ds_utils-0.1.3/squad_ds_utils/__init__.py
--rw-r--r--   0        0        0       40 2023-04-07 11:48:06.846491 squad_ds_utils-0.1.3/squad_ds_utils/exceptions.py
--rw-r--r--   0        0        0      563 2023-04-07 11:57:21.111450 squad_ds_utils-0.1.3/squad_ds_utils/parse.py
--rw-r--r--   0        0        0     2321 2023-04-07 11:48:06.846610 squad_ds_utils-0.1.3/squad_ds_utils/recordings_fetcher.py
--rw-r--r--   0        0        0      628 2023-04-07 11:48:06.846724 squad_ds_utils-0.1.3/squad_ds_utils/secrets.py
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 squad_ds_utils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-19 08:44:34.686815 squad_ds_utils-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 11:28:45.283180 squad_ds_utils-0.1.6/database_connector/__init__.py
+-rw-r--r--   0        0        0      563 2023-05-22 13:03:20.017766 squad_ds_utils-0.1.6/database_connector/constants.py
+-rw-r--r--   0        0        0     1197 2023-05-22 11:28:45.283725 squad_ds_utils-0.1.6/database_connector/sagemaker.py
+-rw-r--r--   0        0        0     1675 2023-05-22 13:15:39.958263 squad_ds_utils-0.1.6/database_connector/snowflake_ds.py
+-rw-r--r--   0        0        0     1437 2023-05-22 11:28:45.284158 squad_ds_utils-0.1.6/database_connector/utils.py
+-rw-r--r--   0        0        0      494 2023-05-22 13:16:55.864076 squad_ds_utils-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 08:44:34.687254 squad_ds_utils-0.1.6/squad_ds_utils/__init__.py
+-rw-r--r--   0        0        0       40 2023-05-19 08:44:34.687346 squad_ds_utils-0.1.6/squad_ds_utils/exceptions.py
+-rw-r--r--   0        0        0      563 2023-05-19 08:44:34.687426 squad_ds_utils-0.1.6/squad_ds_utils/parse.py
+-rw-r--r--   0        0        0     2321 2023-05-19 08:44:34.687525 squad_ds_utils-0.1.6/squad_ds_utils/recordings_fetcher.py
+-rw-r--r--   0        0        0      628 2023-05-19 08:44:34.687608 squad_ds_utils-0.1.6/squad_ds_utils/secrets.py
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 squad_ds_utils-0.1.6/PKG-INFO
```

### Comparing `squad_ds_utils-0.1.3/squad_ds_utils/parse.py` & `squad_ds_utils-0.1.6/squad_ds_utils/parse.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.3/squad_ds_utils/recordings_fetcher.py` & `squad_ds_utils-0.1.6/squad_ds_utils/recordings_fetcher.py`

 * *Files identical despite different names*

### Comparing `squad_ds_utils-0.1.3/squad_ds_utils/secrets.py` & `squad_ds_utils-0.1.6/squad_ds_utils/secrets.py`

 * *Files identical despite different names*

