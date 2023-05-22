# Comparing `tmp/nypl_py_utils-1.0.1.tar.gz` & `tmp/nypl_py_utils-1.0.3.tar.gz`

## Comparing `nypl_py_utils-1.0.1.tar` & `nypl_py_utils-1.0.3.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/CODEOWNERS
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/Makefile
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/.github/workflows/deploy-production.yml
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/.github/workflows/deploy-qa.yml
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/__init__.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/avro_encoder.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/kinesis_client.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/kms_client.py
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/mysql_client.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/oauth2_api_client.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/postgresql_client.py
--rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/postgresql_pool_client.py
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/redshift_client.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/classes/s3_client.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/functions/config_helper.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/functions/log_helper.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/src/nypl_py_utils/functions/obfuscation_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_avro_encoder.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_config_helper.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_kinesis_client.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_kms_client.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_log_helper.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_mysql_client.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_oauth2_api_client.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_obfuscation_helper.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_postgresql_client.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_postgresql_pool_client.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_redshift_client.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/tests/test_s3_client.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/LICENSE
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/README.md
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/CODEOWNERS
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/Makefile
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/.github/workflows/deploy-production.yml
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/.github/workflows/deploy-qa.yml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/__init__.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/avro_encoder.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/kinesis_client.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/kms_client.py
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/mysql_client.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/oauth2_api_client.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/postgresql_client.py
+-rw-r--r--   0        0        0     5864 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/postgresql_pool_client.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/redshift_client.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/classes/s3_client.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/functions/config_helper.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/functions/log_helper.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/functions/obfuscation_helper.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/src/nypl_py_utils/functions/research_catalog_identifier_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_avro_encoder.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_config_helper.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_kinesis_client.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_kms_client.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_log_helper.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_mysql_client.py
+-rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_oauth2_api_client.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_obfuscation_helper.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_postgresql_client.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_postgresql_pool_client.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_redshift_client.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_research_catalog_identifier_helper.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/tests/test_s3_client.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/LICENSE
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/README.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 nypl_py_utils-1.0.3/PKG-INFO
```

### Comparing `nypl_py_utils-1.0.1/CHANGELOG.md` & `nypl_py_utils-1.0.3/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v1.0.3 - 5/19/23
+- Add research_catalog_identifier_helper function
+
+## v1.0.2 - 5/18/23
+- Identical to v1.0.1 -- this was mistakenly deployed to QA without any changes
+
 ## v1.0.1 - 4/3/23
 - Add transaction support to RedshiftClient
 
 ## v1.0.0 - 3/22/23
 - Improve Oauth2ApiClient token refresh and method responses
 - Create separate PostgreSQLClient and PostgreSQLPoolClient classes
 - Update PostgreSQL and MySQL clients to accept write queries implicitly
```

### Comparing `nypl_py_utils-1.0.1/.github/workflows/deploy-production.yml` & `nypl_py_utils-1.0.3/.github/workflows/deploy-production.yml`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/.github/workflows/deploy-qa.yml` & `nypl_py_utils-1.0.3/.github/workflows/deploy-qa.yml`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/.github/workflows/run-unit-tests.yml` & `nypl_py_utils-1.0.3/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/avro_encoder.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/avro_encoder.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/kinesis_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/kinesis_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/kms_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/kms_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/mysql_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/mysql_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/oauth2_api_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/oauth2_api_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/postgresql_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/postgresql_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/postgresql_pool_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/postgresql_pool_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/redshift_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/redshift_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/classes/s3_client.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/classes/s3_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/functions/config_helper.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/functions/config_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,22 @@
     """
     This method loads a YAML config file containing environment variables,
     decrypts whichever are encrypted, and puts them all into os.environ as
     strings.
 
     It requires the YAML file to be split into a 'PLAINTEXT_VARIABLES' section
     and an 'ENCRYPTED_VARIABLES' section.
+
+    Parameters
+        ----------
+        run_type: str
+            The name of the config file to use, e.g. 'devel'
+        file_string: str
+            The path to the config files with the filename as a variable to be
+            interpolated, e.g. 'config/{}.yaml'
     """
 
     env_dict = None
     open_file = file_string.format(run_type)
     logger.info('Loading env file {}'.format(open_file))
     try:
         with open(open_file, 'r') as env_stream:
```

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/functions/log_helper.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/functions/log_helper.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/src/nypl_py_utils/functions/obfuscation_helper.py` & `nypl_py_utils-1.0.3/src/nypl_py_utils/functions/obfuscation_helper.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_avro_encoder.py` & `nypl_py_utils-1.0.3/tests/test_avro_encoder.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_config_helper.py` & `nypl_py_utils-1.0.3/tests/test_config_helper.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_kinesis_client.py` & `nypl_py_utils-1.0.3/tests/test_kinesis_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_kms_client.py` & `nypl_py_utils-1.0.3/tests/test_kms_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_log_helper.py` & `nypl_py_utils-1.0.3/tests/test_log_helper.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_mysql_client.py` & `nypl_py_utils-1.0.3/tests/test_mysql_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_oauth2_api_client.py` & `nypl_py_utils-1.0.3/tests/test_oauth2_api_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_obfuscation_helper.py` & `nypl_py_utils-1.0.3/tests/test_obfuscation_helper.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_postgresql_client.py` & `nypl_py_utils-1.0.3/tests/test_postgresql_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_postgresql_pool_client.py` & `nypl_py_utils-1.0.3/tests/test_postgresql_pool_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_redshift_client.py` & `nypl_py_utils-1.0.3/tests/test_redshift_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/tests/test_s3_client.py` & `nypl_py_utils-1.0.3/tests/test_s3_client.py`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/LICENSE` & `nypl_py_utils-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nypl_py_utils-1.0.1/README.md` & `nypl_py_utils-1.0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,34 @@
 * Connecting to and querying Redshift
 * Making requests to the Oauth2 authenticated APIs such as NYPL Platform API and Sierra
 
 ## Functions
 * Reading a YAML config file and putting the contents in os.environ
 * Creating a logger in the appropriate format
 * Obfuscating a value using bcrypt
