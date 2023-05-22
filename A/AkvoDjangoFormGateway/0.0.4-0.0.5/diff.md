# Comparing `tmp/AkvoDjangoFormGateway-0.0.4.tar.gz` & `tmp/AkvoDjangoFormGateway-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoDjangoFormGateway-0.0.4.tar", last modified: Thu May 18 16:15:58 2023, max compression
+gzip compressed data, was "AkvoDjangoFormGateway-0.0.5.tar", last modified: Mon May 22 10:48:51 2023, max compression
```

## Comparing `AkvoDjangoFormGateway-0.0.4.tar` & `AkvoDjangoFormGateway-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.826419 AkvoDjangoFormGateway-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-18 16:15:58.826419 AkvoDjangoFormGateway-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-18 16:15:58.826419 AkvoDjangoFormGateway-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.814419 AkvoDjangoFormGateway-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.818420 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.822420 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.822420 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.822420 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.826419 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.826419 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-18 16:15:47.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 16:15:58.822420 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-18 16:15:58.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-18 16:15:58.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:15:58.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 16:15:58.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-18 16:15:58.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 16:15:58.000000 AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.471609 AkvoDjangoFormGateway-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/top_level.txt
```

### Comparing `AkvoDjangoFormGateway-0.0.4/LICENSE` & `AkvoDjangoFormGateway-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/PKG-INFO` & `AkvoDjangoFormGateway-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.4/README.md` & `AkvoDjangoFormGateway-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/setup.py` & `AkvoDjangoFormGateway-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/feed.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/feed.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/migrations/0001_initial.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/models.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/models.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/serializers.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,22 @@
 
     def get_form_name(self, obj):
         return obj.form.name
 
 
 class ListDataAnswerSerializer(serializers.ModelSerializer):
     value = serializers.SerializerMethodField()
+    question_type = serializers.SerializerMethodField()
 
     class Meta:
         model = AkvoGatewayAnswer
-        fields = ["question", "value"]
+        fields = ["question", "question_type", "value"]
+
+    def get_question_type(self, obj):
+        return QuestionTypes.FieldStr.get(obj.question.type)
 
     def get_value(self, instance: AkvoGatewayAnswer):
         return get_answer_value(instance)
 
 
 class QuestionDefinitionSerializer(serializers.ModelSerializer):
     question_type = serializers.SerializerMethodField()
```

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,14 @@
                 "created",
                 "updated",
             ],
         )
 
     def test_expected_fields_in_answer(self):
         data = self.answer_serializer.data
-        self.assertEqual(list(data), ["question", "value"])
+        self.assertEqual(list(data), ["question", "question_type", "value"])
         self.assertEqual(str(self.data.first()), self.data.first().name)
 
     def test_value_content_in_answer(self):
         data = self.answer_serializer.data
         self.assertEqual(data["value"], self.answer.name)
         self.assertEqual(str(self.answer), self.answer.data.name)
```

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_init.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_init.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/tests/tests_validation.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/urls.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/urls.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/utils/functions.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/functions.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/utils/validation.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway/views.py` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 )
 from .constants import StatusTypes
 from .feed import Feed
 
 account_sid = settings.TWILIO_ACCOUNT_SID
 auth_token = settings.TWILIO_AUTH_TOKEN
 from_number = settings.TWILIO_PHONE_NUMBER
-client = Client(account_sid, auth_token)
 
 
 @permission_classes([AllowAny])
 class CheckView(GenericViewSet):
     def check(self, request):
         return Response({"message": settings.TWILIO_ACCOUNT_SID})
 
@@ -98,14 +97,15 @@
                 else:
                     feed.set_as_completed(data=datapoint)
                     message = "Thank you!"
             else:
                 message = f"{lq.order}. {lq.text}"
                 message += feed.show_options(question=lq)
 
+        client = Client(account_sid, auth_token)
         feed.send_to_client(
             client=client,
             from_number=from_number,
             body=message,
             to_number=phone,
         )
         return Response(message)
```

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/PKG-INFO` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.4/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt` & `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

