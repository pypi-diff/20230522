# Comparing `tmp/spalah-1.0.1.tar.gz` & `tmp/spalah-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spalah-1.0.1.tar", max compression
+gzip compressed data, was "spalah-1.0.2.tar", max compression
```

## Comparing `spalah-1.0.1.tar` & `spalah-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1217 2022-07-09 12:46:46.000000 spalah-1.0.1/LICENSE
--rw-r--r--   0        0        0     5356 2023-05-20 17:48:37.703026 spalah-1.0.1/README.md
--rw-r--r--   0        0        0     1376 2023-05-21 15:07:41.772148 spalah-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      118 2022-07-09 12:46:46.000000 spalah-1.0.1/spalah/__init__.py
--rw-r--r--   0        0        0      177 2023-05-20 17:33:36.517825 spalah-1.0.1/spalah/dataframe/__init__.py
--rw-r--r--   0        0        0    23329 2023-05-20 17:33:36.518032 spalah-1.0.1/spalah/dataframe/dataframe.py
--rw-r--r--   0        0        0     8813 2023-05-20 17:33:36.518182 spalah-1.0.1/spalah/dataset/DeltaProperty.py
--rw-r--r--   0        0        0      144 2023-05-20 17:33:36.518286 spalah-1.0.1/spalah/dataset/__init__.py
--rw-r--r--   0        0        0      999 2023-05-20 17:33:36.518399 spalah-1.0.1/spalah/dataset/dbfs.py
--rw-r--r--   0        0        0       58 2023-05-20 17:33:36.518507 spalah-1.0.1/spalah/shared/__init__.py
--rw-r--r--   0        0        0      407 2023-05-20 17:33:36.518606 spalah-1.0.1/spalah/shared/logging.py
--rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 spalah-1.0.1/setup.py
--rw-r--r--   0        0        0     6328 1970-01-01 00:00:00.000000 spalah-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1217 2022-07-09 12:46:46.000000 spalah-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5368 2023-05-22 20:10:03.937616 spalah-1.0.2/README.md
+-rw-r--r--   0        0        0     1376 2023-05-22 20:10:10.060793 spalah-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2022-07-09 12:46:46.000000 spalah-1.0.2/spalah/__init__.py
+-rw-r--r--   0        0        0      177 2023-05-20 17:33:36.517825 spalah-1.0.2/spalah/dataframe/__init__.py
+-rw-r--r--   0        0        0    23329 2023-05-20 17:33:36.518032 spalah-1.0.2/spalah/dataframe/dataframe.py
+-rw-r--r--   0        0        0     8834 2023-05-22 20:10:03.938833 spalah-1.0.2/spalah/dataset/DeltaTableConfig.py
+-rw-r--r--   0        0        0      156 2023-05-22 20:10:03.938956 spalah-1.0.2/spalah/dataset/__init__.py
+-rw-r--r--   0        0        0      999 2023-05-20 17:33:36.518399 spalah-1.0.2/spalah/dataset/dbfs.py
+-rw-r--r--   0        0        0       58 2023-05-20 17:33:36.518507 spalah-1.0.2/spalah/shared/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-20 17:33:36.518606 spalah-1.0.2/spalah/shared/logging.py
+-rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 spalah-1.0.2/setup.py
+-rw-r--r--   0        0        0     6340 1970-01-01 00:00:00.000000 spalah-1.0.2/PKG-INFO
```

### Comparing `spalah-1.0.1/LICENSE` & `spalah-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spalah-1.0.1/README.md` & `spalah-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -154,30 +154,30 @@
 ```
 
 ## spalah.dataset
 
 ### Get delta table properties
 
 ```python
-from spalah.dataset import DeltaProperty
+from spalah.dataset import DeltaTableConfig
 
-dp = DeltaProperty(table_path="/path/dataset")
+dp = DeltaTableConfig(table_path="/path/dataset")
 
 print(dp.properties) 
 
 # output: 
 # {'delta.deletedFileRetentionDuration': 'interval 15 days'}
 ```
 
 ### Set delta table properties
 
 ```python
-rom spalah.dataset import DeltaProperty
+rom spalah.dataset import DeltaTableConfig
 
