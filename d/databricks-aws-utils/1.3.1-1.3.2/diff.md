# Comparing `tmp/databricks_aws_utils-1.3.1.tar.gz` & `tmp/databricks_aws_utils-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_aws_utils-1.3.1.tar", max compression
+gzip compressed data, was "databricks_aws_utils-1.3.2.tar", max compression
```

## Comparing `databricks_aws_utils-1.3.1.tar` & `databricks_aws_utils-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/LICENSE
--rw-r--r--   0        0        0      489 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/README.md
--rw-r--r--   0        0        0     2087 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/databricks_aws_utils/__init__.py
--rw-r--r--   0        0        0    10586 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/databricks_aws_utils/delta_table.py
--rw-r--r--   0        0        0     4331 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/databricks_aws_utils/rds.py
--rw-r--r--   0        0        0     2174 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/databricks_aws_utils/s3.py
--rw-r--r--   0        0        0     1499 2023-05-22 13:25:42.955845 databricks_aws_utils-1.3.1/databricks_aws_utils/session.py
--rw-r--r--   0        0        0      959 2023-05-22 13:25:42.959845 databricks_aws_utils-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.1/setup.py
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-22 13:42:27.072530 databricks_aws_utils-1.3.2/LICENSE
+-rw-r--r--   0        0        0      489 2023-05-22 13:42:27.072530 databricks_aws_utils-1.3.2/README.md
+-rw-r--r--   0        0        0     2087 2023-05-22 13:42:27.072530 databricks_aws_utils-1.3.2/databricks_aws_utils/__init__.py
+-rw-r--r--   0        0        0    10620 2023-05-22 13:42:27.072530 databricks_aws_utils-1.3.2/databricks_aws_utils/delta_table.py
+-rw-r--r--   0        0        0     4331 2023-05-22 13:42:27.072530 databricks_aws_utils-1.3.2/databricks_aws_utils/rds.py
+-rw-r--r--   0        0        0     2174 2023-05-22 13:42:27.072530 databricks_aws_utils-1.3.2/databricks_aws_utils/s3.py
+-rw-r--r--   0        0        0     1499 2023-05-22 13:42:27.076530 databricks_aws_utils-1.3.2/databricks_aws_utils/session.py
+-rw-r--r--   0        0        0      959 2023-05-22 13:42:27.076530 databricks_aws_utils-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.2/setup.py
+-rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 databricks_aws_utils-1.3.2/PKG-INFO
```

### Comparing `databricks_aws_utils-1.3.1/LICENSE` & `databricks_aws_utils-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.1/databricks_aws_utils/__init__.py` & `databricks_aws_utils-1.3.2/databricks_aws_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.1/databricks_aws_utils/delta_table.py` & `databricks_aws_utils-1.3.2/databricks_aws_utils/delta_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,18 @@
         del table['UpdateTime']
         del table['DatabaseName']
         del table['IsRegisteredWithLakeFormation']
         del table['CreatedBy']
         del table['VersionId']
         del table['CatalogId']
 
-        table['StorageDescriptor']['SerdeInfo']['Parameters']['table_type'] = 'DELTA'
+        params = table['Parameters'] or {}
+        params['table_type'] = 'DELTA'
+
+        table['Parameters'] = params
         table['StorageDescriptor']['Columns'] = columns
         table['PartitionKeys'] = partitions
 
         self.logger.info("Updating table")
         client.update_table(
             DatabaseName=db_name,
             TableInput=table
```

### Comparing `databricks_aws_utils-1.3.1/databricks_aws_utils/rds.py` & `databricks_aws_utils-1.3.2/databricks_aws_utils/rds.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.1/databricks_aws_utils/s3.py` & `databricks_aws_utils-1.3.2/databricks_aws_utils/s3.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.1/databricks_aws_utils/session.py` & `databricks_aws_utils-1.3.2/databricks_aws_utils/session.py`

 * *Files identical despite different names*

### Comparing `databricks_aws_utils-1.3.1/pyproject.toml` & `databricks_aws_utils-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-aws-utils"
-version = "1.3.1"
+version = "1.3.2"
 description = "Databricks AWS Utils"
 license = "Proprietary"
 authors = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 maintainers = [ "Lucas Vieira <lucas.vieira94@outlook.com>" ]
 readme = "README.md"
 repository = "https://github.com/lucasvieirasilva/databricks-aws-utils"
```

### Comparing `databricks_aws_utils-1.3.1/setup.py` & `databricks_aws_utils-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['databricks_aws_utils']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'databricks-aws-utils',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'Databricks AWS Utils',
     'long_description': '# Databricks AWS Utils\n\nDatabricks AWS Utils is a library to abstract Databricks integration with AWS Services\n\n## Features\n\n- Convert Delta Table to be consumed by AWS Athena with Schema evolution\n- Run queries against AWS RDS using AWS Secrets Manager to retrive the connection properties and returns as Spark DataFrame\n\n## Install\n\n`pip install databricks-aws-utils`\n\n## Contributing\n\n- See our [Contributing Guide](CONTRIBUTING.md)\n\n## Change Log\n\n- See our [Change Log](CHANGELOG.md)\n',
     'author': 'Lucas Vieira',
     'author_email': 'lucas.vieira94@outlook.com',
     'maintainer': 'Lucas Vieira',
     'maintainer_email': 'lucas.vieira94@outlook.com',
     'url': 'https://github.com/lucasvieirasilva/databricks-aws-utils',
```

### Comparing `databricks_aws_utils-1.3.1/PKG-INFO` & `databricks_aws_utils-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-aws-utils
-Version: 1.3.1
+Version: 1.3.2
 Summary: Databricks AWS Utils
 Home-page: https://github.com/lucasvieirasilva/databricks-aws-utils
 License: Proprietary
 Author: Lucas Vieira
 Author-email: lucas.vieira94@outlook.com
 Maintainer: Lucas Vieira
 Maintainer-email: lucas.vieira94@outlook.com
```

