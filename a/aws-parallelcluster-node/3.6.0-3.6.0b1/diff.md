# Comparing `tmp/aws-parallelcluster-node-3.6.0.tar.gz` & `tmp/aws-parallelcluster-node-3.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-parallelcluster-node-3.6.0.tar", last modified: Mon May 22 15:43:58 2023, max compression
+gzip compressed data, was "aws-parallelcluster-node-3.6.0b1.tar", last modified: Thu Apr 27 20:57:52 2023, max compression
```

## Comparing `aws-parallelcluster-node-3.6.0.tar` & `aws-parallelcluster-node-3.6.0b1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.045503 aws-parallelcluster-node-3.6.0/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11358 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/LICENSE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      102 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/NOTICE.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      732 2023-05-22 15:43:58.045503 aws-parallelcluster-node-3.6.0/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      748 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/README.md
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-05-22 15:43:58.045503 aws-parallelcluster-node-3.6.0/setup.cfg
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2298 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/setup.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.037503 aws-parallelcluster-node-3.6.0/src/
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.041503 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      732 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1338 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      257 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       30 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/requires.txt
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)       20 2023-05-22 15:43:57.000000 aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.041503 aws-parallelcluster-node-3.6.0/src/common/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/common/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1284 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/common/ec2_utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.041503 aws-parallelcluster-node-3.6.0/src/common/schedulers/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/common/schedulers/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16552 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/common/schedulers/slurm_commands.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      733 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/common/time_utils.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11793 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/common/utils.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.041503 aws-parallelcluster-node-3.6.0/src/slurm_plugin/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/__init__.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    31297 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/cluster_event_publisher.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    63899 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/clustermgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5071 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/common.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9891 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/computemgtd.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4232 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/console_logger.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17504 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/fleet_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6565 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/fleet_status_manager.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    22150 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/instance_manager.py
-drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-05-22 15:43:58.045503 aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1117 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      343 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      382 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      710 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)      369 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11351 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/resume.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25616 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/slurm_resources.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3658 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/suspend.py
--rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3268 2023-05-22 12:18:56.000000 aws-parallelcluster-node-3.6.0/src/slurm_plugin/task_executor.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11358 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/LICENSE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      102 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/NOTICE.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      734 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      748 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/README.md
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       38 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/setup.cfg
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     2300 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/setup.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.432629 aws-parallelcluster-node-3.6.0b1/src/
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      734 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1338 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      257 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)        1 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       30 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)       20 2023-04-27 20:57:52.000000 aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/common/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1284 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/ec2_utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/common/schedulers/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/schedulers/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    16552 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/schedulers/slurm_commands.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      733 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/time_utils.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11793 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/common/utils.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.436629 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      554 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/__init__.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    31273 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/cluster_event_publisher.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    63899 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/clustermgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     5071 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/common.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     9891 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/computemgtd.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     4232 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/console_logger.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    17504 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     6565 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_status_manager.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    22150 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/instance_manager.py
+drwxr-xr-x   0 jenkins   (2000) jenkins   (1000)        0 2023-04-27 20:57:52.440629 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     1117 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      343 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_computemgtd_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      382 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_fleet_status_manager_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      710 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)      369 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_suspend_logging.conf
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    11351 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/resume.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)    25616 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/slurm_resources.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3658 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/suspend.py
+-rw-r--r--   0 jenkins   (2000) jenkins   (1000)     3268 2023-04-27 19:15:12.000000 aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/task_executor.py
```

### Comparing `aws-parallelcluster-node-3.6.0/LICENSE.txt` & `aws-parallelcluster-node-3.6.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/PKG-INFO` & `aws-parallelcluster-node-3.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.6.0
+Version: 3.6.0b1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.6.0/README.md` & `aws-parallelcluster-node-3.6.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/setup.py` & `aws-parallelcluster-node-3.6.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 console_scripts = [
     "slurm_resume = slurm_plugin.resume:main",
     "slurm_suspend = slurm_plugin.suspend:main",
     "slurm_fleet_status_manager = slurm_plugin.fleet_status_manager:main",
     "clustermgtd = slurm_plugin.clustermgtd:main",
     "computemgtd = slurm_plugin.computemgtd:main",
 ]
-version = "3.6.0"
+version = "3.6.0b1"
 requires = ["boto3>=1.7.55", "retrying>=1.3.3"]
 
 setup(
     name="aws-parallelcluster-node",
     version=version,
     author="Amazon Web Services",
     description="aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.",
```

### Comparing `aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/PKG-INFO` & `aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-parallelcluster-node
-Version: 3.6.0
+Version: 3.6.0b1
 Summary: aws-parallelcluster-node provides the scripts for an AWS ParallelCluster node.
 Home-page: https://github.com/aws/aws-parallelcluster-node
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-parallelcluster-node-3.6.0/src/aws_parallelcluster_node.egg-info/SOURCES.txt` & `aws-parallelcluster-node-3.6.0b1/src/aws_parallelcluster_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/common/__init__.py` & `aws-parallelcluster-node-3.6.0b1/src/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/common/ec2_utils.py` & `aws-parallelcluster-node-3.6.0b1/src/common/ec2_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/common/schedulers/__init__.py` & `aws-parallelcluster-node-3.6.0b1/src/common/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/common/schedulers/slurm_commands.py` & `aws-parallelcluster-node-3.6.0b1/src/common/schedulers/slurm_commands.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/common/time_utils.py` & `aws-parallelcluster-node-3.6.0b1/src/common/time_utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/common/utils.py` & `aws-parallelcluster-node-3.6.0b1/src/common/utils.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/__init__.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/cluster_event_publisher.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/cluster_event_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
                 "detail": {
                     "node-state": state,
                     "count": count,
                 }
             }
 
     def _idle_node_suppler(self, node_type: str, current_time: datetime, idle_nodes: List[SlurmNode]):
-        longest_idle_node = max(idle_nodes, key=lambda node: node.idle_time(current_time)) if idle_nodes else None
+        longest_idle_node = max(idle_nodes, key=lambda node: node.idle_time(current_time))
         yield {
             "detail": {
                 "node-type": node_type,
                 "longest-idle-time": longest_idle_node.idle_time(current_time) if longest_idle_node else 0,
                 "longest-idle-node": self._describe_node(longest_idle_node) if longest_idle_node else None,
                 "count": len(idle_nodes),
             }
```

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/clustermgtd.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/clustermgtd.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/common.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/common.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/computemgtd.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/computemgtd.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/console_logger.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/console_logger.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/fleet_manager.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/fleet_status_manager.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/fleet_status_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/instance_manager.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/instance_manager.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_clustermgtd_logging.conf`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/logging/parallelcluster_resume_logging.conf` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/logging/parallelcluster_resume_logging.conf`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/resume.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/resume.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/slurm_resources.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/slurm_resources.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/suspend.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/suspend.py`

 * *Files identical despite different names*

### Comparing `aws-parallelcluster-node-3.6.0/src/slurm_plugin/task_executor.py` & `aws-parallelcluster-node-3.6.0b1/src/slurm_plugin/task_executor.py`

 * *Files identical despite different names*

