# Comparing `tmp/databricks_common-0.1.5.tar.gz` & `tmp/databricks_common-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.5.tar", max compression
+gzip compressed data, was "databricks_common-0.1.6.tar", max compression
```

## Comparing `databricks_common-0.1.5.tar` & `databricks_common-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.5/README.md
--rw-r--r--   0        0        0       22 2023-05-22 15:04:09.625718 databricks_common-0.1.5/databricks_common/__init__.py
--rw-r--r--   0        0        0     9202 2023-05-22 15:03:18.376728 databricks_common-0.1.5/databricks_common/common.py
--rw-r--r--   0        0        0      245 2023-05-19 02:46:46.079608 databricks_common-0.1.5/databricks_common/main.py
--rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.5/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.5/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.5/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      740 2023-05-22 15:04:06.370456 databricks_common-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.6/README.md
+-rw-r--r--   0        0        0       22 2023-05-22 16:36:42.545590 databricks_common-0.1.6/databricks_common/__init__.py
+-rw-r--r--   0        0        0     9342 2023-05-22 16:38:12.754231 databricks_common-0.1.6/databricks_common/common.py
+-rw-r--r--   0        0        0      258 2023-05-22 15:12:32.530513 databricks_common-0.1.6/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.6/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.6/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.6/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      740 2023-05-22 16:36:47.561484 databricks_common-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.6/PKG-INFO
```

### Comparing `databricks_common-0.1.5/databricks_common/common.py` & `databricks_common-0.1.6/databricks_common/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,19 @@
         ) as e:  # TODO: Choose specific exception in case there is a specific error
             return False
 
     def create(self, comment: str = "") -> None:
         spark.sql(f"CREATE CATALOG {self.name} COMMENT '{comment}'")
 
     def create_if_not_exists(self, comment: str = "") -> None:
-        spark.sql(f"CREATE CATALOG IF NOT EXISTS {self.name} COMMENT '{comment}'")
+        if self.check_exists():
+            # Had to include explicit check due to QUOTA_EXCEEDED error.
+            pass
+        else:
+            spark.sql(f"CREATE CATALOG IF NOT EXISTS {self.name} COMMENT '{comment}'")
 
     def create_schema(self, schema_name: str, comment: str = "") -> None:
         spark.sql(f"CREATE SCHEMA {self.name}.{schema_name} COMMENT '{comment}'")
 
     def create_catalog_in_managed_location(
         self, location_path: str = None, comment: str = ""
     ) -> None:
```

### Comparing `databricks_common-0.1.5/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.6/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_common-0.1.5/pyproject.toml` & `databricks_common-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-common"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Xavier Armitage <xtarmitage@gmail.com>"]
 readme = "README.md"
 packages = [{include = "databricks_common"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

