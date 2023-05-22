# Comparing `tmp/databricks-aws-utils-1.2.1.tar.gz` & `tmp/databricks_aws_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks-aws-utils-1.2.1.tar", max compression
+gzip compressed data, was "databricks_aws_utils-1.3.0.tar", max compression
```

## Comparing `databricks-aws-utils-1.2.1.tar` & `databricks_aws_utils-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/LICENSE
--rw-r--r--   0        0        0      489 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/README.md
--rw-r--r--   0        0        0     2087 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/databricks_aws_utils/__init__.py
--rw-r--r--   0        0        0     9142 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/databricks_aws_utils/delta_table.py
--rw-r--r--   0        0        0     4331 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/databricks_aws_utils/rds.py
--rw-r--r--   0        0        0     2174 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/databricks_aws_utils/s3.py
--rw-r--r--   0        0        0     1499 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/databricks_aws_utils/session.py
--rw-r--r--   0        0        0      952 2023-03-22 14:26:39.458080 databricks-aws-utils-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 databricks-aws-utils-1.2.1/setup.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 databricks-aws-utils-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/LICENSE
+-rw-r--r--   0        0        0      489 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/README.md
+-rw-r--r--   0        0        0     2087 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/databricks_aws_utils/__init__.py
+-rw-r--r--   0        0        0    10565 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/databricks_aws_utils/delta_table.py
+-rw-r--r--   0        0        0     4331 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/databricks_aws_utils/rds.py
+-rw-r--r--   0        0        0     2174 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/databricks_aws_utils/s3.py
+-rw-r--r--   0        0        0     1499 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/databricks_aws_utils/session.py
+-rw-r--r--   0        0        0      959 2023-05-22 12:51:03.078545 databricks_aws_utils-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.0/setup.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.0/PKG-INFO
```

### Comparing `databricks-aws-utils-1.2.1/LICENSE` & `databricks_aws_utils-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks-aws-utils-1.2.1/databricks_aws_utils/__init__.py` & `databricks_aws_utils-1.3.0/databricks_aws_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-aws-utils-1.2.1/databricks_aws_utils/delta_table.py` & `databricks_aws_utils-1.3.0/databricks_aws_utils/delta_table.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from pyspark.sql.session import SparkSession
 
 from databricks_aws_utils import DatabrickAWSUtils
 
 
 class DeltaTableUtils(DatabrickAWSUtils):
     """
-        Delta Table AWS Integration Utils.
+    Delta Table AWS Integration Utils.
 
-        > This Delta Table integration only works if the Databricks use the AWS Glue as the Metastore
+    > This Delta Table integration only works if the Databricks use the AWS Glue as the Metastore
 
-        Args:
-            spark (`SparkSession`): spark session
-            name: (`str`): delta table name, must contain the database (e.g. `<database>.<table>`)
-            aws_region (`str`, optional): AWS region, default `us-east-1`
-            iam_role (`str`, optional): IAM Role ARN, if specified assumes the IAM role to perform the AWS API calls
-            aws_access_key_id (`str`, optional): Temporary AWS Access Key Id
-            aws_secret_access_key (`str`, optional): Temporary AWS Secret Access Key
-            aws_session_token (`str`, optional): Temporary AWS Session Token
+    Args:
+        spark (`SparkSession`): spark session
+        name: (`str`): delta table name, must contain the database (e.g. `<database>.<table>`)
+        aws_region (`str`, optional): AWS region, default `us-east-1`
+        iam_role (`str`, optional): IAM Role ARN, if specified assumes the IAM role to perform the AWS API calls
+        aws_access_key_id (`str`, optional): Temporary AWS Access Key Id
+        aws_secret_access_key (`str`, optional): Temporary AWS Secret Access Key
+        aws_session_token (`str`, optional): Temporary AWS Session Token
 
-        Features:
+    Features:
 
-        - Convert Databricks delta table to AWS Glue Format using symlink_format_manifest to allow the AWS Athena
-            or Presto to consume externally
+    - Convert Databricks delta table to AWS Glue Format using symlink_format_manifest to allow the AWS Athena
+        or Presto to consume externally
     """
 
     def __init__(
         self,
         spark: SparkSession,
         name: str,
         aws_region: Optional[str] = "us-east-1",
@@ -45,27 +45,70 @@
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token
         )
 
         self.spark = spark
         self.name = name
 
