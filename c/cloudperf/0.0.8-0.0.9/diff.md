# Comparing `tmp/cloudperf-0.0.8.tar.gz` & `tmp/cloudperf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudperf-0.0.8.tar", last modified: Fri Mar  1 11:09:26 2019, max compression
+gzip compressed data, was "dist/cloudperf-0.0.9.tar", last modified: Fri Mar  1 11:17:18 2019, max compression
```

## Comparing `cloudperf-0.0.8.tar` & `cloudperf-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:09:26.000000 cloudperf-0.0.8/
--rw-rw-r--   0 bra       (1000) bra       (1000)      994 2019-03-01 09:33:19.000000 cloudperf-0.0.8/setup.py
--rw-rw-r--   0 bra       (1000) bra       (1000)    22906 2019-03-01 11:09:26.000000 cloudperf-0.0.8/PKG-INFO
-drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf/
--rw-rw-r--   0 bra       (1000) bra       (1000)     4431 2019-03-01 09:33:19.000000 cloudperf-0.0.8/cloudperf/core.py
--rw-rw-r--   0 bra       (1000) bra       (1000)     7857 2019-03-01 09:58:13.000000 cloudperf-0.0.8/cloudperf/cli.py
--rw-rw-r--   0 bra       (1000) bra       (1000)     9590 2019-03-01 09:33:19.000000 cloudperf-0.0.8/cloudperf/benchmarks.py
--rw-rw-r--   0 bra       (1000) bra       (1000)      299 2019-03-01 11:09:15.000000 cloudperf-0.0.8/cloudperf/__init__.py
-drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf/providers/
--rw-rw-r--   0 bra       (1000) bra       (1000)     2181 2019-03-01 11:07:40.000000 cloudperf-0.0.8/cloudperf/providers/aws.py
--rw-rw-r--   0 bra       (1000) bra       (1000)        0 2019-03-01 09:33:19.000000 cloudperf-0.0.8/cloudperf/providers/__init__.py
--rw-rw-r--   0 bra       (1000) bra       (1000)    25958 2019-03-01 11:08:36.000000 cloudperf-0.0.8/cloudperf/providers/aws_helpers.py
-drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf.egg-info/
--rw-rw-r--   0 bra       (1000) bra       (1000)    22906 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf.egg-info/PKG-INFO
--rw-rw-r--   0 bra       (1000) bra       (1000)        1 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf.egg-info/dependency_links.txt
--rw-rw-r--   0 bra       (1000) bra       (1000)       10 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf.egg-info/top_level.txt
--rw-rw-r--   0 bra       (1000) bra       (1000)      371 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf.egg-info/SOURCES.txt
--rw-rw-r--   0 bra       (1000) bra       (1000)       89 2019-03-01 11:09:26.000000 cloudperf-0.0.8/cloudperf.egg-info/requires.txt
--rw-rw-r--   0 bra       (1000) bra       (1000)    19799 2019-03-01 09:33:19.000000 cloudperf-0.0.8/README.md
-drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:09:26.000000 cloudperf-0.0.8/bin/
--rwxrwxr-x   0 bra       (1000) bra       (1000)      373 2019-03-01 09:33:19.000000 cloudperf-0.0.8/bin/cloudperf
--rw-rw-r--   0 bra       (1000) bra       (1000)       38 2019-03-01 11:09:26.000000 cloudperf-0.0.8/setup.cfg
+drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:17:18.000000 cloudperf-0.0.9/
+drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:17:18.000000 cloudperf-0.0.9/bin/
+-rwxrwxr-x   0 bra       (1000) bra       (1000)      373 2019-03-01 09:33:19.000000 cloudperf-0.0.9/bin/cloudperf
+drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf/
+-rw-rw-r--   0 bra       (1000) bra       (1000)     9590 2019-03-01 09:33:19.000000 cloudperf-0.0.9/cloudperf/benchmarks.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)     4431 2019-03-01 09:33:19.000000 cloudperf-0.0.9/cloudperf/core.py
+drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf/providers/
+-rw-rw-r--   0 bra       (1000) bra       (1000)        0 2019-03-01 09:33:19.000000 cloudperf-0.0.9/cloudperf/providers/__init__.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)     2181 2019-03-01 11:07:40.000000 cloudperf-0.0.9/cloudperf/providers/aws.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)    25962 2019-03-01 11:16:45.000000 cloudperf-0.0.9/cloudperf/providers/aws_helpers.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)     7857 2019-03-01 09:58:13.000000 cloudperf-0.0.9/cloudperf/cli.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)      299 2019-03-01 11:17:15.000000 cloudperf-0.0.9/cloudperf/__init__.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)    19799 2019-03-01 09:33:19.000000 cloudperf-0.0.9/README.md
+drwxrwxr-x   0 bra       (1000) bra       (1000)        0 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf.egg-info/
+-rw-rw-r--   0 bra       (1000) bra       (1000)    22906 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf.egg-info/PKG-INFO
+-rw-rw-r--   0 bra       (1000) bra       (1000)        1 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf.egg-info/dependency_links.txt
+-rw-rw-r--   0 bra       (1000) bra       (1000)       10 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf.egg-info/top_level.txt
+-rw-rw-r--   0 bra       (1000) bra       (1000)       89 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf.egg-info/requires.txt
+-rw-rw-r--   0 bra       (1000) bra       (1000)      371 2019-03-01 11:17:18.000000 cloudperf-0.0.9/cloudperf.egg-info/SOURCES.txt
+-rw-rw-r--   0 bra       (1000) bra       (1000)    22906 2019-03-01 11:17:18.000000 cloudperf-0.0.9/PKG-INFO
+-rw-rw-r--   0 bra       (1000) bra       (1000)      994 2019-03-01 09:33:19.000000 cloudperf-0.0.9/setup.py
+-rw-rw-r--   0 bra       (1000) bra       (1000)       38 2019-03-01 11:17:18.000000 cloudperf-0.0.9/setup.cfg
```

### Comparing `cloudperf-0.0.8/setup.py` & `cloudperf-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `cloudperf-0.0.8/PKG-INFO` & `cloudperf-0.0.9/cloudperf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudperf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Relative performance index for cloud services
 Home-page: https://github.com/bra-fsn/cloudperf
 Author: NAGY, Attila
 Author-email: nagy.attila@gmail.com
 License: UNKNOWN
 Description: # cloudperf
         ## Measuring the relative performance of cloud resources
```

