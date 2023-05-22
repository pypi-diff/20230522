# Comparing `tmp/AkvoDjangoFormGateway-0.0.5.tar.gz` & `tmp/AkvoDjangoFormGateway-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AkvoDjangoFormGateway-0.0.5.tar", last modified: Mon May 22 10:48:51 2023, max compression
+gzip compressed data, was "AkvoDjangoFormGateway-0.0.6.tar", last modified: Mon May 22 16:17:20 2023, max compression
```

## Comparing `AkvoDjangoFormGateway-0.0.5.tar` & `AkvoDjangoFormGateway-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.471609 AkvoDjangoFormGateway-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-22 10:48:39.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:48:51.475609 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 10:48:51.000000 AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.193673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-22 16:17:10.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:20.189673 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 16:17:20.000000 AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/top_level.txt
```

### Comparing `AkvoDjangoFormGateway-0.0.5/LICENSE` & `AkvoDjangoFormGateway-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/PKG-INFO` & `AkvoDjangoFormGateway-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.5/README.md` & `AkvoDjangoFormGateway-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/setup.py` & `AkvoDjangoFormGateway-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/feed.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         image_url: str = None,
         lat: str = None,
         lng: str = None,
     ) -> str:
         text = body
         if image_url:
             text = image_url
+            return text
         if lat and lng:
             text = json.dumps(
                 [
                     lat,
                     lng,
                 ]
             )
```

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/fake_gateway_data_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/management/commands/gateway_form_seeder.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/migrations/0001_initial.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/models.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/models.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/serializers.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/serializers.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_data_serializers.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_form_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_init.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_init.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_question_serializer.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_seeder_command.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_twilio_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self.assertEqual(response.status_code, 200)
 
         # Photo question
         question = feed.get_question(form=survey, data=datapoint)
         self.assertEqual(response.json(), f"{question.order}. {question.text}")
 
         # Answer wrong photo question no MediaContentType0
-        image = "http://twilio.example/image.png"
+        image = "http://twilio.example/image/caseSensiT1Ve.png"
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "MediaUrl0": image,
         }
         response = client.post("/api/gateway/twilio/", json_form)
         self.assertEqual(response.status_code, 400)
@@ -91,14 +91,17 @@
         json_form = {
             "Body": "",
             "From": f"whatsapp:+{phone_number}",
             "MediaContentType0": image_type,
             "MediaUrl0": image,
         }
         response = client.post("/api/gateway/twilio/", json_form)
+        stored_image = Answers.objects.filter(question=question).first().name
+        self.assertEqual(image, stored_image)
+        self.assertNotEqual(image.lower(), stored_image)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             feed.validate_answer(
                 text="",
                 question=question,
                 data=datapoint,
                 image_type=image_type,
@@ -277,23 +280,23 @@
         self.assertEqual(init, False)
 
     def test_instance_request(self):
         form_id = 1
 
         json_form = {}
         response = client.post(
-            f"/api/gateway/twilio/{form_id}/?format=json", json_form
+            f"/api/gateway/twilio/{form_id}?format=json", json_form
         )
         self.assertEqual(response.status_code, 200)
         # first question shown
         fq = Questions.objects.filter(form=form_id).order_by("order").first()
 
         reply_text = "answer first question"
         json_form = {"Body": reply_text, "From": f"whatsapp:+{phone_number}"}
 
-        response = client.post(f"/api/gateway/twilio/{form_id}/", json_form)
+        response = client.post(f"/api/gateway/twilio/{form_id}", json_form)
         datapoint = feed.get_draft_datapoint(phone=phone_number)
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             feed.validate_answer(text=reply_text, question=fq, data=datapoint),
             True,
         )
```

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/tests/tests_validation.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/tests/tests_validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/urls.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     path(
         "forms/<int:pk>/",
         AkvoFormViewSet.as_view({"get": "retrieve"}),
         name="twilio",
     ),
     path("twilio/", TwilioViewSet.as_view({"post": "create"}), name="twilio"),
     path(
-        "twilio/<int:pk>/",
+        # Twilio recomend to not use extra slash
+        "twilio/<int:pk>",
         TwilioViewSet.as_view({"post": "instance"}),
         name="twilio",
     ),
     path(
         "data/",
         DataViewSet.as_view({"get": "list"}),
         name="twilio",
```

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/functions.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/functions.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/utils/validation.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/utils/validation.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway/views.py` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway/views.py`

 * *Files identical despite different names*

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/PKG-INFO` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AkvoDjangoFormGateway
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Django library that enables seamless integration of messenger services
 Home-page: https://github.com/akvo/Akvo-DjangoFormGateway
 Author: Akvo
 Author-email: tech.consultancy@akvo.org
 Maintainer: Deden Bangkit
 Maintainer-email: deden@akvo.org
 Project-URL: Documentation, https://github.com/akvo/Akvo-DjangoFormGateway
```

### Comparing `AkvoDjangoFormGateway-0.0.5/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt` & `AkvoDjangoFormGateway-0.0.6/src/AkvoDjangoFormGateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