-dp = DeltaProperty(table_path="/path/dataset")
+dp = DeltaTableConfig(table_path="/path/dataset")
 
 dp.properties = {
     "delta.logRetentionDuration": "interval 10 days",
     "delta.deletedFileRetentionDuration": "interval 15 days"
 }
 
 ```
```

### Comparing `spalah-1.0.1/pyproject.toml` & `spalah-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "spalah"
-version = "1.0.1"
+version = "1.0.2"
 description = "Spalah is a set of PySpark dataframe helpers"
 homepage = "https://github.com/avolok/spalah"
 authors = ["Alex Volok <alexandr.volok@gmail.com>"]
 license = "MIT license"
 keywords = ["spalah"]
 classifiers = ["Intended Audience :: Developers", "License :: OSI Approved :: MIT License", "Natural Language :: English", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3.7", "Programming Language :: Python :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10"]
 readme = "README.md"
```

### Comparing `spalah-1.0.1/spalah/dataframe/dataframe.py` & `spalah-1.0.2/spalah/dataframe/dataframe.py`

 * *Files identical despite different names*

### Comparing `spalah-1.0.1/spalah/dataset/DeltaProperty.py` & `spalah-1.0.2/spalah/dataset/DeltaTableConfig.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Union
 from spalah.shared.logging import get_logger
 
 
 logger = get_logger(__name__)
 
 
-class DeltaProperty:
+class DeltaTableConfig:
     """
     Manages Delta Table properties, constraints, etc.
 
 
     Attributes:
         keep_existing_properties (bool): Preserves existing table properties if they are not
                                                 in the input value. Defaults to False
@@ -35,16 +35,16 @@
             spark_session: (SparkSession, optional)  The current spark context.
         Raises:
             ValueError: if values for both 'table_path' and 'table_name' provided
                         provide values to one of them
             ValueError: if values for neither 'table_path' nor 'table_name' provided
                         provide values to one of them
         Examples:
-            >>> from spalah.datalake import DeltaProperty
-            >>> dp = DeltaProperty(table_path="/path/dataset")
+            >>> from spalah.datalake import DeltaTableConfig
+            >>> dp = DeltaTableConfig(table_path="/path/dataset")
             >>> print(dp.properties)
             {'delta.deletedFileRetentionDuration': 'interval 15 days'}
         """
 
         self.spark_session = (
             SparkSession.getActiveSession() if not spark_session else spark_session
         )
@@ -88,16 +88,16 @@
     def properties(self) -> Union[dict, None]:
         """Gets/sets dataset's delta table properties.
 
         Args:
             value (dict):  An input dictionary in the format: `{"property_name": "value"}`
 
         Examples:
-            >>> from spalah.datalake import DeltaProperty
-            >>> dp = DeltaProperty(table_path="/path/dataset")
+            >>> from spalah.datalake import DeltaTableConfig
+            >>> dp = DeltaTableConfig(table_path="/path/dataset")
             >>>
             >>> # get existing properties
             >>> print(dp.properties)
             {'delta.deletedFileRetentionDuration': 'interval 15 days'}
             >>>
             >>> # Adjust the property value from 15 to 30 days
             >>> dp.properties = {'delta.deletedFileRetentionDuration': 'interval 30 days'}
@@ -160,16 +160,16 @@
     def check_constraints(self) -> Union[dict, None]:
         """Gets/sets dataset's delta table check constraints.
 
         Args:
             value (dict):  An input dictionary in the format: `{"property_name": "value"}`
 
         Examples:
-            >>> from spalah.datalake import DeltaProperty
-            >>> dp = DeltaProperty(table_path="/path/dataset")
+            >>> from spalah.datalake import DeltaTableConfig
+            >>> dp = DeltaTableConfig(table_path="/path/dataset")
             >>>
             >>> # get existing constraints
             >>> print(dp.check_constraints)
             {}
             >>>
             >>> # Add a new check constraint
             >>> dp.check_constraints = {'id_is_not_null': 'id is not null'}
```

### Comparing `spalah-1.0.1/spalah/dataset/dbfs.py` & `spalah-1.0.2/spalah/dataset/dbfs.py`

 * *Files identical despite different names*

### Comparing `spalah-1.0.1/setup.py` & `spalah-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['delta-spark>=2.1.0,<2.4', 'pyspark>=3.2.0,<4']
 
 setup_kwargs = {
     'name': 'spalah',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Spalah is a set of PySpark dataframe helpers',
-    'long_description': '# spalah\n\nSpalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.\n\nThe word "spalah" means "spark" in Ukrainian 🇺🇦 \n\n# Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.\n\n```bash\npip install spalah\n```\n\n# Examples of use\nSpalah currently has two different groups of helpers: `dataframe` and `datalake`.\n\n## spalah.dataframe\n\n### slice_dataframe\n\n```python\nfrom spalah.dataframe import slice_dataframe\n\ndf = spark.sql(\n    \'SELECT 1 as ID, "John" AS Name, struct("line1" AS Line1, "line2" AS Line2) AS Address\'\n)\ndf.printSchema()\n\n""" output:\nroot\n |-- ID: integer (nullable = false)\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n |    |-- Line2: string (nullable = false)\n"""\n\n# Create a new dataframe by cutting of root and nested attributes\ndf_result = slice_dataframe(\n    input_dataframe=df,\n    columns_to_include=["Name", "Address"],\n    columns_to_exclude=["Address.Line2"]\n)\ndf_result.printSchema()\n\n""" output:\nroot\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n"""\n```\n\nBeside of nested regular structs it also supported slicing of structs in arrays, including multiple levels of nesting\n\n\n### flatten_schema\n\n```python\nfrom spalah.dataframe import flatten_schema\n\n# Pass the sample dataframe to get the list of all attributes as single dimension list\nflatten_schema(df_complex_schema.schema)\n\n""" output:\n[\'ID\', \'Name\', \'Address.Line1\', \'Address.Line2\']\n"""\n\n\n# Alternatively, the function can return data types of the attributes\nflatten_schema(\n    schema=df_complex_schema.schema,\n    include_datatype=True\n)\n\n""" output:\n[\n    (\'ID\', \'IntegerType\'),\n    (\'Name\', \'StringType\'),\n    (\'Address.Line1\', \'StringType\'),\n    (\'Address.Line2\', \'StringType\')\n]\n"""\n```\n\n### script_dataframe\n\n```python\nfrom spalah.dataframe import script_dataframe\n\nscript = script_dataframe(df)\n\nprint(script)\n\n""" output:\nfrom pyspark.sql import Row\nimport datetime\nfrom decimal import Decimal\nfrom pyspark.sql.types import *\n\n# Scripted data and schema:\n__data = [Row(ID=1, Name=\'John\', Address=Row(Line1=\'line1\', Line2=\'line2\'))]\n\n__schema = {\'type\': \'struct\', \'fields\': [{\'name\': \'ID\', \'type\': \'integer\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Name\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Address\', \'type\': {\'type\': \'struct\', \'fields\': [{\'name\': \'Line1\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Line2\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}]}, \'nullable\': False, \'metadata\': {}}]}\n\noutcome_dataframe = spark.createDataFrame(__data, StructType.fromJson(__schema))\n"""\n```\n\n### SchemaComparer\n\n```python\nfrom spalah.dataframe import SchemaComparer\n\nschema_comparer = SchemaComparer(\n    source_schema = df_source.schema,\n    target_schema = df_target.schema\n)\n\nschema_comparer.compare()\n\n# The comparison results are stored in the class instance properties `matched` and `not_matched`\n\n# Contains a list of matched columns:\nschema_comparer.matched\n\n""" output:\n[MatchedColumn(name=\'Address.Line1\',  data_type=\'StringType\')]\n"""\n\n# Contains a list of all not matched columns with a reason as description of non-match:\nschema_comparer.not_matched\n\n""" output:\n[\n    NotMatchedColumn(\n        name=\'name\', \n        data_type=\'StringType\', \n        reason="The column exists in source and target schemas but it\'s name is case-mismatched"\n    ),\n    NotMatchedColumn(\n        name=\'ID\', \n        data_type=\'IntegerType <=> StringType\', \n        reason=\'The column exists in source and target schemas but it is not matched by a data type\'\n    ),\n    NotMatchedColumn(\n        name=\'Address.Line2\', \n        data_type=\'StringType\', \n        reason=\'The column exists only in the source schema\'\n    )\n]\n"""\n```\n\n## spalah.dataset\n\n### Get delta table properties\n\n```python\nfrom spalah.dataset import DeltaProperty\n\ndp = DeltaProperty(table_path="/path/dataset")\n\nprint(dp.properties) \n\n# output: \n# {\'delta.deletedFileRetentionDuration\': \'interval 15 days\'}\n```\n\n### Set delta table properties\n\n```python\nrom spalah.dataset import DeltaProperty\n\ndp = DeltaProperty(table_path="/path/dataset")\n\ndp.properties = {\n    "delta.logRetentionDuration": "interval 10 days",\n    "delta.deletedFileRetentionDuration": "interval 15 days"\n}\n\n```\nand the standard output is:\n\n```\n2023-05-20 18:27:42,070 INFO      Applying check constraints on \'delta.`/tmp/nested_schema_dataset`\':\n2023-05-20 18:27:42,071 INFO      Checking if constraint \'id_is_not_null\' was already set on delta.`/tmp/nested_schema_dataset`\n2023-05-20 18:27:42,433 INFO      The constraint id_is_not_null has been successfully added to \'delta.`/tmp/nested_schema_dataset`\n```\n\nPlease note that check constraints can be retrieved and set using property: `.check_constraints`\n\nCheck for more information in [examples: dataframe](docs/examples/dataframe.md), [examples: datalake](docs/examples/dataset.md) pages and related [notebook](docs/usage.ipynb)\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)\n',
+    'long_description': '# spalah\n\nSpalah is a set of python helpers to deal with PySpark dataframes, transformations, schemas and Delta Tables.\n\nThe word "spalah" means "spark" in Ukrainian 🇺🇦 \n\n# Installation\n\nUse the package manager [pip](https://pip.pypa.io/en/stable/) to install spalah.\n\n```bash\npip install spalah\n```\n\n# Examples of use\nSpalah currently has two different groups of helpers: `dataframe` and `datalake`.\n\n## spalah.dataframe\n\n### slice_dataframe\n\n```python\nfrom spalah.dataframe import slice_dataframe\n\ndf = spark.sql(\n    \'SELECT 1 as ID, "John" AS Name, struct("line1" AS Line1, "line2" AS Line2) AS Address\'\n)\ndf.printSchema()\n\n""" output:\nroot\n |-- ID: integer (nullable = false)\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n |    |-- Line2: string (nullable = false)\n"""\n\n# Create a new dataframe by cutting of root and nested attributes\ndf_result = slice_dataframe(\n    input_dataframe=df,\n    columns_to_include=["Name", "Address"],\n    columns_to_exclude=["Address.Line2"]\n)\ndf_result.printSchema()\n\n""" output:\nroot\n |-- Name: string (nullable = false)\n |-- Address: struct (nullable = false)\n |    |-- Line1: string (nullable = false)\n"""\n```\n\nBeside of nested regular structs it also supported slicing of structs in arrays, including multiple levels of nesting\n\n\n### flatten_schema\n\n```python\nfrom spalah.dataframe import flatten_schema\n\n# Pass the sample dataframe to get the list of all attributes as single dimension list\nflatten_schema(df_complex_schema.schema)\n\n""" output:\n[\'ID\', \'Name\', \'Address.Line1\', \'Address.Line2\']\n"""\n\n\n# Alternatively, the function can return data types of the attributes\nflatten_schema(\n    schema=df_complex_schema.schema,\n    include_datatype=True\n)\n\n""" output:\n[\n    (\'ID\', \'IntegerType\'),\n    (\'Name\', \'StringType\'),\n    (\'Address.Line1\', \'StringType\'),\n    (\'Address.Line2\', \'StringType\')\n]\n"""\n```\n\n### script_dataframe\n\n```python\nfrom spalah.dataframe import script_dataframe\n\nscript = script_dataframe(df)\n\nprint(script)\n\n""" output:\nfrom pyspark.sql import Row\nimport datetime\nfrom decimal import Decimal\nfrom pyspark.sql.types import *\n\n# Scripted data and schema:\n__data = [Row(ID=1, Name=\'John\', Address=Row(Line1=\'line1\', Line2=\'line2\'))]\n\n__schema = {\'type\': \'struct\', \'fields\': [{\'name\': \'ID\', \'type\': \'integer\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Name\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Address\', \'type\': {\'type\': \'struct\', \'fields\': [{\'name\': \'Line1\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}, {\'name\': \'Line2\', \'type\': \'string\', \'nullable\': False, \'metadata\': {}}]}, \'nullable\': False, \'metadata\': {}}]}\n\noutcome_dataframe = spark.createDataFrame(__data, StructType.fromJson(__schema))\n"""\n```\n\n### SchemaComparer\n\n```python\nfrom spalah.dataframe import SchemaComparer\n\nschema_comparer = SchemaComparer(\n    source_schema = df_source.schema,\n    target_schema = df_target.schema\n)\n\nschema_comparer.compare()\n\n# The comparison results are stored in the class instance properties `matched` and `not_matched`\n\n# Contains a list of matched columns:\nschema_comparer.matched\n\n""" output:\n[MatchedColumn(name=\'Address.Line1\',  data_type=\'StringType\')]\n"""\n\n# Contains a list of all not matched columns with a reason as description of non-match:\nschema_comparer.not_matched\n\n""" output:\n[\n    NotMatchedColumn(\n        name=\'name\', \n        data_type=\'StringType\', \n        reason="The column exists in source and target schemas but it\'s name is case-mismatched"\n    ),\n    NotMatchedColumn(\n        name=\'ID\', \n        data_type=\'IntegerType <=> StringType\', \n        reason=\'The column exists in source and target schemas but it is not matched by a data type\'\n    ),\n    NotMatchedColumn(\n        name=\'Address.Line2\', \n        data_type=\'StringType\', \n        reason=\'The column exists only in the source schema\'\n    )\n]\n"""\n```\n\n## spalah.dataset\n\n### Get delta table properties\n\n```python\nfrom spalah.dataset import DeltaTableConfig\n\ndp = DeltaTableConfig(table_path="/path/dataset")\n\nprint(dp.properties) \n\n# output: \n# {\'delta.deletedFileRetentionDuration\': \'interval 15 days\'}\n```\n\n### Set delta table properties\n\n```python\nrom spalah.dataset import DeltaTableConfig\n\ndp = DeltaTableConfig(table_path="/path/dataset")\n\ndp.properties = {\n    "delta.logRetentionDuration": "interval 10 days",\n    "delta.deletedFileRetentionDuration": "interval 15 days"\n}\n\n```\nand the standard output is:\n\n```\n2023-05-20 18:27:42,070 INFO      Applying check constraints on \'delta.`/tmp/nested_schema_dataset`\':\n2023-05-20 18:27:42,071 INFO      Checking if constraint \'id_is_not_null\' was already set on delta.`/tmp/nested_schema_dataset`\n2023-05-20 18:27:42,433 INFO      The constraint id_is_not_null has been successfully added to \'delta.`/tmp/nested_schema_dataset`\n```\n\nPlease note that check constraints can be retrieved and set using property: `.check_constraints`\n\nCheck for more information in [examples: dataframe](docs/examples/dataframe.md), [examples: datalake](docs/examples/dataset.md) pages and related [notebook](docs/usage.ipynb)\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)\n',
     'author': 'Alex Volok',
     'author_email': 'alexandr.volok@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/avolok/spalah',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `spalah-1.0.1/PKG-INFO` & `spalah-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spalah
-Version: 1.0.1
+Version: 1.0.2
 Summary: Spalah is a set of PySpark dataframe helpers
 Home-page: https://github.com/avolok/spalah
 License: MIT
 Keywords: spalah
 Author: Alex Volok
 Author-email: alexandr.volok@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -180,30 +180,30 @@
 ```
 
 ## spalah.dataset
 
 ### Get delta table properties
 
 ```python
-from spalah.dataset import DeltaProperty
+from spalah.dataset import DeltaTableConfig
 
-dp = DeltaProperty(table_path="/path/dataset")
+dp = DeltaTableConfig(table_path="/path/dataset")
 
 print(dp.properties) 
 
 # output: 
 # {'delta.deletedFileRetentionDuration': 'interval 15 days'}
 ```
 
 ### Set delta table properties
 
 ```python
-rom spalah.dataset import DeltaProperty
+rom spalah.dataset import DeltaTableConfig
 
-dp = DeltaProperty(table_path="/path/dataset")
+dp = DeltaTableConfig(table_path="/path/dataset")
 
 dp.properties = {
     "delta.logRetentionDuration": "interval 10 days",
     "delta.deletedFileRetentionDuration": "interval 15 days"
 }
 
 ```
```