### Comparing `cloudperf-0.0.8/cloudperf/core.py` & `cloudperf-0.0.9/cloudperf/core.py`

 * *Files identical despite different names*

### Comparing `cloudperf-0.0.8/cloudperf/cli.py` & `cloudperf-0.0.9/cloudperf/cli.py`

 * *Files identical despite different names*

### Comparing `cloudperf-0.0.8/cloudperf/benchmarks.py` & `cloudperf-0.0.9/cloudperf/benchmarks.py`

 * *Files identical despite different names*

### Comparing `cloudperf-0.0.8/cloudperf/providers/aws.py` & `cloudperf-0.0.9/cloudperf/providers/aws.py`

 * *Files identical despite different names*

### Comparing `cloudperf-0.0.8/cloudperf/providers/aws_helpers.py` & `cloudperf-0.0.9/cloudperf/providers/aws_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 import requests
 import paramiko
 import pandas as pd
 from dateutil import parser
 from botocore.exceptions import ClientError
 from cloudperf.benchmarks import benchmarks
 from cloudperf.core import sftp_write_file, DictQuery
-from cloudperf.providers.aws import region_map
 
 
 session = boto3.session.Session()
 logger = logging.getLogger(__name__)
 logger.addHandler(NullHandler())
 
 # Self-destruct the machine after 2 hours
@@ -273,14 +272,15 @@
     Args:
         get_instance_types arguments
 
     Returns:
         DataFrame with instance attributes and pricing
 
     """
+    from cloudperf.providers.aws import region_map
     prices = []
     params = {}
 
     for data in get_ec2_instances(**filter_opts):
         try:
             instance_type = data['product']['attributes']['instanceType']
             price = float(list(list(data['terms']['OnDemand'].values())[
```

### Comparing `cloudperf-0.0.8/cloudperf.egg-info/PKG-INFO` & `cloudperf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudperf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Relative performance index for cloud services
 Home-page: https://github.com/bra-fsn/cloudperf
 Author: NAGY, Attila
 Author-email: nagy.attila@gmail.com
 License: UNKNOWN
 Description: # cloudperf
         ## Measuring the relative performance of cloud resources
```

### Comparing `cloudperf-0.0.8/README.md` & `cloudperf-0.0.9/README.md`

 * *Files identical despite different names*

