# Comparing `tmp/aeropress-0.0.8.tar.gz` & `tmp/aeropress-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aeropress-0.0.8.tar", last modified: Thu Jan 31 08:09:36 2019, max compression
+gzip compressed data, was "dist/aeropress-0.0.9.tar", last modified: Thu Jan 31 10:36:18 2019, max compression
```

## Comparing `aeropress-0.0.8.tar` & `aeropress-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 08:09:36.000000 aeropress-0.0.8/
--rw-r--r--   0 murat      (501) staff       (20)     2127 2019-01-31 08:09:36.000000 aeropress-0.0.8/PKG-INFO
--rw-r--r--   0 murat      (501) staff       (20)     1348 2019-01-28 13:53:52.000000 aeropress-0.0.8/README.rst
-drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress/
--rw-r--r--   0 murat      (501) staff       (20)      101 2019-01-30 12:56:06.000000 aeropress-0.0.8/aeropress/__init__.py
--rw-r--r--   0 murat      (501) staff       (20)       22 2019-01-31 08:08:19.000000 aeropress-0.0.8/aeropress/_version.py
-drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress/aws/
--rw-r--r--   0 murat      (501) staff       (20)        0 2019-01-28 13:01:16.000000 aeropress-0.0.8/aeropress/aws/__init__.py
--rw-r--r--   0 murat      (501) staff       (20)     5016 2019-01-29 13:46:59.000000 aeropress-0.0.8/aeropress/aws/alarm.py
--rw-r--r--   0 murat      (501) staff       (20)      419 2019-01-29 12:30:03.000000 aeropress-0.0.8/aeropress/aws/cluster.py
--rw-r--r--   0 murat      (501) staff       (20)     1636 2019-01-29 13:45:05.000000 aeropress-0.0.8/aeropress/aws/log.py
--rw-r--r--   0 murat      (501) staff       (20)     1885 2019-01-29 12:30:49.000000 aeropress-0.0.8/aeropress/aws/metric.py
--rw-r--r--   0 murat      (501) staff       (20)     4869 2019-01-29 13:46:05.000000 aeropress-0.0.8/aeropress/aws/scale.py
--rw-r--r--   0 murat      (501) staff       (20)     3435 2019-01-29 13:57:28.000000 aeropress-0.0.8/aeropress/aws/service.py
--rw-r--r--   0 murat      (501) staff       (20)     5911 2019-01-30 14:20:43.000000 aeropress-0.0.8/aeropress/aws/task.py
--rw-r--r--   0 murat      (501) staff       (20)     4980 2019-01-30 14:04:31.000000 aeropress-0.0.8/aeropress/cli.py
-drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/
--rw-r--r--   0 murat      (501) staff       (20)     2127 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/PKG-INFO
--rw-r--r--   0 murat      (501) staff       (20)      479 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/SOURCES.txt
--rw-r--r--   0 murat      (501) staff       (20)        1 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/dependency_links.txt
--rw-r--r--   0 murat      (501) staff       (20)       50 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/entry_points.txt
--rw-r--r--   0 murat      (501) staff       (20)       11 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/requires.txt
--rw-r--r--   0 murat      (501) staff       (20)       10 2019-01-31 08:09:36.000000 aeropress-0.0.8/aeropress.egg-info/top_level.txt
--rw-r--r--   0 murat      (501) staff       (20)      388 2019-01-31 08:09:36.000000 aeropress-0.0.8/setup.cfg
--rw-r--r--   0 murat      (501) staff       (20)      856 2019-01-28 14:12:58.000000 aeropress-0.0.8/setup.py
+drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 10:36:18.000000 aeropress-0.0.9/
+-rw-r--r--   0 murat      (501) staff       (20)     2127 2019-01-31 10:36:18.000000 aeropress-0.0.9/PKG-INFO
+-rw-r--r--   0 murat      (501) staff       (20)     1348 2019-01-28 13:53:52.000000 aeropress-0.0.9/README.rst
+drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress/
+-rw-r--r--   0 murat      (501) staff       (20)      101 2019-01-30 12:56:06.000000 aeropress-0.0.9/aeropress/__init__.py
+-rw-r--r--   0 murat      (501) staff       (20)       22 2019-01-31 10:36:03.000000 aeropress-0.0.9/aeropress/_version.py
+drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress/aws/
+-rw-r--r--   0 murat      (501) staff       (20)        0 2019-01-28 13:01:16.000000 aeropress-0.0.9/aeropress/aws/__init__.py
+-rw-r--r--   0 murat      (501) staff       (20)     5016 2019-01-29 13:46:59.000000 aeropress-0.0.9/aeropress/aws/alarm.py
+-rw-r--r--   0 murat      (501) staff       (20)      419 2019-01-29 12:30:03.000000 aeropress-0.0.9/aeropress/aws/cluster.py
+-rw-r--r--   0 murat      (501) staff       (20)     1636 2019-01-29 13:45:05.000000 aeropress-0.0.9/aeropress/aws/log.py
+-rw-r--r--   0 murat      (501) staff       (20)     1885 2019-01-29 12:30:49.000000 aeropress-0.0.9/aeropress/aws/metric.py
+-rw-r--r--   0 murat      (501) staff       (20)     4869 2019-01-29 13:46:05.000000 aeropress-0.0.9/aeropress/aws/scale.py
+-rw-r--r--   0 murat      (501) staff       (20)     3435 2019-01-29 13:57:28.000000 aeropress-0.0.9/aeropress/aws/service.py
+-rw-r--r--   0 murat      (501) staff       (20)     5979 2019-01-31 08:45:40.000000 aeropress-0.0.9/aeropress/aws/task.py
+-rw-r--r--   0 murat      (501) staff       (20)     4980 2019-01-31 10:24:47.000000 aeropress-0.0.9/aeropress/cli.py
+drwxr-xr-x   0 murat      (501) staff       (20)        0 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/
+-rw-r--r--   0 murat      (501) staff       (20)     2127 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/PKG-INFO
+-rw-r--r--   0 murat      (501) staff       (20)      479 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/SOURCES.txt
+-rw-r--r--   0 murat      (501) staff       (20)        1 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/dependency_links.txt
+-rw-r--r--   0 murat      (501) staff       (20)       50 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/entry_points.txt
+-rw-r--r--   0 murat      (501) staff       (20)       11 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/requires.txt
+-rw-r--r--   0 murat      (501) staff       (20)       10 2019-01-31 10:36:18.000000 aeropress-0.0.9/aeropress.egg-info/top_level.txt
+-rw-r--r--   0 murat      (501) staff       (20)      388 2019-01-31 10:36:18.000000 aeropress-0.0.9/setup.cfg
+-rw-r--r--   0 murat      (501) staff       (20)      856 2019-01-28 14:12:58.000000 aeropress-0.0.9/setup.py
```

### Comparing `aeropress-0.0.8/PKG-INFO` & `aeropress-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aeropress
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper for deploying Docker images to AWS ECS.
 Home-page: https://github.com/muraty/aeropress
 Author: Omer Murat Yildirim
 Author-email: omermuratyildirim@gmail.com
 License: BSD License
 Description: 
         aeropress