+* Parsing/building Research Catalog identifiers
+
+## Usage
+```python
+# test_file.py
+from nypl_py_utils.classes.kinesis_client import KinesisClient
+from nypl_py_utils.functions.config_helper import load_env_file
+
+load_env_file(...)
+kinesis_client = KinesisClient(...)
+```
+
+```bash
+# requirements.txt
+
+# Do not use any version below 1.0.0
+# All available optional dependencies can be found in pyproject.toml.
+# See the "Managing dependencies" section below for more details.
+nypl-py-utils[kinesis-client,config-helper]==1.0.1
+```
 
 ## Developing locally
 In order to use the local version of the package instead of the global version, use a virtual environment. To set up a virtual environment and install all the necessary dependencies, run:
 
 ```
 python3 -m venv testenv
 source testenv/bin/activate
@@ -34,38 +54,54 @@
 In order to prevent dependency bloat, this package has no required dependencies. Instead, each class and helper file has its own optional dependency set. For instance, if an app needs to use the KMS client and the obfuscation helper, it should add `nypl-py-utils[kms-client, obfuscation-helper]` to the app's requirements. This way, only the required dependencies are installed.
 
 When a new client or helper file is created, a new optional dependency set should be added to `pyproject.toml`. The `development` dependency set, which includes all the dependencies required by all of the classes and tests, should also be updated.
 
 The optional dependency sets also give the developer the option to manually list out the dependencies of the clients rather than relying upon what the package thinks is required, which can be beneficial in certain circumstances. For instance, AWS lambda functions come with `boto3` and `botocore` pre-installed, so it's not necessary to include these (rather hefty) dependencies in the lambda deployment package.
 
 ### Troubleshooting
-If running `main.py` in this virtual environment produces the following error:
+#### Using PostgreSQLClient in an AWS Lambda
+Because `psycopg` requires a statically linked version of the `libpq` library, the `PostgreSQLClient` cannot be installed as-is in an AWS Lambda function. Instead, it must be packaged as follows:
+```bash
+pip install --target ./package nypl-py-utils[postgresql-client]==1.0.1
+
+pip install \
+    --platform manylinux2014_x86_64 \
+    --target=./package \
+    --implementation cp \
+    --python 3.9 \
+    --only-binary=:all: --upgrade \
+    'psycopg[binary]'
+```
+
+#### Using PostgreSQLClient locally
+If using the `PostgreSQLClient` produces the following error locally:
 ```
 ImportError: no pq wrapper available.
 Attempts made:
 - couldn't import psycopg 'c' implementation: No module named 'psycopg_c'
 - couldn't import psycopg 'binary' implementation: No module named 'psycopg_binary'
 - couldn't import psycopg 'python' implementation: dlsym(0x7f8620446f40, PQsslInUse): symbol not found
 ```
 
 then try running:
-```
+```bash
 pip uninstall psycopg
 pip install "psycopg[c]"
 ```
 
 ## Git workflow
 This repo uses the [Main-QA-Production](https://github.com/NYPL/engineering-general/blob/main/standards/git-workflow.md#main-qa-production) git workflow.
 
 [`main`](https://github.com/NYPL/python-utils/tree/main) has the latest and greatest commits, [`qa`](https://github.com/NYPL/python-utils/tree/qa) has what's in our QA environment, and [`production`](https://github.com/NYPL/python-utils/tree/production) has what's in our production environment.
 
 ### Ideal Workflow
 - Cut a feature branch off of `main`
 - Commit changes to your feature branch
 - File a pull request against `main` and assign a reviewer (who must be an owner)
+  - Include relevant updates to pyproject.toml and README
   - In order for the PR to be accepted, it must pass all unit tests, have no lint issues, and update the CHANGELOG (or contain the `Skip-Changelog` label in GitHub)
 - After the PR is accepted, merge into `main`
 - Merge `main` > `qa`
 - Deploy app to QA on GitHub and confirm it works
 - Merge `qa` > `production`
 - Deploy app to production on GitHub and confirm it works
```

### Comparing `nypl_py_utils-1.0.1/pyproject.toml` & `nypl_py_utils-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nypl_py_utils"
-version = "1.0.1"
+version = "1.0.3"
 authors = [
   { name="Aaron Friedman", email="aaronfriedman@nypl.org" },
 ]
 description = "A package containing Python utilities for use across NYPL"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -59,16 +59,19 @@
 config-helper = [
     "nypl_py_utils[kms-client]",
     "PyYAML>=6.0"
 ]
 obfuscation-helper = [
     "bcrypt>=4.0.1"
 ]
+research-catalog-identifier-helper = [
+    "requests>=2.28.1"
+]
 development = [
-    "nypl_py_utils[avro-encoder,kinesis-client,kms-client,mysql-client,oauth2-api-client,postgresql-client,postgresql-pool-client,redshift-client,s3-client,config-helper,obfuscation-helper]",
+    "nypl_py_utils[avro-encoder,kinesis-client,kms-client,mysql-client,oauth2-api-client,postgresql-client,postgresql-pool-client,redshift-client,s3-client,config-helper,obfuscation-helper,research-catalog-identifier-helper]",
     "flake8>=6.0.0",
     "freezegun>=1.2.2",
     "mock>=4.0.3",
     "pytest>=7.2.0",
     "pytest-mock>=3.10.0",
     "requests-mock>=1.10.0"
 ]
```

### Comparing `nypl_py_utils-1.0.1/PKG-INFO` & `nypl_py_utils-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nypl_py_utils
-Version: 1.0.1
+Version: 1.0.3
 Summary: A package containing Python utilities for use across NYPL
 Project-URL: Homepage, https://github.com/NYPL/python-utils
 Project-URL: Bug Tracker, https://github.com/NYPL/python-utils/issues
 Author-email: Aaron Friedman <aaronfriedman@nypl.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Provides-Extra: config-helper
 Requires-Dist: nypl-py-utils[kms-client]; extra == 'config-helper'
 Requires-Dist: pyyaml>=6.0; extra == 'config-helper'
 Provides-Extra: development
 Requires-Dist: flake8>=6.0.0; extra == 'development'
 Requires-Dist: freezegun>=1.2.2; extra == 'development'
 Requires-Dist: mock>=4.0.3; extra == 'development'
-Requires-Dist: nypl-py-utils[avro-encoder,config-helper,kinesis-client,kms-client,mysql-client,oauth2-api-client,obfuscation-helper,postgresql-client,postgresql-pool-client,redshift-client,s3-client]; extra == 'development'
+Requires-Dist: nypl-py-utils[avro-encoder,config-helper,kinesis-client,kms-client,mysql-client,oauth2-api-client,obfuscation-helper,postgresql-client,postgresql-pool-client,redshift-client,research-catalog-identifier-helper,s3-client]; extra == 'development'
 Requires-Dist: pytest-mock>=3.10.0; extra == 'development'
 Requires-Dist: pytest>=7.2.0; extra == 'development'
 Requires-Dist: requests-mock>=1.10.0; extra == 'development'
 Provides-Extra: kinesis-client
 Requires-Dist: boto3>=1.26.5; extra == 'kinesis-client'
 Requires-Dist: botocore>=1.29.5; extra == 'kinesis-client'
 Provides-Extra: kms-client
@@ -40,14 +40,16 @@
 Provides-Extra: postgresql-client
 Requires-Dist: psycopg[binary]>=3.1.6; extra == 'postgresql-client'
 Provides-Extra: postgresql-pool-client
 Requires-Dist: psycopg[binary,pool]>=3.1.6; extra == 'postgresql-pool-client'
 Provides-Extra: redshift-client
 Requires-Dist: botocore>=1.29.5; extra == 'redshift-client'
 Requires-Dist: redshift-connector>=2.0.909; extra == 'redshift-client'
+Provides-Extra: research-catalog-identifier-helper
+Requires-Dist: requests>=2.28.1; extra == 'research-catalog-identifier-helper'
 Provides-Extra: s3-client
 Requires-Dist: boto3>=1.26.5; extra == 's3-client'
 Requires-Dist: botocore>=1.29.5; extra == 's3-client'
 Description-Content-Type: text/markdown
 
 # PythonUtils
 
@@ -64,14 +66,34 @@
 * Connecting to and querying Redshift
 * Making requests to the Oauth2 authenticated APIs such as NYPL Platform API and Sierra
 
 ## Functions
 * Reading a YAML config file and putting the contents in os.environ
 * Creating a logger in the appropriate format
 * Obfuscating a value using bcrypt
+* Parsing/building Research Catalog identifiers
+
+## Usage
+```python
+# test_file.py
+from nypl_py_utils.classes.kinesis_client import KinesisClient
+from nypl_py_utils.functions.config_helper import load_env_file
+
+load_env_file(...)
+kinesis_client = KinesisClient(...)
+```
+
+```bash
+# requirements.txt
+
+# Do not use any version below 1.0.0
+# All available optional dependencies can be found in pyproject.toml.
+# See the "Managing dependencies" section below for more details.
+nypl-py-utils[kinesis-client,config-helper]==1.0.1
+```
 
 ## Developing locally
 In order to use the local version of the package instead of the global version, use a virtual environment. To set up a virtual environment and install all the necessary dependencies, run:
 
 ```
 python3 -m venv testenv
 source testenv/bin/activate
@@ -85,38 +107,54 @@
 In order to prevent dependency bloat, this package has no required dependencies. Instead, each class and helper file has its own optional dependency set. For instance, if an app needs to use the KMS client and the obfuscation helper, it should add `nypl-py-utils[kms-client, obfuscation-helper]` to the app's requirements. This way, only the required dependencies are installed.
 
 When a new client or helper file is created, a new optional dependency set should be added to `pyproject.toml`. The `development` dependency set, which includes all the dependencies required by all of the classes and tests, should also be updated.
 
 The optional dependency sets also give the developer the option to manually list out the dependencies of the clients rather than relying upon what the package thinks is required, which can be beneficial in certain circumstances. For instance, AWS lambda functions come with `boto3` and `botocore` pre-installed, so it's not necessary to include these (rather hefty) dependencies in the lambda deployment package.
 
 ### Troubleshooting
-If running `main.py` in this virtual environment produces the following error:
+#### Using PostgreSQLClient in an AWS Lambda
+Because `psycopg` requires a statically linked version of the `libpq` library, the `PostgreSQLClient` cannot be installed as-is in an AWS Lambda function. Instead, it must be packaged as follows:
+```bash
+pip install --target ./package nypl-py-utils[postgresql-client]==1.0.1
+
+pip install \
+    --platform manylinux2014_x86_64 \
+    --target=./package \
+    --implementation cp \
+    --python 3.9 \
+    --only-binary=:all: --upgrade \
+    'psycopg[binary]'
+```
+
+#### Using PostgreSQLClient locally
+If using the `PostgreSQLClient` produces the following error locally:
 ```
 ImportError: no pq wrapper available.
 Attempts made:
 - couldn't import psycopg 'c' implementation: No module named 'psycopg_c'
 - couldn't import psycopg 'binary' implementation: No module named 'psycopg_binary'
 - couldn't import psycopg 'python' implementation: dlsym(0x7f8620446f40, PQsslInUse): symbol not found
 ```
 
 then try running:
-```
+```bash
 pip uninstall psycopg
 pip install "psycopg[c]"
 ```
 
 ## Git workflow
 This repo uses the [Main-QA-Production](https://github.com/NYPL/engineering-general/blob/main/standards/git-workflow.md#main-qa-production) git workflow.
 
 [`main`](https://github.com/NYPL/python-utils/tree/main) has the latest and greatest commits, [`qa`](https://github.com/NYPL/python-utils/tree/qa) has what's in our QA environment, and [`production`](https://github.com/NYPL/python-utils/tree/production) has what's in our production environment.
 
 ### Ideal Workflow
 - Cut a feature branch off of `main`
 - Commit changes to your feature branch
 - File a pull request against `main` and assign a reviewer (who must be an owner)
+  - Include relevant updates to pyproject.toml and README
   - In order for the PR to be accepted, it must pass all unit tests, have no lint issues, and update the CHANGELOG (or contain the `Skip-Changelog` label in GitHub)
 - After the PR is accepted, merge into `main`
 - Merge `main` > `qa`
 - Deploy app to QA on GitHub and confirm it works
 - Merge `qa` > `production`
 - Deploy app to production on GitHub and confirm it works
```

