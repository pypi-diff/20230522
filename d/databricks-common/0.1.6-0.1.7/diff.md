# Comparing `tmp/databricks_common-0.1.6.tar.gz` & `tmp/databricks_common-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.6.tar", max compression
+gzip compressed data, was "databricks_common-0.1.7.tar", max compression
```

## Comparing `databricks_common-0.1.6.tar` & `databricks_common-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.6/README.md
--rw-r--r--   0        0        0       22 2023-05-22 16:36:42.545590 databricks_common-0.1.6/databricks_common/__init__.py
--rw-r--r--   0        0        0     9342 2023-05-22 16:38:12.754231 databricks_common-0.1.6/databricks_common/common.py
--rw-r--r--   0        0        0      258 2023-05-22 15:12:32.530513 databricks_common-0.1.6/databricks_common/main.py
--rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.6/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.6/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.6/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      740 2023-05-22 16:36:47.561484 databricks_common-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-22 19:24:47.486951 databricks_common-0.1.7/databricks_common/__init__.py
+-rw-r--r--   0        0        0     9354 2023-05-22 19:24:27.859793 databricks_common-0.1.7/databricks_common/common.py
+-rw-r--r--   0        0        0      258 2023-05-22 15:12:32.530513 databricks_common-0.1.7/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.7/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.7/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.7/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      740 2023-05-22 19:24:39.005870 databricks_common-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.7/PKG-INFO
```

### Comparing `databricks_common-0.1.6/databricks_common/common.py` & `databricks_common-0.1.7/databricks_common/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             USING DELTA
             COMMENT '{comment}'
             """
         )
 
     def create_parents_if_not_exists(self) -> None:
         MetastoreCatalog(self.catalog).create_if_not_exists()
-        MetastoreSchema(self.schema_ref).create_if_not_exists()
+        MetastoreSchema.from_string(self.schema_ref).create_if_not_exists()
 
     def describe(self) -> None:
         spark.sql(f"DESC TABLE {self.ref}").display()
 
     def describe_extended(self) -> None:
         spark.sql(f"DESC EXTENDED {self.ref}").display()
```

### Comparing `databricks_common-0.1.6/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.7/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_common-0.1.6/pyproject.toml` & `databricks_common-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-common"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["Xavier Armitage <xtarmitage@gmail.com>"]
 readme = "README.md"
 packages = [{include = "databricks_common"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

