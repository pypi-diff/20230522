# Comparing `tmp/py_auth_amqp_wrapper-0.0.7.tar.gz` & `tmp/py_auth_amqp_wrapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_amqp_wrapper-0.0.7.tar", last modified: Fri May 19 12:03:21 2023, max compression
+gzip compressed data, was "py_auth_amqp_wrapper-0.0.8.tar", last modified: Mon May 22 08:39:59 2023, max compression
```

## Comparing `py_auth_amqp_wrapper-0.0.7.tar` & `py_auth_amqp_wrapper-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_getlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 12:03:21.000000 py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 12:02:51.000000 py_auth_amqp_wrapper-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-19 12:03:21.775524 py_auth_amqp_wrapper-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:39:59.586410 py_auth_amqp_wrapper-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-22 08:39:59.586410 py_auth_amqp_wrapper-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:39:59.586410 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_getlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:39:59.586410 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-22 08:39:59.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-22 08:39:59.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:39:59.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 08:39:59.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 08:39:59.000000 py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 08:39:23.000000 py_auth_amqp_wrapper-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 08:39:59.586410 py_auth_amqp_wrapper-0.0.8/setup.cfg
```

### Comparing `py_auth_amqp_wrapper-0.0.7/LICENSE` & `py_auth_amqp_wrapper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.7/PKG-INFO` & `py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: py_auth_amqp_wrapper
-Version: 0.0.7
+Name: py-auth-amqp-wrapper
+Version: 0.0.8
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_amqp_wrapper
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: AMQP
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/__main__.py` & `py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_getlogger.py` & `py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_getlogger.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_load_config.py` & `py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_load_config.py`

 * *Files identical despite different names*

### Comparing `py_auth_amqp_wrapper-0.0.7/py_auth_amqp_wrapper/_runner.py` & `py_auth_amqp_wrapper-0.0.8/py_auth_amqp_wrapper/_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,11 +154,13 @@
     await service.register_function(user_workflow_change_user)
     await service.register_function(user_workflow_get_all)
     await service.register_function(user_workflow_get_user)
     await service.register_function(group_workflow_add_user_to_group)
     await service.register_function(group_workflow_remove_user_from_group)
     await service.register_function(group_workflow_create_group)
     await service.register_function(group_workflow_delete_group)
-
+    await service.register_function(group_workflow_get_groups)    
+    await service.register_function(group_workflow_group_users)
+    
     await service.serve()
 
     return
```

### Comparing `py_auth_amqp_wrapper-0.0.7/setup.cfg` & `py_auth_amqp_wrapper-0.0.8/setup.cfg`

 * *Files identical despite different names*

