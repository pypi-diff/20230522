# Comparing `tmp/longalpha_utils-0.51.tar.gz` & `tmp/longalpha_utils-0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "longalpha_utils-0.51.tar", last modified: Mon May 22 05:50:04 2023, max compression
+gzip compressed data, was "longalpha_utils-0.52.tar", last modified: Mon May 22 20:01:20 2023, max compression
```

## Comparing `longalpha_utils-0.51.tar` & `longalpha_utils-0.52.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:50:04.036222 longalpha_utils-0.51/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 05:50:04.036222 longalpha_utils-0.51/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:50:04.036222 longalpha_utils-0.51/longalpha_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/messenger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/us_stock_holidays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-22 05:49:53.000000 longalpha_utils-0.51/longalpha_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 05:50:04.036222 longalpha_utils-0.51/longalpha_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 05:50:04.000000 longalpha_utils-0.51/longalpha_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 05:50:04.036222 longalpha_utils-0.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-22 05:49:53.000000 longalpha_utils-0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:01:20.894785 longalpha_utils-0.52/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 20:01:20.894785 longalpha_utils-0.52/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:01:20.890784 longalpha_utils-0.52/longalpha_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/messenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/us_stock_holidays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-22 20:01:07.000000 longalpha_utils-0.52/longalpha_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:01:20.894785 longalpha_utils-0.52/longalpha_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 20:01:20.000000 longalpha_utils-0.52/longalpha_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:01:20.894785 longalpha_utils-0.52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-22 20:01:07.000000 longalpha_utils-0.52/setup.py
```

### Comparing `longalpha_utils-0.51/longalpha_utils/messenger.py` & `longalpha_utils-0.52/longalpha_utils/messenger.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.51/longalpha_utils/transfers.py` & `longalpha_utils-0.52/longalpha_utils/transfers.py`

 * *Files 7% similar despite different names*

```diff
@@ -181,15 +181,34 @@
         objects = [i for i in self.minio_client.list_objects(bucket_name)]
         time_obj = {obj.last_modified: obj for obj in objects}
         latest_time = max([key for key in time_obj.keys() if key is not None])
         latest_obj = time_obj[latest_time]
         return self.get(bucket_name=bucket_name, object_name=latest_obj.object_name)
 
     def list(self, bucket_name: str) -> List[str]:
-        return [i.object_name for i in self.minio_client.list_objects(bucket_name)]
+        return [i.object_name for i in self.minio_client.list_objects(bucket_name, recursive=True)]
+
+    def delete_objects(self, bucket_name:str, prefix:str) -> None:
+        """
+        delete all objects in a bucket with a given prefix
+        Args:
+            bucket_name: Minio bucket_name
+            prefix: prefix of the objects to be deleted
+
+        Returns:
+
+        """
+        objects = self.minio_client.list_objects(
+            bucket_name, prefix,
+            recursive=True
+        )
+
+        for obj in objects:
+            self.minio_client.remove_object(bucket_name, obj.object_name)
+
 
 
 def get_s3_data_spark(
     spark: SparkSession,
     start_date: date,
     end_date: date,
     bucket: str,
```

### Comparing `longalpha_utils-0.51/longalpha_utils/us_stock_holidays.py` & `longalpha_utils-0.52/longalpha_utils/us_stock_holidays.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.51/longalpha_utils/utils.py` & `longalpha_utils-0.52/longalpha_utils/utils.py`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.51/longalpha_utils.egg-info/requires.txt` & `longalpha_utils-0.52/longalpha_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `longalpha_utils-0.51/setup.py` & `longalpha_utils-0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,11 +38,11 @@
     "typing_extensions==4.4.0",
     "urllib3==1.26.14",
     "yagmail==0.15.293",
 ]
 
 setup(
     name="longalpha_utils",
-    version="0.51",
+    version="0.52",
     long_description="Shared utilities for long alpha projects",
     install_requires=REQUIREMENTS,
 )
```

