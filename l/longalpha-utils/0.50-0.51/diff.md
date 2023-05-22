# Comparing `tmp/longalpha_utils-0.50.tar.gz` & `tmp/longalpha_utils-0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.50.tar", last modified: Sun May 21 21:45:07 2023, max compression
+gzip compressed data, was "longalpha_utils-0.51.tar", last modified: Mon May 22 05:50:04 2023, max compression
```

## Comparing `longalpha_utils-0.50.tar` & `longalpha_utils-0.51.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:45:07.515494 longalpha_utils-0.50/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 21:45:07.515494 longalpha_utils-0.50/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:45:07.515494 longalpha_utils-0.50/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-21 21:44:56.000000 longalpha_utils-0.50/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 21:44:56.000000 longalpha_utils-0.50/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-21 21:44:56.000000 longalpha_utils-0.50/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-21 21:44:56.000000 longalpha_utils-0.50/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-21 21:44:56.000000 longalpha_utils-0.50/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-21 21:44:56.000000 longalpha_utils-0.50/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:45:07.515494 longalpha_utils-0.50/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-21 21:45:07.000000 longalpha_utils-0.50/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-21 21:45:07.000000 longalpha_utils-0.50/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:45:07.000000 longalpha_utils-0.50/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-21 21:45:07.000000 longalpha_utils-0.50/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 21:45:07.000000 longalpha_utils-0.50/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 21:45:07.515494 longalpha_utils-0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-21 21:44:56.000000 longalpha_utils-0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:50:04.036222 longalpha_utils-0.51/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 05:50:04.036222 longalpha_utils-0.51/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:50:04.036222 longalpha_utils-0.51/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:50:04.036222 longalpha_utils-0.51/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 05:50:04.036222 longalpha_utils-0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-22 05:49:53.000000 longalpha_utils-0.51/setup.py
```

### Comparing `longalpha_utils-0.50/longalpha_utils/messenger.py` & `longalpha_utils-0.51/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.50/longalpha_utils/transfers.py` & `longalpha_utils-0.51/longalpha_utils/transfers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 from longalpha_utils.utils import multi_union_by_name
 from tqdm import tqdm
 
 
 def init_spark(
     spark_executor_memory: str = "30g",
     spark_driver_memory: str = "90g",
-    minio_endpoint: Optional[str] = None,
-    minio_access_key: Optional[str] = None,
-    minio_secret_key: Optional[str] = None,
+    s3_endpoint: Optional[str] = None,
+    s3_access_key: Optional[str] = None,
+    s3_secret_key: Optional[str] = None,
     additional_configs: Optional[Dict[str, Any]] = None,
 ) -> SparkSession:
     """
     get a spark instance.
 
     if connect_psql is True, then we will connect to psql.
     if minio_endpoint is not None, then we will connect to minio.
     if both are None, then we will connect to local spark.
 
     Note that we are not downloading jars here. We use spark.jars.packages to download jars.
 
     Args:
-        minio_endpoint: minio_endpoint
-        minio_access_key:  minio_access_key
-        minio_secret_key:  minio_secret_key
+        s3_endpoint: minio_endpoint
+        s3_access_key:  minio_access_key
+        s3_secret_key:  minio_secret_key
         spark_executor_memory: size of spark_executor_memory
         spark_driver_memory: size of spark_driver_memory
         additional_configs: additional configs in the form of a dictionary
     Returns:
 
     """
     jars = [
@@ -65,18 +65,18 @@
     # set other configs
     if additional_configs is not None:
         for k, v in additional_configs.items():
             builder.config(k, v)
     # get spark
     spark = builder.getOrCreate()
 
-    if minio_endpoint is not None:
-        spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.endpoint", minio_endpoint)
-        spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.access.key", minio_access_key)
-        spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.secret.key", minio_secret_key)
+    if s3_endpoint is not None:
+        spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.endpoint", s3_endpoint)
+        spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.access.key", s3_access_key)
+        spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.secret.key", s3_secret_key)
         spark.sparkContext._jsc.hadoopConfiguration().set("fs.s3a.connection.ssl.enabled", "false")
 
     return spark
 
 
 class MinioWrapper:
     def __init__(self, minio_url, minio_access_key, minio_secret_key):
```

### Comparing `longalpha_utils-0.50/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.51/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.50/longalpha_utils/utils.py` & `longalpha_utils-0.51/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.50/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.51/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.50/setup.py` & `longalpha_utils-0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.50",
+    version="0.51",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

