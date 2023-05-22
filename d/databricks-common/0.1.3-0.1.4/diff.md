# Comparing `tmp/databricks_common-0.1.3.tar.gz` & `tmp/databricks_common-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.3.tar", max compression
+gzip compressed data, was "databricks_common-0.1.4.tar", max compression
```

## Comparing `databricks_common-0.1.3.tar` & `databricks_common-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.3/README.md
--rw-r--r--   0        0        0       22 2023-05-15 11:54:03.421548 databricks_common-0.1.3/databricks_common/__init__.py
--rw-r--r--   0        0        0     8846 2023-05-15 11:42:32.515474 databricks_common-0.1.3/databricks_common/common.py
--rw-r--r--   0        0        0      195 2023-05-15 10:35:58.597274 databricks_common-0.1.3/databricks_common/main.py
--rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.3/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.3/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.3/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      740 2023-05-15 11:53:52.114143 databricks_common-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2023-05-22 14:30:39.713492 databricks_common-0.1.4/databricks_common/__init__.py
+-rw-r--r--   0        0        0     9239 2023-05-19 04:17:35.507741 databricks_common-0.1.4/databricks_common/common.py
+-rw-r--r--   0        0        0      245 2023-05-19 02:46:46.079608 databricks_common-0.1.4/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.4/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.4/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.4/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      740 2023-05-22 14:30:34.593425 databricks_common-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.4/PKG-INFO
```

### Comparing `databricks_common-0.1.3/databricks_common/common.py` & `databricks_common-0.1.4/databricks_common/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     def __init__(self, name: str, catalog: str, schema: str) -> None:
         self.name = name
         self.catalog = catalog
         self.schema = schema
         self.ref = self._get_ref()
         self.short_ref = self._get_short_ref()
+        self.schema_ref = self._get_schema_ref()
 
     def __repr__(self) -> str:
         cls = self.__class__.__name__
         return f"{cls}({self.ref})"
 
     @classmethod
     def from_string(cls, ref: str) -> "MetastoreTable":
@@ -81,45 +82,44 @@
             f"""
             CREATE TABLE {self.ref}
             USING DELTA
             COMMENT '{comment}'
             """
         )
 
+    def create_parents_if_not_exists(self) -> None:
+        MetastoreCatalog(self.catalog).create_if_not_exists()
+        MetastoreSchema(self.schema_ref).create_if_not_exists()
+
     def describe(self) -> None:
-        """
-        Function to describe a table in Unity Metastore.
-        """
         spark.sql(f"DESC TABLE {self.ref}").display()
 
     def describe_extended(self) -> None:
-        """
-        Function to describe a table in Unity Metastore.
-        """
         spark.sql(f"DESC EXTENDED {self.ref}").display()
 
     def describe_history(self) -> None:
-        """
-        Function to describe a schema in Unity Metastore.
-        """
         spark.sql(f"DESC HISTORY {self.ref}").display()
 
     def read(self):  # noqa
-        """
-        Function to read a table from the catalog.
-        """
         return spark.read.table(self.ref)
 
     def _get_ref(self) -> str:
         return f"{self.catalog}.{self.schema}.{self.name}"
 
     def _get_short_ref(self) -> str:
         return f"{self.schema}.{self.name}"
 
-    def _get_checkpoint_location(self) -> str:
+    def _get_schema_ref(self) -> str:
+        return f"{self.catalog}.{self.schema}"
+
+    def _get_checkpoint_location(
+        self,
+    ) -> (
+        str
+    ):  # TODO: Still in dev. Need to understand if a table has metadata about it's checkpoint location.
         try:
             return self.checkpoint_location
         except AttributeError:
             return f"{self.catalog}.chkpts/{self.schema}/{self.name}"
 
 
 class MetastoreCatalog:
@@ -152,34 +152,33 @@
     def create(self, comment: str = "") -> None:
         spark.sql(f"CREATE CATALOG {self.name} COMMENT '{comment}'")
 
     def create_if_not_exists(self, comment: str = "") -> None:
         spark.sql(f"CREATE CATALOG IF NOT EXISTS {self.name} COMMENT '{comment}'")
 
     def create_schema(self, schema_name: str, comment: str = "") -> None:
-        self.set()
-        spark.sql(f"CREATE SCHEMA {schema_name} COMMENT '{comment}'")
+        spark.sql(f"CREATE SCHEMA {self.name}.{schema_name} COMMENT '{comment}'")
 
     def create_catalog_in_managed_location(
-        self, container_uri: str = None, container_dir: str = None, comment: str = ""
+        self, location_path: str = None, comment: str = ""
     ) -> None:
         spark.sql(
             f"""
             CREATE CATALOG {self.name}
-            MANAGED LOCATION '{container_uri}/{container_dir}/'
+            MANAGED LOCATION '{location_path}'
             COMMENT '{comment}' 
             """
         )
 
     def demo_create_managed_external_catalog(self) -> None:  # TODO: Convert to test
         """
         Function for demo purposes.
         """
         self.create_catalog_in_managed_location(
-            container_uri="abfss://xavierarmitage-container@oneenvadls.dfs.core.windows.net",
+            location_path="abfss://xavierarmitage-container@oneenvadls.dfs.core.windows.net",
             container_dir="lake23",
             comment="Demo comment",
         )
 
     def describe(self) -> None:
         spark.sql(f"DESC CATALOG {self.name}").display()
 
@@ -218,22 +217,30 @@
 
 
 class MetastoreSchema:
     """
     Class to represent a schema in Unity Metastore.
     """
 
-    def __init__(self, catalog: str | MetastoreCatalog, name: str) -> None:
+    def __init__(self, name: str, catalog: str | MetastoreCatalog) -> None:
         if isinstance(catalog, MetastoreCatalog):
             self.catalog = catalog.name
         else:
             self.catalog = catalog
         self.name = name
         self.ref = self._get_ref()
 
+    @classmethod
+    def from_string(cls, ref: str) -> "MetastoreSchema":
+        """
+        Alternative constructor to initialise an MetastoreSchema from a string.
+        """
+        cat, schema = ref.split(".")
+        return cls(name=schema, catalog=cat)
+
     def _set_catalog(self) -> None:
         """
         Function to set the current catalog.
         """
         MetastoreCatalog(self.catalog).set()
 
     def check_exists(self) -> bool:
@@ -241,14 +248,15 @@
         Function to check if a schema exists in Unity Metastore.
         """
         # TODO: There might be a more direct way to do this
         try:
             spark.sql(f"DESC SCHEMA {self.catalog}.{self.name}")
             return True
         except Exception as e:
+            # TODO: update to make exception more specific
             return False
 
     def create(self, comment: str = "") -> None:
         spark.sql(f"CREATE SCHEMA {self.ref} COMMENT '{comment}'")
 
     def create_if_not_exists(self, comment: str = "") -> None:
         spark.sql(f"CREATE SCHEMA IF NOT EXISTS {self.ref} COMMENT '{comment}'")
```

### Comparing `databricks_common-0.1.3/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.4/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_common-0.1.3/pyproject.toml` & `databricks_common-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-common"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Xavier Armitage <xtarmitage@gmail.com>"]
 readme = "README.md"
 packages = [{include = "databricks_common"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

