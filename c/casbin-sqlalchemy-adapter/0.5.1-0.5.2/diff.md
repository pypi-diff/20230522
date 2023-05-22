# Comparing `tmp/casbin_sqlalchemy_adapter-0.5.1.tar.gz` & `tmp/casbin_sqlalchemy_adapter-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_sqlalchemy_adapter-0.5.1.tar", last modified: Sun Apr 16 01:48:19 2023, max compression
+gzip compressed data, was "casbin_sqlalchemy_adapter-0.5.2.tar", last modified: Mon May 22 06:42:32 2023, max compression
```

## Comparing `casbin_sqlalchemy_adapter-0.5.1.tar` & `casbin_sqlalchemy_adapter-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-16 01:48:19.464608 casbin_sqlalchemy_adapter-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-16 01:48:19.000000 casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 01:48:19.464608 casbin_sqlalchemy_adapter-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:48:19.460608 casbin_sqlalchemy_adapter-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-04-16 01:47:39.000000 casbin_sqlalchemy_adapter-0.5.1/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:32.576630 casbin_sqlalchemy_adapter-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 06:41:53.000000 casbin_sqlalchemy_adapter-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-22 06:42:32.576630 casbin_sqlalchemy_adapter-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-22 06:41:53.000000 casbin_sqlalchemy_adapter-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:32.576630 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 06:41:53.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-05-22 06:41:53.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:32.576630 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-22 06:42:32.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 06:42:32.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:42:32.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 06:42:32.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 06:42:32.000000 casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 06:42:32.576630 casbin_sqlalchemy_adapter-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-22 06:41:53.000000 casbin_sqlalchemy_adapter-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:32.576630 casbin_sqlalchemy_adapter-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-05-22 06:41:53.000000 casbin_sqlalchemy_adapter-0.5.2/tests/test_adapter.py
```

### Comparing `casbin_sqlalchemy_adapter-0.5.1/LICENSE` & `casbin_sqlalchemy_adapter-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-0.5.1/PKG-INFO` & `casbin_sqlalchemy_adapter-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_sqlalchemy_adapter
-Version: 0.5.1
+Version: 0.5.2
 Summary: SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/sqlalchemy-adapter
 Author: TechLee
 Author-email: techlee@qq.com
 License: Apache 2.0
 Keywords: casbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `casbin_sqlalchemy_adapter-0.5.1/README.md` & `casbin_sqlalchemy_adapter-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter/adapter.py` & `casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `casbin_sqlalchemy_adapter-0.5.1/casbin_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_sqlalchemy_adapter-0.5.2/casbin_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-sqlalchemy-adapter
-Version: 0.5.1
+Version: 0.5.2
 Summary: SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/sqlalchemy-adapter
 Author: TechLee
 Author-email: techlee@qq.com
 License: Apache 2.0
 Keywords: casbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `casbin_sqlalchemy_adapter-0.5.1/setup.py` & `casbin_sqlalchemy_adapter-0.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,9 +40,8 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-    data_files=[desc_file],
 )
```

### Comparing `casbin_sqlalchemy_adapter-0.5.1/tests/test_adapter.py` & `casbin_sqlalchemy_adapter-0.5.2/tests/test_adapter.py`

 * *Files identical despite different names*