```

### Comparing `aeropress-0.0.8/README.rst` & `aeropress-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress/aws/alarm.py` & `aeropress-0.0.9/aeropress/aws/alarm.py`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress/aws/log.py` & `aeropress-0.0.9/aeropress/aws/log.py`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress/aws/metric.py` & `aeropress-0.0.9/aeropress/aws/metric.py`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress/aws/scale.py` & `aeropress-0.0.9/aeropress/aws/scale.py`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress/aws/service.py` & `aeropress-0.0.9/aeropress/aws/service.py`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress/aws/task.py` & `aeropress-0.0.9/aeropress/aws/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         for container_definition in task_dict['containerDefinitions']:
             container_definitions.append({
                 'name': container_definition['name'],
                 'image': container_definition['image'],
                 'logConfiguration': container_definition['logConfiguration'],
                 'memoryReservation': container_definition['memoryReservation'],
                 'entryPoint': container_definition['entryPoint'],
+                'environment': container_definition['environment'],
             })
 
         logger.info('Creating task definition: %s', task_dict['family'])
         response = ecs_client.register_task_definition(
             family=task_dict['family'],
             taskRoleArn=task_dict['taskRoleArn'],
             executionRoleArn=task_dict['executionRoleArn'],
```

### Comparing `aeropress-0.0.8/aeropress/cli.py` & `aeropress-0.0.9/aeropress/cli.py`

 * *Files identical despite different names*

### Comparing `aeropress-0.0.8/aeropress.egg-info/PKG-INFO` & `aeropress-0.0.9/aeropress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aeropress
-Version: 0.0.8
+Version: 0.0.9
 Summary: Helper for deploying Docker images to AWS ECS.
 Home-page: https://github.com/muraty/aeropress
 Author: Omer Murat Yildirim
 Author-email: omermuratyildirim@gmail.com
 License: BSD License
 Description: 
         aeropress
```

### Comparing `aeropress-0.0.8/setup.py` & `aeropress-0.0.9/setup.py`

 * *Files identical despite different names*

