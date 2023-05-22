# Comparing `tmp/databricks_common-0.1.4.tar.gz` & `tmp/databricks_common-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_common-0.1.4.tar", max compression
+gzip compressed data, was "databricks_common-0.1.5.tar", max compression
```

## Comparing `databricks_common-0.1.4.tar` & `databricks_common-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.4/README.md
--rw-r--r--   0        0        0       22 2023-05-22 14:30:39.713492 databricks_common-0.1.4/databricks_common/__init__.py
--rw-r--r--   0        0        0     9239 2023-05-19 04:17:35.507741 databricks_common-0.1.4/databricks_common/common.py
--rw-r--r--   0        0        0      245 2023-05-19 02:46:46.079608 databricks_common-0.1.4/databricks_common/main.py
--rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.4/databricks_common/utils/get_spark.py
--rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.4/databricks_common/utils/get_spark_local.py
--rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.4/databricks_common/utils/logger_utils.py
--rw-r--r--   0        0        0      740 2023-05-22 14:30:34.593425 databricks_common-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-05-15 10:35:58.596661 databricks_common-0.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-05-22 15:04:09.625718 databricks_common-0.1.5/databricks_common/__init__.py
+-rw-r--r--   0        0        0     9202 2023-05-22 15:03:18.376728 databricks_common-0.1.5/databricks_common/common.py
+-rw-r--r--   0        0        0      245 2023-05-19 02:46:46.079608 databricks_common-0.1.5/databricks_common/main.py
+-rwxr-xr-x   0        0        0      327 2023-05-15 10:35:58.597485 databricks_common-0.1.5/databricks_common/utils/get_spark.py
+-rw-r--r--   0        0        0        0 2023-05-15 10:35:58.597000 databricks_common-0.1.5/databricks_common/utils/get_spark_local.py
+-rw-r--r--   0        0        0      745 2023-05-15 10:35:58.597694 databricks_common-0.1.5/databricks_common/utils/logger_utils.py
+-rw-r--r--   0        0        0      740 2023-05-22 15:04:06.370456 databricks_common-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      433 1970-01-01 00:00:00.000000 databricks_common-0.1.5/PKG-INFO
```

### Comparing `databricks_common-0.1.4/databricks_common/common.py` & `databricks_common-0.1.5/databricks_common/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser
 from typing import Dict, Any
-from pyspark.sql import SparkSession
 from logging import Logger
 
 from databricks_common.utils.logger_utils import get_logger
 from databricks_common.utils.get_spark import spark
 
 _logger = get_logger()
```

### Comparing `databricks_common-0.1.4/databricks_common/utils/logger_utils.py` & `databricks_common-0.1.5/databricks_common/utils/logger_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_common-0.1.4/pyproject.toml` & `databricks_common-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-common"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Xavier Armitage <xtarmitage@gmail.com>"]
 readme = "README.md"
 packages = [{include = "databricks_common"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