+    def to_athena_v3(self) -> None:
+        """
+        Dec 19, 2022, AWS announced the Athena V3 engine now supports Delta Lake tables.
+
+        https://aws.amazon.com/about-aws/whats-new/2022/12/athena-enhances-read-support-delta-lake-table-format/
+
+        However, there are some gotchas and requirements in the integrations.
+
+        - The table needs to have a table property called `table_type` with the value `DELTA`.
+        - AWS Glue should synchronize the columns and partitions with the Glue Catalog, however, for some reason \
+            the columns and partitions are not synchronized for all tables, so it is necessary to synchronize \
+            the columns and partitions manually.
+
+        This method adds the `table_type` property to the table and synchronize the columns and partitions.
+        """
+        db_name, table_name = self.name.split('.')
+        columns, partitions = self.schema_to_glue()
+        client = self.session.client('glue')
+        response = client.get_table(
+            DatabaseName=db_name,
+            Name=table_name
+        )
+
+        table = response['Table']
+        del table['CreateTime']
+        del table['UpdateTime']
+        del table['DatabaseName']
+        del table['IsRegisteredWithLakeFormation']
+        del table['CreatedBy']
+        del table['VersionId']
+        del table['CatalogId']
+
+        table['SerdeInfo']['Parameters']['table_type'] = 'DELTA'
+        table['StorageDescriptor']['Columns'] = columns
+        table['PartitionKeys'] = partitions
+
+        self.logger.info("Updating table")
+        client.update_table(
+            DatabaseName=db_name,
+            TableInput=table
+        )
+        self.logger.info("Table successfully updated")
+
     def to_athena(self, target_database: str, target_table: str) -> None:
         """
-            Converts a Delta table to external table using AWS Athena or Presto
-                format using `symlink_format_manifest`
+        Converts a Delta table to external table using AWS Athena or Presto
+            format using `symlink_format_manifest`
 
-            Presto Integration full documentation:
-            <https://docs.databricks.com/delta/presto-integration.html#limitations>
+        Presto Integration full documentation:
+        <https://docs.databricks.com/delta/presto-integration.html#limitations>
 
-            Args:
-                delta_table (`str`): delta table name
-                target_database (`str`): external database name
-                target_table (`str`): external table name
-                target_table_description (`str`, optional): external table description
+        Args:
+            delta_table (`str`): delta table name
+            target_database (`str`): external database name
+            target_table (`str`): external table name
+            target_table_description (`str`, optional): external table description
         """
 
         columns, partitions = self.schema_to_glue()
         location = self.get_location()
 
         table = DeltaTable.forName(self.spark, self.name)
         client = self.session.client('glue')
@@ -90,55 +133,55 @@
 
         if len(partitions) > 0:
             self.logger.info("Partitions detected, recovering partitions")
             self.spark.catalog.recoverPartitions(f"{target_database}.{target_table}")
 
     def get_table_name(self) -> str:
         """
-            Get delta table name without the database name
+        Get delta table name without the database name
 
-            Returns:
-                `str`: table name
+        Returns:
+            `str`: table name
         """
         return self.name.split('.')[1]
 
     def get_database_name(self) -> str:
         """
-            Get database name from the delta table
+        Get database name from the delta table
 
-            Returns:
-                `str`: database name
+        Returns:
+            `str`: database name
         """
         if '.' not in self.name:
             raise RuntimeError(f"Cannot extract database name from the delta table name '{self.name}'")
 
         return self.name.split('.')[0]
 
     def get_location(self) -> str:
         """
-            Get delta table location
+        Get delta table location
 
-            Returns:
-                `str`: delta table location
+        Returns:
+            `str`: delta table location
         """
         client = self.session.client('glue')
 
         response = client.get_table(
             DatabaseName=self.get_database_name(),
             Name=self.get_table_name()
         )
 
         return response['Table']['StorageDescriptor']['Location']
 
     def schema_to_glue(self) -> Tuple[List[dict], List[dict]]:
         """
-            Extracts the delta table schema and returns in the AWS Glue Format
+        Extracts the delta table schema and returns in the AWS Glue Format
 
-            Returns:
-                `Tuple[List[dict], List[dict]]` columns and partitions
+        Returns:
+            `Tuple[List[dict], List[dict]]` columns and partitions
         """
         columns = []
         partitions = []
         self.logger.info("Extracting table schema...")
         delta_columns = self.spark.catalog.listColumns(self.name)
 
         for column in delta_columns:
@@ -161,50 +204,49 @@
         database_name: str,
         table_name: str,
         columns: List[dict],
         partitions: List[dict],
         location: str,
     ) -> None:
         """
-            Creates the AWS Glue Table
+        Creates the AWS Glue Table
 
-            Args:
-                database_name (`str`): database name
-                table_name (`str`): table name
-                columns (`List[dict]`): schema columns
-                partitions (`List[dict]`): partitions definition
-                location (`str`): delta table location
-                table_description (`str`, optional): table description
+        Args:
+            database_name (`str`): database name
+            table_name (`str`): table name
+            columns (`List[dict]`): schema columns
+            partitions (`List[dict]`): partitions definition
+            location (`str`): delta table location
+            table_description (`str`, optional): table description
         """
         client = self.session.client('glue')
         self.logger.info(f"Creating table '{database_name}.{table_name}'")
         client.create_table(
             DatabaseName=database_name,
             TableInput=self._generate_glue_table_input(table_name, columns, partitions, location)
         )
         self.logger.info(f"Table '{database_name}.{table_name}' successfully created")
 
     def _update_glue_table(
         self,
         table: dict,
         columns: List[dict],
         partitions: List[dict],
-        location: str
+        location: str,
     ):
         """
-            Updates the AWS Glue Table
+        Updates the AWS Glue Table
 
-            Args:
-                session (`Session`): boto3 session
-                database_name (`str`): database name
-                table (`dict`): AWS Glue GetTable operation response
-                columns (`List[dict]`): schema columns
-                partitions (`List[dict]`): partitions definition
-                location (`str`): delta table location
-                table_description (`str`, optional): table description
+        Args:
+            session (`Session`): boto3 session
+            database_name (`str`): database name
+            table (`dict`): AWS Glue GetTable operation response
+            columns (`List[dict]`): schema columns
+            partitions (`List[dict]`): partitions definition
+            location (`str`): delta table location
         """
         client = self.session.client('glue')
         database_name = table['DatabaseName']
         table_name = table['Name']
 
         self.logger.info(f"Updating table '{database_name}.{table_name}'")
         client.update_table(
@@ -217,24 +259,24 @@
         self,
         table_name: str,
         columns: List[dict],
         partitions: List[dict],
         location: str
     ) -> Dict[str, Any]:
         """
-            Builds the AWS Glue TableInput object.
+        Builds the AWS Glue TableInput object.
 
-            Args:
-                table_name (`str`): table name
-                columns (`List[dict]`): schema columns
-                partitions (`List[dict]`): partitions definition
-                location (`str`): delta table location
+        Args:
+            table_name (`str`): table name
+            columns (`List[dict]`): schema columns
+            partitions (`List[dict]`): partitions definition
+            location (`str`): delta table location
 
-            Returns:
-                `Dict[str, Any]`: AWS Glue TableInput object
+        Returns:
+            `Dict[str, Any]`: AWS Glue TableInput object
         """
         return {
             'Name': table_name,
             'Description': '',
             'StorageDescriptor': {
                 'Columns': columns,
                 'Location': f'{location}/_symlink_format_manifest',
```

### Comparing `databricks-aws-utils-1.2.1/databricks_aws_utils/rds.py` & `databricks_aws_utils-1.3.0/databricks_aws_utils/rds.py`

 * *Files identical despite different names*

### Comparing `databricks-aws-utils-1.2.1/databricks_aws_utils/s3.py` & `databricks_aws_utils-1.3.0/databricks_aws_utils/s3.py`

 * *Files identical despite different names*

### Comparing `databricks-aws-utils-1.2.1/databricks_aws_utils/session.py` & `databricks_aws_utils-1.3.0/databricks_aws_utils/session.py`

 * *Files identical despite different names*

### Comparing `databricks-aws-utils-1.2.1/pyproject.toml` & `databricks_aws_utils-1.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "databricks-aws-utils"
-version = "1.2.1"
+version = "1.3.0"
 description = "Databricks AWS Utils"
 license = "Proprietary"
 authors = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 maintainers = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 readme = "README.md"
 repository = "https://github.com/lucasvieirasilva/databricks-aws-utils"
 
   [[tool.poetry.packages]]
   include = "databricks_aws_utils"
 
   [tool.poetry.dependencies]
   python = ">=3.7,<3.10"
 
-  [tool.poetry.dev-dependencies]
+  [tool.poetry.group.dev.dependencies]
   flake8 = "3.9.2"
   autopep8 = "1.5.7"
-  delta-spark = "1.0.0"
-  pyspark = "3.1.2"
+  delta-spark = "^2.3.0"
+  pyspark = "3.3.2"
   boto3 = "1.20.5"
   pydoc-markdown = "4.3.2"
 
 [build-system]
 requires = [ "poetry-core==1.0.3" ]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `databricks-aws-utils-1.2.1/setup.py` & `databricks_aws_utils-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['databricks_aws_utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'databricks-aws-utils',
-    'version': '1.2.1',
+    'version': '1.3.0',
     'description': 'Databricks AWS Utils',
     'long_description': '# Databricks AWS Utils\n\nDatabricks AWS Utils is a library to abstract Databricks integration with AWS Services\n\n## Features\n\n- Convert Delta Table to be consumed by AWS Athena with Schema evolution\n- Run queries against AWS RDS using AWS Secrets Manager to retrive the connection properties and returns as Spark DataFrame\n\n## Install\n\n`pip install databricks-aws-utils`\n\n## Contributing\n\n- See our [Contributing Guide](CONTRIBUTING.md)\n\n## Change Log\n\n- See our [Change Log](CHANGELOG.md)\n',
     'author': 'Lucas Vieira',
     'author_email': 'lucas.vieira94@outlook.com',
     'maintainer': 'Lucas Vieira',
     'maintainer_email': 'lucas.vieira94@outlook.com',
     'url': 'https://github.com/lucasvieirasilva/databricks-aws-utils',
```

### Comparing `databricks-aws-utils-1.2.1/PKG-INFO` & `databricks_aws_utils-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-aws-utils
-Version: 1.2.1
+Version: 1.3.0
 Summary: Databricks AWS Utils
 Home-page: https://github.com/lucasvieirasilva/databricks-aws-utils
 License: Proprietary
 Author: Lucas Vieira
 Author-email: lucas.vieira94@outlook.com
 Maintainer: Lucas Vieira
 Maintainer-email: lucas.vieira94@outlook.com
```

